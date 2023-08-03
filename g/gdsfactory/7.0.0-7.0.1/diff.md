# Comparing `tmp/gdsfactory-7.0.0.tar.gz` & `tmp/gdsfactory-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-7.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gdsfactory-7.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gdsfactory-7.0.0.tar` & `gdsfactory-7.0.1.tar`

### file list

```diff
@@ -1,525 +1,525 @@
--rw-r--r--   0        0        0     1072 2023-08-02 20:27:28.513507 gdsfactory-7.0.0/LICENSE
--rw-r--r--   0        0        0     9595 2023-08-02 20:27:28.513507 gdsfactory-7.0.0/README.md
--rw-r--r--   0        0        0     3417 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/__init__.py
--rw-r--r--   0        0        0     1870 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12537 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3682 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5016 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    16012 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14682 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2864 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2253 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1791 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1856 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/asserts.py
--rw-r--r--   0        0        0    14884 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/cell.py
--rw-r--r--   0        0        0     5959 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/cli.py
--rw-r--r--   0        0        0   102115 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/component.py
--rw-r--r--   0        0        0    24269 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    30803 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1179 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1105 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/L.py
--rw-r--r--   0        0        0    21495 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2599 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    13939 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3168 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2528 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4664 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4319 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1636 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     3048 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2614 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     8029 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2663 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3807 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5338 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5740 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2888 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1593 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1374 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1552 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5933 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8880 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5005 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6080 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2514 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9898 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0    11731 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/component_lattice_generic.py
--rw-r--r--   0        0        0     7130 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2128 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     4667 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_bent.py
--rw-r--r--   0        0        0     3970 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     5829 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-08-02 20:27:28.517501 gdsfactory-7.0.0/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1816 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    13157 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5256 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6743 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3759 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2708 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4262 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2481 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3176 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3245 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4313 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1254 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3578 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2968 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2816 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     7984 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4121 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1188 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1756 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7046 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3225 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     2458 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4651 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7137 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7209 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4942 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4694 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1747 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9054 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1814 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4110 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4650 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3855 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1579 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8722 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3643 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1799 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1218 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1278 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     5005 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mmi.py
--rw-r--r--   0        0        0     3978 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2769 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3801 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3192 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4944 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3293 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7610 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2464 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5822 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12188 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4020 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1264 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6310 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3476 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6016 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6289 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3833 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1915 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-08-02 20:27:28.521496 gdsfactory-7.0.0/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3799 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1115 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1475 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2933 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1059 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/rectangular_ring.py
--rw-r--r--   0        0        0     1476 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3276 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2629 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1260 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4118 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3247 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2348 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     2846 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_double_bend_coupler.py
--rw-r--r--   0        0        0     5102 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7747 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12046 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2909 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1923 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6868 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2743 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4231 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5307 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2281 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3745 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5832 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16624 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9155 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1733 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5289 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2640 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7863 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     8266 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8519 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     6044 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2805 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3955 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      656 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      821 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7973 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3539 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2801 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1235 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1787 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2887 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3886 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3186 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3897 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2430 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2413 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3034 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15895 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4516 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4918 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1065 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     7181 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0    10085 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/config.py
--rw-r--r--   0        0        0    38409 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/constants.py
--rw-r--r--   0        0        0    83618 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2963 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/decorators.py
--rw-r--r--   0        0        0     8406 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/difftest.py
--rw-r--r--   0        0        0      668 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/difftest_git.py
--rw-r--r--   0        0        0     1029 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/events.py
--rw-r--r--   0        0        0      267 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3308 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     7531 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/export/to_gerber.py
--rw-r--r--   0        0        0     1908 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3095 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0    11831 2023-08-02 20:27:28.525490 gdsfactory-7.0.0/gdsfactory/fill.py
--rw-r--r--   0        0        0     7780 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/font.py
--rw-r--r--   0        0        0     8067 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/functions.py
--rw-r--r--   0        0        0     1025 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1957 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0     1008 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/containers.py
--rw-r--r--   0        0        0      169 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8117 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0      161 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0     6192 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0       27 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
--rw-r--r--   0        0        0      494 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/Makefile
--rw-r--r--   0        0        0     4062 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12379 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7235 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3446 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    10697 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      477 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     4338 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      926 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      709 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4312 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1800 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
--rw-r--r--   0        0        0     1519 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    41073 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0    40616 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     5977 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
--rw-r--r--   0        0        0     4258 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1857 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10780 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0     2463 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4869 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3789 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1862 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      567 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2693 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2803 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3540 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1867 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     4954 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7017 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1655 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6614 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3686 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3055 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4184 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4759 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3248 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3810 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2465 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2952 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     3626 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/write_connectivity.py
--rw-r--r--   0        0        0    10476 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1152 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23637 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14481 2023-08-02 20:27:28.529485 gdsfactory-7.0.0/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0     9689 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/grid.py
--rw-r--r--   0        0        0     5083 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/install.py
--rw-r--r--   0        0        0     1855 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3519 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3818 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3796 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4644 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4840 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     5247 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/name.py
--rw-r--r--   0        0        0    11574 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/pack.py
--rw-r--r--   0        0        0    52172 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/path.py
--rw-r--r--   0        0        0    30164 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6092 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5029 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/pixelate.py
--rw-r--r--   0        0        0      303 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/plugins/__init__.py
--rw-r--r--   0        0        0     4262 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/polygon.py
--rw-r--r--   0        0        0    32988 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/port.py
--rw-r--r--   0        0        0    37674 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1259 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1927 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2773 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0     4222 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/from_updk.py
--rw-r--r--   0        0        0    37973 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5997 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5632 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3369 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     1474 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/route_info.py
--rw-r--r--   0        0        0     3767 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2907 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3002 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3031 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8726 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10573 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     9220 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38995 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3879 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      981 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4324 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2796 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    25075 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8642 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6904 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12925 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5258 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1912 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17052 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1486 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9226 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10829 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6090 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3246 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1773 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34260 2023-08-02 20:27:28.533480 gdsfactory-7.0.0/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10037 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22673 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8643 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18074 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4341 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14296 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10141 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5040 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2433 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2767 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0      974 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      698 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      925 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1081 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1621 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2225 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0     1013 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1683 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1733 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0     1030 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      272 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      561 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      565 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      550 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      632 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      847 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0      924 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/23_reticle_passives_grid.py
--rw-r--r--   0        0        0     1177 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/23_reticle_passives_pack.py
--rw-r--r--   0        0        0      381 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      715 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      720 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1434 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1308 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     2393 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2296 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0      989 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4494 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      363 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1065 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/.gitignore
--rw-r--r--   0        0        0    10181 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/00_geometry.py
--rw-r--r--   0        0        0    13583 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/01_references.py
--rw-r--r--   0        0        0     5845 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/02_movement.py
--rw-r--r--   0        0        0    29824 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/03_Path_CrossSection.py
--rw-r--r--   0        0        0     6881 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py
--rw-r--r--   0        0        0    16888 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/03_layer_stack.py
--rw-r--r--   0        0        0    11362 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_geometry.py
--rw-r--r--   0        0        0     5789 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_hierarchy.py
--rw-r--r--   0        0        0     7287 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_pack.py
--rw-r--r--   0        0        0     8093 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_shapes.py
--rw-r--r--   0        0        0    27801 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_routing.py
--rw-r--r--   0        0        0    10894 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_routing_electrical.py
--rw-r--r--   0        0        0    17498 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_routing_non_manhattan.py
--rw-r--r--   0        0        0    12399 2023-08-02 20:27:28.537474 gdsfactory-7.0.0/gdsfactory/samples/notebooks/07_mask.py
--rw-r--r--   0        0        0    15157 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/08_pdk.py
--rw-r--r--   0        0        0    11094 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/08_pdk_examples.py
--rw-r--r--   0        0        0     8585 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/09_pdk_import.py
--rw-r--r--   0        0        0    17564 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/10_yaml_component.py
--rw-r--r--   0        0        0     4684 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/11_get_netlist.py
--rw-r--r--   0        0        0     2114 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/11_get_netlist_spice.py
--rw-r--r--   0        0        0     4477 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/21_drc.py
--rw-r--r--   0        0        0      437 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/Makefile
--rw-r--r--   0        0        0     6217 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/_0_python.py
--rw-r--r--   0        0        0    16372 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/_1_git.py
--rw-r--r--   0        0        0     1092 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/_2_klayout.py
--rw-r--r--   0        0        0     1384 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/_3_vscode.py
--rw-r--r--   0        0        0     8163 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/_4_gdsfactory.py
--rw-r--r--   0        0        0     4412 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/common_mistakes.py
--rw-r--r--   0        0        0     4018 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/dataprep.py
--rw-r--r--   0        0        0     2660 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/declarative_cell.py
--rw-r--r--   0        0        0    13148 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/inkscape_align.png
--rw-r--r--   0        0        0    14726 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/inkscape_distribute.png
--rw-r--r--   0        0        0    71039 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/pathlength_report.png
--rw-r--r--   0        0        0    67563 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png
--rw-r--r--   0        0        0     6558 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/rib_strip_autotransition.py
--rw-r--r--   0        0        0      591 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml
--rw-r--r--   0        0        0      726 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml
--rw-r--r--   0        0        0      822 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml
--rw-r--r--   0        0        0     1417 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml
--rw-r--r--   0        0        0     1508 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml
--rw-r--r--   0        0        0     1405 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml
--rw-r--r--   0        0        0      600 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml
--rw-r--r--   0        0        0      614 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml
--rw-r--r--   0        0        0     1152 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml
--rw-r--r--   0        0        0     1066 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml
--rw-r--r--   0        0        0      778 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml
--rw-r--r--   0        0        0     1423 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml
--rw-r--r--   0        0        0      857 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml
--rw-r--r--   0        0        0        0 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     4361 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      233 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/fab_c_to_updk.py
--rw-r--r--   0        0        0      475 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1893 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1745 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     2483 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     1997 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1283 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     1830 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     1815 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     5043 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     5001 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     2604 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0     4876 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1569 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/show.py
--rw-r--r--   0        0        0      525 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     1689 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/snap.py
--rw-r--r--   0        0        0     4254 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/symbols.py
--rw-r--r--   0        0        0      308 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0      343 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/technology/color_utils.py
--rw-r--r--   0        0        0     7550 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1041 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    19086 2023-08-02 20:27:28.541469 gdsfactory-7.0.0/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    41893 2023-08-02 20:27:28.545464 gdsfactory-7.0.0/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0      674 2023-08-02 20:27:28.545464 gdsfactory-7.0.0/gdsfactory/technology/xml_utils.py
--rw-r--r--   0        0        0     1413 2023-08-02 20:27:28.545464 gdsfactory-7.0.0/gdsfactory/technology/yaml_utils.py
--rw-r--r--   0        0        0    11084 2023-08-02 20:27:28.545464 gdsfactory-7.0.0/gdsfactory/typings.py
--rw-r--r--   0        0        0     5489 2023-08-02 20:27:28.545464 gdsfactory-7.0.0/gdsfactory/watch.py
--rw-r--r--   0        0        0     7419 2023-08-02 20:27:28.545464 gdsfactory-7.0.0/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     4321 2023-08-02 20:27:28.545464 gdsfactory-7.0.0/pyproject.toml
--rw-r--r--   0        0        0    11819 1970-01-01 00:00:00.000000 gdsfactory-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-03 12:18:28.595784 gdsfactory-7.0.1/LICENSE
+-rw-r--r--   0        0        0     9454 2023-08-03 12:18:28.595784 gdsfactory-7.0.1/README.md
+-rw-r--r--   0        0        0     3417 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     1870 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12537 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3682 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5016 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    16012 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14682 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2864 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2253 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1791 2023-08-03 12:18:28.599784 gdsfactory-7.0.1/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1856 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    14884 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/cell.py
+-rw-r--r--   0        0        0     5959 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/cli.py
+-rw-r--r--   0        0        0   102115 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/component.py
+-rw-r--r--   0        0        0    24269 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    30803 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1179 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1105 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    21495 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2599 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    13939 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3168 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2528 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4664 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4319 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1636 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     3048 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2614 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     8029 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2663 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3807 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5338 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5740 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2888 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1593 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1374 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1552 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5933 2023-08-03 12:18:28.603784 gdsfactory-7.0.1/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8880 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5005 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6080 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2514 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9898 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0    11731 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/component_lattice_generic.py
+-rw-r--r--   0        0        0     7130 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2128 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     4667 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_bent.py
+-rw-r--r--   0        0        0     3970 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     5829 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1816 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    13157 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5256 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6743 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3759 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2708 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4262 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2481 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3176 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3245 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4313 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1254 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3578 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2968 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2816 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     7984 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4121 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1188 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1756 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7046 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3225 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     2458 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4651 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7137 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7209 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4942 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4694 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1747 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9054 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1814 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4110 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4650 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3855 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1579 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8722 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3643 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1799 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1218 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1278 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-08-03 12:18:28.607784 gdsfactory-7.0.1/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     5005 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mmi.py
+-rw-r--r--   0        0        0     3978 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2769 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3801 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3192 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4944 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3293 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7610 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2464 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5822 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12188 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4020 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1264 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6310 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3476 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6016 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6289 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3833 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1915 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3799 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1115 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1475 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2933 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1059 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/rectangular_ring.py
+-rw-r--r--   0        0        0     1476 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3276 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2629 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1260 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4118 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3247 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2348 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     2846 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_double_bend_coupler.py
+-rw-r--r--   0        0        0     5102 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7747 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12046 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2909 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1923 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6868 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2743 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4231 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5307 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2281 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3745 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5832 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16624 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9155 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1733 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5289 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2640 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7863 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     8266 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8519 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     6044 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2805 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3955 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      656 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      821 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7973 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3539 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2801 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1235 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1787 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2887 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3886 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3186 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3897 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-08-03 12:18:28.611784 gdsfactory-7.0.1/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2430 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2413 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3034 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15895 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4516 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4918 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1065 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     7181 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0    10085 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/config.py
+-rw-r--r--   0        0        0    38409 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/constants.py
+-rw-r--r--   0        0        0    83618 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2963 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     8406 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/difftest.py
+-rw-r--r--   0        0        0      668 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/difftest_git.py
+-rw-r--r--   0        0        0     1029 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/events.py
+-rw-r--r--   0        0        0      267 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3308 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     7531 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/export/to_gerber.py
+-rw-r--r--   0        0        0     1908 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3095 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0    11831 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7780 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/font.py
+-rw-r--r--   0        0        0     8067 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/functions.py
+-rw-r--r--   0        0        0     1025 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1957 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0     1008 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/containers.py
+-rw-r--r--   0        0        0      169 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8117 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0      161 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0     6192 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0       27 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/.gitignore
+-rw-r--r--   0        0        0      494 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/Makefile
+-rw-r--r--   0        0        0     4062 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12379 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7235 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3446 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    10697 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     4338 2023-08-03 12:18:28.615784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      926 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      709 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4312 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1800 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
+-rw-r--r--   0        0        0     1519 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    41073 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0    40616 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/layers.lyp
+-rw-r--r--   0        0        0     5977 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/tech.lyt
+-rw-r--r--   0        0        0     4258 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1857 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0     6511 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10780 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0     2463 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4869 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3789 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1862 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      567 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2693 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2803 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3540 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1867 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     4954 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7017 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1655 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6614 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3686 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3055 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4184 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4759 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3248 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3810 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2465 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2952 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     3626 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/write_connectivity.py
+-rw-r--r--   0        0        0    10476 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1152 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23637 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14481 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0     9689 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/grid.py
+-rw-r--r--   0        0        0     5083 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/install.py
+-rw-r--r--   0        0        0     1855 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3519 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3818 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3796 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4644 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4840 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     5247 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/name.py
+-rw-r--r--   0        0        0    11574 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/pack.py
+-rw-r--r--   0        0        0    52172 2023-08-03 12:18:28.619784 gdsfactory-7.0.1/gdsfactory/path.py
+-rw-r--r--   0        0        0    30164 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6092 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5029 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0      303 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/plugins/__init__.py
+-rw-r--r--   0        0        0     4262 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/polygon.py
+-rw-r--r--   0        0        0    32988 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/port.py
+-rw-r--r--   0        0        0    37674 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1259 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1927 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2773 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0     4222 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/from_updk.py
+-rw-r--r--   0        0        0    37973 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5997 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5632 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3369 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     1614 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/route_info.py
+-rw-r--r--   0        0        0     3767 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2907 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3002 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3031 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8726 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10573 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     9220 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38995 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3879 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      981 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4324 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2796 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    25075 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8642 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6904 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12925 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5258 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1912 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17052 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1486 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9226 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10829 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6090 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2766 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3246 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1773 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34260 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10037 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22673 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8643 2023-08-03 12:18:28.623784 gdsfactory-7.0.1/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18074 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4341 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14296 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10141 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5040 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2433 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2767 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0      974 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      698 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      925 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1081 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1621 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2225 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0     1013 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1683 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1733 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0     1030 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      272 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      561 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      565 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      550 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      632 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      847 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0      924 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/23_reticle_passives_grid.py
+-rw-r--r--   0        0        0     1177 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/23_reticle_passives_pack.py
+-rw-r--r--   0        0        0      381 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      715 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      720 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1434 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1308 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     2393 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      622 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      569 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2296 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0      989 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4494 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      363 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1065 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/.gitignore
+-rw-r--r--   0        0        0    10181 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/00_geometry.py
+-rw-r--r--   0        0        0    13583 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/01_references.py
+-rw-r--r--   0        0        0     5845 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/02_movement.py
+-rw-r--r--   0        0        0    29824 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/03_Path_CrossSection.py
+-rw-r--r--   0        0        0     6881 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py
+-rw-r--r--   0        0        0    16888 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/03_layer_stack.py
+-rw-r--r--   0        0        0    11362 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_geometry.py
+-rw-r--r--   0        0        0     5789 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_hierarchy.py
+-rw-r--r--   0        0        0     7287 2023-08-03 12:18:28.627784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_pack.py
+-rw-r--r--   0        0        0     8093 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_shapes.py
+-rw-r--r--   0        0        0    27801 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_routing.py
+-rw-r--r--   0        0        0    10894 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_routing_electrical.py
+-rw-r--r--   0        0        0    17498 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_routing_non_manhattan.py
+-rw-r--r--   0        0        0    12399 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/07_mask.py
+-rw-r--r--   0        0        0    15157 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/08_pdk.py
+-rw-r--r--   0        0        0    11094 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/08_pdk_examples.py
+-rw-r--r--   0        0        0     8585 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/09_pdk_import.py
+-rw-r--r--   0        0        0    17564 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/10_yaml_component.py
+-rw-r--r--   0        0        0     4684 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/11_get_netlist.py
+-rw-r--r--   0        0        0     2114 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/11_get_netlist_spice.py
+-rw-r--r--   0        0        0     4477 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/21_drc.py
+-rw-r--r--   0        0        0      437 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/Makefile
+-rw-r--r--   0        0        0     6217 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/_0_python.py
+-rw-r--r--   0        0        0    16372 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/_1_git.py
+-rw-r--r--   0        0        0     1092 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/_2_klayout.py
+-rw-r--r--   0        0        0     1384 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/_3_vscode.py
+-rw-r--r--   0        0        0     8163 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/_4_gdsfactory.py
+-rw-r--r--   0        0        0     4412 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/common_mistakes.py
+-rw-r--r--   0        0        0     4018 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/dataprep.py
+-rw-r--r--   0        0        0     2660 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/declarative_cell.py
+-rw-r--r--   0        0        0    13148 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/inkscape_align.png
+-rw-r--r--   0        0        0    14726 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/inkscape_distribute.png
+-rw-r--r--   0        0        0    71039 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/pathlength_report.png
+-rw-r--r--   0        0        0    67563 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png
+-rw-r--r--   0        0        0     6558 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/rib_strip_autotransition.py
+-rw-r--r--   0        0        0      591 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml
+-rw-r--r--   0        0        0      726 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml
+-rw-r--r--   0        0        0      822 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml
+-rw-r--r--   0        0        0     1417 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml
+-rw-r--r--   0        0        0     1508 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml
+-rw-r--r--   0        0        0     1405 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml
+-rw-r--r--   0        0        0      600 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml
+-rw-r--r--   0        0        0      614 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml
+-rw-r--r--   0        0        0     1152 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml
+-rw-r--r--   0        0        0     1066 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml
+-rw-r--r--   0        0        0      778 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml
+-rw-r--r--   0        0        0     1423 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml
+-rw-r--r--   0        0        0      857 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml
+-rw-r--r--   0        0        0        0 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     3668 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      233 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/fab_c_to_updk.py
+-rw-r--r--   0        0        0      475 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1893 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1745 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     3102 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     2419 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     2252 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     2237 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     6899 2023-08-03 12:18:28.631784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     6857 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     3434 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0     4531 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1569 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/show.py
+-rw-r--r--   0        0        0      525 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     1689 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4254 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      308 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0      343 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/color_utils.py
+-rw-r--r--   0        0        0     7550 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1041 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    19086 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    41893 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0      674 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/xml_utils.py
+-rw-r--r--   0        0        0     1413 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/technology/yaml_utils.py
+-rw-r--r--   0        0        0    11084 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/typings.py
+-rw-r--r--   0        0        0     5489 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/watch.py
+-rw-r--r--   0        0        0     7419 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     4328 2023-08-03 12:18:28.635784 gdsfactory-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11987 1970-01-01 00:00:00.000000 gdsfactory-7.0.1/PKG-INFO
```

### Comparing `gdsfactory-7.0.0/LICENSE` & `gdsfactory-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/README.md` & `gdsfactory-7.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,50 @@
-# gdsfactory 7.0.0
+# gdsfactory 7.0.1
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![Downloads](https://pepy.tech/badge/gdsfactory)](https://pepy.tech/project/gdsfactory)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gdsfactory)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gdsfactory)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gdsfactory)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gdsfactory/binder-sandbox/HEAD)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gdsfactory/gdsfactory)
 
 ![logo](https://i.imgur.com/cN1ZWq8.png)
 
-gdsfactory: An open source platform for end to-end chip design and validation.
+gdsfactory: Your open source platform for end to-end chip design and validation.
 
-gdsfactory is a python library to design chips (Photonics, Analog, Quantum, MEMs, ...), objects for 3D printing or PCBs.
-
-You can describe your hardware in code (python or YAML), verify it (DRC, simulation, extraction) and validate it (to make sure it meets your specifications after fabrication).
+Welcome to gdsfactory, a Python library designed for crafting chips (Photonics, Analog, Quantum, MEMs, and more), 3D printed objects, and PCBs.
+Here, you can code your hardware design in Python or YAML, perform verification through DRC, simulation, and extraction, and validate in the lab to ensure your fabricated chip meets your specifications.
 
 ![workflow](https://i.imgur.com/abvxJJw.png)
 
-It provides you and end to end design flow to:
 
-- Design (Layout, Simulation, Optimization)
-  - Define Components using parametric cells functions in python or YAML.
-  - Test component settings, ports and geometry to avoid unwanted regressions.
-  - Capture design intent in a schematic.
-- Verify (DRC, DFM, LVS)
-  - Run simulations directly from the layout thanks to the simulation interfaces. No need to draw the geometry more than once.
-    - Run Component simulations (solve modes, FDTD, EME, TCAD, thermal ...)
-    - Run Circuit simulations from the Component netlist (Sparameters, Spice ...)
-    - Build Component models and study Design For Manufacturing.
-  - Create DRC rule decks in Klayout.
-  - Ensure complex layouts match their design intent (Layout Versus Schematic).
-- Validate
-  - Define layout and test protocols simultaneously, so when the chips come back you already know how to test and analyze them.
-  - Model extraction: extract the important parameters for each component.
-  - Build a data pipeline from raw data, to structured data and dashboards for monitoring your chip performance.
+We facilitate an end-to-end design flow for you to:
 
-As input, you write python or YAML code.
+- **Design (Layout, Simulation, Optimization)**: Utilize parametric cell functions in Python or YAML to define components. Test component settings, ports, and geometry to avoid unwanted regressions, and capture design intent in a schematic.
+- **Verify (DRC, DFM, LVS)**: Run simulations directly from the layout using our simulation interfaces, removing the need to duplicate geometry drawings. Conduct component and circuit simulations, study design for manufacturing, and ensure complex layouts match their design intent through Layout Versus Schematic verification.
+- **Validate**: Define layout and test protocols simultaneously for efficient chip analysis post-fabrication. Extract essential component parameters, and build a data pipeline from raw data to structured data, and dashboards for monitoring chip performance.
 
-As output you write a GDSII or OASIS file that you can send to your foundry for fabrication.
-It also exports component settings (for measurement and data analysis) and netlists (for circuit simulations) in YAML.
+Your input: Python or YAML text.
+Your output: A GDSII or OASIS file for fabrication, alongside component settings (for measurement and data analysis) and netlists (for circuit simulations) in YAML.
 
 ![layout_to_components](https://i.imgur.com/S96RSil.png)
 
 ![flow](https://i.imgur.com/XbhWJDz.png)
 
-It provides you a common syntax for design (KLayout, gdstk, Ansys Lumerical, tidy3d, MEEP, MPB, DEVSIM, SAX, MEOW ...), verification and validation.
+We provide a common syntax for design (KLayout, gdstk, Ansys Lumerical, tidy3d, MEEP, MPB, DEVSIM, SAX, MEOW ...), verification, and validation.
+
+![tool interfaces](https://i.imgur.com/oHKZ7hW.png)
 
-![tool interfaces](https://i.imgur.com/9fNLRvJ.png)
+Numerous foundries have gdsfactory PDKs available. You may need to contact your foundry to access their gdsfactory PDK, as some are provided under NDA only.
 
-Multiple foundries have gdsfactory PDKs available. Talk to your foundry to access their gdsfactory PDK as some are only provided under NDA:
+Available foundries include:
 
 - AIM photonics PDK
 - AMF photonics PDK
 - TowerSemi PH18 photonics PDK
 - GlobalFoundries 45SPCLO Photonics PDK
 - IMEC photonics PDK
 - HHI Photonics PDK
@@ -66,59 +54,66 @@
 - [VTT](https://github.com/gdsfactory/vtt) (open source)
 
 You can also access:
 
 - instructions on [how to build your own PDK](https://gdsfactory.github.io/gdsfactory/notebooks/08_pdk.html)
 - instructions on [how to import a PDK from a library of fixed GDS cells](https://gdsfactory.github.io/gdsfactory/notebooks/09_pdk_import.html)
 
-## Installation
+![foundry-pdks](https://i.imgur.com/zngqi0B.png)
 
-Use python3.10 or python3.11, as some tools like kfactory are not available for older versions of python. We recommend [VSCode](https://code.visualstudio.com/) as an IDE.
+## Installation
 
-If you don't have python installed on your system you can [download anaconda](https://www.anaconda.com/download/)
+We support Python 3.10 or 3.11, and [VSCode](https://code.visualstudio.com/) as an IDE. If you do not have Python installed, you can [download Anaconda](https://www.anaconda.com/download/).
 
-Once you have python installed, open Anaconda Prompt as Administrator and then install the latest gdsfactory core conda (from conda-forge channel) and most plugins using pip.
+Upon Python installation, open Anaconda Prompt as Administrator and install the latest gdsfactory core conda (from the conda-forge channel) and Optional `cad` visualization extras using pip.
 
 ![anaconda prompt](https://i.imgur.com/eKk2bbs.png)
 
+
 ```
 conda install -c conda-forge gdsfactory -y
-pip install gdsfactory --upgrade
+pip install "gdsfactory[cad]"--upgrade
 ```
 
 Then you can install Klayout-live `klive` integration in the klayout GUI `Tools --> Manage Packages --> Install New Packages --> Klive` as well as the genericpdk layermap `Tools --> Manage Packages --> Install New Packages --> gdsfactory` and restart klayout.
 
 ### Update gdsfactory
 
-You can `pip install gdsfactory --upgrade`
+You can upgrade your gdsfactory package using the following command:
 
-Notice that some PDKs may only work for a specific version of gdsfactory, so make sure you install the correct gdsfactory version specified in the `pyproject.toml` file. This will automatically happen when you install gdsfactory as one of the PDK dependencies. For example `pip install gf180` will install the latest gdsfactory version that has been tested for the GlobalFoundries180 PDK.
+```
+pip install gdsfactory[cad] --upgrade
+```
+
+Please note that some PDKs may only work for a specific version of gdsfactory. Ensure you install the correct gdsfactory version specified in the pyproject.toml file. This will automatically happen when you install gdsfactory as one of the PDK dependencies. For example, pip install gf180 will install the latest gdsfactory version tested for the GlobalFoundries180 PDK.
 
-This code will tell you which gdsfactory you are using:
+To determine your current gdsfactory version, use the following code:
 
 ```
 import gdsfactory as gf
 
 gf.config.print_version()
 ```
 
 ### Docker container
 
-Alternatively, one may use the pre-built Docker image from [hub.docker.com/r/joamatab/gdsfactory](https://hub.docker.com/r/joamatab/gdsfactory) or build it yourself with:
+As an alternative, you can use the pre-built Docker image from [hub.docker.com/r/joamatab/gdsfactory](https://hub.docker.com/r/joamatab/gdsfactory) or build it yourself with:
+
 
 ```bash
 docker build -t joamatab/gdsfactory .
 ```
-For example, VS Code supports development inside a container, see [Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers) for details.
+
+For instance, VS Code supports development inside a container. See [Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers) for details.
 
 ## Plugins
 
-Plugins are hosted in a separate [repo](https://github.com/gdsfactory/gplugins) and installed as part of gdsfactory.
-Notice that plugins allow you to interface with different tools and some of them need to be installed separately.
-Take a look at the [gplugins documentation](https://gdsfactory.github.io/gplugins/)
+We maintain gdsfactory plugins in a [separate package](https://github.com/gdsfactory/gplugins)
+These plugins enable interfaces with different tools, and you might need to install some of the tools separately.
+For more details, please visit the [gplugins documentation](https://gdsfactory.github.io/gplugins/).
 
 ## Getting started
 
 - [See slides](https://docs.google.com/presentation/d/1_ZmUxbaHWo_lQP17dlT1FWX-XD8D9w7-FcuEih48d_0/edit#slide=id.g11711f50935_0_5)
 - [Read docs](https://gdsfactory.github.io/gdsfactory/)
 - [![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://www.youtube.com/@gdsfactory625/playlists)
 - [![Join the chat at https://gitter.im/gdsfactory-dev/community](https://badges.gitter.im/gdsfactory-dev/community.svg)](https://gitter.im/gdsfactory-dev/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
@@ -152,13 +147,12 @@
 
 ---
 
 "I use gdsfactory for all of my photonic tape-outs. The Python interface makes it easy to version control individual photonic components as well as entire layouts, while integrating seamlessly with KLayout and most standard photonic simulation tools, both open-source and commercial.
 
 <div style="text-align: right; margin-right: 10%;">Thomas Dorch - <strong>Freedom Photonics</strong></div>
 
-
 ## Contributors
 
 Thanks to all the contributors that make this awesome project possible!
 
 [![Meet our contributors!](https://contrib.rocks/image?repo=gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/graphs/contributors)
```

### Comparing `gdsfactory-7.0.0/gdsfactory/__init__.py` & `gdsfactory-7.0.1/gdsfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,8 @@
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
 
 
-__version__ = "7.0.0"
+__version__ = "7.0.1"
```

### Comparing `gdsfactory-7.0.0/gdsfactory/add_keepout.py` & `gdsfactory-7.0.1/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_labels.py` & `gdsfactory-7.0.1/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_loopback.py` & `gdsfactory-7.0.1/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_padding.py` & `gdsfactory-7.0.1/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_pins.py` & `gdsfactory-7.0.1/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_ports.py` & `gdsfactory-7.0.1/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_tapers.py` & `gdsfactory-7.0.1/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-7.0.1/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/add_termination.py` & `gdsfactory-7.0.1/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/asserts.py` & `gdsfactory-7.0.1/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/cell.py` & `gdsfactory-7.0.1/gdsfactory/cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/cli.py` & `gdsfactory-7.0.1/gdsfactory/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "7.0.0"
+VERSION = "7.0.1"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-7.0.0/gdsfactory/component.py` & `gdsfactory-7.0.1/gdsfactory/component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/component_layout.py` & `gdsfactory-7.0.1/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/component_reference.py` & `gdsfactory-7.0.1/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/C.py` & `gdsfactory-7.0.1/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/L.py` & `gdsfactory-7.0.1/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/__init__.py` & `gdsfactory-7.0.1/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/add_fiducials.py` & `gdsfactory-7.0.1/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-7.0.1/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/add_trenches.py` & `gdsfactory-7.0.1/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/align.py` & `gdsfactory-7.0.1/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/array_component.py` & `gdsfactory-7.0.1/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/array_with_fanout.py` & `gdsfactory-7.0.1/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/array_with_via.py` & `gdsfactory-7.0.1/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/awg.py` & `gdsfactory-7.0.1/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/bbox.py` & `gdsfactory-7.0.1/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/bend_circular.py` & `gdsfactory-7.0.1/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-7.0.1/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/bend_euler.py` & `gdsfactory-7.0.1/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/bend_port.py` & `gdsfactory-7.0.1/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/bend_s.py` & `gdsfactory-7.0.1/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/bezier.py` & `gdsfactory-7.0.1/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cavity.py` & `gdsfactory-7.0.1/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cdc.py` & `gdsfactory-7.0.1/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cdsem_all.py` & `gdsfactory-7.0.1/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-7.0.1/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-7.0.1/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cdsem_straight.py` & `gdsfactory-7.0.1/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-7.0.1/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/circle.py` & `gdsfactory-7.0.1/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-7.0.1/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-7.0.1/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-7.0.1/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-7.0.1/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/compass.py` & `gdsfactory-7.0.1/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/component_lattice.py` & `gdsfactory-7.0.1/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/component_lattice_generic.py` & `gdsfactory-7.0.1/gdsfactory/components/component_lattice_generic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/component_sequence.py` & `gdsfactory-7.0.1/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/copy_layers.py` & `gdsfactory-7.0.1/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler90.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler90bend.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_bent.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_bent.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_full.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_ring.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_straight.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-7.0.1/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cross.py` & `gdsfactory-7.0.1/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-7.0.1/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-7.0.1/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-7.0.1/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cutback_2x2.py` & `gdsfactory-7.0.1/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cutback_bend.py` & `gdsfactory-7.0.1/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cutback_component.py` & `gdsfactory-7.0.1/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/cutback_splitter.py` & `gdsfactory-7.0.1/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/dbr.py` & `gdsfactory-7.0.1/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/dbr_tapered.py` & `gdsfactory-7.0.1/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/delay_snake.py` & `gdsfactory-7.0.1/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/delay_snake2.py` & `gdsfactory-7.0.1/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/delay_snake3.py` & `gdsfactory-7.0.1/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-7.0.1/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/dicing_lane.py` & `gdsfactory-7.0.1/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/die.py` & `gdsfactory-7.0.1/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/die_bbox.py` & `gdsfactory-7.0.1/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-7.0.1/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/disk.py` & `gdsfactory-7.0.1/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-7.0.1/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ellipse.py` & `gdsfactory-7.0.1/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/extend_ports_list.py` & `gdsfactory-7.0.1/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/extension.py` & `gdsfactory-7.0.1/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/fiber.py` & `gdsfactory-7.0.1/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/fiber_array.py` & `gdsfactory-7.0.1/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/fiducial_squares.py` & `gdsfactory-7.0.1/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-7.0.1/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-7.0.1/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/greek_cross.py` & `gdsfactory-7.0.1/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/hline.py` & `gdsfactory-7.0.1/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-7.0.1/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/litho_calipers.py` & `gdsfactory-7.0.1/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/litho_ruler.py` & `gdsfactory-7.0.1/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/litho_steps.py` & `gdsfactory-7.0.1/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/logo.py` & `gdsfactory-7.0.1/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/loop_mirror.py` & `gdsfactory-7.0.1/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mmi.py` & `gdsfactory-7.0.1/gdsfactory/components/mmi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mmi1x2.py` & `gdsfactory-7.0.1/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-7.0.1/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mmi2x2.py` & `gdsfactory-7.0.1/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-7.0.1/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-7.0.1/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mode_converter.py` & `gdsfactory-7.0.1/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzi.py` & `gdsfactory-7.0.1/gdsfactory/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzi_arm.py` & `gdsfactory-7.0.1/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzi_arms.py` & `gdsfactory-7.0.1/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzi_lattice.py` & `gdsfactory-7.0.1/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-7.0.1/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-7.0.1/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzit.py` & `gdsfactory-7.0.1/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzit_lattice.py` & `gdsfactory-7.0.1/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/mzm.py` & `gdsfactory-7.0.1/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/nxn.py` & `gdsfactory-7.0.1/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/optimal_90deg.py` & `gdsfactory-7.0.1/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-7.0.1/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/optimal_step.py` & `gdsfactory-7.0.1/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/pack_doe.py` & `gdsfactory-7.0.1/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/pad.py` & `gdsfactory-7.0.1/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/pad_gsg.py` & `gdsfactory-7.0.1/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/pads_shorted.py` & `gdsfactory-7.0.1/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-7.0.1/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ramp.py` & `gdsfactory-7.0.1/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/rectangle.py` & `gdsfactory-7.0.1/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-7.0.1/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/rectangular_ring.py` & `gdsfactory-7.0.1/gdsfactory/components/rectangular_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/regular_polygon.py` & `gdsfactory-7.0.1/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/resistance_meander.py` & `gdsfactory-7.0.1/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/resistance_sheet.py` & `gdsfactory-7.0.1/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring.py` & `gdsfactory-7.0.1/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_crow.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_double.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_double_bend_coupler.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_double_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_double_heater.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_double_pn.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_section_based.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_single.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_single_array.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_single_dut.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_single_heater.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/ring_single_pn.py` & `gdsfactory-7.0.1/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/seal_ring.py` & `gdsfactory-7.0.1/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/snspd.py` & `gdsfactory-7.0.1/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/spiral_double.py` & `gdsfactory-7.0.1/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/spiral_external_io.py` & `gdsfactory-7.0.1/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/spiral_heater.py` & `gdsfactory-7.0.1/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-7.0.1/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/splitter_chain.py` & `gdsfactory-7.0.1/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/splitter_tree.py` & `gdsfactory-7.0.1/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight.py` & `gdsfactory-7.0.1/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_array.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_pin.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/straight_rib.py` & `gdsfactory-7.0.1/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/switch_tree.py` & `gdsfactory-7.0.1/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/taper.py` & `gdsfactory-7.0.1/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-7.0.1/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/taper_cross_section.py` & `gdsfactory-7.0.1/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/taper_from_csv.py` & `gdsfactory-7.0.1/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/taper_parabolic.py` & `gdsfactory-7.0.1/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/terminator.py` & `gdsfactory-7.0.1/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/text.py` & `gdsfactory-7.0.1/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/text_freetype.py` & `gdsfactory-7.0.1/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/text_rectangular.py` & `gdsfactory-7.0.1/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-7.0.1/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/triangles.py` & `gdsfactory-7.0.1/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/verniers.py` & `gdsfactory-7.0.1/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/version_stamp.py` & `gdsfactory-7.0.1/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/via.py` & `gdsfactory-7.0.1/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/via_corner.py` & `gdsfactory-7.0.1/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/via_cutback.py` & `gdsfactory-7.0.1/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/via_stack.py` & `gdsfactory-7.0.1/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/via_stack_slot.py` & `gdsfactory-7.0.1/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-7.0.1/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/wafer.py` & `gdsfactory-7.0.1/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/wire.py` & `gdsfactory-7.0.1/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/components/wire_sbend.py` & `gdsfactory-7.0.1/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/config.py` & `gdsfactory-7.0.1/gdsfactory/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from pydantic import BaseModel, BaseSettings, Field
 from rich.console import Console
 from rich.table import Table
 
 if TYPE_CHECKING:
     from loguru import Logger
 
-__version__ = "7.0.0"
+__version__ = "7.0.1"
 PathType = str | pathlib.Path
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-7.0.0/gdsfactory/constants.py` & `gdsfactory-7.0.1/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/cross_section.py` & `gdsfactory-7.0.1/gdsfactory/cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/decorators.py` & `gdsfactory-7.0.1/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/difftest.py` & `gdsfactory-7.0.1/gdsfactory/difftest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/difftest_git.py` & `gdsfactory-7.0.1/gdsfactory/difftest_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/events.py` & `gdsfactory-7.0.1/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/export/to_3d.py` & `gdsfactory-7.0.1/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/export/to_gerber.py` & `gdsfactory-7.0.1/gdsfactory/export/to_gerber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/export/to_np.py` & `gdsfactory-7.0.1/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/export/to_stl.py` & `gdsfactory-7.0.1/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/fill.py` & `gdsfactory-7.0.1/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/font.py` & `gdsfactory-7.0.1/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/functions.py` & `gdsfactory-7.0.1/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/README.md` & `gdsfactory-7.0.1/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/__init__.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/containers.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 1% similar despite different names*

#### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>7.0.0</version>
+  <version>7.0.1</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 1% similar despite different names*

#### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;7.0.0&quot;
+__version__ = &quot;7.0.1&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/layers.lyp` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/layers.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/tech.lyt` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-7.0.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-7.0.1/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/generic_tech/simulation_settings.py` & `gdsfactory-7.0.1/gdsfactory/generic_tech/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/__init__.py` & `gdsfactory-7.0.1/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/boolean.py` & `gdsfactory-7.0.1/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-7.0.1/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-7.0.1/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-7.0.1/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-7.0.1/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-7.0.1/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/check_space.py` & `gdsfactory-7.0.1/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/check_width.py` & `gdsfactory-7.0.1/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-7.0.1/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-7.0.1/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/fillet.py` & `gdsfactory-7.0.1/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/functions.py` & `gdsfactory-7.0.1/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/invert.py` & `gdsfactory-7.0.1/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/layer_priority.py` & `gdsfactory-7.0.1/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/manhattanize.py` & `gdsfactory-7.0.1/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/maskprep.py` & `gdsfactory-7.0.1/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-7.0.1/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/offset.py` & `gdsfactory-7.0.1/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/outline.py` & `gdsfactory-7.0.1/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/trim.py` & `gdsfactory-7.0.1/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/union.py` & `gdsfactory-7.0.1/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/write_connectivity.py` & `gdsfactory-7.0.1/gdsfactory/geometry/write_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/write_drc.py` & `gdsfactory-7.0.1/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/geometry/xor_diff.py` & `gdsfactory-7.0.1/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/get_factories.py` & `gdsfactory-7.0.1/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/get_netlist.py` & `gdsfactory-7.0.1/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/get_netlist_flat.py` & `gdsfactory-7.0.1/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/grid.py` & `gdsfactory-7.0.1/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/install.py` & `gdsfactory-7.0.1/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/klive.py` & `gdsfactory-7.0.1/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/labels/__init__.py` & `gdsfactory-7.0.1/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-7.0.1/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/labels/ehva.py` & `gdsfactory-7.0.1/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-7.0.1/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/labels/siepic.py` & `gdsfactory-7.0.1/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/labels/write_labels.py` & `gdsfactory-7.0.1/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/name.py` & `gdsfactory-7.0.1/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/pack.py` & `gdsfactory-7.0.1/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/path.py` & `gdsfactory-7.0.1/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/pdk.py` & `gdsfactory-7.0.1/gdsfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/picmodel.py` & `gdsfactory-7.0.1/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/pixelate.py` & `gdsfactory-7.0.1/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/polygon.py` & `gdsfactory-7.0.1/gdsfactory/polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/port.py` & `gdsfactory-7.0.1/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/quickplotter.py` & `gdsfactory-7.0.1/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/__init__.py` & `gdsfactory-7.0.1/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/from_dphox.py` & `gdsfactory-7.0.1/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/from_gdspaths.py` & `gdsfactory-7.0.1/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/from_np.py` & `gdsfactory-7.0.1/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/from_phidl.py` & `gdsfactory-7.0.1/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/from_updk.py` & `gdsfactory-7.0.1/gdsfactory/read/from_updk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/from_yaml.py` & `gdsfactory-7.0.1/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/from_yaml_template.py` & `gdsfactory-7.0.1/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/import_gds.py` & `gdsfactory-7.0.1/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/read/labels.py` & `gdsfactory-7.0.1/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/route_info.py` & `gdsfactory-7.0.1/gdsfactory/route_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,57 @@
+from gdsfactory.serialization import clean_value_json
 from gdsfactory.typings import CrossSectionSpec
 
 
 def route_info(
-    cs_type: str, length: float, length_eff: float = None, taper: bool = False, **kwargs
-):
-    """
-    Gets a dictionary of route info, used by pathlength analysis.
+    cs_type: str,
+    length: float,
+    length_eff: float | None = None,
+    taper: bool = False,
+    **kwargs,
+) -> dict[str, float | str]:
+    """Returns route info dict for pathlength analysis.
 
     Args:
-        cs_type: cross section type
-        length: length
-        length_eff: effective length (i.e. an equivalent straight length of a bend)
-        taper: True if this component is a taper
-        kwargs: other attributes to track
+        cs_type: cross section type.
+        length: length.
+        length_eff: effective length (i.e. an equivalent straight length of a bend).
+        taper: True if this component is a taper.
+        kwargs: other attributes to track.
+
     Returns:
-        A dictionary of routing attributes
+        A dictionary of routing attributes.
     """
     if length_eff is None:
         length_eff = length
 
     d = {
-        "type": cs_type,
+        "type": clean_value_json(cs_type),
         "length": length_eff,
         f"{cs_type}_length": length_eff,
         "weight": length_eff,
     }
     if taper:
         d[f"{cs_type}_taper_length"] = length
-    d.update(kwargs)
+    d |= kwargs
     return d
 
 
 def route_info_from_cs(
-    cs: CrossSectionSpec, length: float, length_eff: float = None, **kwargs
-):
-    """
-    Gets a dictionary of route info, used by pathlength analysis.
+    cs: CrossSectionSpec, length: float, length_eff: float | None = None, **kwargs
+) -> dict[str, float | str]:
+    """Returns route info dict for pathlength analysis.
 
     Args:
-        cs: cross section object or spec
-        length: length
-        length_eff: effective length (i.e. an equivalent straight length of a bend)
-        kwargs: other attributes to track
+        cs: cross section object or spec.
+        length: length.
+        length_eff: effective length (i.e. an equivalent straight length of a bend).
+        kwargs: other attributes to track.
+
     Returns:
-        A dictionary of routing attributes
+        A dictionary of routing attributes.
     """
     from gdsfactory import get_cross_section
 
     x = get_cross_section(cs)
-    cs_type = x.info.get("type", str(cs))
+    cs_type = x.info.get("type", clean_value_json(cs))
     return route_info(cs_type, length=length, length_eff=length_eff, **kwargs)
```

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/__init__.py` & `gdsfactory-7.0.1/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-7.0.1/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-7.0.1/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-7.0.1/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-7.0.1/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-7.0.1/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/add_pads.py` & `gdsfactory-7.0.1/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/all_angle.py` & `gdsfactory-7.0.1/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/auto_taper.py` & `gdsfactory-7.0.1/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/factories.py` & `gdsfactory-7.0.1/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/fanout.py` & `gdsfactory-7.0.1/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/fanout2x2.py` & `gdsfactory-7.0.1/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_bundle.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_input_labels.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_route.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_route_astar.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-7.0.1/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/manhattan.py` & `gdsfactory-7.0.1/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/path_length_matching.py` & `gdsfactory-7.0.1/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-7.0.1/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-7.0.1/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-7.0.1/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/route_quad.py` & `gdsfactory-7.0.1/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/route_sharp.py` & `gdsfactory-7.0.1/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/route_south.py` & `gdsfactory-7.0.1/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/sort_ports.py` & `gdsfactory-7.0.1/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/routing/utils.py` & `gdsfactory-7.0.1/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-7.0.1/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/03_move.py` & `gdsfactory-7.0.1/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/04_connect.py` & `gdsfactory-7.0.1/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-7.0.1/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-7.0.1/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-7.0.1/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/11_component_layout.py` & `gdsfactory-7.0.1/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/12_component_refs.py` & `gdsfactory-7.0.1/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-7.0.1/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-7.0.1/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-7.0.1/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-7.0.1/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/17_ports.py` & `gdsfactory-7.0.1/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/20_components.py` & `gdsfactory-7.0.1/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/21_add_fiber_array.py` & `gdsfactory-7.0.1/gdsfactory/samples/21_add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/22_add_fiber_single.py` & `gdsfactory-7.0.1/gdsfactory/samples/22_add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/22_add_pads.py` & `gdsfactory-7.0.1/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/23_reticle.py` & `gdsfactory-7.0.1/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/23_reticle_passives_grid.py` & `gdsfactory-7.0.1/gdsfactory/samples/23_reticle_passives_grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/23_reticle_passives_pack.py` & `gdsfactory-7.0.1/gdsfactory/samples/23_reticle_passives_pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/24_doe_2.py` & `gdsfactory-7.0.1/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/24_doe_3.py` & `gdsfactory-7.0.1/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/30_lidar.py` & `gdsfactory-7.0.1/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-7.0.1/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-7.0.1/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/big_device.py` & `gdsfactory-7.0.1/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-7.0.1/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-7.0.1/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-7.0.1/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/layers.py` & `gdsfactory-7.0.1/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/lvs.py` & `gdsfactory-7.0.1/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/demo/pcell.py` & `gdsfactory-7.0.1/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-7.0.1/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-7.0.1/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/00_geometry.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/00_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/01_references.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/02_movement.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/02_movement.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/03_Path_CrossSection.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/03_Path_CrossSection.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/03_cells_autoname_and_cache.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/03_layer_stack.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/03_layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_geometry.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_hierarchy.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_hierarchy.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_pack.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_components_shapes.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_components_shapes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_routing.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_routing_electrical.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_routing_electrical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/04_routing_non_manhattan.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/04_routing_non_manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/07_mask.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/07_mask.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/08_pdk.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/08_pdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 #
 # Make sure you create a `test_components.py` file for pytest to test your PDK. See for example the tests in the [ubc PDK](https://github.com/gdsfactory/ubc)
 #
 # Pytest-regressions automatically creates the CSV and YAML files for you, as well `gdsfactory.gdsdiff` will store the reference GDS in ref_layouts and check for geometry differences using XOR.
 #
 # gdsfactory is **not** backwards compatible, which means that the package will keep improving and evolving.
 #
-# 1. To make your work stable you should install a specific version and [pin the version](https://martin-thoma.com/python-requirements/) in your `requirements.txt` or `pyproject.toml` as `gdsfactory==7.0.0` replacing `7.0.0` by whatever version you end up using.
+# 1. To make your work stable you should install a specific version and [pin the version](https://martin-thoma.com/python-requirements/) in your `requirements.txt` or `pyproject.toml` as `gdsfactory==7.0.1` replacing `7.0.1` by whatever version you end up using.
 # 2. Before you upgrade gdsfactory to a newer version make sure your tests pass to make sure that things behave as expected
 #
 #
 
 # +
 """This code tests all your cells in the PDK
```

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/08_pdk_examples.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/08_pdk_examples.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/09_pdk_import.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/09_pdk_import.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/10_yaml_component.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/10_yaml_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/11_get_netlist.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/11_get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/11_get_netlist_spice.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/11_get_netlist_spice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/21_drc.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/21_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/_0_python.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/_0_python.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/_1_git.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/_1_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/_2_klayout.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/_2_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/_3_vscode.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/_3_vscode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/_4_gdsfactory.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/_4_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/common_mistakes.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/common_mistakes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/dataprep.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/dataprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/declarative_cell.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/declarative_cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/inkscape_align.png` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/inkscape_align.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/inkscape_distribute.png` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/inkscape_distribute.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/pathlength_report.png` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/pathlength_report.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/images/pathlength_report_highlighted.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/rib_strip_autotransition.py` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/rib_strip_autotransition.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back2.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_around_the_back3.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_bundles01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_bundles02.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_bundles03.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_indirect.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_simple.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_final.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps02_initial.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_steps03.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml` & `gdsfactory-7.0.1/gdsfactory/samples/notebooks/yaml_pics/aar_wonky_connector.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/fab_c.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """FabC example."""
 
 from __future__ import annotations
 
 import pathlib
-from collections.abc import Callable
 from functools import partial
 
 from pydantic import BaseModel
 
 import gdsfactory as gf
-from gdsfactory.add_pins import add_pin_rectangle_inside
-from gdsfactory.component import Component
+from gdsfactory.add_pins import add_pins_inside1nm
 from gdsfactory.cross_section import strip
 from gdsfactory.port import select_ports
 from gdsfactory.technology import LayerLevel, LayerStack
 from gdsfactory.typings import Layer
 
 
 class LayerMap(BaseModel):
@@ -46,42 +44,15 @@
                 zmin=0.22 + 0.1,
                 thickness=0.4,
             ),
         )
     )
 
 
-def add_pins(
-    component: Component,
-    function: Callable = add_pin_rectangle_inside,
-    pin_length: float = 0.5,
-    port_layer: Layer = LAYER.PIN,
-    **kwargs,
-) -> Component:
-    """Add Pin port markers.
-
-    Args:
-        component: to add ports.
-        function: to add pins.
-        pin_length: pin length in um.
-        port_layer: for port.
-        function: kwargs.
-
-    """
-    for p in component.ports.values():
-        function(
-            component=component,
-            port=p,
-            layer=port_layer,
-            layer_label=port_layer,
-            pin_length=pin_length,
-            **kwargs,
-        )
-    return component
-
+add_pins = partial(add_pins_inside1nm, pin_length=0.5)
 
 # cross_sections
 
 xs_nc = partial(
     strip,
     width=WIDTH_NITRIDE_CBAND,
     layer=LAYER.WGN,
@@ -159,18 +130,18 @@
 LAYER_STACK = get_layer_stack_fab_c()
 SPARAMETERS_PATH = pathlib.Path.home() / "fabc"
 
 pdk = gf.Pdk(name="fab_c_demopdk", cells=cells, cross_sections=cross_sections)
 
 
 if __name__ == "__main__":
-    c1 = mmi1x2_nc()
-    print(c1.name)
+    c1 = bend_euler_nc()
+    d = c1.to_dict()
+    print(d)
     # c1 = mmi1x2_nc()
-    # d1 = c1.to_dict()
 
     # c2 = mmi1x2_nc(cache=False)
     # d2 = c2.to_dict()
 
     # from jsondiff import diff
 
     # d = diff(d1, d2)
```

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: bend_euler_e6ca1d65
+name: bend_euler_9272acf4
 ports:
   o1:
     center:
     - 0.0
     - 0.0
     layer:
     - 34
@@ -28,14 +28,21 @@
   changed:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -57,14 +64,21 @@
     angle: 90.0
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -91,14 +105,21 @@
       strip_length: 16.637
       type: strip
       weight: 16.637
     settings:
       add_bbox: null
       add_pins:
         function: add_pins
+        settings:
+          function:
+            function: add_pin_rectangle_inside
+            settings:
+              layer_label: null
+              pin_length: 0.001
+          pin_length: 0.5
       auto_widen: false
       auto_widen_minimum_length: 200.0
       bbox_layers:
       - - 36
         - 0
       bbox_offsets:
       - 3
@@ -130,8 +151,8 @@
       taper_length: 10.0
       width: 1.0
       width_wide: null
     type: strip
     width: 1.0
   info_version: 2
   module: gdsfactory.components.bend_euler
-  name: bend_euler_e6ca1d65
+  name: bend_euler_9272acf4
```

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: grating_coupler_ellipti_23f761ec
+name: grating_coupler_ellipti_b97d3fdf
 ports:
   o1:
     center:
     - 0.0
     - 0.0
     layer:
     - 34
@@ -28,14 +28,21 @@
   changed:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -67,14 +74,21 @@
     big_last_tooth: false
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -98,8 +112,8 @@
     wavelength: 1.554
   function_name: grating_coupler_elliptical
   info:
     polarization: te
     wavelength: 1.554
   info_version: 2
   module: gdsfactory.components.grating_coupler_elliptical
-  name: grating_coupler_ellipti_23f761ec
+  name: grating_coupler_ellipti_b97d3fdf
```

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: mmi1x2_d6895fd3
+name: mmi1x2_d3e2126d
 ports:
   o1:
     center:
     - -10.0
     - 0.0
     layer:
     - 34
@@ -40,14 +40,21 @@
   changed:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -75,14 +82,21 @@
   full:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -102,8 +116,8 @@
     width_mmi: 3
     width_taper: 1.0
     with_bbox: true
   function_name: mmi1x2
   info: {}
   info_version: 2
   module: gdsfactory.components.mmi1x2
-  name: mmi1x2_d6895fd3
+  name: mmi1x2_d3e2126d
```

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: mmi1x2_d48e5220
+name: mmi1x2_2bb20f1f
 ports:
   o1:
     center:
     - -10.0
     - 0.0
     layer:
     - 34
@@ -40,14 +40,21 @@
   changed:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -74,14 +81,21 @@
   full:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -101,8 +115,8 @@
     width_mmi: 2.5
     width_taper: 1.0
     with_bbox: true
   function_name: mmi1x2
   info: {}
   info_version: 2
   module: gdsfactory.components.mmi1x2
-  name: mmi1x2_d48e5220
+  name: mmi1x2_2bb20f1f
```

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: mzi_91c47883
+name: mzi_a1aa14b7
 ports:
   o1:
     center:
     - -10.0
     - 0.0
     layer:
     - 34
@@ -31,14 +31,21 @@
       settings:
         cross_section:
           function: cross_section
           settings:
             add_bbox: null
             add_pins:
               function: add_pins
+              settings:
+                function:
+                  function: add_pin_rectangle_inside
+                  settings:
+                    layer_label: null
+                    pin_length: 0.001
+                pin_length: 0.5
             bbox_layers:
             - - 36
               - 0
             bbox_offsets:
             - 3
             info:
               type: strip
@@ -50,14 +57,21 @@
         with_bbox: true
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -71,14 +85,21 @@
       settings:
         cross_section:
           function: cross_section
           settings:
             add_bbox: null
             add_pins:
               function: add_pins
+              settings:
+                function:
+                  function: add_pin_rectangle_inside
+                  settings:
+                    layer_label: null
+                    pin_length: 0.001
+                pin_length: 0.5
             bbox_layers:
             - - 36
               - 0
             bbox_offsets:
             - 3
             info:
               type: strip
@@ -94,14 +115,21 @@
       settings:
         cross_section:
           function: cross_section
           settings:
             add_bbox: null
             add_pins:
               function: add_pins
+              settings:
+                function:
+                  function: add_pin_rectangle_inside
+                  settings:
+                    layer_label: null
+                    pin_length: 0.001
+                pin_length: 0.5
             bbox_layers:
             - - 36
               - 0
             bbox_offsets:
             - 3
             info:
               type: strip
@@ -143,14 +171,21 @@
       settings:
         cross_section:
           function: cross_section
           settings:
             add_bbox: null
             add_pins:
               function: add_pins
+              settings:
+                function:
+                  function: add_pin_rectangle_inside
+                  settings:
+                    layer_label: null
+                    pin_length: 0.001
+                pin_length: 0.5
             bbox_layers:
             - - 36
               - 0
             bbox_offsets:
             - 3
             info:
               type: strip
@@ -163,14 +198,21 @@
     combiner: null
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -195,14 +237,21 @@
       settings:
         cross_section:
           function: cross_section
           settings:
             add_bbox: null
             add_pins:
               function: add_pins
+              settings:
+                function:
+                  function: add_pin_rectangle_inside
+                  settings:
+                    layer_label: null
+                    pin_length: 0.001
+                pin_length: 0.5
             bbox_layers:
             - - 36
               - 0
             bbox_offsets:
             - 3
             info:
               type: strip
@@ -218,14 +267,21 @@
       settings:
         cross_section:
           function: cross_section
           settings:
             add_bbox: null
             add_pins:
               function: add_pins
+              settings:
+                function:
+                  function: add_pin_rectangle_inside
+                  settings:
+                    layer_label: null
+                    pin_length: 0.001
+                pin_length: 0.5
             bbox_layers:
             - - 36
               - 0
             bbox_offsets:
             - 3
             info:
               type: strip
@@ -239,8 +295,8 @@
     straight_x_top: null
     straight_y: null
     with_splitter: true
   function_name: mzi
   info: {}
   info_version: 2
   module: gdsfactory.components.mzi
-  name: mzi_91c47883
+  name: mzi_a1aa14b7
```

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-7.0.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: straight_e6ca1d65
+name: straight_9272acf4
 ports:
   o1:
     center:
     - 0.0
     - 0.0
     layer:
     - 34
@@ -28,14 +28,21 @@
   changed:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -53,14 +60,21 @@
   full:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -76,14 +90,21 @@
   info:
     cross_section:
       function: cross_section
       settings:
         add_bbox: null
         add_pins:
           function: add_pins
+          settings:
+            function:
+              function: add_pin_rectangle_inside
+              settings:
+                layer_label: null
+                pin_length: 0.001
+            pin_length: 0.5
         bbox_layers:
         - - 36
           - 0
         bbox_offsets:
         - 3
         info:
           type: strip
@@ -99,14 +120,21 @@
       strip_length: 10.0
       type: strip
       weight: 10.0
     settings:
       add_bbox: null
       add_pins:
         function: add_pins
+        settings:
+          function:
+            function: add_pin_rectangle_inside
+            settings:
+              layer_label: null
+              pin_length: 0.001
+          pin_length: 0.5
       auto_widen: false
       auto_widen_minimum_length: 200.0
       bbox_layers:
       - - 36
         - 0
       bbox_offsets:
       - 3
@@ -138,8 +166,8 @@
       taper_length: 10.0
       width: 1.0
       width_wide: null
     type: strip
     width: 1.0
   info_version: 2
   module: gdsfactory.components.straight
-  name: straight_e6ca1d65
+  name: straight_9272acf4
```

### Comparing `gdsfactory-7.0.0/gdsfactory/serialization.py` & `gdsfactory-7.0.1/gdsfactory/serialization.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,34 +15,30 @@
 import toolz
 from omegaconf import DictConfig, OmegaConf
 
 DEFAULT_SERIALIZATION_MAX_DIGITS = 3
 """By default, the maximum number of digits retained when serializing float-like arrays"""
 
 
-def clean_dict(d: dict[str, Any]) -> dict[str, Any]:
-    """Cleans dictionary recursively."""
-    return {
-        k: clean_dict(dict(v)) if isinstance(v, dict) else clean_value_json(v)
-        for k, v in d.items()
-    }
-
-
 def get_string(value: Any) -> str:
     try:
         s = orjson.dumps(
             value, option=orjson.OPT_SERIALIZE_NUMPY, default=clean_value_name
         ).decode()
     except TypeError as e:
         print(f"Error serializing {value!r}")
         raise e
     return s
 
 
-def clean_value_json(value: Any) -> Any:
+def clean_dict(dictionary: dict) -> dict:
+    return {k: clean_value_json(v) for k, v in dictionary.items()}
+
+
+def clean_value_json(value: Any) -> str | int | float | dict | list | bool | None:
     """Return JSON serializable object."""
     from gdsfactory.path import Path
     from gdsfactory.pdk import get_active_pdk
 
     active_pdk = get_active_pdk()
     include_module = active_pdk.cell_decorator_settings.include_module
 
@@ -60,80 +56,74 @@
 
     elif isinstance(value, float | np.inexact | np.float64):
         return float(np.round(value, DEFAULT_SERIALIZATION_MAX_DIGITS))
 
     elif isinstance(value, np.ndarray):
         value = np.round(value, DEFAULT_SERIALIZATION_MAX_DIGITS)
         return orjson.loads(orjson.dumps(value, option=orjson.OPT_SERIALIZE_NUMPY))
+
     elif callable(value) and isinstance(value, functools.partial):
         sig = inspect.signature(value.func)
         args_as_kwargs = dict(zip(sig.parameters.keys(), value.args))
-        args_as_kwargs.update(**value.keywords)
+        args_as_kwargs.update(value.keywords)
         args_as_kwargs = clean_dict(args_as_kwargs)
-        # args_as_kwargs.pop("function", None)
 
         func = value.func
         while hasattr(func, "func"):
             func = func.func
         v = {
             "function": func.__name__,
             "settings": args_as_kwargs,
         }
         if include_module:
             v.update(module=func.__module__)
         return v
 
     elif hasattr(value, "to_dict"):
-        # print(type(value))
         return clean_dict(value.to_dict())
+
     elif callable(value) and isinstance(value, toolz.functoolz.Compose):
-        value = [clean_value_json(value.first)] + [
+        return [clean_value_json(value.first)] + [
             clean_value_json(func) for func in value.funcs
         ]
+
     elif callable(value) and hasattr(value, "__name__"):
-        value = (
+        return (
             {"function": value.__name__, "module": value.__module__}
             if include_module
             else {"function": value.__name__}
         )
+
     elif isinstance(value, Path):
-        value = value.hash_geometry()
+        return value.hash_geometry()
+
     elif isinstance(value, pathlib.Path):
-        value = value.stem
+        return value.stem
+
     elif isinstance(value, dict):
-        value = clean_dict(value.copy())
+        return clean_dict(value.copy())
+
     elif isinstance(value, DictConfig):
-        value = clean_dict(OmegaConf.to_container(value))
+        return clean_dict(OmegaConf.to_container(value))
 
     elif isinstance(value, list | tuple | set):
-        value = [clean_value_json(i) for i in value]
+        return [clean_value_json(i) for i in value]
 
     elif isinstance(value, gdstk.Polygon):
-        value = np.round(value.points, DEFAULT_SERIALIZATION_MAX_DIGITS)
+        return np.round(value.points, DEFAULT_SERIALIZATION_MAX_DIGITS)
+
     else:
         try:
             value_json = orjson.dumps(
                 value, option=orjson.OPT_SERIALIZE_NUMPY, default=clean_value_json
             )
-            value = orjson.loads(value_json)
+            return orjson.loads(value_json)
         except TypeError as e:
             print(f"Error serializing {value!r}")
             raise e
-    return value
-
-    # elif isinstance(value, (tuple, list, ListConfig)):
-    #     value = [clean_value_json(i) for i in value]
-    # elif value is None:
-    #     value = None
-    # elif hasattr(value, "name"):
-    #     value = value.name
-    # elif hasattr(value, "get_name"):
-    #     value = value.get_name()
-    # else:
-    #     value = str(value)
 
 
 def clean_value_name(value: Any) -> str:
     """Returns a string representation of an object."""
     # value1 = clean_value_json(value)
     return str(clean_value_json(value))
 
@@ -149,12 +139,17 @@
     # d = clean_value_json(f)
     # print(f"{d!r}")
     # f = partial(gf.c.straight, length=3)
     # c = f()
     # d = clean_value_json(c)
     # print(d, d)
 
-    f = partial(gf.cross_section.strip, width=3)
+    xs = partial(
+        gf.cross_section.strip,
+        width=3,
+        add_pins=gf.partial(gf.add_pins.add_pins_inside1nm, pin_length=0.1),
+    )
+    f = partial(gf.routing.add_fiber_array, cross_section=xs)
     c = f()
     d = clean_value_json(c)
     print(get_hash(d))
     print(d, d)
```

### Comparing `gdsfactory-7.0.0/gdsfactory/show.py` & `gdsfactory-7.0.1/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/simulation/__init__.py` & `gdsfactory-7.0.1/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/snap.py` & `gdsfactory-7.0.1/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/symbols.py` & `gdsfactory-7.0.1/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/technology/klayout_tech.py` & `gdsfactory-7.0.1/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/technology/layer_map.py` & `gdsfactory-7.0.1/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/technology/layer_stack.py` & `gdsfactory-7.0.1/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/technology/layer_views.py` & `gdsfactory-7.0.1/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/technology/xml_utils.py` & `gdsfactory-7.0.1/gdsfactory/technology/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/technology/yaml_utils.py` & `gdsfactory-7.0.1/gdsfactory/technology/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/typings.py` & `gdsfactory-7.0.1/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/watch.py` & `gdsfactory-7.0.1/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/gdsfactory/write_cells.py` & `gdsfactory-7.0.1/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.0.0/pyproject.toml` & `gdsfactory-7.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent"
 ]
 dependencies = [
   "click",
   "flatdict",
   "gdstk<1",
-  "gplugins<1",  # TODO: remove after we removing deprecated gdsfactory/simulation and gdsfactory/plugins
   "jinja2",
   "loguru<1",
   "matplotlib",
   "numpy",
   "omegaconf<3",
   "orjson",
   "pandas",
@@ -29,15 +28,26 @@
   "rectpack",
   "rich",
   "scipy",
   "shapely<3",
   "toolz",
   "tqdm",
   "types-PyYAML",
-  "watchdog",
+  "watchdog"
+]
+description = "python library to generate GDS layouts"
+keywords = ["eda", "photonics", "python"]
+license = {file = "LICENSE"}
+name = "gdsfactory"
+readme = "README.md"
+requires-python = ">=3.10"
+version = "7.0.1"
+
+[project.optional-dependencies]
+cad = [
   "freetype-py",
   "ipycytoscape",
   "ipyevents",
   "ipykernel",
   "ipympl",
   "ipytree",
   "ipywidgets",
@@ -45,25 +55,17 @@
   "kfactory[git,ipy]==0.7.5",
   "kweb==0.1.1",
   "mapbox_earcut",
   "networkx",
   "pyglet<2",
   "rich-click",
   "scikit-image",
-  "trimesh"
+  "trimesh",
+  "gplugins<1"  # TODO: remove after we remove deprecated gdsfactory/simulation and gdsfactory/plugins
 ]
-description = "python library to generate GDS layouts"
-keywords = ["eda", "photonics", "python"]
-license = {file = "LICENSE"}
-name = "gdsfactory"
-readme = "README.md"
-requires-python = ">=3.10"
-version = "7.0.0"
-
-[project.optional-dependencies]
 dev = [
   "autotyping",
   "black>=21",
   "doc8",
   "ipykernel",
   "jsondiff",
   "mypy",
```

### Comparing `gdsfactory-7.0.0/PKG-INFO` & `gdsfactory-7.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 7.0.0
+Version: 7.0.1
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
 Requires-Dist: flatdict
 Requires-Dist: gdstk<1
-Requires-Dist: gplugins<1
 Requires-Dist: jinja2
 Requires-Dist: loguru<1
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: omegaconf<3
 Requires-Dist: orjson
 Requires-Dist: pandas
@@ -27,30 +26,31 @@
 Requires-Dist: rich
 Requires-Dist: scipy
 Requires-Dist: shapely<3
 Requires-Dist: toolz
 Requires-Dist: tqdm
 Requires-Dist: types-PyYAML
 Requires-Dist: watchdog
-Requires-Dist: freetype-py
-Requires-Dist: ipycytoscape
-Requires-Dist: ipyevents
-Requires-Dist: ipykernel
-Requires-Dist: ipympl
-Requires-Dist: ipytree
-Requires-Dist: ipywidgets
-Requires-Dist: jupytext
-Requires-Dist: kfactory[git,ipy]==0.7.5
-Requires-Dist: kweb==0.1.1
-Requires-Dist: mapbox_earcut
-Requires-Dist: networkx
-Requires-Dist: pyglet<2
-Requires-Dist: rich-click
-Requires-Dist: scikit-image
-Requires-Dist: trimesh
+Requires-Dist: freetype-py ; extra == "cad"
+Requires-Dist: ipycytoscape ; extra == "cad"
+Requires-Dist: ipyevents ; extra == "cad"
+Requires-Dist: ipykernel ; extra == "cad"
+Requires-Dist: ipympl ; extra == "cad"
+Requires-Dist: ipytree ; extra == "cad"
+Requires-Dist: ipywidgets ; extra == "cad"
+Requires-Dist: jupytext ; extra == "cad"
+Requires-Dist: kfactory[git,ipy]==0.7.5 ; extra == "cad"
+Requires-Dist: kweb==0.1.1 ; extra == "cad"
+Requires-Dist: mapbox_earcut ; extra == "cad"
+Requires-Dist: networkx ; extra == "cad"
+Requires-Dist: pyglet<2 ; extra == "cad"
+Requires-Dist: rich-click ; extra == "cad"
+Requires-Dist: scikit-image ; extra == "cad"
+Requires-Dist: trimesh ; extra == "cad"
+Requires-Dist: gplugins<1 ; extra == "cad"
 Requires-Dist: autotyping ; extra == "dev"
 Requires-Dist: black>=21 ; extra == "dev"
 Requires-Dist: doc8 ; extra == "dev"
 Requires-Dist: ipykernel ; extra == "dev"
 Requires-Dist: jsondiff ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
@@ -62,72 +62,61 @@
 Requires-Dist: types-cachetools ; extra == "dev"
 Requires-Dist: xdoctest ; extra == "dev"
 Requires-Dist: autodoc_pydantic ; extra == "docs"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: jupyter-book==0.15.1 ; extra == "docs"
 Requires-Dist: pydata_sphinx_theme==0.13.1 ; extra == "docs"
 Requires-Dist: plotly ; extra == "docs"
+Provides-Extra: cad
 Provides-Extra: dev
 Provides-Extra: docs
 
-# gdsfactory 7.0.0
+# gdsfactory 7.0.1
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![Downloads](https://pepy.tech/badge/gdsfactory)](https://pepy.tech/project/gdsfactory)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gdsfactory)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gdsfactory)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gdsfactory)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gdsfactory/binder-sandbox/HEAD)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gdsfactory/gdsfactory)
 
 ![logo](https://i.imgur.com/cN1ZWq8.png)
 
-gdsfactory: An open source platform for end to-end chip design and validation.
+gdsfactory: Your open source platform for end to-end chip design and validation.
 
-gdsfactory is a python library to design chips (Photonics, Analog, Quantum, MEMs, ...), objects for 3D printing or PCBs.
-
-You can describe your hardware in code (python or YAML), verify it (DRC, simulation, extraction) and validate it (to make sure it meets your specifications after fabrication).
+Welcome to gdsfactory, a Python library designed for crafting chips (Photonics, Analog, Quantum, MEMs, and more), 3D printed objects, and PCBs.
+Here, you can code your hardware design in Python or YAML, perform verification through DRC, simulation, and extraction, and validate in the lab to ensure your fabricated chip meets your specifications.
 
 ![workflow](https://i.imgur.com/abvxJJw.png)
 
-It provides you and end to end design flow to:
 
-- Design (Layout, Simulation, Optimization)
-  - Define Components using parametric cells functions in python or YAML.
-  - Test component settings, ports and geometry to avoid unwanted regressions.
-  - Capture design intent in a schematic.
-- Verify (DRC, DFM, LVS)
-  - Run simulations directly from the layout thanks to the simulation interfaces. No need to draw the geometry more than once.
-    - Run Component simulations (solve modes, FDTD, EME, TCAD, thermal ...)
-    - Run Circuit simulations from the Component netlist (Sparameters, Spice ...)
-    - Build Component models and study Design For Manufacturing.
-  - Create DRC rule decks in Klayout.
-  - Ensure complex layouts match their design intent (Layout Versus Schematic).
-- Validate
-  - Define layout and test protocols simultaneously, so when the chips come back you already know how to test and analyze them.
-  - Model extraction: extract the important parameters for each component.
-  - Build a data pipeline from raw data, to structured data and dashboards for monitoring your chip performance.
+We facilitate an end-to-end design flow for you to:
 
-As input, you write python or YAML code.
+- **Design (Layout, Simulation, Optimization)**: Utilize parametric cell functions in Python or YAML to define components. Test component settings, ports, and geometry to avoid unwanted regressions, and capture design intent in a schematic.
+- **Verify (DRC, DFM, LVS)**: Run simulations directly from the layout using our simulation interfaces, removing the need to duplicate geometry drawings. Conduct component and circuit simulations, study design for manufacturing, and ensure complex layouts match their design intent through Layout Versus Schematic verification.
+- **Validate**: Define layout and test protocols simultaneously for efficient chip analysis post-fabrication. Extract essential component parameters, and build a data pipeline from raw data to structured data, and dashboards for monitoring chip performance.
 
-As output you write a GDSII or OASIS file that you can send to your foundry for fabrication.
-It also exports component settings (for measurement and data analysis) and netlists (for circuit simulations) in YAML.
+Your input: Python or YAML text.
+Your output: A GDSII or OASIS file for fabrication, alongside component settings (for measurement and data analysis) and netlists (for circuit simulations) in YAML.
 
 ![layout_to_components](https://i.imgur.com/S96RSil.png)
 
 ![flow](https://i.imgur.com/XbhWJDz.png)
 
-It provides you a common syntax for design (KLayout, gdstk, Ansys Lumerical, tidy3d, MEEP, MPB, DEVSIM, SAX, MEOW ...), verification and validation.
+We provide a common syntax for design (KLayout, gdstk, Ansys Lumerical, tidy3d, MEEP, MPB, DEVSIM, SAX, MEOW ...), verification, and validation.
+
+![tool interfaces](https://i.imgur.com/oHKZ7hW.png)
 
-![tool interfaces](https://i.imgur.com/9fNLRvJ.png)
+Numerous foundries have gdsfactory PDKs available. You may need to contact your foundry to access their gdsfactory PDK, as some are provided under NDA only.
 
-Multiple foundries have gdsfactory PDKs available. Talk to your foundry to access their gdsfactory PDK as some are only provided under NDA:
+Available foundries include:
 
 - AIM photonics PDK
 - AMF photonics PDK
 - TowerSemi PH18 photonics PDK
 - GlobalFoundries 45SPCLO Photonics PDK
 - IMEC photonics PDK
 - HHI Photonics PDK
@@ -137,59 +126,66 @@
 - [VTT](https://github.com/gdsfactory/vtt) (open source)
 
 You can also access:
 
 - instructions on [how to build your own PDK](https://gdsfactory.github.io/gdsfactory/notebooks/08_pdk.html)
 - instructions on [how to import a PDK from a library of fixed GDS cells](https://gdsfactory.github.io/gdsfactory/notebooks/09_pdk_import.html)
 
-## Installation
+![foundry-pdks](https://i.imgur.com/zngqi0B.png)
 
-Use python3.10 or python3.11, as some tools like kfactory are not available for older versions of python. We recommend [VSCode](https://code.visualstudio.com/) as an IDE.
+## Installation
 
-If you don't have python installed on your system you can [download anaconda](https://www.anaconda.com/download/)
+We support Python 3.10 or 3.11, and [VSCode](https://code.visualstudio.com/) as an IDE. If you do not have Python installed, you can [download Anaconda](https://www.anaconda.com/download/).
 
-Once you have python installed, open Anaconda Prompt as Administrator and then install the latest gdsfactory core conda (from conda-forge channel) and most plugins using pip.
+Upon Python installation, open Anaconda Prompt as Administrator and install the latest gdsfactory core conda (from the conda-forge channel) and Optional `cad` visualization extras using pip.
 
 ![anaconda prompt](https://i.imgur.com/eKk2bbs.png)
 
+
 ```
 conda install -c conda-forge gdsfactory -y
-pip install gdsfactory --upgrade
+pip install "gdsfactory[cad]"--upgrade
 ```
 
 Then you can install Klayout-live `klive` integration in the klayout GUI `Tools --> Manage Packages --> Install New Packages --> Klive` as well as the genericpdk layermap `Tools --> Manage Packages --> Install New Packages --> gdsfactory` and restart klayout.
 
 ### Update gdsfactory
 
-You can `pip install gdsfactory --upgrade`
+You can upgrade your gdsfactory package using the following command:
 
-Notice that some PDKs may only work for a specific version of gdsfactory, so make sure you install the correct gdsfactory version specified in the `pyproject.toml` file. This will automatically happen when you install gdsfactory as one of the PDK dependencies. For example `pip install gf180` will install the latest gdsfactory version that has been tested for the GlobalFoundries180 PDK.
+```
+pip install gdsfactory[cad] --upgrade
+```
+
+Please note that some PDKs may only work for a specific version of gdsfactory. Ensure you install the correct gdsfactory version specified in the pyproject.toml file. This will automatically happen when you install gdsfactory as one of the PDK dependencies. For example, pip install gf180 will install the latest gdsfactory version tested for the GlobalFoundries180 PDK.
 
-This code will tell you which gdsfactory you are using:
+To determine your current gdsfactory version, use the following code:
 
 ```
 import gdsfactory as gf
 
 gf.config.print_version()
 ```
 
 ### Docker container
 
-Alternatively, one may use the pre-built Docker image from [hub.docker.com/r/joamatab/gdsfactory](https://hub.docker.com/r/joamatab/gdsfactory) or build it yourself with:
+As an alternative, you can use the pre-built Docker image from [hub.docker.com/r/joamatab/gdsfactory](https://hub.docker.com/r/joamatab/gdsfactory) or build it yourself with:
+
 
 ```bash
 docker build -t joamatab/gdsfactory .
 ```
-For example, VS Code supports development inside a container, see [Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers) for details.
+
+For instance, VS Code supports development inside a container. See [Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers) for details.
 
 ## Plugins
 
-Plugins are hosted in a separate [repo](https://github.com/gdsfactory/gplugins) and installed as part of gdsfactory.
-Notice that plugins allow you to interface with different tools and some of them need to be installed separately.
-Take a look at the [gplugins documentation](https://gdsfactory.github.io/gplugins/)
+We maintain gdsfactory plugins in a [separate package](https://github.com/gdsfactory/gplugins)
+These plugins enable interfaces with different tools, and you might need to install some of the tools separately.
+For more details, please visit the [gplugins documentation](https://gdsfactory.github.io/gplugins/).
 
 ## Getting started
 
 - [See slides](https://docs.google.com/presentation/d/1_ZmUxbaHWo_lQP17dlT1FWX-XD8D9w7-FcuEih48d_0/edit#slide=id.g11711f50935_0_5)
 - [Read docs](https://gdsfactory.github.io/gdsfactory/)
 - [![Video Tutorials](https://img.shields.io/badge/youtube-Video_Tutorials-red.svg?logo=youtube)](https://www.youtube.com/@gdsfactory625/playlists)
 - [![Join the chat at https://gitter.im/gdsfactory-dev/community](https://badges.gitter.im/gdsfactory-dev/community.svg)](https://gitter.im/gdsfactory-dev/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
@@ -223,14 +219,13 @@
 
 ---
 
 "I use gdsfactory for all of my photonic tape-outs. The Python interface makes it easy to version control individual photonic components as well as entire layouts, while integrating seamlessly with KLayout and most standard photonic simulation tools, both open-source and commercial.
 
 <div style="text-align: right; margin-right: 10%;">Thomas Dorch - <strong>Freedom Photonics</strong></div>
 
-
 ## Contributors
 
 Thanks to all the contributors that make this awesome project possible!
 
 [![Meet our contributors!](https://contrib.rocks/image?repo=gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/graphs/contributors)
```

