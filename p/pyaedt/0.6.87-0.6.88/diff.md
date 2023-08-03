# Comparing `tmp/pyaedt-0.6.87.tar.gz` & `tmp/pyaedt-0.6.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.87.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.88.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.87.tar` & `pyaedt-0.6.88.tar`

### file list

```diff
@@ -1,259 +1,259 @@
--rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.87/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.87/README.md
--rw-r--r--   0        0        0     2629 2023-07-27 16:00:23.701424 pyaedt-0.6.87/pyaedt/__init__.py
--rw-r--r--   0        0        0    26756 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.87/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88967 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    50696 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17066 2023-06-20 15:35:24.349674 pyaedt-0.6.87/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.87/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19948 2023-07-19 13:20:21.575376 pyaedt-0.6.87/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.87/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   136452 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75793 2023-07-20 11:48:09.458225 pyaedt-0.6.87/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36750 2023-06-29 09:15:20.741006 pyaedt-0.6.87/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62949 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/circuit.py
--rw-r--r--   0        0        0    10259 2023-07-20 07:33:55.805436 pyaedt-0.6.87/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    84793 2023-07-25 17:51:34.650594 pyaedt-0.6.87/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1086 2023-06-28 08:36:59.983528 pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    24188 2023-07-24 13:10:38.761320 pyaedt-0.6.87/pyaedt/downloads.py
--rw-r--r--   0        0        0   138814 2023-07-27 13:09:33.142710 pyaedt-0.6.87/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    98725 2023-07-25 16:50:25.973900 pyaedt-0.6.87/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.87/pyaedt/edb_core/dotnet/__init__.py
--rw-r--r--   0        0        0    31509 2023-07-20 07:33:55.805436 pyaedt-0.6.87/pyaedt/edb_core/dotnet/database.py
--rw-r--r--   0        0        0     7909 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/dotnet/layout.py
--rw-r--r--   0        0        0    48515 2023-07-27 16:00:23.701424 pyaedt-0.6.87/pyaedt/edb_core/dotnet/primitive.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    33195 2023-06-12 08:05:31.703949 pyaedt-0.6.87/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    48709 2023-07-25 15:37:16.573778 pyaedt-0.6.87/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.87/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20820 2023-07-17 10:14:12.806355 pyaedt-0.6.87/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     6115 2023-07-24 13:10:38.761320 pyaedt-0.6.87/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    64588 2023-07-25 16:50:25.973900 pyaedt-0.6.87/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32640 2023-07-27 16:00:23.701424 pyaedt-0.6.87/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0   102353 2023-07-27 07:25:08.069862 pyaedt-0.6.87/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    34944 2023-07-10 08:39:13.777984 pyaedt-0.6.87/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.87/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.87/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    68725 2023-06-29 11:46:59.997639 pyaedt-0.6.87/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    47176 2023-06-22 08:21:07.514633 pyaedt-0.6.87/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    47963 2023-07-25 15:36:36.553810 pyaedt-0.6.87/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    50376 2023-07-25 16:50:25.973900 pyaedt-0.6.87/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    58809 2023-06-19 10:47:11.266974 pyaedt-0.6.87/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   111074 2023-07-17 10:14:12.806355 pyaedt-0.6.87/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11500 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/emit.py
--rw-r--r--   0        0        0     6100 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     2825 2023-07-20 07:33:55.805436 pyaedt-0.6.87/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     1621 2023-06-13 17:56:07.965688 pyaedt-0.6.87/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0    11102 2023-07-24 13:10:38.761320 pyaedt-0.6.87/pyaedt/emit_core/interference_classification.py
--rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    13896 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    12252 2023-06-21 12:50:18.007016 pyaedt-0.6.87/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-30 06:59:39.580847 pyaedt-0.6.87/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83443 2023-07-20 11:48:09.458225 pyaedt-0.6.87/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3442 2023-07-13 12:00:19.155166 pyaedt-0.6.87/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    71208 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0     9410 2023-07-20 12:33:36.682607 pyaedt-0.6.87/pyaedt/generic/grpc_plugin.py
--rw-r--r--   0        0        0     3043 2023-07-11 14:47:17.448018 pyaedt-0.6.87/pyaedt/generic/grpc_plugin_dll.py
--rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     7029 2023-07-13 12:00:19.155166 pyaedt-0.6.87/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11405 2023-06-22 08:21:07.514633 pyaedt-0.6.87/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3536 2023-06-21 12:50:18.007016 pyaedt-0.6.87/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.87/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   255524 2023-07-27 13:09:33.142710 pyaedt-0.6.87/pyaedt/hfss.py
--rw-r--r--   0        0        0    84753 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   202984 2023-07-26 12:52:26.502860 pyaedt-0.6.87/pyaedt/icepak.py
--rw-r--r--   0        0        0   127831 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24372 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3972 2023-07-07 09:12:05.234128 pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     3311 2023-07-07 09:12:05.234128 pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     2620 2023-07-05 06:36:09.681010 pyaedt-0.6.87/pyaedt/misc/ansys_cloud.areg
--rw-r--r--   0        0        0     3731 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     5611 2023-07-07 06:30:25.350901 pyaedt-0.6.87/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.87/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-07-25 17:51:34.666219 pyaedt-0.6.87/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120896 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   207873 2023-07-26 13:34:42.288190 pyaedt-0.6.87/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116735 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11407 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   129702 2023-07-13 12:00:19.170793 pyaedt-0.6.87/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.87/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    39728 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49188 2023-07-26 12:52:26.518490 pyaedt-0.6.87/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59316 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53078 2023-07-11 14:47:17.463644 pyaedt-0.6.87/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12661 2023-07-19 13:20:21.575376 pyaedt-0.6.87/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    43135 2023-07-14 12:01:50.451661 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    33551 2023-07-06 12:50:33.852654 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8236 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    64284 2023-07-27 13:36:54.705176 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15185 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31781 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6956 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    65138 2023-07-18 12:25:32.970625 pyaedt-0.6.87/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    33041 2023-07-26 07:08:37.800116 pyaedt-0.6.87/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    50049 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65907 2023-07-26 07:08:37.800116 pyaedt-0.6.87/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23473 2023-07-26 07:08:37.800116 pyaedt-0.6.87/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    34537 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   159025 2023-07-18 12:25:32.970625 pyaedt-0.6.87/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71535 2023-06-21 12:50:18.022631 pyaedt-0.6.87/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.87/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28440 2023-07-11 14:47:17.463644 pyaedt-0.6.87/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53543 2023-07-13 12:00:19.186418 pyaedt-0.6.87/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11976 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    27635 2023-06-26 14:19:11.175189 pyaedt-0.6.87/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   181969 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64120 2023-06-29 09:15:20.756674 pyaedt-0.6.87/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   121445 2023-06-15 12:26:55.582508 pyaedt-0.6.87/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    30706 2023-06-26 13:01:22.142566 pyaedt-0.6.87/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.87/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   126124 2023-06-23 15:25:31.221272 pyaedt-0.6.87/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95976 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/q3d.py
--rw-r--r--   0        0        0    10581 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.87/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.87/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-07-25 17:51:34.681847 pyaedt-0.6.87/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4650 2023-07-26 06:46:58.468961 pyaedt-0.6.87/pyproject.toml
--rw-r--r--   0        0        0    15890 1970-01-01 00:00:00.000000 pyaedt-0.6.87/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-30 06:59:37.486926 pyaedt-0.6.88/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-30 06:59:37.486926 pyaedt-0.6.88/README.md
+-rw-r--r--   0        0        0     2629 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/__init__.py
+-rw-r--r--   0        0        0    27137 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-30 06:59:39.408947 pyaedt-0.6.88/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88876 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    50696 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    16977 2023-08-03 12:17:24.267142 pyaedt-0.6.88/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-30 06:59:39.408947 pyaedt-0.6.88/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19948 2023-07-19 13:20:21.575376 pyaedt-0.6.88/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-30 06:59:39.408947 pyaedt-0.6.88/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-30 06:59:39.424579 pyaedt-0.6.88/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   136349 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-30 06:59:39.424579 pyaedt-0.6.88/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75793 2023-07-20 11:48:09.458225 pyaedt-0.6.88/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.424579 pyaedt-0.6.88/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-30 06:59:39.424579 pyaedt-0.6.88/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36750 2023-06-29 09:15:20.741006 pyaedt-0.6.88/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62949 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10259 2023-07-20 07:33:55.805436 pyaedt-0.6.88/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    85232 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-30 06:59:39.424579 pyaedt-0.6.88/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-30 06:59:39.424579 pyaedt-0.6.88/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1086 2023-06-28 08:36:59.983528 pyaedt-0.6.88/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-30 06:59:39.424579 pyaedt-0.6.88/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-30 06:59:39.440208 pyaedt-0.6.88/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-30 06:59:39.440208 pyaedt-0.6.88/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-30 06:59:39.440208 pyaedt-0.6.88/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-30 06:59:39.440208 pyaedt-0.6.88/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-30 06:59:39.455836 pyaedt-0.6.88/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-30 06:59:39.455836 pyaedt-0.6.88/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-30 06:59:39.455836 pyaedt-0.6.88/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-30 06:59:39.471459 pyaedt-0.6.88/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-30 06:59:39.471459 pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-30 06:59:39.471459 pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-30 06:59:39.487088 pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-30 06:59:39.502713 pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-30 06:59:39.502713 pyaedt-0.6.88/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-30 06:59:39.518353 pyaedt-0.6.88/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-30 06:59:39.518353 pyaedt-0.6.88/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-30 06:59:39.533962 pyaedt-0.6.88/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    24188 2023-07-24 13:10:38.761320 pyaedt-0.6.88/pyaedt/downloads.py
+-rw-r--r--   0        0        0   140135 2023-08-03 12:17:24.282759 pyaedt-0.6.88/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-08-02 11:17:34.959569 pyaedt-0.6.88/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    98725 2023-07-25 16:50:25.973900 pyaedt-0.6.88/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-06-05 09:36:43.922575 pyaedt-0.6.88/pyaedt/edb_core/dotnet/__init__.py
+-rw-r--r--   0        0        0    36340 2023-08-03 08:36:08.250921 pyaedt-0.6.88/pyaedt/edb_core/dotnet/database.py
+-rw-r--r--   0        0        0     7970 2023-08-03 08:36:08.266548 pyaedt-0.6.88/pyaedt/edb_core/dotnet/layout.py
+-rw-r--r--   0        0        0    48515 2023-07-27 16:00:23.701424 pyaedt-0.6.88/pyaedt/edb_core/dotnet/primitive.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.533962 pyaedt-0.6.88/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    33195 2023-06-12 08:05:31.703949 pyaedt-0.6.88/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    48709 2023-07-25 15:37:16.573778 pyaedt-0.6.88/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-30 06:59:39.533962 pyaedt-0.6.88/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      867 2023-05-30 06:59:39.533962 pyaedt-0.6.88/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12243 2023-06-05 09:36:43.938202 pyaedt-0.6.88/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65661 2023-06-05 09:36:43.938202 pyaedt-0.6.88/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20820 2023-07-17 10:14:12.806355 pyaedt-0.6.88/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     8149 2023-08-03 08:36:08.266548 pyaedt-0.6.88/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    64588 2023-07-25 16:50:25.973900 pyaedt-0.6.88/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32640 2023-07-27 16:00:23.701424 pyaedt-0.6.88/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0   101982 2023-07-31 14:33:58.459236 pyaedt-0.6.88/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36324 2023-06-05 09:36:43.938202 pyaedt-0.6.88/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    34944 2023-07-10 08:39:13.777984 pyaedt-0.6.88/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     3923 2023-06-05 14:54:59.781956 pyaedt-0.6.88/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2432 2023-06-05 09:36:43.938202 pyaedt-0.6.88/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    68725 2023-06-29 11:46:59.997639 pyaedt-0.6.88/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-30 06:59:39.549589 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2850 2023-06-05 09:36:43.953828 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-30 06:59:39.565215 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-30 06:59:39.580847 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21800 2023-06-05 09:36:43.953828 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-30 06:59:39.580847 pyaedt-0.6.88/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47176 2023-06-22 08:21:07.514633 pyaedt-0.6.88/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33310 2023-06-05 09:36:43.953828 pyaedt-0.6.88/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0     6183 2023-08-03 08:36:08.266548 pyaedt-0.6.88/pyaedt/edb_core/net_class.py
+-rw-r--r--   0        0        0    48206 2023-08-03 08:36:08.266548 pyaedt-0.6.88/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    50376 2023-07-25 16:50:25.973900 pyaedt-0.6.88/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    58809 2023-06-19 10:47:11.266974 pyaedt-0.6.88/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   111074 2023-07-17 10:14:12.806355 pyaedt-0.6.88/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11500 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/emit.py
+-rw-r--r--   0        0        0     6100 2023-07-06 12:50:33.852654 pyaedt-0.6.88/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3762 2023-08-03 08:20:26.796096 pyaedt-0.6.88/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     2616 2023-08-03 15:52:33.149114 pyaedt-0.6.88/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0        2 2023-05-30 06:59:39.580847 pyaedt-0.6.88/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-07-06 12:50:33.852654 pyaedt-0.6.88/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    27656 2023-08-03 08:20:26.796096 pyaedt-0.6.88/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-30 06:59:39.580847 pyaedt-0.6.88/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    12252 2023-06-21 12:50:18.007016 pyaedt-0.6.88/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.580847 pyaedt-0.6.88/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3285 2023-07-31 12:42:50.939958 pyaedt-0.6.88/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83443 2023-07-20 11:48:09.458225 pyaedt-0.6.88/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3442 2023-07-13 12:00:19.155166 pyaedt-0.6.88/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    71265 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0     9410 2023-07-20 12:33:36.682607 pyaedt-0.6.88/pyaedt/generic/grpc_plugin.py
+-rw-r--r--   0        0        0     3043 2023-07-11 14:47:17.448018 pyaedt-0.6.88/pyaedt/generic/grpc_plugin_dll.py
+-rw-r--r--   0        0        0    25808 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     7029 2023-07-13 12:00:19.155166 pyaedt-0.6.88/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11405 2023-06-22 08:21:07.514633 pyaedt-0.6.88/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3536 2023-06-21 12:50:18.007016 pyaedt-0.6.88/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-30 06:59:39.596468 pyaedt-0.6.88/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   255524 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/hfss.py
+-rw-r--r--   0        0        0    84753 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   202973 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/icepak.py
+-rw-r--r--   0        0        0   132896 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24372 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3972 2023-07-07 09:12:05.234128 pyaedt-0.6.88/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     3311 2023-07-07 09:12:05.234128 pyaedt-0.6.88/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2620 2023-07-05 06:36:09.681010 pyaedt-0.6.88/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     3731 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     5611 2023-07-07 06:30:25.350901 pyaedt-0.6.88/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-30 06:59:39.612097 pyaedt-0.6.88/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-08-03 15:52:33.164739 pyaedt-0.6.88/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-30 06:59:39.627726 pyaedt-0.6.88/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-30 06:59:39.643351 pyaedt-0.6.88/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120896 2023-07-13 12:00:19.170793 pyaedt-0.6.88/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   207873 2023-07-26 13:34:42.288190 pyaedt-0.6.88/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116735 2023-07-13 12:00:19.170793 pyaedt-0.6.88/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11407 2023-07-13 12:00:19.170793 pyaedt-0.6.88/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   129702 2023-07-13 12:00:19.170793 pyaedt-0.6.88/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.643351 pyaedt-0.6.88/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    39728 2023-08-03 15:52:33.180368 pyaedt-0.6.88/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49188 2023-07-26 12:52:26.518490 pyaedt-0.6.88/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59316 2023-08-03 15:52:33.180368 pyaedt-0.6.88/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53078 2023-07-11 14:47:17.463644 pyaedt-0.6.88/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12661 2023-07-19 13:20:21.575376 pyaedt-0.6.88/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    43135 2023-07-14 12:01:50.451661 pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    33551 2023-07-06 12:50:33.852654 pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8236 2023-07-13 12:00:19.186418 pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    64284 2023-07-27 13:36:54.705176 pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15185 2023-07-13 12:00:19.186418 pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.88/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31781 2023-08-03 15:52:33.180368 pyaedt-0.6.88/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-30 06:59:39.658979 pyaedt-0.6.88/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     7133 2023-08-03 12:17:24.298386 pyaedt-0.6.88/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    65260 2023-08-03 12:17:24.298386 pyaedt-0.6.88/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    33041 2023-07-26 07:08:37.800116 pyaedt-0.6.88/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    50212 2023-08-03 15:52:33.180368 pyaedt-0.6.88/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.658979 pyaedt-0.6.88/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65907 2023-07-26 07:08:37.800116 pyaedt-0.6.88/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23880 2023-08-03 12:17:24.298386 pyaedt-0.6.88/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    34851 2023-08-01 10:10:40.663885 pyaedt-0.6.88/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   159025 2023-07-18 12:25:32.970625 pyaedt-0.6.88/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71535 2023-06-21 12:50:18.022631 pyaedt-0.6.88/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-30 06:59:39.658979 pyaedt-0.6.88/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-30 06:59:39.658979 pyaedt-0.6.88/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-30 06:59:39.674599 pyaedt-0.6.88/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-30 06:59:39.674599 pyaedt-0.6.88/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28511 2023-08-03 12:17:24.298386 pyaedt-0.6.88/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53644 2023-08-03 12:17:24.298386 pyaedt-0.6.88/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    12063 2023-08-03 12:17:24.298386 pyaedt-0.6.88/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    27635 2023-06-26 14:19:11.175189 pyaedt-0.6.88/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-30 06:59:39.674599 pyaedt-0.6.88/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   182940 2023-08-03 15:52:33.180368 pyaedt-0.6.88/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64120 2023-06-29 09:15:20.756674 pyaedt-0.6.88/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   121445 2023-06-15 12:26:55.582508 pyaedt-0.6.88/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-30 06:59:39.674599 pyaedt-0.6.88/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.674599 pyaedt-0.6.88/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    30706 2023-06-26 13:01:22.142566 pyaedt-0.6.88/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-30 06:59:39.674599 pyaedt-0.6.88/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   126124 2023-06-23 15:25:31.221272 pyaedt-0.6.88/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95976 2023-08-03 15:52:33.196059 pyaedt-0.6.88/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-08-03 15:52:33.196059 pyaedt-0.6.88/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-30 06:59:39.690227 pyaedt-0.6.88/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10410 2023-06-05 09:36:43.953828 pyaedt-0.6.88/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-08-03 15:52:33.196059 pyaedt-0.6.88/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4651 2023-08-03 15:52:33.196059 pyaedt-0.6.88/pyproject.toml
+-rw-r--r--   0        0        0    15891 1970-01-01 00:00:00.000000 pyaedt-0.6.88/PKG-INFO
```

### Comparing `pyaedt-0.6.87/LICENSE` & `pyaedt-0.6.88/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/README.md` & `pyaedt-0.6.88/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/__init__.py` & `pyaedt-0.6.88/pyaedt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.87"
+__version__ = "0.6.88"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
```

### Comparing `pyaedt-0.6.87/pyaedt/aedt_logger.py` & `pyaedt-0.6.88/pyaedt/aedt_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,30 +119,30 @@
     filename : str, optional
         Name of the file to write messages to. The default is ``None``.
     to_stdout : bool, optional
         Whether to write log messages to stdout. The default is ``False``.
     """
 
     def __init__(self, level=logging.DEBUG, filename=None, to_stdout=False):
+        self._std_out_handler = None
+        self._files_handlers = []
         self.level = level
         self.filename = filename or settings.logger_file_path
         settings.logger_file_path = self.filename
 
         self._global = logging.getLogger("Global")
         if not settings.enable_logger:
             self._global.addHandler(logging.NullHandler())
             return
 
-        self._files_handlers = []
         self._projects = {}
 
         self._global.setLevel(level)
         self._global.addFilter(AppFilter())
 
-        self._std_out_handler = None
         if settings.formatter:
             self.formatter = settings.formatter
         else:
             self.formatter = logging.Formatter(settings.logger_formatter, datefmt=settings.logger_datefmt)
         global_handler = False
         if settings.enable_global_log_file:
             for handler in self._global.handlers:
@@ -583,68 +583,74 @@
             return self._design
         else:
             raise ValueError("The destination must be either 'Project' or 'Design'.")
 
     def disable_desktop_log(self):
         """Disable the log in AEDT."""
         self._log_on_desktop = False
+        self.info("Log on Desktop Message Manager is disabled")
 
     def enable_desktop_log(self):
         """Enable the log in AEDT."""
         self._log_on_desktop = True
+        self.info("Log on Desktop Message Manager is enabled")
 
     def disable_stdout_log(self):
         """Disable printing log messages to stdout."""
         self._log_on_screen = False
         self._global.removeHandler(self._std_out_handler)
-        self.info("StdOut has been disabled")
+        self.info("StdOut is disabled")
 
     def enable_stdout_log(self):
         """Enable printing log messages to stdout."""
         self._log_on_screen = True
         if not self._std_out_handler:
             self._std_out_handler = logging.StreamHandler(sys.stdout)
             self._std_out_handler.setLevel(self.level)
             _logger_stdout_formatter = logging.Formatter("pyaedt %(levelname)s: %(message)s")
 
             self._std_out_handler.setFormatter(_logger_stdout_formatter)
             self._global.addHandler(self._std_out_handler)
         self._global.addHandler(self._std_out_handler)
-        self.info("StdOut has been enabled")
+        self.info("StdOut is enabled")
 
     def disable_log_on_file(self):
         """Disable writing log messages to an output file."""
         self._log_on_file = False
         for _file_handler in self._files_handlers:
             _file_handler.close()
             self._global.removeHandler(_file_handler)
-        self.info("Log on file has been disabled")
+        self.info("Log on file is disabled")
 
     def enable_log_on_file(self):
         """Enable writing log messages to an output file."""
         self._log_on_file = True
         for _file_handler in self._files_handlers:
             self._global.addHandler(_file_handler)
-        self.info("Log on file has been enabled")
+        self.info("Log on file is enabled")
 
     def info(self, msg, *args, **kwargs):
         """Write an info message to the global logger."""
+        if not settings.enable_logger:
+            return
         if args:
             try:
                 msg1 = msg % tuple(str(i) for i in args)
             except TypeError:
                 msg1 = msg
         else:
             msg1 = msg
         self._log_on_dekstop(0, msg1, "Global")
         return self._log_on_handler(0, msg, *args, **kwargs)
 
     def info_timer(self, msg, start_time=None, *args, **kwargs):
         """Write an info message to the global logger with elapsed time.
         Message will have an appendix of type Elapsed time: time."""
+        if not settings.enable_logger:
+            return
         if not start_time:
             start_time = self._timer
         td = time.time() - start_time
         m, s = divmod(td, 60)
         h, m = divmod(m, 60)
         d, h = divmod(h, 24)
         if d > 0:
@@ -661,14 +667,16 @@
         else:
             msg1 = msg
         self._log_on_dekstop(0, msg1, "Global")
         return self._log_on_handler(0, msg, *args, **kwargs)
 
     def warning(self, msg, *args, **kwargs):
         """Write a warning message to the global logger."""
+        if not settings.enable_logger:
+            return
         if args:
             try:
                 msg1 = msg % tuple(str(i) for i in args)
             except TypeError:
                 msg1 = msg
         else:
             msg1 = msg
@@ -685,14 +693,16 @@
         else:
             msg1 = msg
         self._log_on_dekstop(2, msg1, "Global")
         return self._log_on_handler(2, msg, *args, **kwargs)
 
     def debug(self, msg, *args, **kwargs):
         """Write a debug message to the global logger."""
+        if not settings.enable_debug_logger or not settings.enable_logger:
+            return
         if args:
             try:
                 msg1 = msg % tuple(str(i) for i in args)
             except TypeError:
                 msg1 = msg
         else:
             msg1 = msg
```

### Comparing `pyaedt-0.6.87/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.88/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/Analysis.py` & `pyaedt-0.6.88/pyaedt/application/Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,22 +120,19 @@
             new_desktop_session,
             close_on_exit,
             student_version,
             machine,
             port,
             aedt_process_id,
         )
-        self.logger.info("Design Loaded")
         self._setup = None
         if setup_name:
             self.active_setup = setup_name
         self._materials = None
-        self.logger.info("Materials Loaded")
         self._available_variations = self.AvailableVariations(self)
-
         if self.design_type != "Maxwell Circuit":
             self.setups = [self.get_setup(setup_name) for setup_name in self.setup_names]
 
         self.parametrics = ParametricSetups(self)
         self.optimizations = OptimizationSetups(self)
         self._native_components = []
         self.SOLUTIONS = SOLUTIONS()
```

### Comparing `pyaedt-0.6.87/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.88/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.88/pyaedt/application/Analysis3DLayout.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,17 +84,15 @@
             new_desktop_session,
             close_on_exit,
             student_version,
             machine,
             port,
             aedt_process_id,
         )
-        self.logger.info("Analysis Loaded")
         self._modeler = None
-        self.logger.info("Modeler Loaded")
         self._mesh = None
         self._post = None
 
     @property
     def post(self):
         """PostProcessor.
```

### Comparing `pyaedt-0.6.87/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.88/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.88/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.88/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.88/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/Design.py` & `pyaedt-0.6.88/pyaedt/application/Design.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,24 +239,20 @@
         else:
             self.design_solutions = DesignSolution(None, design_type, self._aedt_version)
         self.design_solutions._solution_type = solution_type
         self._temp_solution_type = solution_type
         self.oproject = project_name
         self.odesign = design_name
         AedtObjects.__init__(self, is_inherithed=True)
-        self.logger.info("Aedt Objects initialized")
-
+        self.logger.info("Aedt Objects correctly read")
         if t:
             t.join()
-
         self._variable_manager = VariableManager(self)
         self._project_datasets = []
         self._design_datasets = []
-        # _mtime = self.project_time_stamp
-        self.logger.info("Variable Manager initialized")
 
     @property
     def desktop_class(self):
         """``Desktop`` class.
 
         Returns
         -------
```

### Comparing `pyaedt-0.6.87/pyaedt/application/JobManager.py` & `pyaedt-0.6.88/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/Variables.py` & `pyaedt-0.6.88/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.88/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/application/design_solutions.py` & `pyaedt-0.6.88/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/circuit.py` & `pyaedt-0.6.88/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/common_rpc.py` & `pyaedt-0.6.88/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/desktop.py` & `pyaedt-0.6.88/pyaedt/desktop.py`

 * *Files 5% similar despite different names*

```diff
@@ -354,21 +354,21 @@
                 i += 1
         except:
             logger.warning("No COM UTIL. Closing AEDT....")
         try:
             del Module.pyaedt_initialized
         except:
             pass
+        successfully_closed = False
         try:
             os.kill(pid, 9)
             del Module.oDesktop
             successfully_closed = True
         except:
             pyaedt_logger.error("Something went wrong in closing AEDT.")
-            successfully_closed = False
         finally:
             log = logging.getLogger("Global")
             handlers = log.handlers[:]
             for handler in handlers:
                 handler.close()
                 log.removeHandler(handler)
             return successfully_closed
@@ -496,14 +496,15 @@
         student_version=False,
         machine="",
         port=0,
         aedt_process_id=None,
     ):
         """Initialize desktop."""
         # used in unit test
+        self.launched_by_pyaedt = False
         if os.getenv("PYAEDT_NON_GRAPHICAL", "False").lower() in ("true", "1", "t"):
             non_graphical = os.getenv("PYAEDT_NON_GRAPHICAL", "False").lower() in ("true", "1", "t")
         # used in toolkit scripts
         if os.getenv("PYAEDT_SCRIPT_PROCESS_ID", None):
             print("found process id")
             aedt_process_id = int(os.getenv("PYAEDT_SCRIPT_PROCESS_ID"))
         if os.getenv("PYAEDT_SCRIPT_VERSION", None):
@@ -527,15 +528,26 @@
         self.logfile = None
 
         self._logger = pyaedt_logger
         if settings.enable_screen_logs:
             self._logger.enable_stdout_log()
         else:
             self._logger.disable_stdout_log()
-        self._logger.info("using existing logger.")
+        if settings.enable_file_logs:
+            self._logger.enable_log_on_file()
+        else:
+            self._logger.disable_log_on_file()
+        if settings.enable_desktop_logs and not non_graphical:
+            self._logger.enable_desktop_log()
+        else:
+            self._logger.disable_desktop_log()
+        if settings.enable_debug_logger:
+            self._logger.info("Debug logger is enabled. PyAEDT methods will be logged.")
+        else:
+            self._logger.info("Debug logger is disabled. PyAEDT methods will not be logged.")
 
         if "oDesktop" in dir():  # pragma: no cover
             self.release_on_exit = False
             self._main.oDesktop = oDesktop
             try:
                 settings.non_graphical = oDesktop.GetIsNonGraphical()
             except:
@@ -825,15 +837,15 @@
                 "PyAEDT supports COM initialization in Windows only. To use in Linux, upgrade to AEDT 2022 R2 or later."
             )
         base_path = self._main.sDesktopinstallDirectory
         sys.path.insert(0, base_path)
         sys.path.insert(0, os.path.join(base_path, "PythonFiles", "DesktopPlugin"))
         launch_msg = "AEDT installation Path {}.".format(base_path)
         self.logger.info(launch_msg)
-        self.logger.info("Launching AEDT with module PythonNET.")
+        self.logger.info("Launching AEDT with COM plugin using PythonNET.")
         processID = []
         if is_windows:
             processID = com_active_sessions(version, student_version, non_graphical)
         if student_version and not processID:  # Opens an instance if processID is an empty list
             self._run_student()
         elif non_graphical or new_aedt_session or not processID:
             # Force new object if no non-graphical instance is running or if there is not an already existing process.
@@ -889,41 +901,38 @@
 
             _clr.AddReference("Ansys.Ansoft.CoreCOMScripting")
             AnsoftCOMUtil = __import__("Ansys.Ansoft.CoreCOMScripting")
             self.COMUtil = AnsoftCOMUtil.Ansoft.CoreCOMScripting.Util.COMUtil
             self._main.COMUtil = self.COMUtil
             StandalonePyScriptWrapper = AnsoftCOMUtil.Ansoft.CoreCOMScripting.COM.StandalonePyScriptWrapper
             if non_graphical or new_session:
+                self.launched_by_pyaedt = True
                 return StandalonePyScriptWrapper.CreateObjectNew(non_graphical)
             else:
                 return StandalonePyScriptWrapper.CreateObject(version)
         else:
             base_path = self._main.sDesktopinstallDirectory
             sys.path.insert(0, base_path)
             sys.path.insert(0, os.path.join(base_path, "PythonFiles", "DesktopPlugin"))
             if is_linux:
-                if os.environ.get("LD_LIBRARY_PATH"):
-                    os.environ["LD_LIBRARY_PATH"] = (
-                        os.path.join(base_path, "defer") + os.pathsep + os.environ["LD_LIBRARY_PATH"]
-                    )
-                else:
-                    os.environ["LD_LIBRARY_PATH"] = os.path.join(base_path, "defer")
                 pyaedt_path = os.path.realpath(os.path.join(os.path.dirname(os.path.realpath(__file__)), ".."))
                 os.environ["PATH"] = pyaedt_path + os.pathsep + os.environ["PATH"]
             os.environ["DesktopPluginPyAEDT"] = os.path.join(
                 self._main.sDesktopinstallDirectory, "PythonFiles", "DesktopPlugin"
             )
             launch_msg = "AEDT installation Path {}".format(base_path)
             self.logger.info(launch_msg)
             import pyaedt.generic.grpc_plugin as StandalonePyScriptWrapper
 
+            if new_session:
+                self.launched_by_pyaedt = new_session
             return StandalonePyScriptWrapper.CreateAedtApplication(machine, port, non_graphical, new_session)
 
     def _init_cpython_new(self, non_graphical, new_aedt_session, version, student_version, version_key):
-        self.logger.info("Launching AEDT with the gRPC plugin.")
+        self.logger.info("Launching AEDT using the gRPC plugin.")
         if not self.machine or self.machine in [
             "localhost",
             "127.0.0.1",
             socket.getfqdn(),
             socket.getfqdn().split(".")[0],
         ]:
             self.machine = ""
@@ -974,23 +983,25 @@
         else:
             self.logger.info("AEDT session is starting on gRPC port %s", self.port)
             new_aedt_session = True
 
         if new_aedt_session and settings.use_lsf_scheduler and is_linux:  # pragma: no cover
             out, self.machine = launch_aedt_in_lsf(non_graphical, self.port)
             if out:
+                self.launched_by_pyaedt = True
                 oApp = self._initialize(is_grpc=True, machine=self.machine, port=self.port, new_session=False)
             else:
                 self.logger.error("Failed to start LSF job on machine: %s.", self.machine)
                 return
         elif new_aedt_session:
             installer = os.path.join(self._main.sDesktopinstallDirectory, "ansysedt")
             if not is_linux:
                 installer = os.path.join(self._main.sDesktopinstallDirectory, "ansysedt.exe")
             out, self.port = launch_aedt(installer, non_graphical, self.port)
+            self.launched_by_pyaedt = True
             oApp = self._initialize(
                 is_grpc=True, non_graphical=non_graphical, machine=self.machine, port=self.port, new_session=not out
             )
         else:
             oApp = self._initialize(
                 is_grpc=True,
                 non_graphical=non_graphical,
```

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.88/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/downloads.py` & `pyaedt-0.6.88/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb.py` & `pyaedt-0.6.88/pyaedt/edb.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 import tempfile
 import time
 import traceback
 import warnings
 
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
-from pyaedt.edb_core import Components
-from pyaedt.edb_core import EdbHfss
-from pyaedt.edb_core import EdbLayout
-from pyaedt.edb_core import EdbNets
-from pyaedt.edb_core import EdbSiwave
+from pyaedt.edb_core.components import Components
 from pyaedt.edb_core.dotnet.database import Database
 from pyaedt.edb_core.dotnet.layout import LayoutDotNet
 from pyaedt.edb_core.edb_data.control_file import ControlFile
 from pyaedt.edb_core.edb_data.control_file import convert_technology_file
 from pyaedt.edb_core.edb_data.design_options import EdbDesignOptions
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
 from pyaedt.edb_core.edb_data.hfss_simulation_setup_data import HfssSimulationSetup
@@ -33,17 +29,24 @@
 from pyaedt.edb_core.edb_data.sources import ExcitationPorts
 from pyaedt.edb_core.edb_data.sources import ExcitationProbes
 from pyaedt.edb_core.edb_data.sources import ExcitationSources
 from pyaedt.edb_core.edb_data.sources import SourceType
 from pyaedt.edb_core.edb_data.variables import Variable
 import pyaedt.edb_core.general
 from pyaedt.edb_core.general import convert_py_list_to_net_list
+from pyaedt.edb_core.hfss import EdbHfss
 from pyaedt.edb_core.ipc2581.ipc2581 import Ipc2581
+from pyaedt.edb_core.layout import EdbLayout
 from pyaedt.edb_core.materials import Materials
+from pyaedt.edb_core.net_class import EdbDifferentialPair
+from pyaedt.edb_core.net_class import EdbExtendedNets
+from pyaedt.edb_core.net_class import EdbNetClasses
+from pyaedt.edb_core.nets import EdbNets
 from pyaedt.edb_core.padstack import EdbPadstacks
+from pyaedt.edb_core.siwave import EdbSiwave
 from pyaedt.edb_core.stackup import Stackup
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SolverType
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
@@ -135,16 +138,15 @@
         isaedtowned=False,
         oproject=None,
         student_version=False,
         use_ppe=False,
         technology_file=None,
     ):
         self._clean_variables()
-
-        Database.__init__(self, edbversion, student_version)
+        Database.__init__(self, edbversion=edbversion, student_version=student_version)
         self.standalone = True
         self.oproject = oproject
         self._main = sys.modules["__main__"]
         self.edbversion = edbversion
         self.isaedtowned = isaedtowned
         self.isreadonly = isreadonly
         self.cellname = cellname
@@ -187,22 +189,22 @@
             if settings.enable_local_log_file and self.log_name:
                 self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
             self.open_edb()
         elif not os.path.exists(os.path.join(self.edbpath, "edb.def")):
             self.create_edb()
             if settings.enable_local_log_file and self.log_name:
                 self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
-            self.logger.info("EDB %s was created correctly.", self.edbpath)
+            self.logger.info("EDB %s created correctly.", self.edbpath)
         elif ".aedb" in edbpath:
             self.edbpath = edbpath
             if settings.enable_local_log_file and self.log_name:
                 self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
             self.open_edb()
         if self.active_cell:
-            self.logger.info("EDB was initialized.")
+            self.logger.info("EDB initialized.")
         else:
             self.logger.info("Failed to initialize DLLs.")
 
     def __enter__(self):
         return self
 
     def __exit__(self, ex_type, ex_value, ex_traceback):
@@ -277,16 +279,14 @@
         self._siwave = EdbSiwave(self)
         self._hfss = EdbHfss(self)
         self._nets = EdbNets(self)
         self._core_primitives = EdbLayout(self)
         self._stackup2 = self._stackup
         self._materials = Materials(self)
 
-        self.logger.info("Objects Initialized")
-
     @property
     def cell_names(self):
         """Cell name container.
         Returns
         -------
         list of str, cell names.
         """
@@ -875,18 +875,67 @@
         """
 
         if not self._nets and self.active_db:
             self._nets = EdbNets(self)
         return self._nets
 
     @property
+    def net_classes(self):
+        """Get all net classes.
+
+        Returns
+        -------
+        :class:`pyaedt.edb_core.nets.EdbNetClasses`
+
+        Examples
+        --------
+        >>> edbapp = pyaedt.Edb("myproject.aedb")
+        >>> edbapp.net_classes
+        """
+
+        if self.active_db:
+            return EdbNetClasses(self)
+
+    @property
+    def extended_nets(self):
+        """Get all extended nets.
+
+        Returns
+        -------
+        :class:`pyaedt.edb_core.nets.EdbExtendedNets`
+
+        Examples
+        --------
+        >>> edbapp = pyaedt.Edb("myproject.aedb")
+        >>> edbapp.extended_nets
+        """
+
+        if self.active_db:
+            return EdbExtendedNets(self)
+
+    @property
+    def differential_pairs(self):
+        """Get all differential pairs.
+
+        Returns
+        -------
+        :class:`pyaedt.edb_core.nets.EdbDifferentialPairs`
+
+        Examples
+        --------
+        >>> edbapp = pyaedt.Edb("myproject.aedb")
+        >>> edbapp.differential_pairs
+        """
+        if self.active_db:
+            return EdbDifferentialPair(self)
+
+    @property
     def core_primitives(self):  # pragma: no cover
         """Core primitives.
 
-
         .. deprecated:: 0.6.62
            Use new property :func:`modeler` instead.
 
         Returns
         -------
         Instance of :class: `pyaedt.edb_core.layout.EdbLayout`
```

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/components.py` & `pyaedt-0.6.88/pyaedt/edb_core/components.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/dotnet/database.py` & `pyaedt-0.6.88/pyaedt/edb_core/dotnet/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import settings
 from pyaedt.misc import list_installed_ansysem
 
 
 class HierarchyDotNet:
+    """Hierarchy."""
+
     def __getattr__(self, key):
         try:
             return super().__getattribute__(key)
         except AttributeError:
             try:
                 return getattr(self._hierarchy, key)
             except AttributeError:
@@ -48,14 +50,16 @@
     @property
     def pin_group(self):
         """Edb Dotnet Api Database `Edb.Cell.Hierarchy.PinGroup`."""
         return self._hierarchy.PinGroup
 
 
 class PolygonDataDotNet:
+    """Polygon Data."""
+
     def __getattr__(self, key):  # pragma: no cover
         try:
             return super().__getattribute__(key)
         except AttributeError:
             try:
                 return getattr(self.dotnetobj, key)
             except AttributeError:
@@ -140,14 +144,16 @@
         """
         if isinstance(pdata, list):
             pdata = convert_py_list_to_net_list(pdata)
         return self.dotnetobj.GetConvexHullOfPolygons(pdata)
 
 
 class NetDotNet:
+    """Net Objects."""
+
     def __getattr__(self, key):
         try:
             return super().__getattribute__(key)
         except AttributeError:
             if self.net_obj and key in dir(self.net_obj):
                 obj = self.net_obj
             else:
@@ -170,15 +176,15 @@
         return self.net
 
     @property
     def api_object(self):
         """Return Ansys.Ansoft.Edb object."""
         return self.net_obj
 
-    def find_by_name(self, layout, net):
+    def find_by_name(self, layout, net):  # pragma: no cover
         """Edb Dotnet Api Database `Edb.Net.FindByName`."""
         return NetDotNet(self._app, self.net.FindByName(layout, net))
 
     def create(self, layout, name):
         """Edb Dotnet Api Database `Edb.Net.Create`."""
 
         return NetDotNet(self._app, self.net.Create(layout, name))
@@ -208,21 +214,149 @@
 
     @property
     def is_power_ground(self):
         """Edb Dotnet Api Database `Net.IsPowerGround()` and  `Net.SetIsPowerGround()`."""
         if self.net_obj:
             return self.net_obj.IsPowerGround()
 
+    @property
+    def _api_get_extended_net(self):
+        """The ExtendedNet this Net belongs to if it belongs to a ExtendedNet. If it doesn't belong to an ExtendedNet,
+        a null ExtendedNet is returned
+        """
+        return self.net_obj.GetExtendedNet()
+
     @is_power_ground.setter
     def is_power_ground(self, value):
         if self.net_obj:
             self.net_obj.SetIsPowerGround(value)
 
 
+class NetClassDotNet:
+    """Net Class."""
+
+    def __init__(self, app, api_object=None):
+        self.cell_net_class = app._edb.Cell.NetClass
+        self.api_object = api_object
+        self.edb_api = app._edb
+        self._app = app
+
+    @property
+    def api_nets(self):
+        """Return Edb Nets object dictionary."""
+        return {i.GetName(): i for i in list(self.api_object.Nets)}
+
+    def api_create(self, name):
+        """Edb Dotnet Api Database `Edb.NetClass.Create`."""
+        return NetClassDotNet(self._app, self.cell_net_class.Create(self._app.active_layout, name))
+
+    @property
+    def name(self):
+        """Edb Dotnet Api Database `NetClass.name` and  `NetClass.SetName()`."""
+        if self.api_object:
+            return self.api_object.GetName()
+
+    @name.setter
+    def name(self, value):
+        if self.api_object:
+            self.api_object.SetName(value)
+
+    def add_net(self, name):
+        """Add a new net.
+
+        Parameters
+        ----------
+        name : str
+            The name of the net to be added.
+
+        Returns
+        -------
+        object
+        """
+        if self.api_object:
+            edb_api_net = self.edb_api.Cell.Net.FindByName(self._app.active_layout, name)
+            return self.api_object.AddNet(edb_api_net)
+
+    def delete(self):  # pragma: no cover
+        """Edb Dotnet Api Database `Delete`."""
+
+        if self.api_object:
+            self.api_object.Delete()
+            self.api_object = None
+            return not self.api_object
+
+    @property
+    def is_null(self):
+        """Edb Dotnet Api Database `NetClass.IsNull()`."""
+        if self.api_object:
+            return self.api_object.IsNull()
+
+
+class ExtendedNetDotNet(NetClassDotNet):
+    """Extended net class."""
+
+    def __init__(self, app, api_object=None):
+        super().__init__(app, api_object)
+        self.cell_extended_net = app._edb.Cell.ExtendedNet
+
+    @property
+    def api_class(self):  # pragma: no cover
+        """Return Ansys.Ansoft.Edb class object."""
+        return self.cell_extended_net
+
+    def find_by_name(self, layout, net):  # pragma: no cover
+        """Edb Dotnet Api Database `Edb.ExtendedNet.FindByName`."""
+        return ExtendedNetDotNet(self._app, self.cell_extended_net.FindByName(layout, net))
+
+    def api_create(self, name):
+        """Edb Dotnet Api Database `Edb.ExtendedNet.Create`."""
+        return ExtendedNetDotNet(self._app, self.cell_extended_net.Create(self._app.active_layout, name))
+
+
+class DifferentialPairDotNet(NetClassDotNet):
+    """Differential Pairs."""
+
+    def __init__(self, app, api_object=None):
+        super().__init__(app, api_object)
+        self.cell_diff_pair = app._edb.Cell.DifferentialPair
+
+    @property
+    def api_class(self):  # pragma: no cover
+        """Return Ansys.Ansoft.Edb class object."""
+        return self.cell_diff_pair
+
+    def find_by_name(self, layout, net):  # pragma: no cover
+        """Edb Dotnet Api Database `Edb.DifferentialPair.FindByName`."""
+        return DifferentialPairDotNet(self._app, self.cell_diff_pair.FindByName(layout, net))
+
+    def api_create(self, name):
+        """Edb Dotnet Api Database `Edb.DifferentialPair.Create`."""
+        return DifferentialPairDotNet(self._app, self.cell_diff_pair.Create(self._app.active_layout, name))
+
+    def _api_set_differential_pair(self, net_name_p, net_name_n):
+        edb_api_net_p = self.edb_api.Cell.Net.FindByName(self._app.active_layout, net_name_p)
+        edb_api_net_n = self.edb_api.Cell.Net.FindByName(self._app.active_layout, net_name_n)
+        self.api_object.SetDifferentialPair(edb_api_net_p, edb_api_net_n)
+
+    @property
+    def api_positive_net(self):
+        """Edb Api Positive net object."""
+        if self.api_object:
+            return self.api_object.GetPositiveNet()
+
+    @property
+    def api_negative_net(self):
+        """Edb Api Negative net object."""
+        if self.api_object:
+            return self.api_object.GetNegativeNet()
+
+
 class CellClassDotNet:
+    """Cell Class."""
+
     def __getattr__(self, key):
         try:
             return super().__getattribute__(key)
         except AttributeError:
             try:
                 return getattr(self._cell, key)
             except AttributeError:
@@ -303,14 +437,16 @@
         """Edb Dotnet Api Database `Edb.Cell.Primitive`."""
         from pyaedt.edb_core.dotnet.primitive import PrimitiveDotNet
 
         return PrimitiveDotNet(self._app)
 
 
 class UtilityDotNet:
+    """Utility Edb class."""
+
     def __getattr__(self, key):
         try:
             return super().__getattribute__(key)
         except AttributeError:
             try:
                 return getattr(self.utility, key)
             except AttributeError:
@@ -349,14 +485,16 @@
             return self.utility.Value(value, var_server_cell)
         if set(val_decomposed).intersection(var_names):
             return self.utility.Value(value, var_server_db)
         return self.utility.Value(value)
 
 
 class GeometryDotNet:
+    """Geometry Edb Class."""
+
     def __getattr__(self, key):
         try:
             return super().__getattribute__(key)
         except AttributeError:
             try:
                 return getattr(self.geometry, key)
             except AttributeError:
@@ -435,14 +573,16 @@
         elif height:
             return self.geometry.ArcData(point1, point2, height)
         else:
             return self.geometry.ArcData(point1, point2)
 
 
 class CellDotNet:
+    """Cell Dot net."""
+
     def __getattr__(self, key):
         try:
             return super().__getattribute__(key)
         except AttributeError:
             try:
                 return getattr(self.edb_api, key)
             except AttributeError:
@@ -493,15 +633,17 @@
 
         Returns
         -------
         :class:`pyaedt.edb_core.dotnet.database.GeometryDotNet`"""
         return GeometryDotNet(self._app)
 
 
-class EdbDotNet:
+class EdbDotNet(object):
+    """Edb Dot Net Class."""
+
     def __init__(self, edbversion, student_version=False):
         self._global_logger = pyaedt_logger
         self._logger = pyaedt_logger
         if not edbversion:  # pragma: no cover
             try:
                 edbversion = "20{}.{}".format(list_installed_ansysem()[0][-3:-1], list_installed_ansysem()[0][-1:])
                 self._logger.info("Edb version " + edbversion)
@@ -509,15 +651,14 @@
                 raise Exception("No ANSYSEM_ROOTxxx is found.")
         self.edbversion = edbversion
         self.student_version = student_version
         """Initialize DLLs."""
         from pyaedt.generic.clr_module import _clr
         from pyaedt.generic.clr_module import edb_initialized
 
-        self.student_version = student_version
         if settings.enable_screen_logs:
             self.logger.enable_stdout_log()
         else:  # pragma: no cover
             self.logger.disable_stdout_log()
         if not edb_initialized:  # pragma: no cover
             self.logger.error("Failed to initialize Dlls.")
             return
@@ -570,14 +711,23 @@
         self._edb = edb.Ansoft.Edb
         edbbuilder = __import__("Ansys.Ansoft.EdbBuilderUtils")
         self.edbutils = edbbuilder.Ansoft.EdbBuilderUtils
         self.simSetup = __import__("Ansys.Ansoft.SimSetupData")
         self.simsetupdata = self.simSetup.Ansoft.SimSetupData.Data
 
     @property
+    def student_version(self):
+        """Set the student version flag."""
+        return self._student_version
+
+    @student_version.setter
+    def student_version(self, value):
+        self._student_version = value
+
+    @property
     def logger(self):
         """Logger for EDB.
 
         Returns
         -------
         :class:`pyaedt.aedt_logger.AedtLogger`
         """
@@ -605,15 +755,15 @@
 
 
 class Database(EdbDotNet):
     """Class representing a database object."""
 
     def __init__(self, edbversion, student_version=False):
         """Initialize a new Database."""
-        EdbDotNet.__init__(self, edbversion, student_version)
+        EdbDotNet.__init__(self, edbversion=edbversion, student_version=student_version)
         self._db = None
 
     @property
     def api_class(self):
         """Return Ansys.Ansoft.Edb class object."""
         return self._edb
```

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/dotnet/layout.py` & `pyaedt-0.6.88/pyaedt/edb_core/dotnet/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,18 +122,22 @@
 
         Read-Only.
         """
         return list(self._layout.VoltageRegulators)
 
     @property
     def extended_nets(self):
-        """:obj:`list` of :class:`ExtendedNet <ansys.edb.net.ExtendedNet>` : List of all the extended nets in this \
-        layout.
+        """
+        Get the list of extended nets in the layout. Read-Only.
+
+        Returns
+        -------
+        List[:class:`ExtendedNet <ansys.edb.net.ExtendedNet>`]
+            A list of extended nets.
 
-        Read-Only.
         """
         return list(self._layout.ExtendedNets)
 
     def expanded_extent(self, nets, extent, expansion_factor, expansion_unitless, use_round_corner, num_increments):
         """Get an expanded polygon for the Nets collection.
 
         Parameters
```

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/dotnet/primitive.py` & `pyaedt-0.6.88/pyaedt/edb_core/dotnet/primitive.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/control_file.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2380,22 +2380,14 @@
             Default value is ``1``.
 
         """
         if source_name:
             if node_to_ground in [0, 1, 2]:
                 self._dc_source_terms_to_ground[source_name] = node_to_ground
 
-    def _parse_signal_layer_properties(self, signal_properties):  # pragma: no cover
-        for lay in signal_properties:
-            lp = lay.split(":")
-            try:
-                self.signal_layers_properties.update({lp[0]: [lp[1], lp[2], lp[3], lp[4], lp[5]]})
-            except:
-                print("Missing parameter for layer {0}".format(lp[0]))
-
     def _read_cfg(self):  # pragma: no cover
         """Configuration file reader.
 
         .. deprecated:: 0.6.78
            Use :func:`import_json` instead.
 
         Examples
```

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.88/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/general.py` & `pyaedt-0.6.88/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.88/pyaedt/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.88/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/layout.py` & `pyaedt-0.6.88/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/materials.py` & `pyaedt-0.6.88/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/nets.py` & `pyaedt-0.6.88/pyaedt/edb_core/nets.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
                 if n in self._comps_by_nets_dict:
                     self._comps_by_nets_dict[n].append(comp)
                 else:
                     self._comps_by_nets_dict[n] = [comp]
         return self._comps_by_nets_dict
 
     @pyaedt_function_handler()
-    def get_extended_nets(self, resistor_below=10, inductor_below=1, capacitor_above=1, exception_list=None):
+    def generate_extended_nets(self, resistor_below=10, inductor_below=1, capacitor_above=1, exception_list=None):
         # type: (int | float, int | float, int |float, list) -> list
         """Get extended net and associated components.
 
         Parameters
         ----------
         resistor_below : int, float, optional
             Threshold of resistor value. Search extended net across resistors which has value lower than the threshold.
@@ -248,15 +248,15 @@
         --------
         >>> from pyaedt import Edb
         >>> app = Edb()
         >>> app.nets.get_extended_nets()
         """
         if exception_list is None:
             exception_list = []
-        self._extendend_nets = []
+        _extended_nets = []
         all_nets = list(self.nets.keys())[:]
         net_dicts = self._comps_by_nets_dict if self._comps_by_nets_dict else self.components_by_nets
         comp_dict = self._nets_by_comp_dict if self._nets_by_comp_dict else self.nets_by_components
 
         def get_net_list(net_name, _net_list):
             comps = []
             if net_name in net_dicts:
@@ -267,14 +267,15 @@
                 cmp = self._pedb.components.instances[refdes]
                 is_enabled = cmp.is_enabled
                 if not is_enabled:
                     continue
                 val_type = cmp.type
                 if val_type not in ["Inductor", "Resistor", "Capacitor"]:
                     continue
+
                 val_value = cmp.rlc_values
                 if refdes in exception_list:
                     pass
                 elif val_type == "Inductor" and val_value[1] < inductor_below:
                     pass
                 elif val_type == "Resistor" and val_value[0] < resistor_below:
                     pass
@@ -288,17 +289,23 @@
                         _net_list.append(net)
                         get_net_list(net, _net_list)
 
         while len(all_nets) > 0:
             new_ext = [all_nets[0]]
             get_net_list(new_ext[0], new_ext)
             all_nets = [i for i in all_nets if i not in new_ext]
-            self._extendend_nets.append(new_ext)
+            _extended_nets.append(new_ext)
 
-        return self._extendend_nets
+            if len(new_ext) > 1:
+                i = new_ext[0]
+                for i in new_ext:
+                    if not i.lower().startswith("unnamed"):
+                        break
+                self._pedb.extended_nets.create(i, new_ext)
+        return _extended_nets
 
     @staticmethod
     def _eval_arc_points(p1, p2, h, n=6, tol=1e-12):
         """Get the points of the arc.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.88/pyaedt/edb_core/padstack.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.88/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.88/pyaedt/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/emit.py` & `pyaedt-0.6.88/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.88/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.88/pyaedt/emit_core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import imp
 from importlib import import_module
 import os
 import sys
 
 from pyaedt.aedt_logger import pyaedt_logger as logger
+from pyaedt.emit_core.emit_constants import EmiCategoryFilter
 from pyaedt.emit_core.emit_constants import InterfererType
 from pyaedt.emit_core.emit_constants import ResultType
 from pyaedt.emit_core.emit_constants import TxRxMode
 from pyaedt.emit_core.emit_constants import UnitType
 
 EMIT_API_PYTHON = None
 
@@ -19,15 +20,15 @@
     The backend API is available once a pyaedt.Emit() object has been created. An exception is raised if this method is called before a ``pyaedt.Emit()`` object has been created.
     """
     if not EMIT_API_PYTHON:
         raise Exception("A pyaedt.Emit() object must be initialized before using the EMIT API.")
     return EMIT_API_PYTHON
 
 
-def _init_enums():
+def _init_enums(aedt_version):
     ResultType.EMI = emit_api_python().result_type().emi
     ResultType.DESENSE = emit_api_python().result_type().desense
     ResultType.SENSITIVITY = emit_api_python().result_type().sensitivity
     ResultType.POWER_AT_RX = emit_api_python().result_type().powerAtRx
 
     TxRxMode.TX = emit_api_python().tx_rx_mode().tx
     TxRxMode.RX = emit_api_python().tx_rx_mode().rx
@@ -41,14 +42,25 @@
     UnitType.FREQUENCY = emit_api_python().unit_type().frequency
     UnitType.LENGTH = emit_api_python().unit_type().length
     UnitType.TIME = emit_api_python().unit_type().time
     UnitType.VOLTAGE = emit_api_python().unit_type().voltage
     UnitType.DATA_RATE = emit_api_python().unit_type().dataRate
     UnitType.RESISTANCE = emit_api_python().unit_type().resistance
 
+    numeric_version = int(aedt_version[-3:])
+    if numeric_version >= 241:
+        emi_cat_filter = emit_api_python().emi_category_filter()
+        EmiCategoryFilter.IN_CHANNEL_TX_FUNDAMENTAL = emi_cat_filter.in_channel_tx_fundamental
+        EmiCategoryFilter.IN_CHANNEL_TX_HARMONIC_SPURIOUS = emi_cat_filter.in_channel_tx_harmonic_spurious
+        EmiCategoryFilter.IN_CHANNEL_TX_INTERMOD = emi_cat_filter.in_channel_tx_intermod
+        EmiCategoryFilter.IN_CHANNEL_TX_BROADBAND = emi_cat_filter.in_channel_tx_broadband
+        EmiCategoryFilter.OUT_OF_CHANNEL_TX_FUNDAMENTAL = emi_cat_filter.out_of_channel_tx_fundamental
+        EmiCategoryFilter.OUT_OF_CHANNEL_TX_HARMONIC_SPURIOUS = emi_cat_filter.out_of_channel_tx_harmonic_spurious
+        EmiCategoryFilter.OUT_OF_CHANNEL_TX_INTERMOD = emi_cat_filter.out_of_channel_tx_intermod
+
 
 # need this as a function so that it can be set
 # for the correct aedt version that the user is running
 def _set_api(aedt_version):
     numeric_version = int(aedt_version[-3:])
     desktop_path = os.environ.get(aedt_version)
     if desktop_path and numeric_version > 231:
@@ -58,8 +70,8 @@
             path = os.environ.get(override_path_key)
         sys.path.insert(0, path)
         module_path = imp.find_module("EmitApiPython")[1]
         logger.info("Importing EmitApiPython from: {}".format(module_path))
         global EMIT_API_PYTHON
         EMIT_API_PYTHON = import_module("EmitApiPython")
         logger.info("Loaded {}".format(EMIT_API_PYTHON.EmitApi().get_version(True)))
-        _init_enums()
+        _init_enums(aedt_version)
```

### Comparing `pyaedt-0.6.87/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.88/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.88/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.88/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/clr_module.py` & `pyaedt-0.6.88/pyaedt/generic/clr_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 is_linux = os.name == "posix"
 is_windows = not is_linux
 is_clr = False
 sys.path.append(os.path.join(pyaedt_path, "dlls", "PDFReport"))
 if is_linux and cpython:  # pragma: no cover
     try:
         if os.environ.get("DOTNET_ROOT") is None:
+            runtime = None
             try:
                 import dotnet
 
                 runtime = os.path.join(os.path.dirname(dotnet.__path__))
             except:
                 import dotnetcore2
```

### Comparing `pyaedt-0.6.87/pyaedt/generic/configurations.py` & `pyaedt-0.6.88/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/constants.py` & `pyaedt-0.6.88/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/design_types.py` & `pyaedt-0.6.88/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/filesystem.py` & `pyaedt-0.6.88/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/general_methods.py` & `pyaedt-0.6.88/pyaedt/generic/general_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -2219,15 +2219,15 @@
 
     @logger_datefmt.setter
     def logger_datefmt(self, val):
         self._logger_datefmt = val
 
     @property
     def enable_debug_edb_logger(self):
-        """Enable or disable Logger for any EDB API method."""
+        """Enable or disable Logger for any EDB API methods."""
         return self._enable_debug_edb_logger
 
     @property
     def enable_debug_grpc_api_logger(self):
         """Enable or disable Logger for any grpc API method."""
         return self._enable_debug_grpc_api_logger
 
@@ -2255,15 +2255,15 @@
 
     @enable_debug_internal_methods_logger.setter
     def enable_debug_internal_methods_logger(self, val):
         self._enable_debug_internal_methods_logger = val
 
     @property
     def enable_debug_logger(self):
-        """Return the Environment Variable Content."""
+        """Enable or disable Logger for any AEDT API methods. Additionally, enables debug logging messages."""
         return self._enable_debug_logger
 
     @enable_debug_logger.setter
     def enable_debug_logger(self, val):
         self._enable_debug_logger = val
```

### Comparing `pyaedt-0.6.87/pyaedt/generic/grpc_plugin.py` & `pyaedt-0.6.88/pyaedt/generic/grpc_plugin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/grpc_plugin_dll.py` & `pyaedt-0.6.88/pyaedt/generic/grpc_plugin_dll.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.88/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.88/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/pdf.py` & `pyaedt-0.6.88/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/plot.py` & `pyaedt-0.6.88/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/process.py` & `pyaedt-0.6.88/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.88/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.88/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/toolkit.py` & `pyaedt-0.6.88/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.88/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/hfss.py` & `pyaedt-0.6.88/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.88/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/icepak.py` & `pyaedt-0.6.88/pyaedt/icepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -2609,16 +2609,19 @@
         -------
         :class:`pyaedt.modules.Mesh.MeshOperation`
         """
         version = self.aedt_version_id[-3:]
         ansys_install_dir = os.environ.get("ANSYS{}_DIR".format(version), "")
         if not ansys_install_dir:
             ansys_install_dir = os.environ.get("AWP_ROOT{}".format(version), "")
-        assert ansys_install_dir, "Fluent {} has to be installed on to generate mesh.".format(version)
-        assert os.getenv("ANSYS{}_DIR".format(version))
+        assert ansys_install_dir, "Fluent {} has to be installed to generate mesh. Please set ANSYS{}_DIR".format(
+            version, version
+        )
+        if not os.getenv("ANSYS{}_DIR".format(version)):
+            os.environ["ANSYS{}_DIR".format(version)] = ansys_install_dir
         if not object_lists:
             object_lists = self.get_liquid_objects()
             assert object_lists, "No Fluids objects found."
         if not min_size or not max_size:
             dims = []
             # try:
             #     dim = self.modeler["Region"].shortest_edge()[0].length
@@ -2718,25 +2721,22 @@
         # Fluent command line parameters: -meshing -i <journal> -hidden -tm<x> (# processors for meshing) -wait
         fl_ucommand = [
             cmd,
             "3d",
             "-meshing",
             "-hidden",
             "-i",
-            '"' + fl_uscript_file_pointer + '"',
         ]
         self.logger.info("Fluent is starting in Background with command line")
+        if is_linux:
+            fl_ucommand = ["bash"] + fl_ucommand + [fl_uscript_file_pointer]
+        else:
+            fl_ucommand = ["bash"] + fl_ucommand + ['"' + fl_uscript_file_pointer + '"']
         self.logger.info(" ".join(fl_ucommand))
         subprocess.call(fl_ucommand)
-        if os.path.exists(mesh_file_pointer + ".trn"):
-            os.remove(mesh_file_pointer + ".trn")
-        if os.path.exists(fl_uscript_file_pointer):
-            os.remove(fl_uscript_file_pointer)
-        if os.path.exists(sab_file_pointer):
-            os.remove(sab_file_pointer)
         if os.path.exists(mesh_file_pointer):
             self.logger.info("'" + mesh_file_pointer + "' has been created.")
             return self.mesh.assign_mesh_from_file(object_lists, mesh_file_pointer)
         self.logger.error("Failed to create msh file")
 
         return False
```

### Comparing `pyaedt-0.6.87/pyaedt/maxwell.py` & `pyaedt-0.6.88/pyaedt/maxwell.py`

 * *Files 2% similar despite different names*

```diff
@@ -2739,14 +2739,142 @@
             }
         )
         bound = MaxwellParameters(self, force_name, props, "LayoutForce")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
 
+    @pyaedt_function_handler()
+    def assign_tangential_h_field(
+        self,
+        faces,
+        x_component_real=0,
+        x_component_imag=0,
+        y_component_real=0,
+        y_component_imag=0,
+        coordinate_system="Global",
+        origin=None,
+        u_pos=None,
+        reverse=False,
+        bound_name=None,
+    ):
+        """Assign a tangential H field boundary to a list of faces.
+
+        Parameters
+        ----------
+        faces : list of int  or :class:`pyaedt.modeler.cad.object3d.Object3d`
+            List of objects to assign an end connection to.
+        x_component_real : float, str, optional
+            X component value real part. The default is ``0``.
+        x_component_imag : float, str, optional
+            X component value imaginary part. The default is ``0``.
+        y_component_real : float, str, optional
+            Y component value real part. The default is ``0``.
+        y_component_imag : float, str, optional
+            Y component value imaginary part. The default is ``0``.
+        coordinate_system : str, optional
+            Coordinate system to use for the UV vector.
+        origin : list, optional
+            Origin of the UV vector.
+            The default is ``None`, in which case the bottom left vertex is used.
+        u_pos : list, optional
+            Direction of the U vector.
+            The default is ``None``, in which case the top left vertex is used.
+        reverse : bool, optional
+            Whether the vector is reversed. The default is ``False``.
+        bound_name : str, optional
+            Name of the end connection boundary.
+            The default is ``None``, in which case the default name is used.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Newly created object when successful, ``False`` when failed.
+
+        References
+        ----------
+
+        >>> oModule.AssignTangentialHField
+        """
+        if self.solution_type not in ["EddyCurrent", "Magnetostatic"]:
+            self.logger.error("Tangential H Field is applicable only to Eddy current.")
+            return False
+        objects = self.modeler.convert_to_selections(faces, True)
+        if not bound_name:
+            bound_name = generate_unique_name("TangentialHField")
+        props = OrderedDict(
+            {
+                "Faces": objects,
+            }
+        )
+        if isinstance(objects[0], str):
+            props = OrderedDict(
+                {
+                    "Objects": objects,
+                }
+            )
+        props["ComponentXReal"] = x_component_real
+        if self.solution_type == "EddyCurrent":
+            props["ComponentXImag"] = x_component_imag
+        props["ComponentYReal"] = y_component_real
+        if self.solution_type == "EddyCurrent":
+            props["ComponentYImag"] = y_component_imag
+        if not origin and isinstance(objects[0], int):
+            edges = self.modeler.get_face_edges(objects[0])
+            origin = self.oeditor.GetEdgePositionAtNormalizedParameter(edges[0], 0)
+            if not u_pos:
+                u_pos = self.oeditor.GetEdgePositionAtNormalizedParameter(edges[0], 1)
+
+        props["CoordSysVector"] = OrderedDict({"Coordinate System": coordinate_system, "Origin": origin, "UPos": u_pos})
+        props["ReverseV"] = reverse
+        bound = BoundaryObject(self, bound_name, props, "Tangential H Field")
+        if bound.create():
+            self._boundaries[bound.name] = bound
+            return bound
+        return False
+
+    @pyaedt_function_handler()
+    def assign_zero_tangential_h_field(self, faces, bound_name=None):
+        """Assign a zero tangential H field boundary to a list of faces.
+
+        Parameters
+        ----------
+        faces : list of int or :class:`pyaedt.modeler.cad.object3d.Object3d`
+            List of objects to assign an end connection to.
+        bound_name : str, optional
+            Name of the end connection boundary. The default is ``None``, in which case the
+            default name is used.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Newly created object. ``False`` if it fails.
+
+        References
+        ----------
+
+        >>> oModule.AssignZeroTangentialHField
+        """
+        if self.solution_type not in ["EddyCurrent"]:
+            self.logger.error("Tangential H Field is applicable only to Eddy current.")
+            return False
+        objects = self.modeler.convert_to_selections(faces, True)
+        if not bound_name:
+            bound_name = generate_unique_name("ZeroTangentialHField")
+        props = OrderedDict(
+            {
+                "Faces": objects,
+            }
+        )
+        bound = BoundaryObject(self, bound_name, props, "Zero Tangential H Field")
+        if bound.create():
+            self._boundaries[bound.name] = bound
+            return bound
+        return False
+
 
 class Maxwell2d(Maxwell, FieldAnalysis3D, object):
     """Provides the Maxwell 2D app interface.
 
     This class allows you to connect to an existing Maxwell 2D design or create a
     new Maxwell 2D design if one does not exist.
```

### Comparing `pyaedt-0.6.87/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.88/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/mechanical.py` & `pyaedt-0.6.88/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/Console.py_build` & `pyaedt-0.6.88/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.88/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.88/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.88/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.88/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.88/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/amat.xml` & `pyaedt-0.6.88/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/ansys_cloud.areg` & `pyaedt-0.6.88/pyaedt/misc/ansys_cloud.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/console_setup.py` & `pyaedt-0.6.88/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.88/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.88/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.88/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.88/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/misc.py` & `pyaedt-0.6.88/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.88/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.88/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.88/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.88/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.88/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.88/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/misc/template.acf` & `pyaedt-0.6.88/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.88/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.88/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.88/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.88/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.88/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.88/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/calculators.py` & `pyaedt-0.6.88/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.88/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.88/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.88/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.88/pyaedt/modeler/modeler2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
     This class is inherited in the caller application and is accessible through the modeler variable
     object( eg. ``rmxprt.modeler``).
 
     """
 
     def __init__(self, app):
+        app.logger.reset_timer()
         Modeler.__init__(self, app)
+        app.logger.info_timer("ModelerRMxprt class has been initialized!")
 
     @property
     def oeditor(self):
         """oEditor Module.
 
         References
         ----------
@@ -47,14 +49,15 @@
     >>> my_modeler = app.modeler
     """
 
     def __init__(self, application):
         GeometryModeler.__init__(self, application, is3d=False)
         Primitives2D.__init__(self)
         self._primitives = self
+        self.logger.info("Modeler2D class has been initialized!")
 
     def __get__(self, instance, owner):
         self._app = instance
         return self
 
     @property
     def primitives(self):
```

### Comparing `pyaedt-0.6.87/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.88/pyaedt/modeler/modeler3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,18 @@
     --------
     >>> from pyaedt import Hfss
     >>> hfss = Hfss()
     >>> my_modeler = hfss.modeler
     """
 
     def __init__(self, application):
+        application.logger.reset_timer()
         GeometryModeler.__init__(self, application, is3d=True)
         Primitives3D.__init__(self)
+        application.logger.info_timer("Modeler3D class has been initialized!")
 
     def __get__(self, instance, owner):
         self._app = instance
         return self
 
     @property
     def primitives(self):
```

### Comparing `pyaedt-0.6.87/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.88/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.88/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1474,23 +1474,25 @@
         comp_name = self.modeler.oeditor.CreateComponent(args)
         comp = ComponentsSubCircuit3DLayout(self, comp_name.split(";")[-1])
         self.components_3d[comp_name.split(";")[-1]] = comp
         if create_ports:
             self.oeditor.CreatePortsOnComponentsByNet(["NAME:Components", comp.name], [], "Port", "0", "0", "0")
         return comp  #
 
-    def create_text(self, text, position, angle=0, font_size=12):
+    def create_text(self, text, position, placement_layer="PostProcessing", angle=0, font_size=12):
         """Create a text primitive object.
 
         Parameters
         ----------
         text : str
             Name for the text primitive object.
         position : list
             Position of the text.
+        placement_layer : str, optional
+            Layer where text will be placed. The default value is ``"PostProcessing"``.
         angle : float, optional
             Angle of the text. The default value is ``0``.
         font_size : int, optional
             Font size. The default value is ``12``.
 
         Returns
         -------
@@ -1501,15 +1503,15 @@
         args = [
             "NAME:Contents",
             "textGeometry:=",
             [
                 "Name:=",
                 name,
                 "LayerName:=",
-                "Postprocessing",
+                placement_layer,
                 "x:=",
                 position[0],
                 "y:=",
                 position[1],
                 "ang:=",
                 angle,
                 "isPlot:=",
```

### Comparing `pyaedt-0.6.87/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.88/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modeler/schematic.py` & `pyaedt-0.6.88/pyaedt/modeler/schematic.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,20 @@
     --------
     >>> from pyaedt import Circuit
     >>> app = Circuit()
     >>> my_modeler = app.modeler
     """
 
     def __init__(self, app):
+        app.logger.reset_timer()
         self._app = app
         self._schematic_units = "meter"
         Modeler.__init__(self, app)
         self.wire = Wire(self)
+        app.logger.info_timer("ModelerCircuit class has been initialized!")
 
     @property
     def o_def_manager(self):
         """AEDT Definition manager."""
         return self._app.odefinition_manager
 
     @property
@@ -417,15 +419,15 @@
                         ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", property_value]],
                     ],
                 ]
             )
         else:
             self.logger.error("Wrong Property Value")
             return False
-        self.logger.info("Property {} Changed correctly.".format(property_name))
+        self.logger.debug("Property {} Changed correctly.".format(property_name))
         return True
 
     @pyaedt_function_handler()
     def _get_components_selections(self, selections, return_as_list=True):
         sels = []
         if not isinstance(selections, list):
             selections = [selections]
@@ -469,14 +471,15 @@
     def __init__(self, app):
         self._app = app
         ModelerCircuit.__init__(self, app)
         self._schematic = NexximComponents(self)
         self._layouteditor = None
         self.layers = Layers(self, roughnessunits="um")
         self._primitives = Primitives3DLayout(app)
+        self.logger.info("ModelerNexxim class has been initialized!")
 
     @property
     def layouteditor(self):
         """Return the Circuit Layout Editor.
 
         References
         ----------
@@ -665,14 +668,15 @@
 
     """
 
     def __init__(self, app):
         self._app = app
         ModelerCircuit.__init__(self, app)
         self._components = TwinBuilderComponents(self)
+        self.logger.info("ModelerTwinBuilder class has been initialized!")
 
     @property
     def components(self):
         """
         .. deprecated:: 0.4.13
            Use :func:`TwinBuilder.modeler.schematic` instead.
 
@@ -700,14 +704,15 @@
 
     """
 
     def __init__(self, app):
         self._app = app
         ModelerCircuit.__init__(self, app)
         self.components = EmitComponents(app, self)
+        self.logger.info("ModelerEmit class has been initialized!")
 
 
 class ModelerMaxwellCircuit(ModelerCircuit):
     """ModelerMaxwellCircuit class.
 
     Parameters
     ----------
@@ -715,14 +720,15 @@
 
     """
 
     def __init__(self, app):
         self._app = app
         ModelerCircuit.__init__(self, app)
         self._components = MaxwellCircuitComponents(self)
+        self.logger.info("ModelerMaxwellCircuit class has been initialized!")
 
     @property
     def schematic(self):
         """Schematic Object.
 
         Returns
         -------
```

### Comparing `pyaedt-0.6.87/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.88/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,16 +404,16 @@
         .. note::
            The PyVista module rebuilds the mesh and the overlap fields on the mesh.
 
         Parameters
         ----------
         quantity : str
             Quantity to plot (e.g. ``"Mag_E"``).
-        object_list : str
-            List of objects or faces to which apply the Field Plot.
+        object_list : str, list
+            Objects or faces to which apply the Field Plot.
         plot_type  : str, optional
             Plot type. Options are ``"Surface"``, ``"Volume"``, ``"CutPlane"``.
         setup_name : str, optional
             Setup and sweep name on which create the field plot. Default is None for nominal setup usage.
         intrinsics : dict, optional.
             Intrinsic dictionary that is needed for the export.
             The default is ``None`` which try to retrieve intrinsics from setup.
@@ -551,21 +551,29 @@
             If `None` aedt opacity will be applied to each object.
 
         Returns
         -------
         :class:`pyaedt.generic.plot.ModelPlotter`
             Model Object.
         """
+        if intrinsics is None:
+            intrinsics = {}
         if not export_path:
             export_path = self._app.working_directory
 
         v = 0
         fields_to_add = []
+        is_intrinsics = True
+        if variation_variable in self._app.variable_manager.independent_variables:
+            is_intrinsics = False
         for el in variation_list:
-            intrinsics[variation_variable] = el
+            if is_intrinsics:
+                intrinsics[variation_variable] = el
+            else:
+                self._app[variation_variable] = el
             if plot_type == "Surface":
                 plotf = self.create_fieldplot_surface(object_list, quantity, setup_name, intrinsics)
             elif plot_type == "Volume":
                 plotf = self.create_fieldplot_volume(object_list, quantity, setup_name, intrinsics)
             else:
                 plotf = self.create_fieldplot_cutplane(object_list, quantity, setup_name, intrinsics)
             if plotf:
```

### Comparing `pyaedt-0.6.87/pyaedt/modules/Boundary.py` & `pyaedt-0.6.88/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.88/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.88/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.88/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.88/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/Material.py` & `pyaedt-0.6.88/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.88/pyaedt/modules/MaterialLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,26 +39,27 @@
     --------
     >>> from pyaedt import Hfss
     >>> app = Hfss()
     >>> materials = app.materials
     """
 
     def __init__(self, app):
+        app.logger.reset_timer()
         self._app = app
         self._color_id = 0
         self._mats = []
         self._mats_lower = []
         self._desktop = self._app.odesktop
         self._oproject = self._app.oproject
         self.logger = self._app.logger
-        self.logger.info("Successfully loaded project materials !")
         # self.material_keys = self._get_materials()
         self.material_keys = {}
         self._surface_material_keys = {}
         self._load_from_project()
+        app.logger.info_timer("Material library initialized and project materials loaded successfully!")
 
     @property
     def odefinition_manager(self):
         """Definition Manager from AEDT."""
         return self._app.odefinition_manager
 
     @property
```

### Comparing `pyaedt-0.6.87/pyaedt/modules/Mesh.py` & `pyaedt-0.6.88/pyaedt/modules/Mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,21 +326,23 @@
     >>> from pyaedt import Hfss
     >>> aedtapp = Hfss()
     >>> cylinder = aedtapp.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
     >>> model_resolution = aedtapp.mesh.assign_model_resolution(cylinder, 1e-4, "ModelRes1")
     """
 
     def __init__(self, app):
+        app.logger.reset_timer()
         self._app = app
         self._odesign = self._app.odesign
         self.modeler = self._app.modeler
         self.logger = self._app.logger
         self.id = 0
         self._meshoperations = None
         self._globalmesh = None
+        app.logger.info_timer("Mesh class has been initialized!")
 
     @pyaedt_function_handler()
     def __getitem__(self, part_id):
         """Get the object ``Mesh`` for a given mesh operation name.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.87/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.88/pyaedt/modules/Mesh3DLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,24 +127,25 @@
     Parameters
     ----------
     app : :class:`pyaedt.application.Analysis3DLayout.FieldAnalysis3DLayout`
 
     """
 
     def __init__(self, app):
+        app.logger.reset_timer()
         self._app = app
 
         self.logger = self._app.logger
         self._odesign = self._app._odesign
         self.modeler = self._app.modeler
         self.id = 0
 
         self.meshoperations = self._get_design_mesh_operations()
 
-        pass
+        app.logger.info_timer("Mesh class has been initialized!")
 
     @pyaedt_function_handler()
     def generate_mesh(self, name):
         """Generate the mesh for a design.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.87/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.88/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.88/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.88/pyaedt/modules/PostProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1849,18 +1849,20 @@
 
     >>> from pyaedt import Hfss
     >>> aedtapp = Hfss()
     >>> post = aedtapp.post
     """
 
     def __init__(self, app):
+        app.logger.reset_timer()
         self._app = app
         self._post_osolution = self._app.osolution
         self.field_plots = self._get_fields_plot()
         PostProcessorCommon.__init__(self, app)
+        app.logger.info_timer("PostProcessor class has been initialized!")
 
     @property
     def _primitives(self):  # pragma: no cover
         """Primitives.
 
         Returns
         -------
@@ -2127,48 +2129,65 @@
         quantity_name,
         scalar_function="Maximum",
         solution=None,
         variation_dict=None,
         isvector=False,
         intrinsics=None,
         phase=None,
+        object_name="AllObjects",
+        object_type="volume",
+        adjacent_side=False,
     ):
         """Use the field calculator to Compute Scalar of a Field.
 
         Parameters
         ----------
         quantity_name : str
             Name of the quantity to export. For example, ``"Temp"``.
+        scalar_function : str, optional
+            The name of the scalar function. For example, ``"Maximum"``, ``"Integrate"``.
+            The default is ``"Maximum"``.
         solution : str, optional
             Name of the solution in the format ``"solution : sweep"``. The default is ``None``.
         variation_dict : dict, optional
             Dictionary of all variation variables with their values.
+            e.g. ``['power_block:=', ['0.6W'], 'power_source:=', ['0.15W']]``
             The default is ``None``.
         isvector : bool, optional
             Whether the quantity is a vector. The  default is ``False``.
         intrinsics : str, optional
             This parameter is mandatory for a frequency field
             calculation. The default is ``None``.
         phase : str, optional
             Field phase. The default is ``None``.
+        object_name : str, optional
+            Name of the object. For example, ``"Box1"``.
+            The default is ``"AllObjects"``.
+        object_type : str, optional
+            Type of the object - ``"volume"``, ``"surface"``, ``"point"``.
+            The default is ``"volume"``.
+        adjacent_side : bool, optional
+            To query quantity value on adjacent side for object_type = "surface", pass ``True``.
+            The default is ``False``.
 
         Returns
         -------
         float
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.EnterQty
         >>> oModule.CopyNamedExprToStack
         >>> oModule.CalcOp
         >>> oModule.EnterQty
         >>> oModule.EnterVol
-        >>> oModule.CalculatorWrite
+        >>> oModule.ClcEval
+        >>> GetTopEntryValue
         """
         self.logger.info("Exporting {} field. Be patient".format(quantity_name))
         if not solution:
             solution = self._app.existing_analysis_sweeps[0]
         self.ofieldsreporter.CalcStack("clear")
         if isvector:
             try:
@@ -2181,17 +2200,25 @@
             self.ofieldsreporter.CalcOp("Mag")
         else:
             try:
                 self.ofieldsreporter.EnterQty(quantity_name)
             except:
                 self.logger.info("Quantity {} not present. Trying to get it from Stack".format(quantity_name))
                 self.ofieldsreporter.CopyNamedExprToStack(quantity_name)
-        obj_list = "AllObjects"
+        obj_list = object_name
         if scalar_function:
-            self.ofieldsreporter.EnterVol(obj_list)
+            if object_type == "volume":
+                self.ofieldsreporter.EnterVol(obj_list)
+            elif object_type == "surface":
+                if adjacent_side:
+                    self.ofieldsreporter.EnterAdjacentSurf(obj_list)
+                else:
+                    self.ofieldsreporter.EnterSurf(obj_list)
+            elif object_type == "point":
+                self.ofieldsreporter.EnterPoint(obj_list)
             self.ofieldsreporter.CalcOp(scalar_function)
         if not variation_dict:
             variation_dict = self._app.available_variations.nominal_w_values
         if intrinsics:
             if "Transient" in solution:
                 variation_dict.append("Time:=")
                 variation_dict.append(intrinsics)
@@ -2199,25 +2226,19 @@
                 variation_dict.append("Freq:=")
                 variation_dict.append(intrinsics)
                 variation_dict.append("Phase:=")
                 if phase:
                     variation_dict.append(phase)
                 else:
                     variation_dict.append("0deg")
-        file_name = os.path.join(self._app.working_directory, generate_unique_name("temp_fld") + ".fld")
-        self.ofieldsreporter.CalculatorWrite(file_name, ["Solution:=", solution], variation_dict)
-        value = None
-        if os.path.exists(file_name) or settings.remote_rpc_session:
-            with open_file(file_name, "r") as f:
-                lines = f.readlines()
-                lines = [line.strip() for line in lines]
-                value = lines[-1]
-            os.remove(file_name)
+
+        self.ofieldsreporter.ClcEval(solution, variation_dict)
+        value = self.ofieldsreporter.GetTopEntryValue(solution, variation_dict)
         self.ofieldsreporter.CalcStack("clear")
-        return float(value)
+        return float(value[0])
 
     @pyaedt_function_handler()
     def export_field_file_on_grid(
         self,
         quantity_name,
         solution=None,
         variation_dict=None,
```

### Comparing `pyaedt-0.6.87/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.88/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.88/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.88/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.88/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/report_templates.py` & `pyaedt-0.6.88/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/modules/solutions.py` & `pyaedt-0.6.88/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/q3d.py` & `pyaedt-0.6.88/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/rmxprt.py` & `pyaedt-0.6.88/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.88/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.88/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.88/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.88/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.88/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/siwave.py` & `pyaedt-0.6.88/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyaedt/twinbuilder.py` & `pyaedt-0.6.88/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.87/pyproject.toml` & `pyaedt-0.6.88/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,51 +38,51 @@
     "ipython==8.13.0; python_version < '3.9'",
     "ipython==8.14.0; python_version >= '3.9'",
     "imageio==2.31.1",
     "joblib==1.3.1",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
-    "numpy==1.25.1; python_version > '3.9'",
+    "numpy==1.25.2; python_version > '3.9'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.3; python_version > '3.7'",
     "pytest==7.4.0",
     "pytest-cov==4.1.0",
     "pytest-xdist==3.3.1",
-    "pyvista==0.40.2; python_version > '3.7'",
+    "pyvista==0.41.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "scikit-learn==1.3.0",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
-    "ansys-sphinx-theme==0.9.9",
+    "ansys-sphinx-theme==0.10.0",
     "imageio==2.31.1",
     "imageio-ffmpeg==0.4.8",
     "ipython==8.13.0; python_version < '3.9'",
     "ipython==8.14.0; python_version >= '3.9'",
-    "ipywidgets==8.0.7",
+    "ipywidgets==8.1.0",
     "joblib==1.3.1",
     "jupyterlab==4.0.3",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.2; python_version > '3.7'",
     "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.40.2; python_version > '3.7'",
+    "pyvista==0.41.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "recommonmark==0.7.1",
     "scikit-learn==1.3.0",
-    "Sphinx==7.1.0",
+    "Sphinx==7.1.2",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.24.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
@@ -91,35 +91,35 @@
     "openpyxl==3.1.2",
 ]
 full = [
     "imageio",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
-    "numpy==1.25.1; python_version > '3.9'",
+    "numpy==1.25.2; python_version > '3.9'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.3; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.40.2; python_version > '3.7'",
+    "pyvista==0.41.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
     "imageio",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.2; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.9'",
-    "numpy==1.25.1; python_version > '3.9'",
+    "numpy==1.25.2; python_version > '3.9'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.3; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.40.2; python_version > '3.7'",
+    "pyvista==0.41.1; python_version > '3.7'",
     "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
```

### Comparing `pyaedt-0.6.87/PKG-INFO` & `pyaedt-0.6.88/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.87
+Version: 0.6.88
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,84 +21,84 @@
 Requires-Dist: rpyc==5.3.1
 Requires-Dist: psutil
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
 Requires-Dist: imageio ; extra == "all"
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.2 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.9')
-Requires-Dist: numpy==1.25.1 ; extra == "all" and ( python_version > '3.9')
+Requires-Dist: numpy==1.25.2 ; extra == "all" and ( python_version > '3.9')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
-Requires-Dist: pyvista==0.40.2 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.41.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.10.0 ; extra == "doc"
 Requires-Dist: imageio==2.31.1 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: ipython==8.13.0 ; extra == "doc" and ( python_version < '3.9')
 Requires-Dist: ipython==8.14.0 ; extra == "doc" and ( python_version >= '3.9')
-Requires-Dist: ipywidgets==8.0.7 ; extra == "doc"
+Requires-Dist: ipywidgets==8.1.0 ; extra == "doc"
 Requires-Dist: joblib==1.3.1 ; extra == "doc"
 Requires-Dist: jupyterlab==4.0.3 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.2 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.40.2 ; extra == "doc" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.41.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.3.0 ; extra == "doc"
-Requires-Dist: Sphinx==7.1.0 ; extra == "doc"
+Requires-Dist: Sphinx==7.1.2 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.24.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
 Requires-Dist: openpyxl==3.1.2 ; extra == "doc"
 Requires-Dist: imageio ; extra == "full"
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.2 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.9')
-Requires-Dist: numpy==1.25.1 ; extra == "full" and ( python_version > '3.9')
+Requires-Dist: numpy==1.25.2 ; extra == "full" and ( python_version > '3.9')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
-Requires-Dist: pyvista==0.40.2 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.41.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests" and ( python_version < '3.9')
 Requires-Dist: ipython==8.14.0 ; extra == "tests" and ( python_version >= '3.9')
 Requires-Dist: imageio==2.31.1 ; extra == "tests"
 Requires-Dist: joblib==1.3.1 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.2 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.9')
-Requires-Dist: numpy==1.25.1 ; extra == "tests" and ( python_version > '3.9')
+Requires-Dist: numpy==1.25.2 ; extra == "tests" and ( python_version > '3.9')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
-Requires-Dist: pyvista==0.40.2 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.41.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: scikit-learn==1.3.0 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bugs, https://github.com/ansys/pyaedt/issues
 Project-URL: Discussions, https://github.com/ansys/pyaedt/discussions
```

