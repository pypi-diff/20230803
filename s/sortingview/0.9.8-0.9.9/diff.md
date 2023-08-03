# Comparing `tmp/sortingview-0.9.8.tar.gz` & `tmp/sortingview-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortingview-0.9.8.tar", last modified: Thu Jul 21 16:16:03 2022, max compression
+gzip compressed data, was "sortingview-0.9.9.tar", last modified: Wed Jul 27 16:34:46 2022, max compression
```

## Comparing `sortingview-0.9.8.tar` & `sortingview-0.9.9.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.735164 sortingview-0.9.8/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2022-04-19 16:15:36.000000 sortingview-0.9.8/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)      546 2022-07-21 16:16:03.735164 sortingview-0.9.8/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     6205 2022-07-05 20:37:11.000000 sortingview-0.9.8/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.723164 sortingview-0.9.8/bin/
--rw-rw-r--   0 magland   (1000) magland   (1000)      106 2022-04-19 16:18:51.000000 sortingview-0.9.8/bin/sortingview-start-backend
--rw-rw-r--   0 magland   (1000) magland   (1000)      526 2022-07-21 16:16:03.735164 sortingview-0.9.8/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      413 2022-07-14 09:38:08.000000 sortingview-0.9.8/setup.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.723164 sortingview-0.9.8/sortingview/
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.727164 sortingview-0.9.8/sortingview/SpikeSortingView/
--rw-rw-r--   0 magland   (1000) magland   (1000)      790 2022-07-21 16:13:51.000000 sortingview-0.9.8/sortingview/SpikeSortingView/Figure.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1137 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/SpikeSortingView/MultiTimeseries.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     6607 2022-07-05 20:25:43.000000 sortingview-0.9.8/sortingview/SpikeSortingView/SpikeSortingView.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      588 2022-07-05 20:14:25.000000 sortingview-0.9.8/sortingview/SpikeSortingView/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      981 2022-07-05 19:41:25.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_autocorrelograms_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1520 2022-07-05 19:49:36.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_average_waveforms_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1016 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_autocorrelograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1703 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_average_waveforms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      708 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_electrode_geometry.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      532 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_live_cross_correlograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      947 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_mountain_layout.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1301 2022-06-30 15:29:03.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_raster_plot.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1579 2022-06-30 15:29:11.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_spike_amplitudes.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1262 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_summary.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2350 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_create_units_table.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1383 2022-07-09 12:03:53.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_cross_correlograms_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      482 2022-07-05 19:57:14.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_electrode_geometry_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1272 2022-07-05 19:37:54.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_raster_plot_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1114 2022-07-13 16:28:45.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_sorting_summary_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1555 2022-07-09 12:04:31.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_spike_amplitudes_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2399 2022-07-05 19:21:08.000000 sortingview-0.9.8/sortingview/SpikeSortingView/_units_table_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      259 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/create_console_view.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      265 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/create_epochs.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1720 2022-05-27 18:27:18.000000 sortingview-0.9.8/sortingview/SpikeSortingView/create_position_pdf_plot.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1258 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/create_position_plot.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      396 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/create_raw_traces_plot.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      651 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/create_spike_raster_plot.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.727164 sortingview-0.9.8/sortingview/SpikeSortingView/helpers/
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/helpers/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3228 2022-04-29 16:06:39.000000 sortingview-0.9.8/sortingview/SpikeSortingView/helpers/compute_correlogram_data.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    11460 2022-07-05 20:20:56.000000 sortingview-0.9.8/sortingview/SpikeSortingView/prepare_spikesortingview_data.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      765 2022-07-05 14:43:45.000000 sortingview-0.9.8/sortingview/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.727164 sortingview-0.9.8/sortingview/backend/
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-04-19 16:23:07.000000 sortingview-0.9.8/sortingview/backend/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      382 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/backend/_verify_oauth2_token.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3228 2022-07-21 15:17:57.000000 sortingview-0.9.8/sortingview/backend/compute_correlogram_data.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2783 2022-06-23 19:05:43.000000 sortingview-0.9.8/sortingview/backend/start_backend.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      471 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/backend/start_backend_cli.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.731164 sortingview-0.9.8/sortingview/load_extractors/
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.731164 sortingview-0.9.8/sortingview/load_extractors/MdaRecordingExtractorV2/
--rw-rw-r--   0 magland   (1000) magland   (1000)    17849 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/load_extractors/MdaRecordingExtractorV2/MdaRecordingExtractorV2.py
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/load_extractors/MdaRecordingExtractorV2/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/load_extractors/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.731164 sortingview-0.9.8/sortingview/load_extractors/binextractors/
--rw-rw-r--   0 magland   (1000) magland   (1000)      117 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/load_extractors/binextractors/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2043 2022-07-12 19:12:31.000000 sortingview-0.9.8/sortingview/load_extractors/binextractors/bin1recordingextractor.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2676 2022-05-13 15:15:32.000000 sortingview-0.9.8/sortingview/load_extractors/binextractors/bin2recordingextractor.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2483 2022-06-01 20:13:06.000000 sortingview-0.9.8/sortingview/load_extractors/copy_recording_extractor.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2126 2022-06-01 20:12:37.000000 sortingview-0.9.8/sortingview/load_extractors/copy_sorting_extractor.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1951 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/load_extractors/get_recording_object.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1861 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/load_extractors/get_sorting_object.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.731164 sortingview-0.9.8/sortingview/load_extractors/h5extractors/
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.731164 sortingview-0.9.8/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/
--rw-rw-r--   0 magland   (1000) magland   (1000)     6138 2022-06-01 19:57:27.000000 sortingview-0.9.8/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/TimeseriesModel_Hdf5.py
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-06-29 20:28:59.000000 sortingview-0.9.8/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-06-29 14:52:21.000000 sortingview-0.9.8/sortingview/load_extractors/h5extractors/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1873 2022-06-01 19:29:53.000000 sortingview-0.9.8/sortingview/load_extractors/h5extractors/h5recordingextractorv1.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3297 2022-07-11 15:34:44.000000 sortingview-0.9.8/sortingview/load_extractors/load_recording_extractor.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2315 2022-06-23 19:06:17.000000 sortingview-0.9.8/sortingview/load_extractors/load_sorting_extractor.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    15311 2022-06-23 19:06:42.000000 sortingview-0.9.8/sortingview/load_extractors/mdaio.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      401 2022-07-11 15:18:30.000000 sortingview-0.9.8/sortingview/load_extractors/save_recording.py
--rw-rw-r--   0 magland   (1000) magland   (1000)       97 2022-07-21 16:15:31.000000 sortingview-0.9.8/sortingview/version.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.735164 sortingview-0.9.8/sortingview/views/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1124 2022-07-05 13:47:35.000000 sortingview-0.9.8/sortingview/views/Autocorrelograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1778 2022-07-15 12:14:07.000000 sortingview-0.9.8/sortingview/views/AverageWaveforms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1069 2022-07-05 13:48:08.000000 sortingview-0.9.8/sortingview/views/Box.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1397 2022-07-07 17:24:31.000000 sortingview-0.9.8/sortingview/views/CrossCorrelograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      520 2022-07-05 19:57:01.000000 sortingview-0.9.8/sortingview/views/ElectrodeGeometry.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      751 2022-07-13 19:56:18.000000 sortingview-0.9.8/sortingview/views/LayoutItem.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      426 2022-07-13 19:38:34.000000 sortingview-0.9.8/sortingview/views/Markdown.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1098 2022-07-05 15:05:04.000000 sortingview-0.9.8/sortingview/views/MountainLayout.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1174 2022-07-05 13:49:19.000000 sortingview-0.9.8/sortingview/views/RasterPlot.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      369 2022-07-05 14:45:20.000000 sortingview-0.9.8/sortingview/views/SortingCuration.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1796 2022-07-05 19:32:34.000000 sortingview-0.9.8/sortingview/views/SortingSummary.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1478 2022-07-07 17:48:41.000000 sortingview-0.9.8/sortingview/views/SpikeAmplitudes.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      983 2022-07-05 14:45:45.000000 sortingview-0.9.8/sortingview/views/Splitter.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      956 2022-07-13 19:58:13.000000 sortingview-0.9.8/sortingview/views/TabLayout.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3741 2022-07-21 13:49:56.000000 sortingview-0.9.8/sortingview/views/TiledImage.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1211 2022-07-20 15:28:36.000000 sortingview-0.9.8/sortingview/views/UnitLocations.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1385 2022-07-15 15:14:51.000000 sortingview-0.9.8/sortingview/views/UnitMetricsGraph.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1168 2022-07-05 14:45:25.000000 sortingview-0.9.8/sortingview/views/UnitSimilarityMatrix.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1375 2022-07-05 14:45:29.000000 sortingview-0.9.8/sortingview/views/UnitsTable.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2262 2022-07-21 16:14:01.000000 sortingview-0.9.8/sortingview/views/View.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1062 2022-07-20 15:31:41.000000 sortingview-0.9.8/sortingview/views/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.735164 sortingview-0.9.8/sortingview/views/franklab/
--rw-rw-r--   0 magland   (1000) magland   (1000)     7710 2022-07-14 18:56:00.000000 sortingview-0.9.8/sortingview/views/franklab/TrackPositionAnimationV1.py
--rw-rw-r--   0 magland   (1000) magland   (1000)       84 2022-07-14 18:10:27.000000 sortingview-0.9.8/sortingview/views/franklab/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.735164 sortingview-0.9.8/sortingview/workspace/
--rw-rw-r--   0 magland   (1000) magland   (1000)    23848 2022-07-09 11:48:58.000000 sortingview-0.9.8/sortingview/workspace/Workspace.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      122 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/workspace/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3231 2022-06-29 21:52:58.000000 sortingview-0.9.8/sortingview/workspace/_get_sorting_curation.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     4421 2022-06-23 19:06:53.000000 sortingview-0.9.8/sortingview/workspace/_old_workspace.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1797 2022-06-30 15:24:14.000000 sortingview-0.9.8/sortingview/workspace/_spikesortingview.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      383 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/workspace/create_workspace.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      110 2022-05-13 12:51:54.000000 sortingview-0.9.8/sortingview/workspace/load_workspace.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-21 16:16:03.723164 sortingview-0.9.8/sortingview.egg-info/
--rw-rw-r--   0 magland   (1000) magland   (1000)      546 2022-07-21 16:16:03.000000 sortingview-0.9.8/sortingview.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     4247 2022-07-21 16:16:03.000000 sortingview-0.9.8/sortingview.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2022-07-21 16:16:03.000000 sortingview-0.9.8/sortingview.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      108 2022-07-21 16:16:03.000000 sortingview-0.9.8/sortingview.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       12 2022-07-21 16:16:03.000000 sortingview-0.9.8/sortingview.egg-info/top_level.txt
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.879599 sortingview-0.9.9/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2022-04-19 16:15:36.000000 sortingview-0.9.9/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)      546 2022-07-27 16:34:46.879599 sortingview-0.9.9/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     6205 2022-07-05 20:37:11.000000 sortingview-0.9.9/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.871599 sortingview-0.9.9/bin/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      106 2022-04-19 16:18:51.000000 sortingview-0.9.9/bin/sortingview-start-backend
+-rw-rw-r--   0 magland   (1000) magland   (1000)      526 2022-07-27 16:34:46.879599 sortingview-0.9.9/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      413 2022-07-14 09:38:08.000000 sortingview-0.9.9/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.871599 sortingview-0.9.9/sortingview/
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/SpikeSortingView/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      790 2022-07-21 16:13:51.000000 sortingview-0.9.9/sortingview/SpikeSortingView/Figure.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1137 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/SpikeSortingView/MultiTimeseries.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     6607 2022-07-05 20:25:43.000000 sortingview-0.9.9/sortingview/SpikeSortingView/SpikeSortingView.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      588 2022-07-05 20:14:25.000000 sortingview-0.9.9/sortingview/SpikeSortingView/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      981 2022-07-05 19:41:25.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_autocorrelograms_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1520 2022-07-05 19:49:36.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_average_waveforms_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1016 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_autocorrelograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1703 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_average_waveforms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      708 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_electrode_geometry.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      532 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_live_cross_correlograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      947 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_mountain_layout.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1301 2022-06-30 15:29:03.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_raster_plot.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1579 2022-06-30 15:29:11.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_spike_amplitudes.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1262 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_summary.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2350 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_create_units_table.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1383 2022-07-09 12:03:53.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_cross_correlograms_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      482 2022-07-05 19:57:14.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_electrode_geometry_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1272 2022-07-05 19:37:54.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_raster_plot_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1114 2022-07-13 16:28:45.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_sorting_summary_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1555 2022-07-09 12:04:31.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_spike_amplitudes_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2399 2022-07-05 19:21:08.000000 sortingview-0.9.9/sortingview/SpikeSortingView/_units_table_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      259 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/create_console_view.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      265 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/create_epochs.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1720 2022-05-27 18:27:18.000000 sortingview-0.9.9/sortingview/SpikeSortingView/create_position_pdf_plot.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1258 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/create_position_plot.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      396 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/create_raw_traces_plot.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      651 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/create_spike_raster_plot.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/SpikeSortingView/helpers/
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/helpers/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3228 2022-04-29 16:06:39.000000 sortingview-0.9.9/sortingview/SpikeSortingView/helpers/compute_correlogram_data.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11460 2022-07-05 20:20:56.000000 sortingview-0.9.9/sortingview/SpikeSortingView/prepare_spikesortingview_data.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      765 2022-07-05 14:43:45.000000 sortingview-0.9.9/sortingview/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/backend/
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-04-19 16:23:07.000000 sortingview-0.9.9/sortingview/backend/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      382 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/backend/_verify_oauth2_token.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3228 2022-07-21 15:17:57.000000 sortingview-0.9.9/sortingview/backend/compute_correlogram_data.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2783 2022-06-23 19:05:43.000000 sortingview-0.9.9/sortingview/backend/start_backend.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      471 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/backend/start_backend_cli.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/load_extractors/
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/load_extractors/MdaRecordingExtractorV2/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    17849 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/load_extractors/MdaRecordingExtractorV2/MdaRecordingExtractorV2.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/load_extractors/MdaRecordingExtractorV2/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/load_extractors/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/load_extractors/binextractors/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      117 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/load_extractors/binextractors/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2043 2022-07-12 19:12:31.000000 sortingview-0.9.9/sortingview/load_extractors/binextractors/bin1recordingextractor.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2676 2022-05-13 15:15:32.000000 sortingview-0.9.9/sortingview/load_extractors/binextractors/bin2recordingextractor.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2483 2022-06-01 20:13:06.000000 sortingview-0.9.9/sortingview/load_extractors/copy_recording_extractor.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2126 2022-06-01 20:12:37.000000 sortingview-0.9.9/sortingview/load_extractors/copy_sorting_extractor.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1951 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/load_extractors/get_recording_object.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1861 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/load_extractors/get_sorting_object.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/load_extractors/h5extractors/
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.875599 sortingview-0.9.9/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     6138 2022-06-01 19:57:27.000000 sortingview-0.9.9/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/TimeseriesModel_Hdf5.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-06-29 20:28:59.000000 sortingview-0.9.9/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2022-06-29 14:52:21.000000 sortingview-0.9.9/sortingview/load_extractors/h5extractors/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1873 2022-06-01 19:29:53.000000 sortingview-0.9.9/sortingview/load_extractors/h5extractors/h5recordingextractorv1.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3297 2022-07-11 15:34:44.000000 sortingview-0.9.9/sortingview/load_extractors/load_recording_extractor.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2315 2022-06-23 19:06:17.000000 sortingview-0.9.9/sortingview/load_extractors/load_sorting_extractor.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    15311 2022-06-23 19:06:42.000000 sortingview-0.9.9/sortingview/load_extractors/mdaio.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      401 2022-07-11 15:18:30.000000 sortingview-0.9.9/sortingview/load_extractors/save_recording.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       97 2022-07-27 16:34:24.000000 sortingview-0.9.9/sortingview/version.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.879599 sortingview-0.9.9/sortingview/views/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1124 2022-07-05 13:47:35.000000 sortingview-0.9.9/sortingview/views/Autocorrelograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1778 2022-07-15 12:14:07.000000 sortingview-0.9.9/sortingview/views/AverageWaveforms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1069 2022-07-05 13:48:08.000000 sortingview-0.9.9/sortingview/views/Box.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1397 2022-07-07 17:24:31.000000 sortingview-0.9.9/sortingview/views/CrossCorrelograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      520 2022-07-05 19:57:01.000000 sortingview-0.9.9/sortingview/views/ElectrodeGeometry.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      751 2022-07-13 19:56:18.000000 sortingview-0.9.9/sortingview/views/LayoutItem.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      426 2022-07-13 19:38:34.000000 sortingview-0.9.9/sortingview/views/Markdown.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1098 2022-07-05 15:05:04.000000 sortingview-0.9.9/sortingview/views/MountainLayout.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1174 2022-07-05 13:49:19.000000 sortingview-0.9.9/sortingview/views/RasterPlot.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      369 2022-07-05 14:45:20.000000 sortingview-0.9.9/sortingview/views/SortingCuration.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      625 2022-07-21 21:40:05.000000 sortingview-0.9.9/sortingview/views/SortingCuration2.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      522 2022-07-22 13:20:16.000000 sortingview-0.9.9/sortingview/views/SortingSelection.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1796 2022-07-05 19:32:34.000000 sortingview-0.9.9/sortingview/views/SortingSummary.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1478 2022-07-07 17:48:41.000000 sortingview-0.9.9/sortingview/views/SpikeAmplitudes.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      983 2022-07-05 14:45:45.000000 sortingview-0.9.9/sortingview/views/Splitter.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      956 2022-07-13 19:58:13.000000 sortingview-0.9.9/sortingview/views/TabLayout.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3767 2022-07-27 16:34:00.000000 sortingview-0.9.9/sortingview/views/TiledImage.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1211 2022-07-20 15:28:36.000000 sortingview-0.9.9/sortingview/views/UnitLocations.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1385 2022-07-15 15:14:51.000000 sortingview-0.9.9/sortingview/views/UnitMetricsGraph.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1168 2022-07-05 14:45:25.000000 sortingview-0.9.9/sortingview/views/UnitSimilarityMatrix.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1375 2022-07-05 14:45:29.000000 sortingview-0.9.9/sortingview/views/UnitsTable.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2262 2022-07-21 16:14:01.000000 sortingview-0.9.9/sortingview/views/View.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1156 2022-07-22 13:20:25.000000 sortingview-0.9.9/sortingview/views/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.879599 sortingview-0.9.9/sortingview/views/franklab/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     7710 2022-07-14 18:56:00.000000 sortingview-0.9.9/sortingview/views/franklab/TrackPositionAnimationV1.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       84 2022-07-14 18:10:27.000000 sortingview-0.9.9/sortingview/views/franklab/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.879599 sortingview-0.9.9/sortingview/workspace/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    23848 2022-07-09 11:48:58.000000 sortingview-0.9.9/sortingview/workspace/Workspace.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      122 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/workspace/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3231 2022-06-29 21:52:58.000000 sortingview-0.9.9/sortingview/workspace/_get_sorting_curation.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4421 2022-06-23 19:06:53.000000 sortingview-0.9.9/sortingview/workspace/_old_workspace.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1797 2022-06-30 15:24:14.000000 sortingview-0.9.9/sortingview/workspace/_spikesortingview.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      383 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/workspace/create_workspace.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      110 2022-05-13 12:51:54.000000 sortingview-0.9.9/sortingview/workspace/load_workspace.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2022-07-27 16:34:46.871599 sortingview-0.9.9/sortingview.egg-info/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      546 2022-07-27 16:34:46.000000 sortingview-0.9.9/sortingview.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4323 2022-07-27 16:34:46.000000 sortingview-0.9.9/sortingview.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2022-07-27 16:34:46.000000 sortingview-0.9.9/sortingview.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      108 2022-07-27 16:34:46.000000 sortingview-0.9.9/sortingview.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       12 2022-07-27 16:34:46.000000 sortingview-0.9.9/sortingview.egg-info/top_level.txt
```

### Comparing `sortingview-0.9.8/LICENSE` & `sortingview-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/PKG-INFO` & `sortingview-0.9.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortingview
-Version: 0.9.8
+Version: 0.9.9
 Summary: Web app for viewing results of ephys spike sorting
 Home-page: https://github.com/magland/sortingview
 Author: Jeremy Magland and Jeff Soules
 Author-email: jmagland@flatironinstitute.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/magland/sortingview/issues
 Platform: UNKNOWN
```

### Comparing `sortingview-0.9.8/README.md` & `sortingview-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/setup.cfg` & `sortingview-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sortingview
-version = 0.9.8
+version = 0.9.9
 author = Jeremy Magland and Jeff Soules
 author_email = jmagland@flatironinstitute.org
 description = Web app for viewing results of ephys spike sorting
 url = https://github.com/magland/sortingview
 include_package_data = True
 project_urls = 
 	Bug Tracker = https://github.com/magland/sortingview/issues
```

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/Figure.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/Figure.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/MultiTimeseries.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/MultiTimeseries.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/SpikeSortingView.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/SpikeSortingView.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/__init__.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/__init__.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_autocorrelograms_view.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_autocorrelograms_view.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_average_waveforms_view.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_average_waveforms_view.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_autocorrelograms.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_average_waveforms.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_average_waveforms.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_electrode_geometry.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_electrode_geometry.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_live_cross_correlograms.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_live_cross_correlograms.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_mountain_layout.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_mountain_layout.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_raster_plot.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_raster_plot.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_spike_amplitudes.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_spike_amplitudes.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_summary.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_summary.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_create_units_table.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_create_units_table.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_cross_correlograms_view.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_cross_correlograms_view.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_raster_plot_view.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_raster_plot_view.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_sorting_summary_view.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_sorting_summary_view.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_spike_amplitudes_view.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_spike_amplitudes_view.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/_units_table_view.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/_units_table_view.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/create_position_pdf_plot.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/create_position_pdf_plot.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/create_position_plot.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/create_position_plot.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/create_spike_raster_plot.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/create_spike_raster_plot.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/helpers/compute_correlogram_data.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/helpers/compute_correlogram_data.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/SpikeSortingView/prepare_spikesortingview_data.py` & `sortingview-0.9.9/sortingview/SpikeSortingView/prepare_spikesortingview_data.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/__init__.py` & `sortingview-0.9.9/sortingview/__init__.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/backend/compute_correlogram_data.py` & `sortingview-0.9.9/sortingview/backend/compute_correlogram_data.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/backend/start_backend.py` & `sortingview-0.9.9/sortingview/backend/start_backend.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/MdaRecordingExtractorV2/MdaRecordingExtractorV2.py` & `sortingview-0.9.9/sortingview/load_extractors/MdaRecordingExtractorV2/MdaRecordingExtractorV2.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/binextractors/bin1recordingextractor.py` & `sortingview-0.9.9/sortingview/load_extractors/binextractors/bin1recordingextractor.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/binextractors/bin2recordingextractor.py` & `sortingview-0.9.9/sortingview/load_extractors/binextractors/bin2recordingextractor.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/copy_recording_extractor.py` & `sortingview-0.9.9/sortingview/load_extractors/copy_recording_extractor.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/copy_sorting_extractor.py` & `sortingview-0.9.9/sortingview/load_extractors/copy_sorting_extractor.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/get_recording_object.py` & `sortingview-0.9.9/sortingview/load_extractors/get_recording_object.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/get_sorting_object.py` & `sortingview-0.9.9/sortingview/load_extractors/get_sorting_object.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/TimeseriesModel_Hdf5.py` & `sortingview-0.9.9/sortingview/load_extractors/h5extractors/TimeseriesModel_Hdf5/TimeseriesModel_Hdf5.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/h5extractors/h5recordingextractorv1.py` & `sortingview-0.9.9/sortingview/load_extractors/h5extractors/h5recordingextractorv1.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/load_recording_extractor.py` & `sortingview-0.9.9/sortingview/load_extractors/load_recording_extractor.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/load_sorting_extractor.py` & `sortingview-0.9.9/sortingview/load_extractors/load_sorting_extractor.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/load_extractors/mdaio.py` & `sortingview-0.9.9/sortingview/load_extractors/mdaio.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/Autocorrelograms.py` & `sortingview-0.9.9/sortingview/views/Autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/AverageWaveforms.py` & `sortingview-0.9.9/sortingview/views/AverageWaveforms.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/Box.py` & `sortingview-0.9.9/sortingview/views/Box.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/CrossCorrelograms.py` & `sortingview-0.9.9/sortingview/views/CrossCorrelograms.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/ElectrodeGeometry.py` & `sortingview-0.9.9/sortingview/views/ElectrodeGeometry.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/LayoutItem.py` & `sortingview-0.9.9/sortingview/views/LayoutItem.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/MountainLayout.py` & `sortingview-0.9.9/sortingview/views/MountainLayout.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/RasterPlot.py` & `sortingview-0.9.9/sortingview/views/RasterPlot.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/SortingSummary.py` & `sortingview-0.9.9/sortingview/views/SortingSummary.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/SpikeAmplitudes.py` & `sortingview-0.9.9/sortingview/views/SpikeAmplitudes.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/Splitter.py` & `sortingview-0.9.9/sortingview/views/Splitter.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/TabLayout.py` & `sortingview-0.9.9/sortingview/views/TabLayout.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/TiledImage.py` & `sortingview-0.9.9/sortingview/views/TiledImage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from concurrent.futures import ThreadPoolExecutor
 import os
-from typing import List, Union
+from typing import Any, List, Union
 import numpy as np
-import pyvips
 import kachery_cloud as kcl
 from .View import View
 
 
 class TiledImageLayer:
-    def __init__(self, label: str, data: Union[np.array, pyvips.Image]) -> None:
+    def __init__(self, label: str, data: Union[np.array, Any]) -> None:
+        import pyvips
         self.label = label
         self.data=data
         if isinstance(data, pyvips.Image):
             image: pyvips.Image = data
         else:
             assert data.dtype == np.uint8, 'Data must be of type uint8'
             image: pyvips.Image = pyvips.Image.new_from_array(data)
@@ -22,14 +22,15 @@
 class TiledImage(View):
     def __init__(self, *, tile_size: int, layers: List[TiledImageLayer]) -> None:
         super().__init__('TiledImage')
         self._tile_size = tile_size
         self._layers = layers
 
     def to_dict(self) -> dict:
+        import pyvips
         data = {
             'type': self.type,
             'layers': []
         }
         for L in self._layers:
             layer_label: str = L.label
             image: pyvips.Image = L.image
```

### Comparing `sortingview-0.9.8/sortingview/views/UnitLocations.py` & `sortingview-0.9.9/sortingview/views/UnitLocations.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/UnitMetricsGraph.py` & `sortingview-0.9.9/sortingview/views/UnitMetricsGraph.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/UnitSimilarityMatrix.py` & `sortingview-0.9.9/sortingview/views/UnitSimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/UnitsTable.py` & `sortingview-0.9.9/sortingview/views/UnitsTable.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/View.py` & `sortingview-0.9.9/sortingview/views/View.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/views/__init__.py` & `sortingview-0.9.9/sortingview/views/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,7 +14,9 @@
 from .ElectrodeGeometry import ElectrodeGeometry
 from .SpikeAmplitudes import SpikeAmplitudes, SpikeAmplitudesItem
 from .UnitLocations import UnitLocations, UnitLocationsItem
 from .Markdown import Markdown
 from .TabLayout import TabLayoutItem, TabLayout
 from .UnitMetricsGraph import UnitMetricsGraphMetric, UnitMetricsGraphUnit, UnitMetricsGraph
 from .TiledImage import TiledImage, TiledImageLayer
+from .SortingCuration2 import SortingCuration2
+from .SortingSelection import SortingSelection
```

### Comparing `sortingview-0.9.8/sortingview/views/franklab/TrackPositionAnimationV1.py` & `sortingview-0.9.9/sortingview/views/franklab/TrackPositionAnimationV1.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/workspace/Workspace.py` & `sortingview-0.9.9/sortingview/workspace/Workspace.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/workspace/_get_sorting_curation.py` & `sortingview-0.9.9/sortingview/workspace/_get_sorting_curation.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/workspace/_old_workspace.py` & `sortingview-0.9.9/sortingview/workspace/_old_workspace.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview/workspace/_spikesortingview.py` & `sortingview-0.9.9/sortingview/workspace/_spikesortingview.py`

 * *Files identical despite different names*

### Comparing `sortingview-0.9.8/sortingview.egg-info/PKG-INFO` & `sortingview-0.9.9/sortingview.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortingview
-Version: 0.9.8
+Version: 0.9.9
 Summary: Web app for viewing results of ephys spike sorting
 Home-page: https://github.com/magland/sortingview
 Author: Jeremy Magland and Jeff Soules
 Author-email: jmagland@flatironinstitute.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/magland/sortingview/issues
 Platform: UNKNOWN
```

### Comparing `sortingview-0.9.8/sortingview.egg-info/SOURCES.txt` & `sortingview-0.9.9/sortingview.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 sortingview/views/CrossCorrelograms.py
 sortingview/views/ElectrodeGeometry.py
 sortingview/views/LayoutItem.py
 sortingview/views/Markdown.py
 sortingview/views/MountainLayout.py
 sortingview/views/RasterPlot.py
 sortingview/views/SortingCuration.py
+sortingview/views/SortingCuration2.py
+sortingview/views/SortingSelection.py
 sortingview/views/SortingSummary.py
 sortingview/views/SpikeAmplitudes.py
 sortingview/views/Splitter.py
 sortingview/views/TabLayout.py
 sortingview/views/TiledImage.py
 sortingview/views/UnitLocations.py
 sortingview/views/UnitMetricsGraph.py
```

