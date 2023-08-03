# Comparing `tmp/cytosim-0.0.3.tar.gz` & `tmp/cytosim-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytosim-0.0.3.tar", last modified: Wed Aug  2 09:53:45 2023, max compression
+gzip compressed data, was "cytosim-0.0.4.tar", last modified: Thu Aug  3 15:38:29 2023, max compression
```

## Comparing `cytosim-0.0.3.tar` & `cytosim-0.0.4.tar`

### file list

```diff
@@ -1,980 +1,609 @@
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.503219 cytosim-0.0.3/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2023-08-01 11:52:34.000000 cytosim-0.0.3/.gitignore
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4328 2023-08-01 11:52:34.000000 cytosim-0.0.3/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2023-08-01 11:52:34.000000 cytosim-0.0.3/LICENSE.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-02 09:53:45.503219 cytosim-0.0.3/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2023-08-01 11:52:34.000000 cytosim-0.0.3/PYCYTOSIM.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3752 2023-08-01 11:52:34.000000 cytosim-0.0.3/README.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2023-08-01 11:52:34.000000 cytosim-0.0.3/WARRANTY.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/cym/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      514 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/actin.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/amplify.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1218 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/arp23.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3330 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/ashbya.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      614 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_couple.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1127 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_custom.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1897 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_france.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      759 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_guided.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      884 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_pull3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      913 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_texas.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1108 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/aster_tracker.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/axon.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1374 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/axon.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1399 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/baseball.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      897 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/bead.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/bipolar.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      858 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/buckling.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/buckling.cym.tpl
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/capture.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2274 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/capture_amplified.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      856 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/catastrophe_outside.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/celegans.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1385 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/change.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      563 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/change_confine.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      752 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/change_space.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      873 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/confine_instability.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      983 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_always.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1250 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_anchored.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_clamped.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1222 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_connect.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1135 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/contract_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1857 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      891 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/couple.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3110 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/couple_fork.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1140 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/crushed_shell.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1107 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      922 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_fibers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      954 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_planar.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1233 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cut_saved.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3683 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cytokinesis.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      869 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/cytoplasmic_flow.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1266 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/dogic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3225 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/endocytosis.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2103 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/endocytosis.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9924 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/entangled.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/event.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      945 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fast_diffusion1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      951 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fast_diffusion2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      353 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1203 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_anchor.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_athermal.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      837 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_bent.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      615 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_buckle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      998 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_classic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      834 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      625 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_forces.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1365 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_glue.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      601 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_grow.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1728 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_mixed.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1329 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_omega.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      847 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fiber_treadmill.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      868 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/field.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      715 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/field_bind.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      637 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/field_cut.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      703 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/fountain.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/frap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1277 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/friction.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      968 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1009 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_arcs.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_collect.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1680 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_drag.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1522 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_east.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1353 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_flip.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1959 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_flip_track.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1404 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_flippers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1770 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_gate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1126 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_path.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1334 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_ratchet.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1686 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_sort.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1898 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_sort_ortho.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1654 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_sorter.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1349 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_spiral.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_steric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1369 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_stripe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1245 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_surface.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      901 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_texas.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_trap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1547 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_west.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1624 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_west_blur.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1675 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/glide_yingyang.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/granules.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1274 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_chew.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_cut.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_digit.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      828 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_move.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      861 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_nucleate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      984 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_rescue.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1330 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_slide.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_track.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2408 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/hand_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3579 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/lacroix.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1053 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/magic_key.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      672 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/microtubule.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1760 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/minifilaments.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1850 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/minifilaments1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1605 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/minifilaments2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motif.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1554 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motif_blur.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1132 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motile_bead.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1145 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/motor_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1006 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/move.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2376 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/muscle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      972 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/muscle_smooth.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/needles.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nematic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      663 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nucleate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      842 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nucleate_edge.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1106 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/nucleus.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1249 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1411 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2044 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap3D_16.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1362 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/overlap_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      458 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/packed_beads.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      459 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/packed_beads_2D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1326 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/packed_gel.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1364 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/placement.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1356 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/pombe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1528 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/pombe_classic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1724 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/pombe_meiotic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1311 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/push_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1142 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/radial.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1124 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/ring_motors.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1066 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1012 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self_cortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      754 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self_vortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1086 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/self_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      764 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/side_movement.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      658 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/single.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/smiley.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1387 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/solid.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      499 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/solid_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      690 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/space_axisymmetric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      597 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/space_ellipse.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1122 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/sphere.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1097 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spider.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2417 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle3.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3712 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_celegans.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1601 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_centering.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1585 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_centering_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2199 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_compression.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3423 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_pombe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25433 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_pombe_em.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31549 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_pombe_em1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7568 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spindle_yeast.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      676 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spiral.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      977 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/spool.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1080 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      640 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_artefact.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bead_fiber_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      460 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bead_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      399 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bead_periodic2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      940 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bundle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1243 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_bundling.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      667 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_cylinder.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      857 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      535 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      846 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      654 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_fiber_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_sphere.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1910 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/steric_test.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      957 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/swimmers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      841 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_binding1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1077 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_binding2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1262 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_binding3.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      735 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_bindingP.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      439 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_fiber_diffusion.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      419 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/test_single_diffusion.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      550 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/texas.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/toy.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      906 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/toy_start.cmi
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      892 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/transport.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1035 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/triangle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1591 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/tug_of_war.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1485 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/walkers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1137 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/wash.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/yossi.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1407 2023-08-01 11:52:34.000000 cytosim-0.0.3/cym/zigzag.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/cytosim.xcodeproj/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   336632 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/project.pbxproj
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.403219 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3081 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2846 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2828 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2876 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2377 2023-08-01 11:52:34.000000 cytosim-0.0.3/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   210863 2023-08-01 11:52:34.000000 cytosim-0.0.3/demo_frame.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    81188 2023-08-01 11:52:34.000000 cytosim-0.0.3/demo_pycytosim.ipynb
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/code/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   106956 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/doxygen.cfg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      652 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5727 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/layout.xml
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/mainpage.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4859 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/code/objects.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/compile/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4678 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/cygwin.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      931 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/dimensionality.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6519 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/intel_mkl.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      845 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/linux.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1663 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/multithreading.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1361 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/options.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2371 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/compile/vectorization.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.431219 cytosim-0.0.3/doc/cpython/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28284 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/cpython.css
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6251 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/cpython_doc.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   101654 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/doc_PyCytoplay.html
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100729 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/doc_PyCytosim.html
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9278 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/cpython/read_cpython.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   123267 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/data/cytosim.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29497 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/data/modularity.png
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/examples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6671 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/biblio.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/examples/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33685 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/actin.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42409 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/ashbya.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30331 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/celegans.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    60174 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/centering.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65951 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/droplets.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    50739 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/endocytosis.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    97182 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/minifilaments.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    77302 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/nematics.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100226 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/network.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5254 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/patterns.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   110273 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/spindle.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    51623 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/spindle_length.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16497 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/data/spombe.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2240 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/examples/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1813 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.435219 cytosim-0.0.3/doc/main/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/cheat.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/credits.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/examples.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5237 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/executables.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57247 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/faq.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1711 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/file_types.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3256 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/movies.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3969 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/overview.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5837 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/run_slurm.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7840 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/runs.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3784 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/main/starter.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/misc/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4057 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/misc/Cytosim.tmbundle.zip
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/outreach/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1717 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/controller.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/outreach/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57904 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/CRI-2018-11a.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    39021 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/CRI-2018-11b.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   102453 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/Cambridge-2019-05a.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    61861 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/data/Cambridge-2019-05b.jpg
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/outreach/games/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/games/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      198 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6378 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/installation1.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5304 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/outreach/installation2.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.439219 cytosim-0.0.3/doc/rendering/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)  1462588 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/actin.blend
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4264 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-actin-ico.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-actin-sphere.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-actin.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4413 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/import-links.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4086 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      292 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/rendering/remove-actin.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.443219 cytosim-0.0.3/doc/sim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12156 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/commands.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2675 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/config.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.443219 cytosim-0.0.3/doc/sim/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      928 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/forces.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6040 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/forces.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/meca_links.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3284 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      263 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric.tex
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21888 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric3D.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11926 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/steric_math.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65261 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/data/varying_time_step.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9082 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/fiber_dynamics.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1679 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/fibers.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1283 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/forces.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2513 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/graphics.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      611 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1527 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/motor_detachment.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3731 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/numerical_precision.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4246 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/objects.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       85 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/parameters.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8951 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/placement.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6988 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/report.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2687 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/spaces.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3458 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/steric.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3473 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/stochastic.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1882 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/sim/units.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.443219 cytosim-0.0.3/doc/tutorials/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.447219 cytosim-0.0.3/doc/tutorials/code/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4790 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/collect.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/config.cym.tpl
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      710 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/master.sh
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    15382 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/preconfig
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/code/scan.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.447219 cytosim-0.0.3/doc/tutorials/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3334 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/ashbya.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      793 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1234 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/aster_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4119 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/capture.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19449 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/end_tracking.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28111 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/filament_buckling.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/gliding.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28234 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/polarity_sorting.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1010 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/data/self.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.447219 cytosim-0.0.3/doc/tutorials/images/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4591 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/H.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4483 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/XTV.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11568 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/aster-vs-nematic.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19716 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/bind_also_end.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    27299 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/bind_end.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20037 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/couples.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7406 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/crosslinks.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32919 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/droplets.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12570 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/force_velocity.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3561 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/gliding1.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3617 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/gliding2.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57401 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/kinesin_tetramers.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/meca_links.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10190 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/images/nematic-vs-polar.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      227 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_bipolarity.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3031 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_capture.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12562 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_centering.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7861 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_contract2.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5433 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_contract3.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7185 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_contract_motor.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5985 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_gliding.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23732 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_introduction.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      680 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_nucleus.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14458 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_polar_nematic.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      224 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_polarity.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7287 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_scans.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2543 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_scripting.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11632 2023-08-01 11:52:34.000000 cytosim-0.0.3/doc/tutorials/tuto_self.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      356 2023-08-01 11:52:34.000000 cytosim-0.0.3/example.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/examples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      591 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/avoid.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2061 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/callbacks_pycytoplay.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      622 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/flock.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5745 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytoplay_callbacks.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   321969 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_construct.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   279239 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_extend.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   139505 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_flock.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6248 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_import3D.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   160711 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_meca.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4782 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_obj_3D.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   492525 2023-08-01 11:52:34.000000 cytosim-0.0.3/examples/pycytosim_objects.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2023-08-01 11:52:34.000000 cytosim-0.0.3/makefile
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12556 2023-08-01 11:52:34.000000 cytosim-0.0.3/makefile.inc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/python/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/python/look/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/collect.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/compare_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/get_data.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_image.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_movie.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_page.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/make_plots.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/read_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/scan.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/look/tell.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.451219 cytosim-0.0.3/python/misc/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/battery_test.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/cleanup.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/compare.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/plot.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/pyned.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/misc/reduce.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.455219 cytosim-0.0.3/python/run/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/go_sim.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/go_sim_lib.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23500 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/preconfig.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/submit_one.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2023-08-01 11:52:34.000000 cytosim-0.0.3/python/run/submit_slurm.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2023-08-02 09:53:45.503219 cytosim-0.0.3/setup.cfg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2415 2023-08-02 09:52:25.000000 cytosim-0.0.3/setup.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.455219 cytosim-0.0.3/src/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2023-08-02 09:05:14.000000 cytosim-0.0.3/src/CMakeLists.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/base/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/array.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/assert_macro.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/backtrace.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/backtrace.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/buddy.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/exceptions.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/exceptions.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filepath.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filepath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filewrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/filewrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/glossary.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/glossary.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/inventoried.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/inventory.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/inventory.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/iowrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/iowrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/messages.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/messages.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/node_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/node_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/noder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/operator_new.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/print_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/print_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/property_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/stream_func.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/stream_func.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tictoc.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tictoc.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/timer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tokenizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/base/tokenizer.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/cpython/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4555 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/couple_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13219 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/fiber_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/glossary_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6128 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/hand_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6486 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/interface_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8178 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/meca_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3303 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/object_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/organizer_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2330 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/point_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9076 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/python_frame.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3217 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/python_utilities.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8838 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/simul_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/single_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5534 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/solid_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/space_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2669 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/cpython/thread_modules.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/cytosim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       23 2023-08-01 15:26:59.000000 cytosim-0.0.3/src/cytosim/__init__.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.459219 cytosim-0.0.3/src/cytosim.egg-info/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22584 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-01 12:00:54.000000 cytosim-0.0.3/src/cytosim.egg-info/not-zip-safe
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        8 2023-08-02 09:53:45.000000 cytosim-0.0.3/src/cytosim.egg-info/top_level.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.467219 cytosim-0.0.3/src/disp/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12450 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17737 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29713 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/display_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/fiber_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/fiber_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glapp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/gle_color_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glu_unproject.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/glut.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/grid_display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/grid_display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/line_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/line_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/miniz.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/miniz.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen_fbo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/offscreen_glx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/opengl.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/point_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/point_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/save_image.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/save_image.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/spng.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/spng.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5971 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/disp/view_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/math/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-avx2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-params.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-params19937.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT-sse2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/SFMT.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/accumulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/allocator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/bicgstab.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/cblas.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/clapack.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/dgtsv.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/dim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/evaluator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/gmres.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/grid_base.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/isometry.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/linear_operator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix11.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix11.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix22.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix22.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix33.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix33.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrix44.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matrixbase.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesym2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesymblk.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/matsparsesymblk.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/platonic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/pointsonsphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/pointsonsphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/project_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/project_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/quaternion.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random_vector.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/random_vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/rasterizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/real.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/simd.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/simd_print.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/smath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vecprint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/math/vector4.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/check_dump.m
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/installation/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/RtMidi.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/RtMidi.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/installation/builder/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/0-live.command
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config0.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config1.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config2.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config3.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config4.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config5.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config6.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config7.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/config8.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/builder/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/cytobuilder.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/cytomaster.cpp
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.475219 cytosim-0.0.3/src/misc/installation/cytomaster.xcodeproj/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/makefile
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.479219 cytosim-0.0.3/src/misc/installation/master/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/0-live.command
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config0.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config4.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config6.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config7.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config8.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/config9.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/master/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/rtmidi_c.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/misc/installation/rtmidi_c.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.479219 cytosim-0.0.3/src/play/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play_keys.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play_menus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/play_mouse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/play/player_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.491219 cytosim-0.0.3/src/sim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/bead_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/chain.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/chain.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/common.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couple_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.491219 cytosim-0.0.3/src/sim/couples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/bridge_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/couple_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/couple_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/crosslink_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/duo_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/fork_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/couples/shackle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/event_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_grid2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16712 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_segment.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_segment.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_site.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fiber_site.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.491219 cytosim-0.0.3/src/sim/fibers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4522 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/field_values.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/frame_reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/frame_reader.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6855 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_monitor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hand_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.495219 cytosim-0.0.3/src/sim/hands/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/actor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/chewer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1914 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/cutter_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/digit_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/dynein_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/kinesin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/mighty_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/motor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/myosin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/nucleator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/regulator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/rescuer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/slider_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/tracker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/hands/walker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interface.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interface.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/interpolation4.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/lattice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/lattice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22723 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca1d.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/meca_inter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil_project.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecafil_projectmat.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecapoint.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/mecapoint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/modulo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/modulo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/movable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/movable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/object_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizer_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.499219 cytosim-0.0.3/src/sim/organizers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/aster_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/bundle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/fake_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/organizers/nucleus_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/parser.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/parser.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/point_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/point_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sim_thread.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19507 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_custom.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_file.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/simul_step.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/single_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.499219 cytosim-0.0.3/src/sim/singles/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/picket_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/singles/wrist_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/solid_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/space_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.499219 cytosim-0.0.3/src/sim/spaces/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_banana.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_banana.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_capsule.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_capsule.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinder.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderP.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderP.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_cylinderZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_dice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_dice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_periodic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_periodic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9540 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygonZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_polygonZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ring.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_ring.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_square.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_square.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_strip.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_strip.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_torus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/spaces/space_torus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/sphere_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/splash.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/sim/splash.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.503219 cytosim-0.0.3/src/test/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_blas.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_code.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_cxx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_dispatch.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_gillespie.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glos.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glut.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_glut3D.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_math.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_omp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_opengl.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_pipe.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_quaternion.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_signal.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_simd.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_sizeof.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_string.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/test/test_vbo.cc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-02 09:53:45.503219 cytosim-0.0.3/src/tools/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-02 09:32:07.000000 cytosim-0.0.3/src/tools/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/cymart.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/frametool.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10045 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/pycytoplay.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5543 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/pycytosim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/pycytosim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/reportF.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2023-08-01 11:52:34.000000 cytosim-0.0.3/src/tools/sieve.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:29.001384 cytosim-0.0.4/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2023-08-03 15:27:32.000000 cytosim-0.0.4/.gitignore
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4328 2023-08-03 15:27:32.000000 cytosim-0.0.4/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2023-08-03 15:27:32.000000 cytosim-0.0.4/LICENSE.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4751 2023-08-03 15:38:29.001384 cytosim-0.0.4/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2023-08-03 15:27:32.000000 cytosim-0.0.4/PYCYTOSIM.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3752 2023-08-03 15:27:32.000000 cytosim-0.0.4/README.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2023-08-03 15:27:32.000000 cytosim-0.0.4/WARRANTY.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.957384 cytosim-0.0.4/cytosim.egg-info/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4751 2023-08-03 15:38:28.000000 cytosim-0.0.4/cytosim.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14193 2023-08-03 15:38:28.000000 cytosim-0.0.4/cytosim.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-03 15:38:28.000000 cytosim-0.0.4/cytosim.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-03 15:38:28.000000 cytosim-0.0.4/cytosim.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       18 2023-08-03 15:38:28.000000 cytosim-0.0.4/cytosim.egg-info/top_level.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2023-08-03 15:27:32.000000 cytosim-0.0.4/makefile
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12556 2023-08-03 15:27:32.000000 cytosim-0.0.4/makefile.inc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.957384 cytosim-0.0.4/pycytosim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12108 2023-08-03 15:28:09.000000 cytosim-0.0.4/pycytosim/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       23 2023-08-03 15:28:09.000000 cytosim-0.0.4/pycytosim/__init__.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.957384 cytosim-0.0.4/python/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.957384 cytosim-0.0.4/python/look/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/collect.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/compare_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/get_data.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/make_image.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/make_movie.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/make_page.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/make_plots.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/read_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/scan.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/look/tell.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.957384 cytosim-0.0.4/python/misc/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/misc/battery_test.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/misc/cleanup.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/misc/compare.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/misc/plot.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/misc/pyned.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/misc/reduce.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.957384 cytosim-0.0.4/python/run/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/run/go_sim.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/run/go_sim_lib.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23500 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/run/preconfig.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/run/submit_one.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2023-08-03 15:27:32.000000 cytosim-0.0.4/python/run/submit_slurm.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2023-08-03 15:38:29.001384 cytosim-0.0.4/setup.cfg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5205 2023-08-03 15:38:19.000000 cytosim-0.0.4/setup.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.957384 cytosim-0.0.4/src/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/CMakeLists.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.961384 cytosim-0.0.4/src/base/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/array.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/assert_macro.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/backtrace.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/backtrace.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/buddy.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/exceptions.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/exceptions.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/filepath.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/filepath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/filewrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/filewrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/glossary.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/glossary.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/inventoried.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/inventory.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/inventory.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/iowrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/iowrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/messages.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/messages.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/node_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/node_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/noder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/operator_new.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/print_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/print_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/property.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/property.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/property_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/property_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/stream_func.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/stream_func.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/tictoc.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/tictoc.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/timer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/tokenizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/base/tokenizer.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.961384 cytosim-0.0.4/src/cpython/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4555 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/couple_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13219 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/fiber_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/glossary_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6128 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/hand_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6486 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/interface_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8178 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/meca_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3303 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/object_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/organizer_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2330 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/point_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9076 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/python_frame.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3217 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/python_utilities.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8838 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/simul_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/single_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5534 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/solid_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/space_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2669 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/cpython/thread_modules.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.965384 cytosim-0.0.4/src/disp/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12450 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17737 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29713 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/display_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/fiber_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/fiber_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/glapp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/gle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/gle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/gle_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/gle_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/gle_color_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/gle_color_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/glu_unproject.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/glut.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/grid_display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/grid_display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/line_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/line_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/miniz.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/miniz.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/offscreen.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/offscreen.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/offscreen_fbo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/offscreen_glx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/opengl.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/point_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/point_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/save_image.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/save_image.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/spng.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/spng.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/view.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/view.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5971 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/view_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/disp/view_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.973384 cytosim-0.0.4/src/math/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/SFMT-avx2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/SFMT-common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/SFMT-params.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/SFMT-params19937.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/SFMT-sse2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/SFMT.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/SFMT.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/accumulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/allocator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/bicgstab.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/cblas.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/clapack.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/dgtsv.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/dim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/evaluator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/gmres.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/grid_base.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/isometry.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/linear_operator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix11.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix11.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix22.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix22.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix33.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix33.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrix44.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matrixbase.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesym.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesym.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesym1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesym1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesym2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesym2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesymblk.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/matsparsesymblk.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/platonic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/pointsonsphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/pointsonsphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/project_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/project_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/quaternion.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/random.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/random_vector.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/random_vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/rasterizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/real.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/simd.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/simd_print.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/smath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vecprint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/math/vector4.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.973384 cytosim-0.0.4/src/misc/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/check_dump.m
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.973384 cytosim-0.0.4/src/misc/installation/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/RtMidi.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/RtMidi.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.973384 cytosim-0.0.4/src/misc/installation/builder/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/0-live.command
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config0.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config1.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config2.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config3.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config4.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config5.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config6.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config7.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/config8.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/builder/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/cytobuilder.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/cytomaster.cpp
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.973384 cytosim-0.0.4/src/misc/installation/cytomaster.xcodeproj/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/makefile
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.973384 cytosim-0.0.4/src/misc/installation/master/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/0-live.command
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config0.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config4.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config6.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config7.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config8.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/config9.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/master/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/rtmidi_c.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/misc/installation/rtmidi_c.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.977384 cytosim-0.0.4/src/play/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/play.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/play.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/play_keys.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/play_menus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/play_mouse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/player.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/player.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/player_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/player_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/play/player_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.985384 cytosim-0.0.4/src/sim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/bead.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/bead.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/bead_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/bead_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/bead_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/bead_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/chain.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/chain.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/common.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couple.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couple.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couple_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couple_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couple_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couple_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.989384 cytosim-0.0.4/src/sim/couples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/bridge.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/bridge.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/bridge_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/bridge_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/couple_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/couple_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/crosslink.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/crosslink.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/crosslink_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/crosslink_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/crosslink_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/crosslink_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/duo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/duo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/duo_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/duo_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/duo_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/duo_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/fork.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/fork.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/fork_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/fork_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/shackle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/shackle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/shackle_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/shackle_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/shackle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/couples/shackle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/event.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/event.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/event_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/event_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_grid2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16712 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_segment.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_segment.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_site.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fiber_site.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.989384 cytosim-0.0.4/src/sim/fibers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/classic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/classic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/classic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/classic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/dynamic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/dynamic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/dynamic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/dynamic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/growing_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/growing_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/growing_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/growing_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/treadmilling_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/treadmilling_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/treadmilling_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/fibers/treadmilling_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/field.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/field.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4522 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/field_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/field_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/field_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/field_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/field_values.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/frame_reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/frame_reader.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hand.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6855 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hand.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hand_monitor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hand_monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hand_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hand_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.993384 cytosim-0.0.4/src/sim/hands/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/actor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/actor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/actor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/actor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/chewer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/chewer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/chewer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/chewer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/cutter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/cutter.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1914 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/cutter_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/cutter_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/digit.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/digit.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/digit_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/digit_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/dynein.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/dynein.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/dynein_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/dynein_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/kinesin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/kinesin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/kinesin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/kinesin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/mighty.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/mighty.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/mighty_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/mighty_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/motor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/motor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/motor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/motor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/myosin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/myosin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/myosin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/myosin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/nucleator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/nucleator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/nucleator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/nucleator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/regulator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/regulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/regulator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/regulator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/rescuer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/rescuer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/rescuer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/rescuer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/slider.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/slider.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/slider_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/slider_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/tracker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/tracker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/tracker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/tracker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/walker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/walker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/walker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/hands/walker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/interface.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/interface.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/interpolation.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/interpolation.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/interpolation4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/interpolation4.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/lattice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/lattice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/meca.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22723 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/meca.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/meca1d.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/meca_inter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecafil.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecafil.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecafil_project.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecafil_projectmat.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecapoint.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/mecapoint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/modulo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/modulo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/movable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/movable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/object.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/object.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/object_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/object_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizer_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizer_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.993384 cytosim-0.0.4/src/sim/organizers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/aster.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/aster.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/aster_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/aster_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/bundle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/bundle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/bundle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/bundle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/fake.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/fake.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/fake_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/fake_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/nucleus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/nucleus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/nucleus_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/organizers/nucleus_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/parser.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/parser.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/point_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/point_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sim_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sim_thread.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19507 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul_custom.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul_file.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul_report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/simul_step.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/single.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/single.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/single_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/single_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/single_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/single_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.993384 cytosim-0.0.4/src/sim/singles/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/picket.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/picket.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/picket_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/picket_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/wrist.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/wrist.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/wrist_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/singles/wrist_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/solid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/solid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/solid_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/solid_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/solid_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/solid_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/space.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/space_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/space_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/space_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/space_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.997384 cytosim-0.0.4/src/sim/spaces/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_banana.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_banana.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_capsule.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_capsule.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_cylinder.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_cylinder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_cylinderP.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_cylinderP.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_cylinderZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_cylinderZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_dice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_dice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_periodic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_periodic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9540 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_polygonZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_polygonZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_ring.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_ring.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_square.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_square.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_strip.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_strip.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_torus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/spaces/space_torus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sphere_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sphere_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sphere_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/sphere_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/splash.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/sim/splash.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:28.997384 cytosim-0.0.4/src/test/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_blas.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_code.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_cxx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_dispatch.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_gillespie.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_glos.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_glut.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_glut3D.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_math.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_omp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_opengl.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_pipe.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_quaternion.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_signal.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_simd.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_sizeof.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_string.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/test/test_vbo.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-03 15:38:29.001384 cytosim-0.0.4/src/tools/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/cymart.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/frametool.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10045 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/pycytoplay.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5543 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/pycytosim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/pycytosim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/reportF.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2023-08-03 15:27:32.000000 cytosim-0.0.4/src/tools/sieve.cc
```

### Comparing `cytosim-0.0.3/.gitignore` & `cytosim-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/CMakeLists.txt` & `cytosim-0.0.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/LICENSE.txt` & `cytosim-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/PKG-INFO` & `cytosim-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cytosim
-Version: 0.0.3
-Summary: Cytosim: Langevin dynamics of active polymer networks
-Keywords: simulation actin microtubule polymer
-Platform: Windows
-Platform: Linux
-Platform: Mac OS-X
-Platform: Unix
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Cytosim
 
 Cytosim is a cytoskeleton simulation suite designed to handle large systems of flexible filaments with associated proteins such as molecular motors. It is a versatile base that has been used to study actin and microtubule systems in 1D, 2D and 3D. It is built around a cross-platform C++ core engine running on UNIX, Mac OSX, GNU/Linux and within Cygwin on Windows. The code is modular and extensible, making Cytosim a convenient base that can be customized to meet particular tasks. Some of the most common tasks encountered during a simulation project are implemented in Python.
 
 ![Cytosim](doc/data/cytosim.png)
 
 Cytosim is a suite of command-line tools with simulation and display capabilities. The simulation is specified in a [configuration file](doc/sim/config.md), defining objects with their parameters and a suite of operations, such as advancing time, saving frames or [generating reports](doc/sim/report.md). Here is a basic example, with parameters specified in [units of seconds, micrometers and pico-Newtons](doc/sim/units.md).
```

### Comparing `cytosim-0.0.3/PYCYTOSIM.md` & `cytosim-0.0.4/PYCYTOSIM.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/README.md` & `cytosim-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: cytosim
+Version: 0.0.4
+Summary: Cytosim: Langevin dynamics of active polymer networks
+Keywords: simulation actin microtubule polymer
+Platform: Windows
+Platform: Linux
+Platform: Mac OS-X
+Platform: Unix
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Cytosim
 
 Cytosim is a cytoskeleton simulation suite designed to handle large systems of flexible filaments with associated proteins such as molecular motors. It is a versatile base that has been used to study actin and microtubule systems in 1D, 2D and 3D. It is built around a cross-platform C++ core engine running on UNIX, Mac OSX, GNU/Linux and within Cygwin on Windows. The code is modular and extensible, making Cytosim a convenient base that can be customized to meet particular tasks. Some of the most common tasks encountered during a simulation project are implemented in Python.
 
 ![Cytosim](doc/data/cytosim.png)
 
 Cytosim is a suite of command-line tools with simulation and display capabilities. The simulation is specified in a [configuration file](doc/sim/config.md), defining objects with their parameters and a suite of operations, such as advancing time, saving frames or [generating reports](doc/sim/report.md). Here is a basic example, with parameters specified in [units of seconds, micrometers and pico-Newtons](doc/sim/units.md).
```

### Comparing `cytosim-0.0.3/WARRANTY.txt` & `cytosim-0.0.4/WARRANTY.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/cym/amplify.cym` & `cytosim-0.0.4/src/misc/installation/master/config2.cym`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,65 @@
-%{
- @example amplify.cym
- A Nucleator that is only active if it is bound
-
- F. Nedelec, April 2011
-}
+% Self-organization of filaments driven by bivalent motors
+% FJN for Nuit Blanche, 6.10.2018
 
 set simul system
 {
-    time_step = 0.001
-    viscosity = 10
+    dim = 2
+    time_step = 0.01
+    viscosity = 0.1
+    display = ( style=2; delay=20; period=4; zoom=0.6; label="Self organization -" )
 }
 
 set space cell
 {
-    shape = capsule
-}
-
-new cell
-{
-    length = 10
-    radius = 2
+    shape = circle
 }
 
-set fiber microtubule
+set fiber filament
 {
-    rigidity = 20
+    rigidity = 10
     segmentation = 0.5
     confine = inside, 100
-    activity = grow;
-    growing_speed = 1;
+    display = ( color=blue; width = 1; )
 }
 
-new 1 microtubule
+set hand motor
 {
-    length = 4
-    position = -3 0 0
-    direction = 1 0 0
-    plus_end = grow
+    binding= 2, 0.02
+    unbinding = 0.25, 3
+    
+    activity = move
+    unloaded_speed = 0.8
+    stall_force = 5
+
+    bind_also_end = 1
+    hold_growing_end = 1
+
+    display = ( color=green, dark_green; size=7; width=7; )
 }
 
-set hand activator
+set couple complex
 {
-    binding = 10, 0.5
-    unbinding = 0, 3
-    display = ( size=7; color=green, gray; )
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 10
 }
 
-set hand nucleator
+new cell
 {
-    unbinding = 0, 3
-    activity = nucleate
-    nucleate = 1, microtubule, ( length=0.1; plus_end=grow; )
-    nucleation_angle = 0.3 % almost parallel
-    display = ( size=7; color=white; )
+    radius = 14
 }
 
-set couple complex
+new 256 filament
 {
-    hand1 = activator
-    hand2 = nucleator
-    activity = fork
-    torque = 100, 0.3
-    diffusion = 1
-    stiffness = 100
-    trans_activated = 1
-    length = 0.1
+    length = 8
 }
 
-new 100 complex
+new 4096 complex
 
-run system
+run 100000 system
 {
-    nb_steps = 5000
-    nb_frames = 10
+    nb_frames = 50
 }
+
+
```

### Comparing `cytosim-0.0.3/cym/ashbya.cym` & `cytosim-0.0.4/src/misc/installation/master/config9.cym`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 % Viscosity 900 times water, from Tolic-Norrelykke et al. 2004.
 % Speed of flow 0.15 -- 1.28 um/min from Table 1 Lang et al. 2010 MBoC, 21, 18-28
 % Speed of flow in mutant ~ 0.75 um/min from Grava and Philippsen 2010 MBoC 21, 3680-3692; Grava et al. 2011 EC, 10, 7, 902-915.
 % The flow (specified in um/s) should be slightly higher to compensate for brownian.
 
 set simul system
 {  
+    dim = 3
     time_step = 0.05
     viscosity = 0.9    
     steric = 1, 100
     flow = 0.009 0 0
 }
 
 set system display
@@ -23,31 +24,30 @@
     back_color  = dark_gray;
     multisample = 3;
 }
 
 set space cell
 {
     shape = cylinderP
-    display = ( color=0x00000033, black )
+    display = ( color=0x00000033, black; visible=3;)
 }
 
 new cell
 {
-    length = 30
+    length = 15
     radius = 1.5
 }
 
-
 % Values for MT dynamics in Ashbya gossypii from Grava and Philippsen MBoC 2010 21, 3680-3692
 % Assumption that catastrophe rate = growing speed / average MT length
 % MT length obtained from raw data of Grava and Philippsen MBoC 2010 21, 3680-3692
 % Fit on trucated exponential distribution, Fraile and Garcia-Ortega JoAM 2005 44, 1620-25
 % Only MT between 1 to 20 um considered for fit as high number of very short MT observed by ET in Gibeaux et al. JCS 2012
 
-set fiber microtubule
+set fiber filament
 { 
     steric = 1, 0.025
     confine = inside, 100
     rigidity = 20
     segmentation = 0.5
     activity = classic
     growing_speed = 0.108, 0
@@ -63,15 +63,15 @@
     binding_range = 0.075
     unbinding_rate = 0.64 % 0.64 in King and Schroer, NCB 2000, 2
     unbinding_force = 7
     activity = motor
     unloaded_speed = -0.025 % Gennerich et al. Cell 2007, 131, 952-965 = 0.05 um/s
     bind_also_end = 1
     stall_force = 7 % Shingyoji et al. Nature 1998, 393 = 6 pN ; Gennerich et al. Cell 2007, 131, 952-965 = 7 pN
-    display = ( color=white, gray; size=8; )
+    display = ( color=white, gray; size=8; back_color=black )
 }
 
 set single anchored_dynein
 {
     hand = dynein
     stiffness = 500
     activity = fixed
@@ -86,15 +86,15 @@
 }
 
 set hand nucleator
 {
     binding = 0, 0.05
     unbinding = 0, inf
     activity = nucleate
-    nucleate = 1, microtubule, ( length=0.5; plus_end=grow; )
+    nucleate = 1, filament, ( length=0.5; plus_end=grow; )
     display = ( size=15; color=orange; )
 }
 
 set single handle
 {
     hand = nucleator
     stiffness = 500
```

### Comparing `cytosim-0.0.3/cym/aster_couple.cym` & `cytosim-0.0.4/src/misc/installation/builder/config1.cym`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,128 @@
-% Two asters interacting with hetero-complexes
-% F. Nedelec, April 2010
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.005
-    viscosity = 0.1
+    time_step = 0.01
+    viscosity = 0.5
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=2; period=2; zoom=0.98; label="Cytoskeleton" )
 }
 
 set space cell
 {
-    shape = circle
+    shape = polygon
+    display = ( color=dark_gray; width=4; )
 }
 
-new cell
+set fiber filament
 {
-    radius = 7
+    rigidity = 10
+    segmentation = 0.25
+    confine = inside, 100
+    lattice = 1, 0.010
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 15
+    total_polymer = 5000
+
+    display = ( plus_end=10; minus_end=8; color=dark_gray; width=2; )
 }
 
-set fiber microtubule
+set hand nucleator
 {
-    rigidity = 20
-    segmentation = 0.5
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=gray; }
 }
 
-set hand dynein 
+set single protein
 {
-    binding_rate = 10
-    binding_range = 0.01
-    unbinding_rate = 0.2
-    unbinding_force = 3
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
+}
+
+set hand motor
+{
+    binding = 9, 0.02
+    unbinding = 0.2, 3
     
-    activity = move
-    unloaded_speed = -1
-    stall_force = 6
+    activity = walk
+    step_size = 0.010
+
+    unloaded_speed = 1.0
+    stall_force = 5
 
-    display = { size=8; color=0xFF00FFFF; }
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=4; )
 }
 
-set hand kinesin 
+set couple bimotor
 {
-    binding_rate = 10
-    binding_range = 0.01
-    unbinding_rate = 0.2
-    unbinding_force = 3
-    
-    activity = move
-    unloaded_speed = 0.8
-    stall_force = 6
-    display = { size=8; color=0x00FF00FF; }
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 1
+    length = 0.1
 }
 
-set couple complex 
+set hand dynein
 {
-    hand1 = kinesin
+    binding = 9, 0.02
+    unbinding = 0.25, 3
+
+    activity = walk
+    step_size = 0.010
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=7; width=4; )
+}
+
+set couple bidynein
+{
+    hand1 = dynein
     hand2 = dynein
-    diffusion = 0.20
-    stiffness = 200
+    stiffness = 100
+    diffusion = 1
+    length = 0.1
 }
 
-set solid core
+set hand binder
 {
-    confine = 1, 100
-    display = ( style=3 )
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-set aster centrosome
+set couple bibinder
 {
-    stiffness = 1000, 500
+    hand1 = binder
+    hand2 = binder
+    stiffness = 100
+    diffusion = 1
 }
 
-new 2 centrosome
+new cell
 {
-    solid = core
-    radius = 1
-    point1 = center, 1
-    fibers = 32, microtubule, ( plus_end=grow; length = 7; )
+    points=10 -5.7, 10 5.7, -10 5.7, -10 -5.7;
 }
 
-new 5001 complex
+new 4 filament { length=24; position=rectangle 2 4; orientation=1 -0.1 0; }
+new 4 filament { length=24; position=rectangle 2 4; orientation=1 0.1 0; }
+new 1000 bimotor
 
-run system
+run 10000000 system
 {
-    nb_steps = 5000
-    nb_frames = 50
+    nb_frames = 0
 }
```

### Comparing `cytosim-0.0.3/cym/aster_dynamic.cym` & `cytosim-0.0.4/src/misc/installation/master/config0.cym`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,79 @@
-% A confined aster
-% F. Nedelec, April 2010 - Sep 2017
+% motors moving on one filament
+% FJN 8.05.2019
 
 set simul system
 {
-    time_step = 0.001
-    viscosity = 0.01
+    time_step = 0.005
+    viscosity = 0.02
+    display = ( point_size=12; zoom = 0.8; )
 }
 
 set space cell
 {
     shape = sphere
 }
 
 new cell
 {
     radius = 5
 }
 
-set fiber microtubule
+set fiber filament
 {
     rigidity = 20
-    segmentation = 0.5
+    segmentation = 0.25
     confine = inside, 100
-    
-    activity = classic
-    growing_speed    = 0.5
-    growing_force    = 1.67
-    shrinking_speed  = -0.85
-    catastrophe_rate = 0.1, 0.5
-    rescue_rate      = 0
-    min_length       = 0.5
-    persistent       = 0
- 
-    display = ( line_width = 4; )
+    display = ( line_width=2; plus_end=14, 2; )
 }
 
-set solid core
+new filament
 {
-    display = ( style = 3 )
+    length = 9
+    position = ( 0 0 0 )
 }
 
-set aster centrosome
+set hand motor
 {
-    stiffness = 1000, 500
-    nucleate = 1, microtubule, ( plus_end=grow; length=1; )
+    binding = 10, 0.05
+    unbinding = 0.2, 3
+    
+    activity = move
+    unloaded_speed = 1
+    stall_force = 5
+    display = ( size=12; color=green )
 }
 
-new centrosome
-{
-    solid = core
-    radius = 0.25
-    point1 = center, 0.25
-    fibers = 32, microtubule, ( plus_end=grow; length = 1; )
-    position = 4 0
-}
 
 set hand dynein
 {
-    binding_rate = 5
-    binding_range = 0.02
-    unbinding_rate = 0.5
-    unbinding_force = 2
-    
+    binding = 10, 0.05
+    unbinding = 0.2, 3
+     
     activity = move
     unloaded_speed = -1
     stall_force = 5
-    display = ( color = light_blue; size=7;  )
+    display = ( size=12; color=red )
 }
 
-set single grafted
+
+set single mobile
 {
-    hand = dynein
-    stiffness = 100
-    activity = fixed
+    hand = motor
+    diffusion = 0.1
 }
 
-new 0 grafted
+set single motile
 {
-    position = inside
+    hand = dynein
+    diffusion = 0.1
 }
 
-run 100000 system
+new 100 mobile
+new 100 motile
+
+run system
 {
-    nb_frames = 100
+    nb_steps = 40000
+    nb_frames = 50
 }
+
```

### Comparing `cytosim-0.0.3/cym/aster_france.cym` & `cytosim-0.0.4/src/misc/installation/master/config1.cym`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-% An aster confined within 'France' with a Nucleus
-% Gaelle Letort (2017) and FJN, 7.10.2018
+% An aster confined within 'France'
+% Gaelle Letort (2017) and FJN for Nuit Blanche, 6.10.2018
 
 set simul system
 {
     time_step = 0.005
     viscosity = 0.2
     steric = 1, 33
     display = ( delay=2; period=20; style=2; zoom=0.6; point_size=9; )
@@ -11,26 +11,19 @@
 
 set space cell
 {
     shape = polygon
     display = ( visible=3; width=9; color=0x0000FFFF; period=8; )
 }
 
-new cell
-{
-    file = france.txt
-    height = 2
-    scale = 0.25
-}
-
-set fiber microtubule
+set fiber filament
 {
     rigidity = 20
     segmentation = 0.25
-    confine = inside, 100
+    confine = inside, 500
     
     activity         = dynamic
     unit_length      = 0.008
     growing_speed    = 0.2
     shrinking_speed  = -0.5
     hydrolysis_rate  = 0.4
     growing_force    = 1.7
@@ -43,29 +36,29 @@
     %growing_force    = 1.67
 
     min_length       = 0.25
     persistent       = 1
     rebirth_rate     = 1.0
 }
 
-set hand kinesin
+set hand motor
 {
     binding= 2, 0.02
     unbinding = 0.25, 3
     
     activity = move
     unloaded_speed = 0.6
     stall_force = 5
 
     display = ( color=green; size=16; width=7; )
 }
 
 set single complex
 {
-    hand = kinesin
+    hand = motor
     diffusion = 1
 }
 
 set hand dynein
 {
     binding= 5, 0.01
     unbinding = 0.25, 3
@@ -73,15 +66,15 @@
     activity = move
     unloaded_speed = -1.0
     stall_force = 5
 
     display = ( color=red; size=16; width=8; )
 }
 
-set single motor
+set single simplex
 {
     hand = dynein
     stiffness = 100
     diffusion = 1
 }
 
 set solid core
@@ -98,22 +91,30 @@
 
 new centrosome
 {
     type = regular
     solid = core
     radius = 0.25
     point1 = center, 0.25
-    fibers = 48, microtubule, ( length = 0.25; plus_end = grow; )
+    fibers = 48, filament, ( length = 0.25; plus_end = grow; )
+}
+
+
+new cell
+{
+    file = france.txt
+    height = 2
+    scale = 0.25
 }
 
 new core
 {
-    sphere1 = 0 0 0, 1.0, 12 motor
+    sphere1 = 0 0 0, 1.0, 12 protein
 }
 
 new 256 complex
-new 128 motor
+new 128 simplex
 
 run 1000000 system
 {
     nb_frames = 100
 }
```

### Comparing `cytosim-0.0.3/cym/aster_pull.cym` & `cytosim-0.0.4/src/misc/installation/master/config4.cym`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,81 @@
-% A confined aster with cortical pulling motors
-% F. Nedelec, April 2010
+% Contraction of a network of flexible filaments
+% FJN for Nuit Blanche, 6.10.2018
 
 set simul system
 {
+    dim = 2
     time_step = 0.005
-    viscosity = 0.1
+    viscosity = 0.5
+    precondition = 1
+    display = ( style=2; delay=20; period=2; zoom=0.95; )
 }
 
 set space cell
 {
-    shape = sphere
+    shape = capsule
+    display = ( color=dark_gray; width=10; )
 }
 
-new cell
+set fiber filament
 {
-    radius = 10
+    rigidity = 0.1
+    segmentation = 0.128
+    display = ( width = 1.0; color=gray; )
 }
 
-set fiber microtubule
+set hand motor
 {
-    rigidity = 30
-    segmentation = 0.5
-    display = ( line=4, 2; )
+    binding = 5, 0.025
+    unbinding = 0.1, 4
+    
+    activity = move
+    unloaded_speed = 0.4
+    stall_force = 5
+
+    display = ( color=green; size=7; width=7; )
 }
 
-set solid core
+set couple complex
 {
-    display = ( style=3 )
+    hand1 = motor
+    hand2 = motor
+    stiffness = 400
+    diffusion = 10
 }
 
-set aster centrosome
+set hand binder
 {
-    stiffness = 1000, 500
+    binding = 4, 0.025
+    unbinding = 0.2, 6
+    display = ( color=blue; size=7; width=7; )
 }
 
-new centrosome
+set couple crosslinker
 {
-    solid = core
-    radius = 1
-    point1 = center, 1
-    fibers = 32, microtubule, ( length = 10; plus_end = grow; )
+    hand1 = binder
+    hand2 = binder
+    stiffness = 400
+    diffusion = 10
 }
 
-set hand dynein
+new cell
 {
-    binding_rate = 5
-    binding_range = 0.02
-    unbinding_rate = 0.1
-    unbinding_force = 3
-    
-    activity = move
-    unloaded_speed = -1
-    stall_force = 5
+    length = 9
+    radius = 2.5
 }
 
-set single grafted
+new 128 filament
 {
-    hand = dynein
-    stiffness = 100
-    activity = fixed
+    length = 3.2
 }
 
-new 200 grafted
+new 2500 complex
+new 3000 crosslinker
 
-
-run system 
+run 10000 system
 {
-    nb_steps = 20000
-    nb_frames = 100
+    nb_frames = 50
+    %event = 100, ( delete 1 filament; new filament { length = 3.6; } )
 }
+
+
```

### Comparing `cytosim-0.0.3/cym/aster_pull3D.cym` & `cytosim-0.0.4/src/misc/installation/builder/config0.cym`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,128 @@
-% A confined aster with cortical pulling motors
-% F. Nedelec, April 2010
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.005
-    viscosity = 0.1
+    time_step = 0.01
+    viscosity = 0.5
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=2; zoom=0.9; label="Cytoskeleton" )
 }
 
 set space cell
 {
-    shape = sphere
+    shape = polygon
+    display = ( color=dark_gray; width=4; )
 }
 
-new cell
+set fiber filament
 {
-    radius = 10
+    rigidity = 10
+    segmentation = 0.75
+    confine = inside, 100
+    lattice = 1, 0.010
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 15
+    total_polymer = 5000
+
+    display = ( plus_end=5; color=dark_gray; width=1; )
 }
 
-set fiber microtubule
+set hand nucleator
 {
-    confine = inside, 100
-    rigidity = 30
-    segmentation = 0.5
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=gray; }
 }
 
-set solid core
+set single protein
 {
-    display = ( style=3 )
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
-set aster centrosome
+set hand motor
 {
-    stiffness = 1000, 500
+    binding = 9, 0.02
+    unbinding = 0.2, 3
+    
+    activity = walk
+    step_size = 0.010
+
+    unloaded_speed = 1.0
+    stall_force = 5
+
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-new 1 centrosome
+set couple bimotor
 {
-    solid  = core
-    radius = 1
-    point1 = center, 1
-    fibers = 32, microtubule, ( plus_end=grow; length = 10; )
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 1
+    length = 0.1
 }
 
 set hand dynein
 {
-    binding_rate = 5
-    binding_range = 0.02
-    unbinding_rate = 0.1
-    unbinding_force = 3
-    
-    activity = move
-    unloaded_speed = -1
-    stall_force = 5
-    display = ( color = blue )
+    binding = 9, 0.02
+    unbinding = 0.25, 3
+
+    activity = walk
+    step_size = 0.010
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=7; width=5; )
 }
 
-set single graftedD
+set couple bidynein
 {
-    hand = dynein
+    hand1 = dynein
+    hand2 = dynein
     stiffness = 100
-    activity = fixed
+    diffusion = 1
+    length = 0.1
 }
 
-set hand kinesin
+set hand binder
 {
-    binding_rate = 5
-    binding_range = 0.02
-    unbinding_rate = 0.1
-    unbinding_force = 3
-    
-    activity = move
-    unloaded_speed = -1
-    stall_force = 5
-    display = ( color = green )
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-set single graftedK
+set couple bibinder
 {
-    hand = kinesin
+    hand1 = binder
+    hand2 = binder
     stiffness = 100
-    activity = fixed
+    diffusion = 1
 }
 
-new 200 graftedK { position=surface; placement = anywhere,, ( x > 0 ); }
-new 200 graftedD { position=surface; placement = anywhere,, ( x < 0 ); }
+new cell
+{
+    points=17 -10, 17 10, -17 10, -17 -10;
+}
 
+new 7 filament { length=24; position=rectangle 4 6; orientation=1 -0.05 0; }
+new 2 filament { length=24; position=0 0; orientation=1 0.1 0; }
+new 1000 bimotor
 
-run system 
+run 10000000 system
 {
-    nb_steps = 20000
-    nb_frames = 100
+    nb_frames = 0
 }
```

### Comparing `cytosim-0.0.3/cym/bipolar.cym` & `cytosim-0.0.4/src/misc/installation/builder/config.cym`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,135 @@
-% A set of objects that will self-assemble into a bipolar structure
-% F. Nedelec, 29 May 2014
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.001
-    viscosity = 0.1
-    steric = 0, 100
-}
-
-set system display
-{
-    delay=3;
-    period=8;
-    point_size=8; 
-    style=2;
+    time_step = 0.01
+    viscosity = 0.5
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=2; zoom=0.65; label="Cytoskeleton" )
 }
 
 set space cell
 {
-    shape = sphere
-    display = ( visible=1; width=2; )
+    shape = polygon
 }
 
-new cell
+set fiber filament
 {
-    radius = 8
-}
+    rigidity = 10
+    segmentation = 1.0
+    confine = inside, 100
 
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 10
+    total_polymer = 5000
 
-set fiber microtubule
+    display = ( color=white; width=0.5; )
+}
+
+set hand nucleator
 {
-    rigidity = 20
-    segmentation = 0.75
-    steric = 1, 0.03
-    confine = inside, 1
-    display = ( color=white; line_width=3; )
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=white; }
 }
 
-set hand numa 
+set single protein
 {
-    binding = 500, 0.25
-    unbinding = 0, 6
-    display = ( color=gray )
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
-set hand dynein 
+set hand motor
 {
-    binding = 10, 0.15
-    unbinding = 0.2, 6
+    binding = 9, 0.01
+    unbinding = 0.25, 3
     
-    activity    = move
-    unloaded_speed   = -1
+    activity = move
+    unloaded_speed = 1.0
     stall_force = 5
 
-    display = ( color=green )
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set couple motor
+set couple bimotor
 {
-    hand1 = numa
-    hand2 = dynein
-    diffusion = 0
-    stiffness = 200
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 10
 }
 
-set hand kinesin 
+set hand dynein
 {
-    binding = 10, 0.02
-    unbinding = 0.2, 6
-    
-    activity    = move
-    unloaded_speed   = 0.1
-    stall_force = 6
+    binding = 9, 0.01
+    unbinding = 0.25, 3
 
-    display = ( color=orange )
-}
+    activity = move
+    unloaded_speed = -1.0
+    stall_force = 3
 
-set couple kinesin5 
-{
-    hand1 = kinesin
-    hand2 = kinesin
-    diffusion = 5
-    stiffness = 200
-}
+    bind_also_end = 1
+    hold_growing_end = 0.98
 
+    display = ( color=orange, 0xAA6E0077; size=7; width=5; )
+}
 
-set solid core
+set couple bidynein
 {
-    display=(style=5;)
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 10
 }
 
-set aster chromosome
+set hand binder
 {
-    focus = plus_end
-    stiffness = 1000, 500
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-set aster centrosome
+set couple bibinder
 {
-    focus = minus_end
-    stiffness = 1000, 500
+    hand1 = binder
+    hand2 = binder
+    stiffness = 100
+    diffusion = 1
 }
 
-repeat 10
-{
-new core
+new cell
 {
-    point1 = center, 0.5
+    order = 6
+    radius = 13
 }
 
-new chromosome
+new 100 protein
+new 4000 bimotor
+
+run 1000 system
 {
-    solid = last
-    radius = 0.5, 0.3
-    fibers = 2, microtubule, ( length=4; attach = 13 motor, 0.5, minus_end, exponential; )
-    type = regular
-    placement = off
-}
+    nb_frames = 2
 }
 
-new 2 centrosome
+change cell { order=4; radius=15; angle=0.7853; }
+
+run 1000 system
 {
-    solid = core
-    radius = 0.5, 0.2
-    type = radial
-    fibers = 24, microtubule, ( length = 3.5 )
+    nb_frames = 2
 }
 
-new 1000 kinesin5
-
+change cell { points=16 -10, 16 10, -16 10, -16 -10; }
 
-run 100000 system 
+run 10000000 system
 {
-    nb_frames = 500
+    nb_frames = 0
 }
```

### Comparing `cytosim-0.0.3/cym/contract.cym` & `cytosim-0.0.4/src/misc/installation/builder/config7.cym`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,129 @@
-% A contractile network
-% Dec 2015
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.001
-    viscosity = 0.2
+    time_step = 0.01
+    viscosity = 0.1
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=2; zoom=0.9; label="Cytoskeleton" )
 }
 
-set system display { style=2; point_size=5; }
-
 set space cell
 {
-    shape = circle
+    shape = polygon
+    display = ( color=dark_gray; width=4; )
 }
 
-new cell
+set fiber filament
 {
-    radius = 7
+    rigidity = 20
+    segmentation = 0.5
+    confine = inside, 100
+    lattice = 1, 0.010
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 10
+    total_polymer = 5000
+
+    display = ( plus_end=5; color=dark_gray; width=1; )
 }
 
-set fiber filament
+set hand nucleator
 {
-    rigidity = 0.5
-    segmentation = 0.25
-    display = ( line=0.5, 1; color=gray; )
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=gray; }
+}
+
+set single protein
+{
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
 set hand motor
 {
-    binding = 10, 0.02
-    unbinding = 0.1, inf
+    binding = 9, 0.02
+    unbinding = 0.2, 3
+
+    activity = walk
+    step_size = 0.010
 
-    activity = move
-    unloaded_speed = -0.2
-    stall_force = 6
-    display = ( width=0.5; color=green; )
+    unloaded_speed = 1.0
+    stall_force = 5
+
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set couple complex
+set couple bimotor
 {
     hand1 = motor
     hand2 = motor
-    stiffness = 250
-    diffusion = 10
-    fast_diffusion = 1
+    stiffness = 100
+    diffusion = 1
+    length = 0.1
+}
+
+set hand dynein
+{
+    binding = 9, 0.02
+    unbinding = 0.25, 3
+
+    activity = walk
+    step_size = 0.010
+
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=7; width=5; )
+}
+
+set couple bidynein
+{
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 1
+    length = 0.1
 }
 
 set hand binder
 {
-    binding = 10, 0.02
-    unbinding = 0.2, inf
-    display = ( width=0.5; color=blue; )
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-set couple crosslinker
+set couple bibinder
 {
     hand1 = binder
     hand2 = binder
-    stiffness = 250
-    diffusion = 10
-    fast_diffusion = 1
+    stiffness = 100
+    diffusion = 1
 }
 
-new 250 filament
+new cell
 {
-    length = 5
+    points=10 -7, 10 7, -10 7, -10 -7;
 }
 
-new 2000 crosslinker
-new 1000 complex
+new 7 filament { length=10; position=rectangle 4 6; orientation=1 -0.05 0; }
+new 2 filament { length=10; position=0 0; orientation=1 0.1 0; }
+new 1000 bimotor
 
-run 100000 system
-{   
-    nb_frames = 50
+run 10000000 system
+{
+    nb_frames = 0
 }
-
```

### Comparing `cytosim-0.0.3/cym/contract_anchored.cym` & `cytosim-0.0.4/src/misc/installation/builder/config6.cym`

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,128 @@
-% A contractile actin gel attached on its edges
-% F. Nedelec 16 Dec 2017
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.001
-    viscosity = 0.05
+    time_step = 0.01
+    viscosity = 0.5
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=2; zoom=0.6; label="Cytoskeleton" )
 }
 
-
 set space cell
 {
-    shape = capsule
+    shape = polygon
+    display = ( color=dark_gray; width=4; )
 }
 
-new cell
+set fiber filament
 {
-    length = 30
-    radius = 5
+    rigidity = 10
+    segmentation = 0.4
+    confine = inside, 100
+    lattice = 1, 0.010
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 10
+    total_polymer = 5000
+
+    display = ( color=dark_gray; width=1; )
 }
 
-set hand myosin
+set hand nucleator
 {
-    binding = 10, 0.005
-    unbinding = 0.02, 3
-    
-    activity = move
-    unloaded_speed = 1
-    stall_force = 5
-    display = ( size=4; color=orange )
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=white; }
 }
 
-set hand binder
+set single protein
 {
-    binding = 10, 0.005
-    unbinding = 0.02, 3
-    display = ( size=4; color=gray )
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
-set hand holder
+set hand motor
 {
-    binding = 10, 0.02
-    unbinding = 0, inf
-    display = ( size=6; color=green )
+    binding = 9, 0.02
+    unbinding = 0, 3
+    
+    activity = walk
+    step_size = 0.010
+    dangling_chance = 0.99
+    unbinding_chance = 0.005
+
+    unloaded_speed = 1.0
+    stall_force = 5
+
+    bind_also_end = 1
+    hold_growing_end = 1
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set single anchor
+set couple bimotor
 {
-    hand = holder
-    stiffness = 1000
-    activity = fixed
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 10
 }
 
-set couple motor
+set hand dynein
 {
-    hand1 = myosin
-    hand2 = myosin
-    stiffness = 500
-    fast_diffusion = 1
+    binding = 9, 0.02
+    unbinding = 0.25, 3
+
+    activity = walk
+    step_size = 0.010
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=7; width=5; )
 }
 
-set couple crosslinker
+set couple bidynein
 {
-    hand1 = binder
-    hand2 = binder
-    stiffness = 500
-    fast_diffusion = 1
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 10
 }
 
-set fiber actin
+set hand binder
 {
-    rigidity = 0.1
-    segmentation = 0.1
-    display = ( line=1, 2; )
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-new 1000 actin
+set couple bibinder
 {
-    length = 5
+    hand1 = binder
+    hand2 = binder
+    stiffness = 100
+    diffusion = 1
 }
 
-new 50 anchor ( rectangle 0 4 at  10 0 )
-new 50 anchor ( rectangle 0 4 at -10 0 )
-
-% give some time to let things bind:
-run 1000 system
+new cell
+{
+    order = 7
+    radius = 11
+}
 
-new 5000 motor
-new 5000 crosslinker
+new 64 protein
+new 2000 bimotor
 
-run 1000 system
-{   
-    nb_frames = 10
+run 10000000 system
+{
+    nb_frames = 0
 }
```

### Comparing `cytosim-0.0.3/cym/contract_clamped.cym` & `cytosim-0.0.4/src/misc/installation/builder/config2.cym`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,122 @@
-% A contractile actin gel attached on its edges
-% F. Nedelec 12 May 2015
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.005
-    viscosity = 0.05
+    time_step = 0.01
+    viscosity = 0.25
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=2; period=2; zoom=0.6; label="Cytoskeleton" )
 }
 
-
 set space cell
 {
-    shape = circle
+    shape = polygon
+    display = ( color=gray; width=4; )
 }
 
-new cell
+set fiber filament
+{
+    rigidity = 20
+    segmentation = 0.7
+    confine = inside, 100
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 10
+    total_polymer = 5000
+
+    display = ( color=dark_gray; width=1; )
+}
+
+set hand nucleator
 {
-    radius = 8
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=5; color=gray; }
 }
 
-set fiber actin
+set single protein
 {
-    rigidity = 0.1
-    segmentation = 0.2
-    confine = off, 100
-    glue = 3, anchor
-    display = ( line=1, 2; )
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
-set hand myosin
+set hand motor
 {
-    binding_rate = 10
-    binding_range = 0.005
-    unbinding_rate = 0.02
-    unbinding_force = 3
+    binding = 9, 0.01
+    unbinding = 0.25, 3
     
     activity = move
-    unloaded_speed = 1
-    stall_force = 6
-    display = ( size=4; color=orange )
+    unloaded_speed = 1.0
+    stall_force = 5
+
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set hand binder
+set couple bimotor
 {
-    binding_rate = 10
-    binding_range = 0.005
-    unbinding_rate = 0.02
-    unbinding_force = 3
-    display = ( size=4; color=gray )
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 10
 }
 
-set hand glue
+set hand dynein
 {
-    binding_rate = 10
-    binding_range = 0.005
-    unbinding_rate = 0
-    unbinding_force = inf
-    display = ( size=6; color=green )
+    binding = 9, 0.01
+    unbinding = 0.25, 3
+
+    activity = move
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=5; width=4; )
 }
 
-set single anchor
+set couple bidynein
 {
-    hand = glue
-    stiffness = 500
-    activity = fixed
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 10
 }
 
-set couple motor
+set hand binder
 {
-    hand1 = myosin
-    hand2 = myosin
-    stiffness = 500
-    diffusion = fast
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-set couple crosslinker
+set couple bibinder
 {
     hand1 = binder
     hand2 = binder
-    stiffness = 500
-    diffusion = fast
+    stiffness = 100
+    diffusion = 1
 }
 
-new 300 actin
+new cell
 {
-    length = 5
+    order = 7
+    radius = 11
 }
 
-run 5 system
-
-change actin { glue = 0 }
+new 300 protein
+new 4000 bimotor
 
-new 5000 motor
-new 5000 crosslinker
-
-run 1000 system
-{   
-    nb_frames = 10
+run 10000000 system
+{
+    nb_frames = 0
 }
```

### Comparing `cytosim-0.0.3/cym/contract_periodic.cym` & `cytosim-0.0.4/src/misc/installation/builder/config8.cym`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,128 @@
-% A contractile network in half_periodic box
-% FJN, 09.01.2020
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.001
+    time_step = 0.01
     viscosity = 0.5
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=2; label="Cytoskeleton" )
 }
 
-set system display { style=2; point_size=5; }
-
 set space cell
 {
-    shape = semi_periodic
+    shape = polygon
+    display = ( color=dark_gray; width=4; )
 }
 
-new cell
+set fiber filament
 {
-    length = 10, 2
+    rigidity = 10
+    segmentation = 0.25
+    confine = inside, 100
+    lattice = 1, 0.010
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 15
+    total_polymer = 5000
+
+    display = ( plus_end=5; color=dark_gray; width=2; )
 }
 
-set fiber filament
+set hand nucleator
 {
-    rigidity = 0.5
-    segmentation = 0.1
-    confine = inside, 100
-    display = ( line=0.5, 1; color=gray; )
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=gray; }
+}
+
+set single protein
+{
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
 set hand motor
 {
-    binding = 10, 0.02
-    unbinding = 0.1, inf
+    binding = 9, 0.02
+    unbinding = 0.2, 3
+    
+    activity = walk
+    step_size = 0.010
 
-    activity = move
-    unloaded_speed = -0.2
-    stall_force = 6
-    display = ( width=0.5; color=green; )
+    unloaded_speed = 1.0
+    stall_force = 5
+
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set couple complex
+set couple bimotor
 {
     hand1 = motor
     hand2 = motor
-    stiffness = 250
-    diffusion = 10
-    fast_diffusion = 1
+    stiffness = 100
+    diffusion = 1
+    length = 0.1
 }
 
-set hand binder
+set hand dynein
 {
-    binding = 10, 0.02
-    unbinding = 0.1, inf
-    display = ( width=0.5; color=blue; )
+    binding = 9, 0.02
+    unbinding = 0.25, 3
+
+    activity = walk
+    step_size = 0.010
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=7; width=5; )
 }
 
-set couple crosslinker
+set couple bidynein
 {
-    hand1 = binder
-    hand2 = binder
-    stiffness = 250
-    diffusion = 10
-    fast_diffusion = 1
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 1
+    length = 0.1
 }
 
-new 60 filament
+set hand binder
 {
-    length = 4
-    placement = all_inside
-}
+    binding = 21, 0.012
+    unbinding = 0.5, 3
 
-new 200 crosslinker
-new 200 complex
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
+}
 
-new event
+set couple bibinder
 {
-    delay = 1;
-    code = "report fiber:tension *"
+    hand1 = binder
+    hand2 = binder
+    stiffness = 100
+    diffusion = 1
 }
 
-run 100000 system
+new cell
 {
-    nb_frames = 100
+    points=10 -5.7, 10 5.7, -10 5.7, -10 -5.7;
 }
 
+new 7 filament { length=24; position=rectangle 4 6; orientation=1 -0.05 0; }
+new 2 filament { length=24; position=0 0; orientation=1 0.1 0; }
+new 1000 bimotor
+
+run 10000000 system
+{
+    nb_frames = 0
+}
```

### Comparing `cytosim-0.0.3/cym/cut_saved.cym` & `cytosim-0.0.4/src/misc/installation/builder/config5.cym`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,124 @@
-% a laser cut with file storage
-% F. Nedelec
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.001
-    viscosity = 0.05
+    time_step = 0.01
+    viscosity = 0.2
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=2; zoom=0.6; label="Cytoskeleton" )
 }
 
-
 set space cell
 {
-    shape = circle
+    shape = polygon
+    display = ( color=gray; width=4; )
 }
 
-new cell
+set fiber filament
 {
-    radius = 5
+    rigidity = 10
+    segmentation = 0.5
+    confine = inside, 100
+
+    activity      = classic
+    growing_speed = 0.5
+    shrinking_speed = -2.0
+    catastrophe_rate = 0.05
+    max_length    = 10
+    total_polymer = 5000
+
+    display = ( color=dark_gray; width=1; )
 }
 
-set fiber actin
+set hand nucleator
 {
-    rigidity = 0.1
-    segmentation = 0.25
-    confine = inside, 100
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=gray; }
+}
+
+set single protein
+{
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
-set hand myosin
+set hand motor
 {
-    binding_rate = 10
-    binding_range = 0.01
-    unbinding_rate = 0.01
-    unbinding_force = 3
+    binding = 9, 0.01
+    unbinding = 0.25, 3
     
     activity = move
-    unloaded_speed = 1
+    unloaded_speed = 1.0
     stall_force = 5
-    display = { size = 4; color=green }
+
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set hand binder
+set couple bimotor
 {
-    binding_rate = 10
-    binding_range = 0.01
-    unbinding_rate = 0.01
-    unbinding_force = 3
-    display = { size = 2; color=blue }
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 10
 }
 
+set hand dynein
+{
+    binding = 9, 0.01
+    unbinding = 0.25, 3
+
+    activity = move
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
 
-set couple motor
+    display = ( color=blue, 0x0000AA77; size=7; width=5; )
+}
+
+set couple bidynein
+{
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 10
+}
+
+set hand binder
 {
-    hand1 = myosin
-    hand2 = myosin
-    stiffness = 250
-    diffusion = fast
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-set couple crosslinker
+set couple bibinder
 {
     hand1 = binder
     hand2 = binder
-    stiffness = 250
-    diffusion = fast
+    stiffness = 100
+    diffusion = 1
 }
 
-new 100 actin
+new cell
 {
-    length = 5
+    order = 8
+    radius = 11
 }
 
-new 2500 motor
-new 2500 crosslinker
-
-run 500 system
-
-export objects cut.cmo { append=0; binary=0 }
-
-cut actin { plane = 1 0 0, 0 }
-cut actin { plane = 0 1 0, 0 }
-
-run 1000 system
-
-export objects cut.cmo { append=1; binary=0 }
-import objects cut.cmo { append=0; frame=1; }
-
-run 1000 system
-
-export objects cut.cmo { append=1; binary=0 }
+new 64 protein
+new 2000 bimotor
 
+run 10000000 system
+{
+    nb_frames = 0
+}
```

### Comparing `cytosim-0.0.3/cym/endocytosis.cym` & `cytosim-0.0.4/src/misc/installation/master/config6.cym`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 % F. Nedelec, in Switzerland towards Bern, 27.11.2013
 % F. Nedelec, Strasbourg, 19-21.09.2015
 % Using implicit torque, F. Nedelec, Cambridge, 03.2019
 
 set simul system
 {
     dim = 3
-    time_step = 0.0002
-    viscosity = 1
+    time_step = 0.001
+    viscosity = 10
     steric = 1, 50000
     steric_max_range = 0.05
-    display = ( point_value=0.001; style=3; back_color=black; zoom=2; rotation=0.81 -0.59 0 0; )
+    display = ( point_value=0.001; style=3; back_color=black; zoom=1.5; rotation= 0.81 -0.59 0 0; )
 }
 
 % simulation space
 set space cylinder
 {
     shape = cylinderZ
     display = ( color=0x00000044, dark_gray; visible=3 )
 }
 
-% flat disc at the base of the cell:
+% very thin cylinder at the base of the cell:
 set space base
 {
     shape = cylinderZ
     display = ( color=0x0000FF44; visible=1 )
 }
 
 % just a single point:
@@ -33,34 +33,26 @@
     shape = cylinderZ
     display = ( color=red; visible=3 )
 }
 
 set fiber actin
 {
     rigidity = 0.08
-    steric = 1, 0.0035  % should be greater than 0.0035 nm
-    segmentation = 0.00275   % 0.0055 is 2 monomers
+    steric = 1, 0.004  % should be greater than 0.0035 nm
+    segmentation = 0.0055   % 0.0055 is 2 monomers
     confine = inside, 50000, cylinder
     drag_radius = 0.004
     lattice = 1, 0.00275
 
     activity = grow
     growing_speed = 0.550   % Berro JMB 2010 says 550 nm/s or 200 monomers / sec
     growing_force = inf
     max_length = 0.055
-}
-
-set actin display
-{
-    line = 7, 1;
-    point = 7, 0;
-    color = 0xFF000077, 0xFF000077;
-    end_color = red, orange;
-    end_size = 7;
-    line_caps = 2;
+    
+    display = ( line=7, 1; point=7, 0; color=0xFF000077, 0xFF000077; end_color=red, orange; end_size=7; line_caps=2; )
 }
 
 set hand binder
 {
     binding = 10, 0.018
     unbinding = 0.5, inf
     
@@ -112,24 +104,23 @@
     activity = bridge
     length = 0.012
 }
 
 set solid blob
 {
     steric = 1
-    viscosity = 50
-    confine = inside, 10000, pin
+    confine = inside, 20000, pin
     display = ( color=blue; style=1; )
 }
 
 new cylinder
 {
-    radius = 0.150
-    bottom = -0.030
-    top = 0.100
+     radius = 0.150
+     bottom = -0.030
+     top = 0.100
 }
 new base
 {
     radius = 0.050
     bottom = -0.030
     top = -0.027
 }
@@ -149,17 +140,16 @@
     point2 = 0 0 0.010, 0
     position = 0 0 -0.040
     placement = anywhere
 }
 
 new 3 actin
 {
-    length = 0.00275;
+    length = 0.0055;
     position = 0 0 -0.030
-    plus_end=grow;
 }
 
 new link
 {
     base = solid1, point2
     attach = fiber1, 0
 }
@@ -175,23 +165,23 @@
     base = solid1, point2
     attach = fiber3, 0
 }
 
 
 run system
 {
-    nb_steps = 10000
+    nb_steps = 2000
     nb_frames = 50
 }
 
 mark actin { mark = 0; }
 
 run system
 {
-    nb_steps = 20000
+    nb_steps = 4000
     nb_frames = 100
 }
 
 change blob
 {
     confine = none
 }
```

### Comparing `cytosim-0.0.3/cym/fiber_glue.cym` & `cytosim-0.0.4/src/misc/installation/master/config8.cym`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,91 @@
-%{
- @example fiber_glue.cym
- Parameter fiber:glue is set link fiber with the boundaries:
- - it creates a Single, everytime a fiber contacts the surface.
- - the Single is deleted if the associated Hand detaches.
- .
- F. Nedelec, February 2011
-}
+% Microtubules in interphase S.pombe
+% Francois Nedelec, Aug. 4, 2009
+% NOTE: parameters use units of picoNewton, micrometer, second
+
 
 set simul system
 {
-    time_step = 0.01
-    viscosity = 0.1
-    display = { delay=4; }
+    dim = 3
+    time_step  = 0.01
+    kT         = 0.0042
+    viscosity  = 0.9
+    precondition = 0
+    display = ( delay=4; )
 }
 
-set space cell
+set space cytoplasm
 {
-    shape = sphere
+    shape = capsule
+    display = ( color=red; visible=0; )
 }
 
-new cell
-{
-    radius = 5
-}
-
-set hand strong_hand
+set space cell
 {
-    unbinding_rate = 0
-    unbinding_force = 1e6
-    hold_growing_end = 1
-    hold_shrinking_end = 1
-    display = { size=8 }
+    shape = capsule
+    display = ( color=0x7777770F, black; visible=3; )
 }
 
-set single cortical_glue
-{
-    hand = strong_hand
-    stiffness = 10
-    activity = fixed
-}
 
-set fiber microtubule
+set fiber filament
 {
-    rigidity = 30
-    segmentation = 0.5
-    confine = inside, 100
-    glue = 2, cortical_glue
-
+    rigidity       = 30
+    segmentation   = 0.5
+    confine        = inside, 200, cytoplasm
+    
     activity        = dynamic
     unit_length     = 0.008
-    growing_speed   = 0.16
-    shrinking_speed = -0.25
-    hydrolysis_rate = 0.06
+    growing_speed   = 0.06
+    shrinking_speed = -0.15
+    hydrolysis_rate = 0.058
     growing_force   = 1.7
     persistent      = 1
     rebirth_rate    = 1
     min_length      = 0.5
+    display = ( line_width=5; plus_end=15; minus_end=15; )
+}
+
+set sphere envelope
+{
+    point_mobility = 0.05
+    confine        = all_inside, 200, cytoplasm
+    piston_effect  = 1
     
-    display = { line=8, 2; point=1; speckles=7, 2, 0.25; tension=-10 }
+    display = ( color=0x0000FF88; size=12; style=15 )
+}
+
+set bundle bunch
+{
+    overlap   = 0.5
+    stiffness = 1000
 }
 
-set solid core
+set nucleus noyau
 {
-    display = ( style=3 )
+    stiffness  = 200
 }
 
-set aster centrosome
+new cytoplasm
 {
-    stiffness = 1000, 500
+    length = 10
+    radius = 1.62
 }
 
-new centrosome
+new cell
 {
-    solid = core
-    radius = 0.5
-    fibers = 20, microtubule, ( length = 2; plus_end = grow; )
-    position = 0 0 0
+    length = 10.2
+    radius = 1.72
 }
 
+new noyau
+{
+    sphere       = envelope
+    bundles      = 4, bunch, (fibers=2, filament, (length=0.5; plus_end=grow;))
+    radius       = 1.1
+    position     = 3.5 0 0
+}
 
-run 100000 system
+run system
 {
-    nb_frames = 100
+    nb_steps   = 50000
+    nb_frames  = 100
 }
```

### Comparing `cytosim-0.0.3/cym/france.txt` & `cytosim-0.0.4/src/misc/installation/builder/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/cym/glide_stripe.cym` & `cytosim-0.0.4/src/misc/installation/builder/config4.cym`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,122 @@
-% A gliding assay, with stripes of two motors of opposite directionality
-% run in 2D
-
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    dim = 2
-    time_step = 0.005
-    viscosity = 0.5
-    display = { window_size=800,400 }
+    time_step = 0.01
+    viscosity = 0.2
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=4; zoom=0.6; label="Cytoskeleton" )
 }
 
 set space cell
 {
-    shape = periodic
+    shape = polygon
+    display = ( color=gray; width=4; )
 }
 
-new cell
+set fiber filament
 {
-    length = 20, 10
+    rigidity = 10
+    segmentation = 0.4
+    confine = inside, 100
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 10
+    total_polymer = 5000
+
+    display = ( color=dark_gray; width=1; )
 }
 
-set fiber microtubule
+set hand nucleator
 {
-    %taxol-stabilized microtubule are more flexible 
-    rigidity = 10
-    segmentation = 0.5
-    display = { line_width=6 }
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=gray; }
 }
 
-set hand kinesin
+set single protein
 {
-    binding_rate = 5
-    binding_range = 0.01
-    unbinding_rate = 0.3
-    unbinding_force = 3
-        
-    activity = move
-    unloaded_speed = 0.6
-    stall_force = 6
-
-    display = { color=0x0000FF99; size=8 }
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
-set hand dynein
+set hand motor
 {
-    binding_rate = 5
-    binding_range = 0.01
-    unbinding_rate = 0.3
-    unbinding_force = 3
+    binding = 9, 0.01
+    unbinding = 0.25, 3
     
     activity = move
-    unloaded_speed = -0.6
-    stall_force = 6
+    unloaded_speed = 1.0
+    stall_force = 5
 
-    display = { color=0xFF990099; size=8 }
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set single gKinesin
+set couple bimotor
 {
-    hand = kinesin
+    hand1 = motor
+    hand2 = motor
     stiffness = 100
-    activity = fixed
+    diffusion = 10
 }
 
-set single gDynein
+set hand dynein
 {
-    hand = dynein
-    stiffness = 100
-    activity = fixed
+    binding = 9, 0.01
+    unbinding = 0.25, 3
+
+    activity = move
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=7; width=5; )
 }
 
-new 2 microtubule
+set couple bidynein
 {
-    length = 12
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 10
 }
 
-new 2500 gKinesin ( stripe  -5  5  )
-new 1200 gDynein  ( stripe   5  10 )
-new 1200 gDynein  ( stripe -10 -5  )
+set hand binder
+{
+    binding = 21, 0.012
+    unbinding = 0.5, 3
 
-set system display
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
+}
+
+set couple bibinder
 {
-    label = (Motor stripes -)
-    delay = 10
-    tile  = 1, 1
-    style = 2
+    hand1 = binder
+    hand2 = binder
+    stiffness = 100
+    diffusion = 1
 }
 
-run system
+new cell
 {
-    nb_steps = 10000
-    nb_frames = 50
+    order = 9
+    radius = 11
 }
 
+new 64 protein
+new 2000 bimotor
+
+run 10000000 system
+{
+    nb_frames = 0
+}
```

### Comparing `cytosim-0.0.3/cym/minifilaments1.cym` & `cytosim-0.0.4/src/misc/installation/builder/config3.cym`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,122 @@
-%
-% Here, multifunctional motors are build using a rigid mini-filament backbone,
-% and using `specificity' we constrain the binding to anti-parallel configuration.
-%
-% F. Nedelec, 06.09.2018
+% Self-organization of filaments driven by bivalent motors
+% FJN for Festival of plants, 14.05.2019
 
 set simul system
 {
-    time_step = 0.001
-    viscosity = 0.1
-    display = ( style=2; point_size=9; line_width=4; )
+    time_step = 0.01
+    viscosity = 0.2
+    precondition = 0
+    binding_grid_step = 0.25
+    display = ( style=2; delay=4; period=2; zoom=0.6; label="Cytoskeleton" )
 }
 
 set space cell
 {
-    shape = circle
-}
-
-new cell
-{
-    radius = 1
+    shape = polygon
+    display = ( color=gray; width=4; )
 }
 
 set fiber filament
 {
-    binding_key = 1
-    rigidity = 1
-    segmentation = 0.1
-    display = ( line=1, 1; color=white; tension=10;)
+    rigidity = 10
+    segmentation = 0.5
+    confine = inside, 100
+
+    activity      = grow
+    growing_speed = 0.5
+    max_length    = 10
+    total_polymer = 5000
+
+    display = ( color=dark_gray; width=1; )
 }
 
-set fiber myofilament
-{
-    binding_key = 2
-    confine = inside, 1
-    rigidity = 100
-    segmentation = 1
-    display = ( line=3; color=dark_green; tension=1; )
+set hand nucleator
+{
+    unbinding = 0, 3
+    activity = nucleate
+    nucleate = 1.0, filament, ( length=0.1; plus_end=grow; )
+    display = { size=7; color=gray; }
 }
 
-set hand binder
+set single protein
 {
-    binding_key = 3
-    binding = 5, 0.01
-    unbinding = 0, inf
-    display = ( color=green; )
+    hand = nucleator
+    diffusion = 0.1
+    stiffness = 100
 }
 
 set hand motor
 {
-    binding_key = 1
-    binding = 5, 0.1
-    unbinding = 1, inf
+    binding = 9, 0.01
+    unbinding = 0.25, 3
     
     activity = move
-    unloaded_speed = 0.5
-    stall_force = 6
-    
-    display = ( color=green, 0x00FF00B0; )
+    unloaded_speed = 1.0
+    stall_force = 5
+
+    bind_also_end = 0
+    hold_growing_end = 0.98
+
+    display = ( color=green, 0x00EE0044; size=7; width=5; )
 }
 
-set single holder
+set couple bimotor
 {
-    hand = binder
-    stiffness = 250
-    activity = fixed
+    hand1 = motor
+    hand2 = motor
+    stiffness = 100
+    diffusion = 10
 }
 
-set couple myosinP
+set hand dynein
 {
-    hand1 = binder
-    hand2 = motor
-    stiffness = 400
-    diffusion = 100
-    specificity = parallel
+    binding = 9, 0.01
+    unbinding = 0.25, 3
+
+    activity = move
+    unloaded_speed = -1.0
+    stall_force = 3
+
+    bind_also_end = 1
+    hold_growing_end = 0.98
+
+    display = ( color=blue, 0x0000AA77; size=7; width=5; )
 }
 
-set couple myosinA
+set couple bidynein
 {
-    hand1 = binder
-    hand2 = motor
-    stiffness = 400
-    diffusion = 100
-    specificity = antiparallel
+    hand1 = dynein
+    hand2 = dynein
+    stiffness = 100
+    diffusion = 10
 }
 
-new 2 filament
+set hand binder
 {
-    length = 2
-    position = 0 0 0
-    % immobilize the two ends:
-    attach1 = holder, 0, plus_end
-    attach2 = holder, 0, minus_end
+    binding = 21, 0.012
+    unbinding = 0.5, 3
+
+    display = ( color=blue, 0x0000FF77; size=7; width=5; )
 }
 
-new 16 myofilament
+set couple bibinder
 {
-    length = 0.3
-    % attach a motor at each end:
-    attach1 = myosinA, 0   , minus_end
-    attach2 = myosinA, 0.02, minus_end
-    attach3 = myosinA, 0.04, minus_end
-    attach4 = myosinP, 0.04, plus_end
-    attach5 = myosinP, 0.02, plus_end
-    attach6 = myosinP, 0   , plus_end
+    hand1 = binder
+    hand2 = binder
+    stiffness = 100
+    diffusion = 1
 }
 
-run 10000 system
-{   
-    nb_frames = 20
+new cell
+{
+    order = 8
+    radius = 11
 }
 
+new 64 protein
+new 2000 bimotor
 
+run 10000000 system
+{
+    nb_frames = 0
+}
```

### Comparing `cytosim-0.0.3/doc/tutorials/code/collect.py` & `cytosim-0.0.4/python/look/collect.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
-# collect.py
+# collect.py renames files from subdirectories
 #
-# Copyright F. Nedelec, 2007--2018
+# Copyright F. Nedelec, 2007--2021
 
 
 """
 Synopsis:
     
     Rename files or folders following a pattern containing an integer index,
     as in 'image0001.png'. The file will be moved in the current directory
@@ -21,21 +21,21 @@
     collect.py PATTERN [INTEGER] [--copy] PATH1 [PATH2] [PATH3] ...
 
 Arguments:
     
     PATTERN specifies the name of the output files, and should contain a variable
     part that will be replaced by an integer. It can be a 'scanf' compatible 
     pattern such as '%i' or '%0Xi', for example 'image%04i.png'.
-    A character '%' repeated multiple times, such as `%%%%` or `%%%%%%`, can be 
-    used to directly specify the size of the integer portion of the name.
+    A character '%' repeated multiple times, such as `%%%%` or `%%%%%%`, can
+    also be used to specify the size of the integer portion of the name.
     
-    The pattern can include a directory, and if this directory does not exist,
-    collect.py will attemtps to create it before moving the file.
+    The pattern can include a '/' that would indicate a directory, and if this
+    directory does not exist, collect.py will create it before moving the file.
 
-    if specified, --copy will copy the files/directory instead of moving them
+    if specified, `--copy` will copy the files/directory instead of moving them
     
     if specified, INTEGER is the first index to be used (default=0)
 
     PATH1, PATH2, etc. is a list of files or directories
 
 Examples:
     
@@ -44,102 +44,93 @@
     
     collect.py --copy image%%%%.png 1 run*/image.png
        will copy the image files, starting at index 1
 
     collect.py run%%%%/config.cym config*.cym
        will create directories `run????` and move the `config*.cym` files into them
     
-F. Nedelec, 2012--2018. Last modified 2.10.2017
+F. Nedelec, 2012--2021. Last modified 6.10.2021
 """
 
 
 import sys, shutil, os, curses.ascii
 
 
 #------------------------------------------------------------------------
 
-def copy_recursive(src, dst):
-    """Copy directory recursively"""
-    if os.path.isfile(src):
-        shutil.copy2(src, dst)
-    elif os.path.isdir(src):
-        try:
-            os.mkdir(dst)
-        except OSError:
-            pass
-        files = os.listdir(src)
-        for f in files:
-            s = os.path.join(src, f)
-            d = os.path.join(dst, f)
-            copy_recursive(s, d)
+def cannonical_pattern(arg):
+    """check for repeated '%' character, replacing printf syntax: %04i """
+    c = arg.count('%')
+    for n in range(c,1,-1):
+        if arg.find('%'*n) > 0:
+            return arg.replace('%'*n, '%0'+str(n)+'i', 1);
+    return arg
 
 
-def main(args):
-    """rename files"""
-    do_copy = False
-    arg = args.pop(0);
-    # check if 'copy' specified before pattern
-    if arg=='-c' or arg=='--copy' or arg=='copy=1':
-        do_copy = True
-        pattern = args.pop(0);
-    else:
-        pattern = arg
+def validate_pattern(arg):
     # check validity of the pattern
-    if os.path.isfile(pattern):
+    if os.path.isfile(arg):
         sys.stderr.write("Error: first argument should be the pattern used to build output file name")
-        return 1
+        sys.exit(1)
     try:
-        res = ( pattern % 0 )
+        res = ( arg % 0 )
     except:
-        # check for repeated '%' character:
-        for n in range(10,0,-1):
-            s = pattern.find('%'*n)
-            if s > 0:
-                pattern = pattern.replace('%'*n, '%0'+str(n)+'i', 1);
-                break
-        try:
-            res = ( pattern % 0 )
-        except:
-            sys.stderr.write("Error: the pattern should accept an integer: eg. '%04i'\n")
-            return 1
+        arg = cannonical_pattern(arg)
+    try:
+        res = ( arg % 0 )
+    except:
+        sys.stderr.write("Error: the pattern should accept an integer: eg. '%04i'\n")
+        sys.exit(1)
     for c in res:
         if curses.ascii.isspace(c):
             sys.stderr.write("Error: the pattern includes or generates white space character\n")
-            return 1
-    # go
-    paths = []
-    idx = 0
+            sys.exit(1)
+    return arg
+
+
+def main(args):
+    """rename files"""
+    do_copy = False
+    arg = args[0]
+    # check if 'copy' specified before pattern
+    if arg=='-c' or arg=='--copy' or arg=='copy=1':
+        do_copy = True
+        args.pop(0);
+    # get pattern for moving files:
+    pattern = validate_pattern(args.pop(0))
     # parse arguments:
+    idx = 0
+    paths = []
     for arg in args:
         if arg=='-c' or arg=='--copy' or arg=='copy=1':
             do_copy = True
         elif args[0].isdigit():
             idx = int(args[0])
         elif os.path.isfile(arg) or os.path.isdir(arg):
             paths.append(arg)
         else:
             sys.stderr.write("Error: '%s' is not a file or directory" % arg)
             return 1
-    # process all files
+    # process all files:
     res = []
     for src in paths:
         while idx < 1000000:
             dst = pattern % idx
             idx += 1
             if dst == src:
                 res.append(dst)
                 break
             if not os.path.exists(dst):
-                #make directory if name include a directory that does not exist:
+                #make directory if name includes a non-existent directory:
                 dir = os.path.dirname(dst)
                 if dir and not os.path.isdir(dir):
                     os.mkdir(dir)
                 # process file:
                 if do_copy:
-                    copy_recursive(src, dst)
+                    shutil.copytree(src, dst)
                 else:
                     os.rename(src, dst)
                 res.append(dst)
                 print("%s -> %s" % (src, dst))
                 break
     return res
```

### Comparing `cytosim-0.0.3/doc/tutorials/code/scan.py` & `cytosim-0.0.4/python/look/scan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,163 @@
 #!/usr/bin/env python
 #
-# scan.py
+# scan.py executes a given command sequentially or in parallel, in specified directories
 #
-# copyright  F. Nedelec and S. Dmitrieff 2007--2018
+# Copyright  F. Nedelec and S. Dmitrieff; 2007--2022
 
 """
-    Execute specified command in given directories, sequentially using a given number of processes
+    Execute specified command in given directories, sequentially or in parallel,
+    using independent threads.
  
 Syntax:
 
-    scan.py command directory1 [directory2] [directory3] [...] [jobs=N]
+    scan.py command [-][+] directory1 [directory2] [directory3] [...] [jobs=INTEGER]
     
-Example:
+    if '-' is specified, output is limited to what the command does
+    if '+' is specified, the directory path is printed without decoration
+    if 'jobs' is set, run in parallel using specified number of threads
+
+Examples:
     
+    scan.py 'play image' run*
     scan.py 'play image' run* jobs=2
     
-F. Nedelec, 02.2011, 09.2012, 03.2013, 01.2014, 06.2017
-S. Dmitreff, 06.2017
+    
+F. Nedelec 02.2011, 09.2012, 03.2013, 01.2014, 06.2017, 07.2021, 21.03.2022, 8.04.2022
+S. Dmitreff 06.2017
 """
 
 try:
     import sys, os, subprocess
 except ImportError:
     sys.stderr.write("Error: could not load necessary python modules\n")
     sys.exit()
 
-executable = 'pwd'
-out = sys.stderr
-njobs = 1
+err = sys.stderr
+out = sys.stdout
+verbose = 2
 
 #------------------------------------------------------------------------
 
-def execute(path):
+def assemble(path, lines, verb):
+    """
+    Assembles lines for output according to 'verb' argument
+    """
+    res = ''
+    if verb == 2:
+        sys.stderr.write('-  '*24+path+"\n")
+        for s in lines:
+            res += s
+    elif verb == 1:
+        res = os.path.basename(path) + " "
+        for s in lines:
+            res += s.replace('\n', ' ')
+        res += '\n'
+    else:
+        for s in lines:
+            res += s
+    return res
+
+
+def execute(tool, path, verb):
     """
     run executable in specified directory
     """
-    os.chdir(path)
-    out.write('-  '*24+path+"\n")
+    lines = []
     try:
-        subprocess.call(executable, shell=True)
+        os.chdir(path)
+        sub = subprocess.Popen(tool, shell=True, stdout=subprocess.PIPE)
+        for s in sub.stdout:
+            lines.append(s.decode())
+        sub.stdout.close()
     except Exception as e:
-        sys.stderr.write("Error: %s\n" % repr(e));
+        err.write("Error: %s\n" % repr(e));
+    res = assemble(path, lines, verb)
+    out.write(res)
+    out.flush()
 
 
-def execute_queue(queue):
+def worker(queue):
     """
-    run executable sequentially in directories specified in paths
+    run executable taking argument from queue
     """
     while True:
         try:
-            arg = queue.get(True, 1)
-            execute(arg)
+            t, p, v = queue.get(True, 1)
         except:
             break;
+        execute(t, p, v)
 
 
 def main(args):
     """
         read command line arguments and process command
     """
-    global executable
+    global verbose
+    
+    if args[0] == '-':
+        verbose = 0
+        args.pop(0)
+    elif args[0] == '+':
+        verbose = 1
+        args.pop(0)
+    
     try:
-        executable = args[0]
+        tool = args[0]
     except:
-        out.write("Error: you should specify a command to execute\n")
+        err.write("Missing command: scan.py command [-][+] directory1 [directory2]...\n")
         return 1
 
     njobs = 1
     paths = []
     for arg in args[1:]:
         if os.path.isdir(arg):
             paths.append(os.path.abspath(arg))
         elif arg.startswith('nproc=') or arg.startswith('njobs='):
             njobs = int(arg[6:])
         elif arg.startswith('jobs='):
             njobs = int(arg[5:])
+        elif arg == '-':
+            verbose = 0
+        elif arg == '+':
+            verbose = 1
         else:
-            out.write("  Warning: unexpected argument `%s'\n" % arg)
+            err.write("  Warning: unexpected argument `%s'\n" % arg)
             sys.exit()
 
     if not paths:
-        out.write("Error: you should specify at least one directory\n")
+        err.write("Missing directories: scan.py command [-][+] directory1 [directory2]...\n")
+        err.write(" (scan.py would execute `%s`)\n"%tool)
         return 2
     
-    if njobs > len(paths):
-        njobs = len(paths)
+    njobs = min(njobs, len(paths))
     
-    #process in parallel with child threads:
     if njobs > 1:
+        #process in parallel with child threads:
         try:
             from multiprocessing import Process, Queue
             queue = Queue()
             for p in paths:
-                queue.put(p)
-            jobs = [Process(target=execute_queue, args=(queue,)) for n in range(njobs)]
-            for job in jobs:
-                job.start()
-            for job in jobs:
-                job.join()
+                queue.put((tool, p, verbose))
+            jobs = []
+            for n in range(njobs):
+                j = Process(target=worker, args=(queue,))
+                jobs.append(j)
+                j.start()
+            # wait for completion of all jobs:
+            for j in jobs:
+                j.join()
             return 0
         except ImportError:
-            out.write("Warning: multiprocessing unavailable\n")
+            err.write("Warning: multiprocessing module unavailable\n")
     #process sequentially:
     for p in paths:
-        execute(p)
+        execute(tool, p, verbose)
     return 0
 
 #------------------------------------------------------------------------
 
 if __name__ == "__main__":
-    if len(sys.argv) < 2 or sys.argv[1].endswith("help"):
+    if len(sys.argv) < 3 or sys.argv[1].endswith("help"):
         print(__doc__)
     else:
         main(sys.argv[1:])
```

### Comparing `cytosim-0.0.3/doc/tutorials/tuto_centering.md` & `cytosim-0.0.4/src/sim/simul_prop.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,366 +1,294 @@
-# Tutorial: Aster Positionning
+// Cytosim was created by Francois Nedelec. Copyright 2007-2017 EMBL.
+#ifndef SIMUL_PROP_H
+#define SIMUL_PROP_H
+
+
+#include "real.h"
+#include "vector.h"
+#include "property.h"
+
+class SpaceProp;
+class Simul;
+class Space;
+
+
+/**
+ Enables capacity to simulate constant fluid flow that transports all objects
+ Option normally OFF
+ */
+#define NEW_CYTOPLASMIC_FLOW 0
+
+/**
+ @defgroup Parameters All object parameters
+ List of parameters for user-accessible objects.
+ */
+
+
+/// Property for Simul
+/** 
+ There is normally only one instantiation of this class.
+ 
+ @ingroup Properties
+ */
+class SimulProp : public Property
+{
+    friend class Simul;
+    
+public:
+    
+    /**
+     @defgroup Properties All Object Properties
+     List of properties accessible to the user.
+     */
+
+    /**
+     @defgroup SimulPar Parameters of Simul
+     @ingroup Parameters
+     @{
+     */
+    
+    
+    /// Current time in the simulated world
+    real      time;
+
+    /// A small interval of time
+    /**
+     The `time_step` is the amount of time between two consecutive simulation states.
+     It controls the precision of the simulation, at the expense of computation.\n
+     We expect that the numerical result will converge to the true mathematical solution
+     of the equations when `time_step` becomes infinitely small, but we do not necessarily 
+     know how fast this convergence will be. Thus it is not usually possible to 
+     calculate the precision as a function of the `time_step`.\n
+     To check that `time_step` is appropriate for a particular problem, one should 
+     always run several simulations where `time_step` is varied systematically.
+     
+     Useful rules:
+     - A smaller time step is always preferable, provided that the time to run the simulation
+     remains acceptable,
+     - You should always check that the results of two simulations with <em>time_step=h</em>\
+     and <em>time_step=h/2</em> are identical. If this is not the case, then `h`\
+     is most likely not an appropriate value for `time_step`,
+     - If some reaction in the simulation occures with a rate R, then `time_step`\
+     should be such that <em>time_step * R << 1</em>. In practice `time_step * R` should not be higher than 0.2.
+     .
+     */
+    real      time_step;
+    
+    
+    /// Ambient viscosity
+    /**
+     The viscosity of the medium should be given in units of pN.s/um^2 = Pa.s.
+     <em>The default value is 1</em>
+     
+     Medium                | Viscosity | Reference                             |
+     ----------------------|-----------|----------------------------------------
+     Water                 |  0.001    | http://en.wikipedia.org/wiki/Viscosity
+     C.elegans embryo      |  ~1       | Daniels et al. 10.1529/biophysj.105.080606  http://dx.doi.org/10.1529/biophysj.105.080606
+     C.elegans embryo      |  ~0.5     | Garzon-Coral et al. 10.1126/science.aad9745  http://dx.doi.org/10.1126/science.aad9745
+     S.pombe               |  ~1       | Tolic et al. PRL 93, 078102 (2004). http://dx.doi.org/10.1103/PhysRevLett.93.078102
+     D.melanogaster embryo |  ~0.312   | Mechanical Aspects of Drosophila Gastrulation, Oleg Polyakov PhD Thesis. Princeton U., 9.2013
+     Cleared egg cytoplasm |  ~0.02    | Valentine et al. Biophys J 88, 680–689 (2005). http://dx.doi.org/10.1529/biophysj.104.048025
+     Cultivated cells      |  ~1       | Kole et al. Mol Bio Cell 15, 3475--84 (2004) http://dx.doi.org/10.1091/mbc.E04-03-0218
+     
+     Note that non-linear effects are not taken into account in Cytosim. Hydrodynamic effects are also neglected, such that the drag coefficient of a collection of objects is simply the sum of the individual drag coefficients. However, an `effective` viscosity can be set for each object class, and with this option, it is possible to adjust the drag coefficient of the collection to a realistic value.
+     */
+    real      viscosity;
+    
+#if NEW_CYTOPLASMIC_FLOW
+    /// uniform and constant fluid flow
+    Vector    flow;
+#endif
+
+    /// Energy of Brownian motion in the system = Temperature * Boltzman constant
+    /**
+     <em>kT</em> is the product of the [Boltzmann constant](http://en.wikipedia.org/wiki/Boltzmann_constant) `k`
+     by the [Thermodynamic temperature](http://en.wikipedia.org/wiki/Thermodynamic_temperature) in Kelvin:
+     - k = 1.38065 x 10^-23 Joule/Kelvin = 13.8065 x 10^-6 pN.um / Kelvin
+     - Kelvin = Celsius + 273.15
+     .
+     
+     Celsius   | Kelvin   |  kT            |
+     ----------|----------|-----------------
+     ~10 C     |  283 K   |  0.0039  pN.um
+     ~24 C     |  297 K   |  0.0041  pN.um
+     ~31 C     |  303 K   |  0.0042  pN.um
+     ~39 C     |  312 K   |  0.0043  pN.um
+
+     <em>default value = 0.0042</em>
+     */
+    real      kT;
+    
+    
+    /// 32-bits seed for random number generator
+    /**
+     The simulation uses SFMT, a fast Mersenne Twister to generate pseudo-random numbers
+     http://en.wikipedia.org/wiki/Mersenne_twister
+     
+     The generator is initialized from `random_seed` specified in the config file,
+     but if `random_seed == 0`, it is set automatically during initialization.
+    
+     <em>default value = 0</em>
+     */
+    unsigned int random_seed;
+    
+    
+    /// Desired precision in the motion of the objects
+    /**
+     The motion of the objects is solved with a residual error that is lower than `tolerance * B`, 
+     where `B` is the typical Brownian displacement of the objects in one time step.\n
+     <em>Thus one should set 0 < tolerance < 0.1</em>\n
+     Lowering tolerance increases precision at the expense of CPU time.
+     In the special case where 'kT==0', the maximum residual is simply `tolerance`.
+     
+     <em>default value = 0.05</em>
+    */
+    real      tolerance;
+    
+    
+    /// Precision threshold for stochastic events
+    /** 
+     A warning message is issued for a rate K if:
+     
+         K * time_step > acceptable_prob
+     
+     In most implementations, a stochastic event (binding/unbinding) may only occur once
+     during a time_step, and this becomes inaccurate if ( K * time_step is not small compared to 1 ).
+     
+     A user may control the `rate overflow' by adjusting `acceptable_prob` and monitoring the
+     warning messages.
+     
+     <em>default value = 0.5</em>
+     */
+    real      acceptable_prob;
+    
+    
+    /// A flag to enable preconditionning when solving the system of equations
+    /**
+     This parameter can affect the performance greatly, and it is always a good idea
+     to try the different accepted values of `precondition`:
+     - 0 : do not use preconditionning
+     - 1 : use a block preconditionner
+     .
+     
+     With `precondition = 1`, Cytosim calculates a matrix (the preconditionner)
+     that is approximately equal to the inverse of the matrix that characterize the
+     dynamical system. Using this preconditionner can reduce the number of iterations
+     needed to converge to a solution, resulting in a potential overall speedup.
+     However, calculating the preconditionner itself is costly, and performing an
+     iteration with preconditionning is also more expensive than without.
+     Hence there is a complex tradeoff, and the performance will vary.
+     In some cases, using `precondition=1` can degrade preformance, 
+     in particular if some objects have many vertices.
+     
+     If there is only one filament in the system, `precondition=0` should perform best.
+     With many filaments, trying `precondition = [0, 1]' is the recommended strategy.
+     <em>default value = 0</em>
+     */
+    int       precondition;
+
+    
+    /// A flag to control the engine that implement steric interactions between objects
+    int       steric;
+    
+    /// Stiffness for repulsive steric interaction
+    real      steric_stiffness_push[2];
+    
+    /// Stiffness for attractive steric interaction
+    real      steric_stiffness_pull[2];
+    
+    /// Lattice size used to determine steric interactions
+    /**
+     Cytosim uses a divide-and-conquer approach to find pairs of objects that are 
+     close enough to interact, based on a dividing the Space with a rectangular grid (see PointGrid).
+     
+     `steric_max_range` defines the minimum size of the cells in the grid.
+     A finer grid reduces false positives, but increases the amount of memory occupied by the grid,
+     and the number calculations that are necessary to maintain and clear the grid.
+     
+     Thus optimal performance is usually obtained for an intermediate value of `steric_max_range`.
+     However `steric_max_range` must remain greater than the maximum interaction distance,
+     otherwise some interacting pairs will be missed. 
+     Experimentation is usually necessary to find the best value.
+     
+     The maximum distance at which an object may interact with a sibling is its diameter.
+     Generally, `steric_max_range` should be greater or equal to the sum of the radiuses,
+     of any two object that may interact.
+     In the case of fiber, the `interaction-radius` is a combination of the segmentation,
+     and the radius: sqrt( (4/3*segmentation)^2 + 4*radius^2 )
+
+     If the parameter is not set, cytosim attempts to calculate `steric_max_range` automatically.
+     */
+    real      steric_max_range;
+    
+    
+    /// Lattice size used to determine the attachment of Hand to Fiber
+    /**
+     Cytosim uses a divide-and-conquer approach to detect which Fibers are near a given point,
+     witout testing every Fiber. This is necessary to determine onto which Fiber a Hand may bind.
+     The algorithm is based on partitionning Space with a rectangular grid
+     with cells of size `binding_grid_step` (see FiberGrid).
+
+     `binding_grid_step` affects the execution speed of the algorithm, but not its result.
+     Smaller values of binding_grid_step reduce the number of false positives, 
+     but requires more memory and housekeeping calculations. 
+     Memory requirements also increase with the physical dimensions of the system, 
+     to the power DIM (the dimensionality, set at compilation time).
+     */
+    real      binding_grid_step;
+    
+    /// level of verbosity
+    int           verbose;
+
+    /// Name of configuration file (<em>default = config.cym</em>)
+    std::string   config_file;
+    
+    /// Name of output property file (<em>default = properties.cmo</em>)
+    std::string   property_file;
+    
+    /// Name of output trajectory file (also known as `trajectory`, <em>default = objects.cmo</em>)
+    std::string   trajectory_file;
+    
+    /// If `true`, any pre-existing trajectory_file will be erased (<em>default = true</em>)
+    bool          clear_trajectory;
+    
+    /// If `true` free couples are not saved/read to/from file (<em>default = false</em>)
+    bool          skip_free_couple;
+    
+    /// Display parameters (see @ref DisplayPar)
+    std::string   display;
+
+    /// @}
+
+    /// this is set to true when 'display' is modified, and to 'false' when it is read
+    bool          display_fresh;
+
+public:
+    
+    /// constructor
+    SimulProp(const std::string& n) : Property(n) { clear(); }
+    
+    /// destructor
+    ~SimulProp()  { }
+    
+    /// identifies the property
+    std::string category() const { return "simul"; }
+    
+    /// set default values
+    void clear();
+    
+    /// set from a Glossary
+    void read(Glossary&);
+    
+    /// check and derive parameters
+    void complete(Simul const&);
+
+    /// return a carbon copy of object
+    Property* clone() const { return new SimulProp(*this); }
 
-Authors: Alessandro De Simone and Pierre Gonczy (2015) and Francois Nedelec (15.09.2017)
+    /// write all values
+    void write_values(std::ostream&) const;
 
-### Objective
+};
 
-This tutorial is inspired by the problem of centering: how can the cell define its center?
-It considers a radial array of microtubules (an [aster](http://en.wikipedia.org/wiki/Aster_%28cell_biology%29)) confined within fixed boundaries, and examine the role of some of the important parameters of this system.
-
-This tutorial can be performed with 2D or 3D simulations, equally.
-Note that 2D simulations tend to be easier to visualize, but 3D simulations are more realistic.
-To select 2D or 3D, you need to get the corresponding executables (sim and play) which are specifically made for one dimensionality.
-
-This is the basis of [this article](http://dx.doi.org/10.1016/j.celrep.2016.01.077):
-
->**Dynein transmits polarized actomyosin cortical flows to promote centrosome separation.**  
->De Simone A, Nedelec F and Gönczy P  
->Cell Reports Vol 14 (9) 2016
-
-
-### Preamble
-
-We assume here that you have already followed [Tutorial 1](tuto_introduction.md), and that you are now familiar with the general syntax of Cytosim's configuration files, and you can run a live simulation from the command-line.
-
-# Step 1 - Microtubules
-
-You should first set a basic configuration file, defining a `fiber` class called `microtubule`.
-Start with a fresh empty directory and a new configuration file:
-
-    set simul system
-    {
-        time_step = 0.001
-        viscosity = 0.01
-        display = ( style=2; point_size=7 )
-    }
-    
-    set space cell
-    {
-        shape = sphere
-    }
-    
-    new cell
-    {
-        radius = 5
-    }
-
-    set fiber microtubule
-    {
-        rigidity = 20
-        segmentation = 0.5
-        confine = inside, 100
-    
-        display = ( line_width = 2 )
-    }
-    
-    new microtubule
-    {
-        length = 1
-    }
-    
-    run 100000 system
-    {
-        nb_frames = 100
-    }
-
-Check that this works as expected, and verify that the values of the parameters are reasonable.
-
-### Use growing microtubules
-
-Set the `activity` of the microtubule to make it grow smoothly, up to a maximum length of 10.
-For this, add 4 lines to the paragraph that defines the fiber class:
-
-    set fiber microtubule
-    {
-        ...
-        activity = classic
-        growing_speed = 1
-        growing_force = 1.67
-        total_polymer = 10
-        ...
-    }
-
-In addition, one needs to specify the initial state of the microtubule, by adding one line in the 'new' command where they are created:
-
-    new microtubule
-    {
-        length = 1
-        end_state = grow
-    }
-
-
-The growing_speed is specified here in um/s. Since the amount of polymer is limited, the assembly rate will decrease as the filament gets longer. Specifically, growth rate will be linearly dependent on the availability of polymer:
-
-    speed = growing_speed * free_polymer
-
-Where `free_polymer` is a number in [0,1], representing the fraction of free monomers:
-
-    free_polymer = 1.0 - sum(all_fiber_length) / total_polymer
-
-You can press `r` in the live simulation to display detailed information about the length of the filaments.
-You will notice that the growth slows down as the length approaches the 'total_polymer' value of 10um.
-
-### Frictionless boundaries
-
-Cytosim's boundaries are without friction. This means that the force exerted by the boundary on a filament is always exactly orthogonal to the boundary at the point of contact. This is thought to be appropriate to represent the plasma membrane, which is a fluid bilayer.
-Note however that many cells have a cortex, which is a mesh of actin filaments anchored to the membrane. If the microtubule tip get entangled within the cortex, one could expect some effective friction.
-
-What happens when the microtubule becomes as long as the box diameter?
-
-What happens when it is longer?
-
-### Stalled growth
-
-The growth of a microtubule can stop because monomers are exhausted, or because force prevents elongation. The later case may happen in particular when the ends are pushing against the boundary.
-
-The parameter `growing_force` defines the amount of force that polymerization can sustain. 
-This is the level of force at which the microtubule will exhibit significantly slower growth.
-Hence the microtubule will stall due to force when both ends touch the box, if the buckling force is higher than thand `growing_force`.
-
-What is the buckling force of a microtubule of length L? What is the value for L = 10?
-
-Can you adjust the parameters of the simulation such as to stall microtubule growth?
-
-
-# Step 2 - Aster of microtubules
-
-An aster is a composite objects, in which microtubules are anchored at their minus-end onto a object called a `solid`. The `solid` is an object that behaves like a rigid body: it can move by translation and rotation, but it will not deform. By anchoring the microtubules to a solid, we can establish a radial array that resembles a real aster. The structure of the aster is however imposed by the simulation, i.e. its structural integrity is completely independent from the action of motor complexes, which are absent here.
-
-Remove the free microtubule:
-
-    new 0 microtubule
-
-and define a solid called `core` and the aster, by adding these paragraphs:
-
-    set solid core
-    {
-        display = ( style = 3; )
-    }
-    
-    set aster star
-    {
-        stiffness = 1000, 500
-    }
-    
-    new star
-    {
-        solid = core
-        radius = 0.5
-        fibers = 25, microtubule, ( plus_end=grow; length = 0.1; )
-    }
-
-The solid named `core` is used for the construction of the aster, but only graphical properties are defined. For the `aster` object, we defined:
-
-* `solid = core` specifies the attachment `solid` for the fibers,
-* `fibers = 25, microtubule` defines the number and the class of fibers used to compose the aster,
-* `radius` set the radius of the aster solid (here called `core`) which is at its center.
-
-The aster has 25 microtubules, and they are all initially 0.1 micro-meter long. Their minus-ends are anchored onto the solid with links of stiffness `1000` and `500` (which will be explained shortly), while their plus end pointing out. 
-
-The complete configuration file is here: [aster.cym](data/aster.cym).
-
-### Microtubule length
-
-Parameter `fiber_length` within the `new aster` block defines the initial length of the microtubules. The fiber will grow, but the sum of their lengths cannot exceed `total_polymer=10`, and thus they will not be able to extend longer than `~10/25 um`. You need to increase `total_polymer` to allow them to grow longer.
-
-What happens when microtubules are able to grow up to about the radius of the box?
-
-What happens when microtubules are able to grow longer than this?
-
-### Links and stiffnesses
-
-To physically connect Fibers and Solid, constraining both position and direction, each Fiber is attached to the Solid in two points:
-
-* at the end of the Fiber (the minus-end)
-* at an intermediate point of the Fiber at some distance from this end.
-
-These different links can have different stiffnesses:
-
-* stiffness[0] for the link 1 at the end of the Fiber
-* stiffness[1] for the link 2 at the intermediate point of the Fiber. 
-
-Set one of the stiffness value to zero, and observe the effect on the aster.
-
-Can you observe centering? Is it stable?
-
-### Hollow core
-
-You can specify two values for `radius` to place the microtubules minus-end a little away from the center.
-This can be useful to avoid the very high density of filaments in the center, which is not realistic.
-
-    new star
-    {
-        radius = 0.5, 0.5
-        ...
-    }
-
-Check the difference visually.
-
-### Initial position
-
-You can specify the initial position within he `new` command, in the same way as most objects:
-
-    new star
-    {
-        ...
-        position = center
-    }
-
-or to place it near the edge: 
-
-    new star
-    {
-        ...
-        position = 4 0 0
-    }
-
-### Drag coefficient
-
-In the model, the drag of an aster is the sum of all the drag of the solid and microtubules attached to it. The drag is thus approximatly proportional to the total amount of microtubules-length. Asters with more microtubules, or with longer ones are more difficult to move than asters with less microtubules or shorter ones. This is a simplifying approximation which ignores hydrodynamic interactions.
-
-The drag coefficient affect the speed at which an aster will move under some force, but this should not have much effect on the equilibrium position that will eventually be reached, if one waits long enough.
-
-# Step 3 - Centering by Pushing
-
-## Small cell
-
-Microtubules growing from a centrosome will exert pushing forces against the cell edge; note that the compressive force that a microtubule can sustain before buckling decreases with its length squared:
-
-    F = 2 * rigidity / length^2 
-
-Position the aster 1 um away from the cell edge to start with, in a cell with a radius of 5 um and a total amount of polymer such that the microtubule lengths are equal to the cell radius . Does the aster center itself? How stable is the final position? 
-
-## Large cell
-
-Is the pushing mechanism efficient in a larger cell, say with a radius of 15 um? 
-Change cell size by modifying the geometry line:
-
-    new cell
-    {
-        radius = 15
-    }
-
-Place the aster 1 um away from the cell membrane by modifying the position line:
-    
-    new star
-    {
-        position = 14 0 0
-    }
-
-What happens? Adjust the total amount of polymer so that all fibers can growth up to a length equal to the radius of the cell
-
-## Cell shape
-
-Try different shapes, while keeping the size similar:
-
-    set space cell
-    {
-        shape = capsule
-    }
-    new cell
-    {
-        length = 8, 2
-    }
-
-and:
-    
-    set space cell
-    {
-        shape = dice
-    }
-    new cell
-    {
-        length = 8, 8;
-        radius = 2;
-    }
-
-Do you find that centration is different when the cells has 'corners'?
-
-
-# Step 4 - Microtubule Dynamicity
-
-Set the cell radius back to 5 um and the position to “4 0”. Now you will explore the importance of microtubule dynamics. Enable the standard two-state model of dynamic instability as follows:
-
-    set fiber microtubule
-    {
-        ...
-        activity         = classic
-        growing_speed    = 0.5
-        shrinking_speed  = -0.85
-        catastrophe_rate = 0.05,  0.5
-        rescue_rate      = 0
-        growing_force    = 1.67
-        min_length       = 0.5
-        ...
-    }
-
-You can start with the complete configuration file [aster_dynamic.cym](data/aster_dynamic.cym).
-
-Make sure that the fibers start with a length larger than `min_length`. 
-
-## Nucleation
-
-If the fiber class from which the aster is constructed is dynamic, you can specify a nucleation rate:
-    
-    set aster star
-    {
-        ...
-        nucleate = 1, microtubule, ( length = 1 )
-    }
-
-This will be the rate a which an empty site will be re-populated, leading to a steady-state in which the number of microtubules may vary.
-    
-The mean length of the microtubules is then equal to `growing_speed/catastrophe_rate` at equilibrium.
-Increase (and then decrease) microtubule catastrophe rate, and run the two simulations in turn. Describe the events.
-
-# Step 5 - Cytoplasmic Motors
-
-Reset `catastrophe_rate` to 0.1 and add 2000 motors distributed at fixed points throughout the cytoplasm:
-
-    set hand dynein
-    {
-        binding_rate = 5
-        binding_range = 0.02
-        unbinding_rate = 1
-        unbinding_force = 2
-        
-        activity = move
-        unloaded_speed = -1
-        stall_force = 5
-        display = ( color = green, dark_gray )
-    }
-    
-    set single grafted
-    {
-        hand = dynein
-        stiffness = 100
-        activity = fixed
-    }
-    
-    new 2000 grafted
-
-Do cytoplasmic motors help centration? Is the final position more stable? 
-Can you imagine why? 
-
-Is the result very different if these motors are minus-end directed or plus-end directed? 
-
-Next, repeat this in the large cell. Compare the result with the situation without such motors.
-
-### Placement of motors
-
-Place the motors at a maximum distance of 0.1 from the edge of the cell:
-
-    new 2000 grafted
-    {
-        position = edge 0.1
-    }
-
-Take a few minutes to guess what will happen with plus-end and with minus-end directed motors... write your predictions on paper and only then, run the corresponding simulations.
-Check the outcome and verify your prediction.
-
-
-## The end
-
-Congratulation, you have completed the tutorial.
-Please help us to improve this material by sending us your feedback.
+#endif
```

### Comparing `cytosim-0.0.3/doc/tutorials/tuto_contract2.md` & `cytosim-0.0.4/src/sim/couple_prop.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,207 @@
-# Tutorial: Comparison of Contractile Mechanisms
+// Cytosim was created by Francois Nedelec. Copyright 2007-2017 EMBL.
+#ifndef COUPLE_PROP_H
+#define COUPLE_PROP_H
+
+#include "real.h"
+#include "property.h"
+#include "hand_prop.h"
+#include "common.h"
+
+class Couple;
+class Space;
+
+/// Property for Couple
+/**
+ @ingroup Properties
+*/
+class CoupleProp : public Property
+{
+    friend class Couple;
+    
+public:
+    
+    /// indicates a specificity for crosslinking two fibers
+    /** 
+     The criteria is based on the angle defined by the two fibers.
+     Since fibers are oriented, the angle in Radian is well defined between -PI and +PI:
+     - 0 corresponds to parallel fibers having the same orientation,
+     - PI/2 correspond to orthogonal fibers,
+     - -PI corresponds to parallel fibers having opposite orientation (antiparallel)
+     .
+     The allowed angle correspond to +/- 60 degree, which is rather arbitrary.
+     */
+    enum Specificity 
+    {
+        BIND_ALWAYS,           ///< can bind in any configuration
+        BIND_PARALLEL,         ///< can link two fibers only if `cosine(angle) > 0.5`
+        BIND_NOT_PARALLEL,     ///< can link two fibers only if `cosine(angle) < 0.5`
+        BIND_ANTIPARALLEL,     ///< can link two fibers only if `cosine(angle) < -0.5`
+        BIND_NOT_ANTIPARALLEL, ///< can link two fibers only if `cosine(angle) > -0.5`
+        BIND_ORTHOGONAL        ///< can link two fibers only if `-sqrt(3)/2 < cosine(angle) < sqrt(3)/2`
+    };
+    
+    /**
+     @defgroup CouplePar Parameters of Couple
+     @ingroup Parameters
+     @{
+     */
+    
+    
+    /// name of first Hand in Couple
+    std::string  hand1;
+    
+    /// name of second Hand in Couple
+    std::string  hand2;
+    
+    /// stiffness of link between the two Hands while linking (pN/um)
+    real         stiffness;
+    
+    /// resting length of the link (um)
+    real         length;
+    
+    /// diffusion coefficient while unattached (um^2/s)
+    real         diffusion;
+    
+    /// if set > 0, assumes uniform concentration of diffusing Couple
+    /**
+     The possible values for `fast_diffusion` are:
+     
+     - 0: disabled.
+       Every Couple is explicitly represented by a diffusing point. The
+       unattached Couple move randomly, with the specified diffusion constant,
+       and they may accumulate at certain regions of the simulation space. That
+       happens in particular with asters when the motors move inward. In fact,
+       the aster can act like a black hole for the motors, in certain conditions.
+
+     - 1: attach Couple along the length of filaments
+       It is assumed that free Couples are uniformly distributed, and they are 
+       thus not explicitly represented. In this mode, Cytosim will only keep a 
+       count of the number of free Couples, and directly attach these Couples by
+       one of their Hand, at positions of the fibers selected randomly, irrespective
+       of the manner in which the filaments are distributed spatially.
+       In this mode, the Couple diffusion constant is not relevant.
+
+     - 2: attach Couple only at growing PLUS_ENDS
+       Similar to mode 1, but Hand1 of Couple is directly attached to the plus tips
+       of growing fibers. The number of attachments is proportional to the new
+       polymer mass, which is `time_step * growing_speed`, but occurs otherwise
+       equally to every filaments.
+     .
+     
+     Enabling `fast_diffusion` can make the simulation a bit faster when there
+     are a lot of Couples, but another reason to use this mode is that it makes
+     the model simpler, since the fraction of bound/free Couples can then be calculated
+     analytically. This also avoid the accumulation of motors in aster and other
+     organized structures, which are stronger in a 2D geometry, compared to 3D. 
+     Thus one may wish to enable `fast_diffusion` in a 2D simulation to better
+     represent a 3D system.
+     
+     `fast_diffusion` does not affect Couples in the attached state.
+     */
+    int          fast_diffusion;
+    
+    /// if ( trans_activated == 1 ), Hand2 is active only if Hand1 is bound
+    /**
+     Both Hands of a Couple are normally equally active. With this feature,
+     the activity of Hand2 is conditioned on Hand1 being attached.
+     In other words, Hand2 remains inactive if Hand1 is not attached.
+     This is very useful for example to make a nucleator that nucleates only after
+     it has docked on an existing filament.
+     */
+    bool         trans_activated;
+
+    /// prevents both Hands from binding at the same position on a Fiber (default=true)
+    /**
+     By default, the two Hands of a Couple may not bind at the same position on 
+     the same Fiber. Such a degenerate binding may be impossible due to the molecular 
+     configuration of the complex. Note that no restriction is imposed if the Hands
+     attempt to bind to different fibers, or to the same fiber at distant positions. 
+     The exact criteria is that the Hands cannot bind onto the same segment, or 
+     to segments that have a point in common.
+     
+     Setting `stiff==false`, however, allows the two hands from the Couple to bind 
+     nearby positions on the same fiber. In such a degenerate configuration, the 
+     link is unproductive as it cannot produce force, but the feature may be useful 
+     to combine activities such as cutting and motors.
+     */
+    bool         stiff;
+    
+    /// Specificity of binding to a pair a Fiber
+    /**
+     Set to limit the binding to only certain configurations:
+     - `off`             : no restriction (default)
+     - `parallel`        : parallel filaments with an angle below 60 degrees
+     - `antiparallel`    : anti-parallel filaments with an angle below 60 degrees
+     - `not_parallel`    : anti-parallel filaments with an angle below 120 degrees
+     - `not_antiparallel`: parallel filaments with an angle below 120 degrees
+     - `orthogonal`      : filaments with an angle between 60 and 120 degrees
+     .
+     This limit the attachment of a Hand when the other Hand is already attached,
+     as a function of the angle that is defined by the already bound filament,
+     and the potential new one. The first attachment of any Hand is unrestricted.
+     */
+    Specificity  specificity;
+
+    /// Confinement can be `off`, `inside` (default) or `surface`
+    Confinement  confine;
+    
+    /// Unused Parameter: confinement stiffness (also known as `confine[1]`)
+    //real         confine_stiffness;
+    
+    /// name of space used for confinement (also known as `confine[2]`)
+    std::string  confine_space;
+    
+    /// specialization
+    /**
+     @copydetails CoupleGroup
+     */
+    std::string  activity;
+    
+    /// @}
+    
+    /// pointer to Property of Hand 1
+    HandProp *    hand1_prop;
+    /// pointer to Property of Hand 2
+    HandProp *    hand2_prop;
+
+protected:
+    
+    real          diffusion_dt;
+    /// pointer to actual confinement Space, derived from `confine_space`
+    Space const*  confine_space_ptr;
+
+public:
+    
+    /// constructor
+    CoupleProp(const std::string& n) : Property(n)  { clear(); }
+    
+    /// destructor
+    ~CoupleProp() { }
+    
+    /// create a Couple having this property
+    virtual Couple * newCouple(Glossary * = nullptr) const;
+    
+    /// identifies the property
+    std::string category() const { return "couple"; }
+    
+    /// set default values
+    void clear();
+    
+    /// set from a Glossary
+    void read(Glossary&);
+    
+    /// compute derived parameter values
+    void complete(Simul const&);
+    
+    /// return a carbon copy of object
+    Property* clone() const { return new CoupleProp(*this); }
+
+    /// write all values
+    void write_values(std::ostream&) const;
+  
+    /// return volume of confine_space
+    real spaceVolume() const;
+};
 
-Authors: Julio Belmonte (20.12.2018)
+#endif
 
-# Objective
-
-Learn how to set up a simple simulation of a contractile actomyosin network due to the end-dwelling property of motors and compare it with the standard buckling-mediated contraction.
-
-This tutorial is based on the following paper:
-
-[Polarity sorting drives remodeling of actin-myosin networks](http://jcs.biologists.org/content/132/4/jcs219717)
-V Wollrab, JM Belmonte, L Baldauf, M Leptin, F Nedelec, GH Koenderink
-Journal of Cell Science, 132, 219717 (2019)
-
-
-### Preamble
-
-This tutorial should be done in 2D using `play`, by manually editing the configuration file. You can copy-paste the commands directly from this file into `config.cym` in your text editor.
-
-This tutorial assumes that you have already completed the first tutorial on contractile systems [Network contraction driven by motors](tuto_contract1.md).
-
-
-# Introduction
-
-In this tutorial we will focus on a different contraction mechanism: polarity sorting. Here contraction relies on the presence of molecular motors that dwells at the end of the filament instead of automatically detaching. Because of this property, end-dwelling motors end up bring the same end of filaments together, thus contracting cytoskeletal networks into asters
-
-![polarity_sorting](data/polarity_sorting.png)
-
-
-# Minimal model
-
-The first step in this tutorial is to set up a simple systems with a single filament and a few motors and test the end dwelling property of the motor. 
-
-Lets create a small simulation space with radius 2 um and add single actin filament of length 3 um at the center:
-
-    set simul tutorial
-    {
-        time_step = 0.01
-    }
-    
-    set space cell 
-    {
-        shape = circle
-    }
-    
-    new cell
-    {
-        radius = 2
-    }
-
-    set fiber actin
-    {
-        rigidity = 0.075
-        segmentation = 0.15
-    }
-    
-    new 1 fiber actin
-    {
-        length = 4
-        position = 0,0
-    }
-    
-    run 5000 simul *
-    {
-        nb_frames = 50
-    }
-
-
-When we add an object with the command `new` we also have the option of specifing its position with the option `position`. Here we used the coordinates 0,0 to indicate the center of the space. You can modify these coordinated to place the filament anywhere inside (or outside) the circular space. Note that side the `orientation` option was not used, every time the simulation is called the filament is placed at a random orientation.
-
-
-Now let's define and add 10 myosin motors to the simulation:
-
-    set hand motor
-    {
-        binding_rate = 10
-        binding_range = 0.1
-        unbinding_rate = 0.1
-        unbinding_force = 6
-
-        display = ( color=green; size=4; )
-        
-        activity = move
-        unloaded_speed = 2
-        stall_force = 4
-    }
-    
-    set couple myosin
-    {
-        hand1 = motor
-        hand2 = motor
-        diffusion = 1
-        length = 0.1
-        stiffness = 100
-    }
-
-    new 10 couple myosin
-
-
-Run the simulation and note what happens to the motor when it reaches the end of the filament. Does it stays there for a while or does it detach automatically?
-
-
-Now let's change the behavior of the motors in such a way that they will now dwell at the end of the filaments instead of detaching instantaneously after reaching the end. To do that we add the property `hold_growing_end` to the hand properties:
-
-    set hand motor
-    {
-     ...
-     hold_growing_end = 1
-     ...
-    }
-
-With this property turned on the myosin now stay and accumulate at the plus end of the filament. Note that they eventually detach due to their inherent unbinding rate.
-
- 
-# Polarity-Sorting Contraction
-
-Now let's see how this mechanism can lead to network contraction. First let's explore ta simpler case with 2 filaments. Run it a few times and not the final state of the simulation. Next repeat the simulations again with `hold_growing_end = 0` to check what happens.
-
-This simple case illustrates the key-feature of the end-dwelling motors, which is their ability to have one hand dwelling at the end of a filament while the other hand keeps walking along the second filament. This has the effect of bringing the two ends of the filament together. To see this feature better add the following display option to visualize the ends of the filaments:
-
-    set fiber actin
-    {
-     ...
-     display = ( end_style=2,4; )
-     ...
-    }
-
-To better appreciate how the end-dwelling property of the motor leads to the polarity sorting of networks let's make a bigger simulations with multiple filaments. Create a simulation with radius 4 um, 100 filaments randomly distributed inside the space and 300 motors. 
-
-Note how the final patter of this simulations resembles an aster, in contrast to the knot-like shape obtained with the filament buckling mechanism from the previous tutorial [Network contraction driven by motors](tuto_contract1.md). Because in this final shape all the minus-ends face the external of the aster and the plus-ends face the center of the aster this contraction mechanism is knowns as the Polarity-Sorting mechanism.
-
-
-Now turn the end-dwelling property of the motors off and check how the network behaves. Do you still get a polarity-sorted aster? Is the network still contractile?
-
-Make a bigger simulation in a larger space and with more filaments, but keep the number of  motors unchanged. Do you still get a single aster? Vary the number of motors and filaments and check when you get multiple asters, when you get a single one, and when you get none.
-
-
-# Filament-Buckling vs. Polarity-Sorting Mechanisms
-
-Let's compare both mechanism of network contraction.
-
-Set the size of the simulation to be a radius of size 5 um, with 250 actin filaments of length 3 um, and 600 myosin. This setting should be sufficient to drive contraction of the whole networks into a single aster via the polarity sorted mechanism.
-
-Now lets turn this simulation into a an example of a contractile network via the filament buckling mechanism. To do so the first thing we need to do is to turn off the end-dwelling property of the motor (`hold_growing_end = 0`) and confirm again that the network ceases do contract. Then, lets add crosslinkers back to the mix:
-
-    set hand binder
-    {
-        binding_rate = 10
-        binding_range = 0.1
-        unbinding_rate = 0.1
-        unbinding_force = 6
-    
-        display = ( color=blue; size=4; )
-    }
-    
-    set couple crosslinker
-    {
-        hand1 = binder
-        hand2 = binder
-        diffusion = 1
-        length = 0.1
-        stiffness = 100
-    } 
-
-To keep the connectivity the same as before, lets reduce the number of myosin to 200 and add 400 crosslinkers. Does the network still contract? How does the final shape of the network compare with the Polarity-Sorting mechanism? Would you say it contracts more or less than before? Faster or slower?
-
-
-Now let's check how each mechanism perform under different filament stiffness. Change the rigidity of the filaments from actin values (`0.075`) to microtubule values (`22`). Does the Filament-Buckling mechanism still works? What about the Polarity-Sorting?
-
-
-While the two mechanism are conceptually very distinct, there is no reason why both of them could not be actin simultaneously to drive network contraction. Repeat the simulations again for actin-like rigidity (`rigidity = 0.075`) and add 300 units of crosslinkers and end-dwelling myosins. Does the network still contract?
-
-Try varying the ratio of crosslinkers to end-dwelling myosin. Do you not any difference in network contraction? Can you tell when each of the mechanisms is dominant? Is that what you would expect given the requirements of each mechanism?
-
-
-# The end!
-
-Congratulations, you have completed the tutorial. If you have suggestions on this material, please email us at *feedback AT cytosim.org*
```

### Comparing `cytosim-0.0.3/makefile` & `cytosim-0.0.4/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/makefile.inc` & `cytosim-0.0.4/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/index.md` & `cytosim-0.0.4/python/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/compare_config.py` & `cytosim-0.0.4/python/look/compare_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/get_data.py` & `cytosim-0.0.4/python/look/get_data.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/make_image.py` & `cytosim-0.0.4/python/look/make_image.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/make_movie.py` & `cytosim-0.0.4/python/look/make_movie.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/make_page.py` & `cytosim-0.0.4/python/look/make_page.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/make_plots.py` & `cytosim-0.0.4/python/look/make_plots.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/read_config.py` & `cytosim-0.0.4/python/look/read_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/look/tell.py` & `cytosim-0.0.4/python/look/tell.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/misc/battery_test.py` & `cytosim-0.0.4/python/misc/battery_test.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/misc/cleanup.py` & `cytosim-0.0.4/python/misc/cleanup.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/misc/compare.py` & `cytosim-0.0.4/python/misc/compare.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/misc/plot.py` & `cytosim-0.0.4/python/misc/plot.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/misc/pyned.py` & `cytosim-0.0.4/python/misc/pyned.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/misc/reduce.py` & `cytosim-0.0.4/python/misc/reduce.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/run/go_sim.py` & `cytosim-0.0.4/python/run/go_sim.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/run/go_sim_lib.py` & `cytosim-0.0.4/python/run/go_sim_lib.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/run/preconfig.py` & `cytosim-0.0.4/python/run/preconfig.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/run/submit_one.py` & `cytosim-0.0.4/python/run/submit_one.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/python/run/submit_slurm.py` & `cytosim-0.0.4/python/run/submit_slurm.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/CMakeLists.txt` & `cytosim-0.0.4/src/base/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/array.h` & `cytosim-0.0.4/src/base/array.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/assert_macro.h` & `cytosim-0.0.4/src/base/assert_macro.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/backtrace.cc` & `cytosim-0.0.4/src/base/backtrace.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/backtrace.h` & `cytosim-0.0.4/src/base/backtrace.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/buddy.h` & `cytosim-0.0.4/src/base/buddy.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/exceptions.h` & `cytosim-0.0.4/src/base/exceptions.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/filepath.cc` & `cytosim-0.0.4/src/base/filepath.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/filepath.h` & `cytosim-0.0.4/src/base/filepath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/filewrapper.cc` & `cytosim-0.0.4/src/base/filewrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/filewrapper.h` & `cytosim-0.0.4/src/base/filewrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/glossary.cc` & `cytosim-0.0.4/src/base/glossary.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/glossary.h` & `cytosim-0.0.4/src/base/glossary.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/inventoried.h` & `cytosim-0.0.4/src/base/inventoried.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/inventory.cc` & `cytosim-0.0.4/src/base/inventory.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/inventory.h` & `cytosim-0.0.4/src/base/inventory.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/iowrapper.cc` & `cytosim-0.0.4/src/base/iowrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/iowrapper.h` & `cytosim-0.0.4/src/base/iowrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/makefile.inc` & `cytosim-0.0.4/src/base/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/messages.cc` & `cytosim-0.0.4/src/base/messages.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/messages.h` & `cytosim-0.0.4/src/base/messages.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/node_list.cc` & `cytosim-0.0.4/src/base/node_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/node_list.h` & `cytosim-0.0.4/src/base/node_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/noder.h` & `cytosim-0.0.4/src/base/noder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/operator_new.cc` & `cytosim-0.0.4/src/base/operator_new.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/print_color.cc` & `cytosim-0.0.4/src/base/print_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/print_color.h` & `cytosim-0.0.4/src/base/print_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/property.cc` & `cytosim-0.0.4/src/base/property.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/property.h` & `cytosim-0.0.4/src/base/property.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/property_list.cc` & `cytosim-0.0.4/src/base/property_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/property_list.h` & `cytosim-0.0.4/src/base/property_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/stream_func.cc` & `cytosim-0.0.4/src/base/stream_func.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/stream_func.h` & `cytosim-0.0.4/src/base/stream_func.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/tictoc.cc` & `cytosim-0.0.4/src/base/tictoc.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/tictoc.h` & `cytosim-0.0.4/src/base/tictoc.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/timer.h` & `cytosim-0.0.4/src/base/timer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/tokenizer.cc` & `cytosim-0.0.4/src/base/tokenizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/base/tokenizer.h` & `cytosim-0.0.4/src/base/tokenizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/couple_modules.h` & `cytosim-0.0.4/src/cpython/couple_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/fiber_modules.h` & `cytosim-0.0.4/src/cpython/fiber_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/glossary_modules.h` & `cytosim-0.0.4/src/cpython/glossary_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/hand_modules.h` & `cytosim-0.0.4/src/cpython/hand_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/interface_modules.h` & `cytosim-0.0.4/src/cpython/interface_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/meca_modules.h` & `cytosim-0.0.4/src/cpython/meca_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/object_modules.h` & `cytosim-0.0.4/src/cpython/object_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/organizer_modules.h` & `cytosim-0.0.4/src/cpython/organizer_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/point_modules.h` & `cytosim-0.0.4/src/cpython/point_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/python_frame.h` & `cytosim-0.0.4/src/cpython/python_frame.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/python_utilities.h` & `cytosim-0.0.4/src/cpython/python_utilities.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/simul_modules.h` & `cytosim-0.0.4/src/cpython/simul_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/single_modules.h` & `cytosim-0.0.4/src/cpython/single_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/solid_modules.h` & `cytosim-0.0.4/src/cpython/solid_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/space_modules.h` & `cytosim-0.0.4/src/cpython/space_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cpython/thread_modules.h` & `cytosim-0.0.4/src/cpython/thread_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/cytosim.egg-info/PKG-INFO` & `cytosim-0.0.4/cytosim.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 Metadata-Version: 2.1
 Name: cytosim
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cytosim: Langevin dynamics of active polymer networks
 Keywords: simulation actin microtubule polymer
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Cytosim
 
 Cytosim is a cytoskeleton simulation suite designed to handle large systems of flexible filaments with associated proteins such as molecular motors. It is a versatile base that has been used to study actin and microtubule systems in 1D, 2D and 3D. It is built around a cross-platform C++ core engine running on UNIX, Mac OSX, GNU/Linux and within Cygwin on Windows. The code is modular and extensible, making Cytosim a convenient base that can be customized to meet particular tasks. Some of the most common tasks encountered during a simulation project are implemented in Python.
```

### Comparing `cytosim-0.0.3/src/disp/CMakeLists.txt` & `cytosim-0.0.4/src/disp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display.cc` & `cytosim-0.0.4/src/disp/display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display.h` & `cytosim-0.0.4/src/disp/display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display1.cc` & `cytosim-0.0.4/src/disp/display1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display1.h` & `cytosim-0.0.4/src/disp/display1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display2.cc` & `cytosim-0.0.4/src/disp/display2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display2.h` & `cytosim-0.0.4/src/disp/display2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display3.cc` & `cytosim-0.0.4/src/disp/display3.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display3.h` & `cytosim-0.0.4/src/disp/display3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display_prop.cc` & `cytosim-0.0.4/src/disp/display_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/display_prop.h` & `cytosim-0.0.4/src/disp/display_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/fiber_disp.cc` & `cytosim-0.0.4/src/disp/fiber_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/fiber_disp.h` & `cytosim-0.0.4/src/disp/fiber_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/glapp.cc` & `cytosim-0.0.4/src/disp/glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/glapp.h` & `cytosim-0.0.4/src/disp/glapp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/gle.cc` & `cytosim-0.0.4/src/disp/gle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/gle.h` & `cytosim-0.0.4/src/disp/gle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/gle_color.cc` & `cytosim-0.0.4/src/disp/gle_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/gle_color.h` & `cytosim-0.0.4/src/disp/gle_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/gle_color_list.cc` & `cytosim-0.0.4/src/disp/gle_color_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/gle_color_list.h` & `cytosim-0.0.4/src/disp/gle_color_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/glu_unproject.cc` & `cytosim-0.0.4/src/disp/glu_unproject.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/grid_display.cc` & `cytosim-0.0.4/src/disp/grid_display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/grid_display.h` & `cytosim-0.0.4/src/disp/grid_display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/line_disp.h` & `cytosim-0.0.4/src/disp/line_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/makefile.inc` & `cytosim-0.0.4/src/disp/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/miniz.c` & `cytosim-0.0.4/src/disp/miniz.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/miniz.h` & `cytosim-0.0.4/src/disp/miniz.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/offscreen.cc` & `cytosim-0.0.4/src/disp/offscreen.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/offscreen.h` & `cytosim-0.0.4/src/disp/offscreen.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/offscreen_fbo.cc` & `cytosim-0.0.4/src/disp/offscreen_fbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/offscreen_glx.cc` & `cytosim-0.0.4/src/disp/offscreen_glx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/point_disp.cc` & `cytosim-0.0.4/src/disp/point_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/point_disp.h` & `cytosim-0.0.4/src/disp/point_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/save_image.cc` & `cytosim-0.0.4/src/disp/save_image.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/save_image.h` & `cytosim-0.0.4/src/disp/save_image.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/spng.c` & `cytosim-0.0.4/src/disp/spng.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/spng.h` & `cytosim-0.0.4/src/disp/spng.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/view.cc` & `cytosim-0.0.4/src/disp/view.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/view.h` & `cytosim-0.0.4/src/disp/view.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/view_prop.cc` & `cytosim-0.0.4/src/disp/view_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/disp/view_prop.h` & `cytosim-0.0.4/src/disp/view_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/index.md` & `cytosim-0.0.4/src/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/CMakeLists.txt` & `cytosim-0.0.4/src/math/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/SFMT-avx2.h` & `cytosim-0.0.4/src/math/SFMT-avx2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/SFMT-common.h` & `cytosim-0.0.4/src/math/SFMT-common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/SFMT-params.h` & `cytosim-0.0.4/src/math/SFMT-params.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/SFMT-params19937.h` & `cytosim-0.0.4/src/math/SFMT-params19937.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/SFMT-sse2.h` & `cytosim-0.0.4/src/math/SFMT-sse2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/SFMT.c` & `cytosim-0.0.4/src/math/SFMT.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/SFMT.h` & `cytosim-0.0.4/src/math/SFMT.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/accumulator.h` & `cytosim-0.0.4/src/math/accumulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/allocator.h` & `cytosim-0.0.4/src/math/allocator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/bicgstab.h` & `cytosim-0.0.4/src/math/bicgstab.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/cblas.h` & `cytosim-0.0.4/src/math/cblas.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/clapack.h` & `cytosim-0.0.4/src/math/clapack.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/dgtsv.c` & `cytosim-0.0.4/src/math/dgtsv.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/evaluator.h` & `cytosim-0.0.4/src/math/evaluator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/gmres.h` & `cytosim-0.0.4/src/math/gmres.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/grid.h` & `cytosim-0.0.4/src/math/grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/grid_base.h` & `cytosim-0.0.4/src/math/grid_base.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/isometry.h` & `cytosim-0.0.4/src/math/isometry.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/linear_operator.h` & `cytosim-0.0.4/src/math/linear_operator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/makefile.inc` & `cytosim-0.0.4/src/math/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix.cc` & `cytosim-0.0.4/src/math/matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix.h` & `cytosim-0.0.4/src/math/matrix.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix11.cc` & `cytosim-0.0.4/src/math/matrix11.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix11.h` & `cytosim-0.0.4/src/math/matrix11.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix22.cc` & `cytosim-0.0.4/src/math/matrix22.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix22.h` & `cytosim-0.0.4/src/math/matrix22.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix33.cc` & `cytosim-0.0.4/src/math/matrix33.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix33.h` & `cytosim-0.0.4/src/math/matrix33.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrix44.h` & `cytosim-0.0.4/src/math/matrix44.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matrixbase.h` & `cytosim-0.0.4/src/math/matrixbase.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparse.cc` & `cytosim-0.0.4/src/math/matsparse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparse.h` & `cytosim-0.0.4/src/math/matsparse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesym.cc` & `cytosim-0.0.4/src/math/matsparsesym.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesym.h` & `cytosim-0.0.4/src/math/matsparsesym.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesym1.cc` & `cytosim-0.0.4/src/math/matsparsesym1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesym1.h` & `cytosim-0.0.4/src/math/matsparsesym1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesym2.cc` & `cytosim-0.0.4/src/math/matsparsesym2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesym2.h` & `cytosim-0.0.4/src/math/matsparsesym2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesymblk.cc` & `cytosim-0.0.4/src/math/matsparsesymblk.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/matsparsesymblk.h` & `cytosim-0.0.4/src/math/matsparsesymblk.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/monitor.h` & `cytosim-0.0.4/src/math/monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/platonic.cc` & `cytosim-0.0.4/src/math/platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/platonic.h` & `cytosim-0.0.4/src/math/platonic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/pointsonsphere.cc` & `cytosim-0.0.4/src/math/pointsonsphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/pointsonsphere.h` & `cytosim-0.0.4/src/math/pointsonsphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/polygon.cc` & `cytosim-0.0.4/src/math/polygon.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/polygon.h` & `cytosim-0.0.4/src/math/polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/project_ellipse.cc` & `cytosim-0.0.4/src/math/project_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/project_ellipse.h` & `cytosim-0.0.4/src/math/project_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/quaternion.h` & `cytosim-0.0.4/src/math/quaternion.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/random.cc` & `cytosim-0.0.4/src/math/random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/random.h` & `cytosim-0.0.4/src/math/random.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/random_vector.cc` & `cytosim-0.0.4/src/math/random_vector.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/random_vector.h` & `cytosim-0.0.4/src/math/random_vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/rasterizer.cc` & `cytosim-0.0.4/src/math/rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/rasterizer.h` & `cytosim-0.0.4/src/math/rasterizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/real.h` & `cytosim-0.0.4/src/math/real.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/simd.h` & `cytosim-0.0.4/src/math/simd.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/simd_print.h` & `cytosim-0.0.4/src/math/simd_print.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/smath.h` & `cytosim-0.0.4/src/math/smath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vecprint.h` & `cytosim-0.0.4/src/math/vecprint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector.h` & `cytosim-0.0.4/src/math/vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector1.cc` & `cytosim-0.0.4/src/math/vector1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector1.h` & `cytosim-0.0.4/src/math/vector1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector2.cc` & `cytosim-0.0.4/src/math/vector2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector2.h` & `cytosim-0.0.4/src/math/vector2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector3.cc` & `cytosim-0.0.4/src/math/vector3.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector3.h` & `cytosim-0.0.4/src/math/vector3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector4.cc` & `cytosim-0.0.4/src/math/vector4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/math/vector4.h` & `cytosim-0.0.4/src/math/vector4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/check_dump.m` & `cytosim-0.0.4/src/misc/check_dump.m`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/RtMidi.cpp` & `cytosim-0.0.4/src/misc/installation/RtMidi.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/RtMidi.h` & `cytosim-0.0.4/src/misc/installation/RtMidi.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/builder/0-live.command` & `cytosim-0.0.4/src/misc/installation/builder/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/builder/france.txt` & `cytosim-0.0.4/src/misc/installation/master/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/cytobuilder.cpp` & `cytosim-0.0.4/src/misc/installation/cytobuilder.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/cytomaster.cpp` & `cytosim-0.0.4/src/misc/installation/cytomaster.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/cytomaster.xcodeproj/project.pbxproj` & `cytosim-0.0.4/src/misc/installation/cytomaster.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/makefile` & `cytosim-0.0.4/src/misc/installation/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/master/0-live.command` & `cytosim-0.0.4/src/misc/installation/master/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/master/config7.cym` & `cytosim-0.0.4/src/misc/installation/master/config7.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/rtmidi_c.cpp` & `cytosim-0.0.4/src/misc/installation/rtmidi_c.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/misc/installation/rtmidi_c.h` & `cytosim-0.0.4/src/misc/installation/rtmidi_c.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/CMakeLists.txt` & `cytosim-0.0.4/src/play/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/makefile.inc` & `cytosim-0.0.4/src/play/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/play.cc` & `cytosim-0.0.4/src/play/play.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/play_keys.cc` & `cytosim-0.0.4/src/play/play_keys.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/play_menus.cc` & `cytosim-0.0.4/src/play/play_menus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/play_mouse.cc` & `cytosim-0.0.4/src/play/play_mouse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/player.cc` & `cytosim-0.0.4/src/play/player.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/player.h` & `cytosim-0.0.4/src/play/player.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/player_disp.cc` & `cytosim-0.0.4/src/play/player_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/player_prop.cc` & `cytosim-0.0.4/src/play/player_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/play/player_prop.h` & `cytosim-0.0.4/src/play/player_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/CMakeLists.txt` & `cytosim-0.0.4/src/sim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/bead.cc` & `cytosim-0.0.4/src/sim/bead.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/bead.h` & `cytosim-0.0.4/src/sim/bead.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/bead_set.cc` & `cytosim-0.0.4/src/sim/bead_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/bead_set.h` & `cytosim-0.0.4/src/sim/bead_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/chain.cc` & `cytosim-0.0.4/src/sim/chain.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/chain.h` & `cytosim-0.0.4/src/sim/chain.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/common.h` & `cytosim-0.0.4/src/sim/common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couple.cc` & `cytosim-0.0.4/src/sim/couple.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couple.h` & `cytosim-0.0.4/src/sim/couple.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couple_prop.cc` & `cytosim-0.0.4/src/sim/couple_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couple_prop.h` & `cytosim-0.0.4/src/sim/hand_prop.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,207 +1,252 @@
 // Cytosim was created by Francois Nedelec. Copyright 2007-2017 EMBL.
-#ifndef COUPLE_PROP_H
-#define COUPLE_PROP_H
+
+#ifndef HAND_PROP
+#define HAND_PROP
 
 #include "real.h"
-#include "property.h"
-#include "hand_prop.h"
 #include "common.h"
+#include "property.h"
+
+
+/// enables "bind_only_free_end" to limit binding of Hands to Fibers
+#define NEW_BIND_ONLY_FREE_END 0
 
-class Couple;
-class Space;
+class Hand;
+class HandMonitor;
+class PointDisp;
 
-/// Property for Couple
+/// Property for Hand
 /**
  @ingroup Properties
 */
-class CoupleProp : public Property
+class HandProp : public Property
 {
-    friend class Couple;
+    friend class Hand;
     
 public:
+      
+    /// return one of the Property derived from HandProp
+    static HandProp * newProperty(const std::string& n, Glossary&);
     
-    /// indicates a specificity for crosslinking two fibers
-    /** 
-     The criteria is based on the angle defined by the two fibers.
-     Since fibers are oriented, the angle in Radian is well defined between -PI and +PI:
-     - 0 corresponds to parallel fibers having the same orientation,
-     - PI/2 correspond to orthogonal fibers,
-     - -PI corresponds to parallel fibers having opposite orientation (antiparallel)
-     .
-     The allowed angle correspond to +/- 60 degree, which is rather arbitrary.
-     */
-    enum Specificity 
-    {
-        BIND_ALWAYS,           ///< can bind in any configuration
-        BIND_PARALLEL,         ///< can link two fibers only if `cosine(angle) > 0.5`
-        BIND_NOT_PARALLEL,     ///< can link two fibers only if `cosine(angle) < 0.5`
-        BIND_ANTIPARALLEL,     ///< can link two fibers only if `cosine(angle) < -0.5`
-        BIND_NOT_ANTIPARALLEL, ///< can link two fibers only if `cosine(angle) > -0.5`
-        BIND_ORTHOGONAL        ///< can link two fibers only if `-sqrt(3)/2 < cosine(angle) < sqrt(3)/2`
-    };
+public:
     
     /**
-     @defgroup CouplePar Parameters of Couple
+     @defgroup HandPar Parameters of Hand
      @ingroup Parameters
      @{
      */
     
+    /// rate of attachment when the Hand is within `binding_range` (also known as `binding[0]`)
+    /**
+     This has units of 1/second.
+     The molecular binding_rate of conventional kinesin is 4.7 +/- 2.4 /s:
+         Leduc et al. PNAS 2004 vol. 101 no. 49 17096-17101
+         http://dx.doi.org/10.1073/pnas.0406598101 \n
+         http://www.pnas.org/content/101/49/17096.abstract
+     
+     <em>default value = 0</em>
+     */
+    real         binding_rate;
+    
+    
+    /// maximum distance at which the Hand can bind (also known as `binding[1]`)
+    real         binding_range;
+    
+    
+    /// can be set to restrict binding to certain type of Fiber
+    /**
+     The binding to a fiber is allowed only if the keys of the Hand and Fiber match.
+     The test uses a BITWISE-AND of the two keys:
+
+         if ( fiber:binding_key & hand:binding_key )
+             allowed = true;
+         else
+             allowed = false;
+
+     Thus, with `binding_key==0' attachment is completely disabled, and in general
+     one needs to look at the bit-pattern of the number in base 2. For example
+     `1` can bind to `3` but not to `2`.
+     
+     <em>default value = all-bits-at-1</em>
+     */
+    unsigned int binding_key;
+    
+    
+    /// detachment rate in the absence of load (also known as `unbinding[0]`)
+    /**
+     This defines a detachment opportunity that is proportional to time.
+     Kramers theory specifies that the detachment rate depends on the force
+     in the link:
+     
+         RATE = unbinding_rate * exp( FORCE / unbinding_force )
+     
+     where FORCE is the norm of the tension in the link holding the Hand,
+     and `unbinding_rate' and `unbinding_force' are two parameters.
+     By setting `unbinding_force=inf', unbinding is made independent of load.
+     
+     Two articles:
+         Mechanics of the kinesin step
+         Carter, N. & Cross, R. Nature 435, 308–312 (2005).
+         http://dx.doi.org/doi:10.1038/nature03528
+     and
+         Examining kinesin processivity within a general gating framework
+         Andreasson et al. eLife 2015;4:e07403
+         http://dx.doi.org/10.7554/eLife.07403
+     provide similar values for conventional kinesin:
+
+         unbinding_rate = 1 / s
+         unbinding_force ~ 2 pN
+     
+     <em>default value = 0</em>
+     (see @ref Stochastic)
+     */
+    real         unbinding_rate;
+    
+    
+    /// characteristic force of unbinding (also known as `unbinding[1]`)
+    /**
+     @copydetails unbinding_rate
+     
+     <em>default value = inf</em>
+     */
+    real         unbinding_force;
+    
+    
+    /// if true, the Hand can also bind directly to the tip of fibers
+    /**
+     The value of `bind_also_end` affects Hands that are located at a position
+     for which the orthogonal projection on the fiber backbone is beyond one
+     of the end. In this case, the attachement will occur only if `bind_also_end`
+     is set and matches this end. Attachment will occur at the end of the fiber,
+     if the distance is shorter than `binding_range`.
+     
+     Values for  are `off`, `minus_end`, `plus_end` and `both_ends`.
+     
+     In other words, setting 'bind_also_end==true', will extend the capture
+     regions of the fibers to include one or two hemi-spheres at the ends of
+     the fibers, with a radius `binding_range`.
+     
+     <em>default value = off</em>
+     */
+    int          bind_also_end;
     
-    /// name of first Hand in Couple
-    std::string  hand1;
     
-    /// name of second Hand in Couple
-    std::string  hand2;
+    /// if true, the Hand can bind only near the ends of the fibers
+    /**
+     This determines that a Hand can only bind near the ends of the fiber.
+     This parameter can be 'none', 'plus_end', 'minus_end' or 'both_ends'.
+     Binding is allowed on positions located within a distance 'bind_end_range'
+     from the specified end ('bind_end_range' is specified as `bind_only_end[1]`).
+     
+     <em>default value = off</em>
+     */
+    FiberEnd     bind_only_end;
     
-    /// stiffness of link between the two Hands while linking (pN/um)
-    real         stiffness;
     
-    /// resting length of the link (um)
-    real         length;
-    
-    /// diffusion coefficient while unattached (um^2/s)
-    real         diffusion;
-    
-    /// if set > 0, assumes uniform concentration of diffusing Couple
-    /**
-     The possible values for `fast_diffusion` are:
-     
-     - 0: disabled.
-       Every Couple is explicitly represented by a diffusing point. The
-       unattached Couple move randomly, with the specified diffusion constant,
-       and they may accumulate at certain regions of the simulation space. That
-       happens in particular with asters when the motors move inward. In fact,
-       the aster can act like a black hole for the motors, in certain conditions.
-
-     - 1: attach Couple along the length of filaments
-       It is assumed that free Couples are uniformly distributed, and they are 
-       thus not explicitly represented. In this mode, Cytosim will only keep a 
-       count of the number of free Couples, and directly attach these Couples by
-       one of their Hand, at positions of the fibers selected randomly, irrespective
-       of the manner in which the filaments are distributed spatially.
-       In this mode, the Couple diffusion constant is not relevant.
-
-     - 2: attach Couple only at growing PLUS_ENDS
-       Similar to mode 1, but Hand1 of Couple is directly attached to the plus tips
-       of growing fibers. The number of attachments is proportional to the new
-       polymer mass, which is `time_step * growing_speed`, but occurs otherwise
-       equally to every filaments.
-     .
-     
-     Enabling `fast_diffusion` can make the simulation a bit faster when there
-     are a lot of Couples, but another reason to use this mode is that it makes
-     the model simpler, since the fraction of bound/free Couples can then be calculated
-     analytically. This also avoid the accumulation of motors in aster and other
-     organized structures, which are stronger in a 2D geometry, compared to 3D. 
-     Thus one may wish to enable `fast_diffusion` in a 2D simulation to better
-     represent a 3D system.
-     
-     `fast_diffusion` does not affect Couples in the attached state.
-     */
-    int          fast_diffusion;
-    
-    /// if ( trans_activated == 1 ), Hand2 is active only if Hand1 is bound
-    /**
-     Both Hands of a Couple are normally equally active. With this feature,
-     the activity of Hand2 is conditioned on Hand1 being attached.
-     In other words, Hand2 remains inactive if Hand1 is not attached.
-     This is very useful for example to make a nucleator that nucleates only after
-     it has docked on an existing filament.
-     */
-    bool         trans_activated;
-
-    /// prevents both Hands from binding at the same position on a Fiber (default=true)
-    /**
-     By default, the two Hands of a Couple may not bind at the same position on 
-     the same Fiber. Such a degenerate binding may be impossible due to the molecular 
-     configuration of the complex. Note that no restriction is imposed if the Hands
-     attempt to bind to different fibers, or to the same fiber at distant positions. 
-     The exact criteria is that the Hands cannot bind onto the same segment, or 
-     to segments that have a point in common.
-     
-     Setting `stiff==false`, however, allows the two hands from the Couple to bind 
-     nearby positions on the same fiber. In such a degenerate configuration, the 
-     link is unproductive as it cannot produce force, but the feature may be useful 
-     to combine activities such as cutting and motors.
-     */
-    bool         stiff;
-    
-    /// Specificity of binding to a pair a Fiber
-    /**
-     Set to limit the binding to only certain configurations:
-     - `off`             : no restriction (default)
-     - `parallel`        : parallel filaments with an angle below 60 degrees
-     - `antiparallel`    : anti-parallel filaments with an angle below 60 degrees
-     - `not_parallel`    : anti-parallel filaments with an angle below 120 degrees
-     - `not_antiparallel`: parallel filaments with an angle below 120 degrees
-     - `orthogonal`      : filaments with an angle between 60 and 120 degrees
-     .
-     This limit the attachment of a Hand when the other Hand is already attached,
-     as a function of the angle that is defined by the already bound filament,
-     and the potential new one. The first attachment of any Hand is unrestricted.
-     */
-    Specificity  specificity;
+    /// cutoff associated with `bind_only_end` where hand may bind (set as `bind_only_end[1]`)
+    real         bind_end_range;
 
-    /// Confinement can be `off`, `inside` (default) or `surface`
-    Confinement  confine;
+#if NEW_BIND_ONLY_FREE_END
+    /// if true, only bind fiber tip if no other hand is bound already
+    bool         bind_only_free_end;
+#endif
     
-    /// Unused Parameter: confinement stiffness (also known as `confine[1]`)
-    //real         confine_stiffness;
+    /// if false, the Hand will detach immediately upon reaching a growing or a static fiber end
+    /**
+     A Hand may reach the tip of the fiber on which it is bound, because it has
+     moved, and `hold_growing_end` will determine the probability of detachment
+     in this case. A value of 0 leads to immediate detachment.
+     With a value of 1, the hand will remain attached.
+     
+     <em>default = 0</em>
+     */
+    real         hold_growing_end;
+    
+    
+    /// if false, the Hand will detach immediately upon reaching a shrinking fiber end
+    /**
+     A Hand may reach the tip of the fiber on which it is bound,
+     of the tip of the fiber may reach a immobile hand because it is disassembling.
+     When this happens, `hold_shrinking_end` will determine if the Hand
+     will detach or not.
+     If `hold_shrinking_end` is true, the hand will be relocated to track the end.
+
+     <em>default = false</em>
+     */
+    real         hold_shrinking_end;
     
-    /// name of space used for confinement (also known as `confine[2]`)
-    std::string  confine_space;
     
     /// specialization
     /**
-     @copydetails CoupleGroup
+     @copydetails HandGroup
      */
     std::string  activity;
     
-    /// @}
     
-    /// pointer to Property of Hand 1
-    HandProp *    hand1_prop;
-    /// pointer to Property of Hand 2
-    HandProp *    hand2_prop;
-
-protected:
-    
-    real          diffusion_dt;
-    /// pointer to actual confinement Space, derived from `confine_space`
-    Space const*  confine_space_ptr;
+    /// display parameters (see @ref PointDispPar)
+    std::string  display;
+    
+    /** @} */
 
 public:
+
+    /// derived variable: 1.0/unbinding_force
+    real   unbinding_force_inv;
+    
+    /// derived variable = probability to bind in one `time_step`;
+    real   binding_prob;
+    
+    /// derived variable = square(binding_range);
+    real   binding_range_sqr;
+    
+    /// derived variable = unbinding_rate * time_step;
+    real   unbinding_rate_dt;
+    
+    /// flag to indicate that `display` has a new value
+    bool   display_fresh;
+    
+public:
+
+    /// the display parameters for this category of Hand
+    PointDisp * disp;
     
     /// constructor
-    CoupleProp(const std::string& n) : Property(n)  { clear(); }
+    HandProp(const std::string& n) : Property(n), disp(nullptr) { clear(); }
     
     /// destructor
-    ~CoupleProp() { }
-    
-    /// create a Couple having this property
-    virtual Couple * newCouple(Glossary * = nullptr) const;
+    ~HandProp() { }
     
+    /// return a Hand with this property
+    virtual Hand * newHand(HandMonitor*) const;
+
     /// identifies the property
-    std::string category() const { return "couple"; }
+    std::string category() const { return "hand"; }
     
     /// set default values
     void clear();
     
     /// set from a Glossary
-    void read(Glossary&);
+    virtual void read(Glossary&);
     
-    /// compute derived parameter values
-    void complete(Simul const&);
+    /// compute values derived from the parameters
+    virtual void complete(Simul const&);
     
-    /// return a carbon copy of object
-    Property* clone() const { return new CoupleProp(*this); }
+    /// perform additional tests for the validity of parameters, given the elasticity
+    virtual void checkStiffness(real stiff, real len, real mul, real kT) const;
+    
+    /// Attachment rate per unit length of fiber
+    real bindingSectionRate() const;
+    
+    /// Attachment probability per unit length of fiber in one time_step
+    real bindingSectionProb() const;
 
     /// write all values
     void write_values(std::ostream&) const;
-  
-    /// return volume of confine_space
-    real spaceVolume() const;
+    
+    /// return a carbon copy of object
+    Property* clone() const { return new HandProp(*this); }
 };
 
+
 #endif
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cytosim-0.0.3/src/sim/couple_set.cc` & `cytosim-0.0.4/src/sim/couple_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couple_set.h` & `cytosim-0.0.4/src/sim/couple_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/bridge.cc` & `cytosim-0.0.4/src/sim/couples/bridge.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/bridge.h` & `cytosim-0.0.4/src/sim/couples/bridge.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/bridge_prop.cc` & `cytosim-0.0.4/src/sim/couples/bridge_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/bridge_prop.h` & `cytosim-0.0.4/src/sim/couples/bridge_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/couple_long.cc` & `cytosim-0.0.4/src/sim/couples/couple_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/couple_long.h` & `cytosim-0.0.4/src/sim/couples/couple_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/crosslink.cc` & `cytosim-0.0.4/src/sim/couples/crosslink.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/crosslink.h` & `cytosim-0.0.4/src/sim/couples/crosslink.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/crosslink_long.cc` & `cytosim-0.0.4/src/sim/couples/crosslink_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/crosslink_long.h` & `cytosim-0.0.4/src/sim/couples/crosslink_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/crosslink_prop.cc` & `cytosim-0.0.4/src/sim/couples/crosslink_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/crosslink_prop.h` & `cytosim-0.0.4/src/sim/couples/crosslink_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/duo.cc` & `cytosim-0.0.4/src/sim/couples/duo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/duo.h` & `cytosim-0.0.4/src/sim/couples/duo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/duo_long.cc` & `cytosim-0.0.4/src/sim/couples/duo_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/duo_long.h` & `cytosim-0.0.4/src/sim/couples/duo_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/duo_prop.cc` & `cytosim-0.0.4/src/sim/couples/duo_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/duo_prop.h` & `cytosim-0.0.4/src/sim/couples/duo_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/fork.cc` & `cytosim-0.0.4/src/sim/couples/fork.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/fork.h` & `cytosim-0.0.4/src/sim/couples/fork.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/fork_prop.cc` & `cytosim-0.0.4/src/sim/couples/fork_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/fork_prop.h` & `cytosim-0.0.4/src/sim/couples/fork_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/shackle.cc` & `cytosim-0.0.4/src/sim/couples/shackle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/shackle.h` & `cytosim-0.0.4/src/sim/couples/shackle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/shackle_long.cc` & `cytosim-0.0.4/src/sim/couples/shackle_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/shackle_long.h` & `cytosim-0.0.4/src/sim/couples/shackle_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/shackle_prop.cc` & `cytosim-0.0.4/src/sim/couples/shackle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/couples/shackle_prop.h` & `cytosim-0.0.4/src/sim/couples/shackle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/event.cc` & `cytosim-0.0.4/src/sim/event.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/event.h` & `cytosim-0.0.4/src/sim/event.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/event_set.cc` & `cytosim-0.0.4/src/sim/event_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/event_set.h` & `cytosim-0.0.4/src/sim/event_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber.cc` & `cytosim-0.0.4/src/sim/fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber.h` & `cytosim-0.0.4/src/sim/fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_grid.cc` & `cytosim-0.0.4/src/sim/fiber_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_grid.h` & `cytosim-0.0.4/src/sim/fiber_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_grid2.cc` & `cytosim-0.0.4/src/sim/fiber_grid2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_prop.cc` & `cytosim-0.0.4/src/sim/fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_prop.h` & `cytosim-0.0.4/src/sim/fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_segment.cc` & `cytosim-0.0.4/src/sim/fiber_segment.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_segment.h` & `cytosim-0.0.4/src/sim/fiber_segment.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_set.cc` & `cytosim-0.0.4/src/sim/fiber_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_set.h` & `cytosim-0.0.4/src/sim/fiber_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_site.cc` & `cytosim-0.0.4/src/sim/fiber_site.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fiber_site.h` & `cytosim-0.0.4/src/sim/fiber_site.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/classic_fiber.cc` & `cytosim-0.0.4/src/sim/fibers/classic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/classic_fiber.h` & `cytosim-0.0.4/src/sim/fibers/classic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.cc` & `cytosim-0.0.4/src/sim/fibers/classic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/classic_fiber_prop.h` & `cytosim-0.0.4/src/sim/fibers/classic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/dynamic_fiber.cc` & `cytosim-0.0.4/src/sim/fibers/dynamic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/dynamic_fiber.h` & `cytosim-0.0.4/src/sim/fibers/dynamic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.cc` & `cytosim-0.0.4/src/sim/fibers/dynamic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/dynamic_fiber_prop.h` & `cytosim-0.0.4/src/sim/fibers/dynamic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/growing_fiber.cc` & `cytosim-0.0.4/src/sim/fibers/growing_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/growing_fiber.h` & `cytosim-0.0.4/src/sim/fibers/growing_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.cc` & `cytosim-0.0.4/src/sim/fibers/growing_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/growing_fiber_prop.h` & `cytosim-0.0.4/src/sim/fibers/growing_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.cc` & `cytosim-0.0.4/src/sim/fibers/treadmilling_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber.h` & `cytosim-0.0.4/src/sim/fibers/treadmilling_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.cc` & `cytosim-0.0.4/src/sim/fibers/treadmilling_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/fibers/treadmilling_fiber_prop.h` & `cytosim-0.0.4/src/sim/fibers/treadmilling_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/field.cc` & `cytosim-0.0.4/src/sim/field.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/field.h` & `cytosim-0.0.4/src/sim/field.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/field_prop.cc` & `cytosim-0.0.4/src/sim/field_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/field_prop.h` & `cytosim-0.0.4/src/sim/field_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/field_set.cc` & `cytosim-0.0.4/src/sim/field_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/field_set.h` & `cytosim-0.0.4/src/sim/field_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/field_values.h` & `cytosim-0.0.4/src/sim/field_values.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/frame_reader.cc` & `cytosim-0.0.4/src/sim/frame_reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/frame_reader.h` & `cytosim-0.0.4/src/sim/frame_reader.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hand.cc` & `cytosim-0.0.4/src/sim/hand.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hand.h` & `cytosim-0.0.4/src/sim/hand.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hand_monitor.h` & `cytosim-0.0.4/src/sim/hand_monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hand_prop.cc` & `cytosim-0.0.4/src/sim/hand_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/actor.cc` & `cytosim-0.0.4/src/sim/hands/actor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/actor.h` & `cytosim-0.0.4/src/sim/hands/actor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/actor_prop.cc` & `cytosim-0.0.4/src/sim/hands/actor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/actor_prop.h` & `cytosim-0.0.4/src/sim/hands/actor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/chewer.cc` & `cytosim-0.0.4/src/sim/hands/chewer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/chewer.h` & `cytosim-0.0.4/src/sim/hands/chewer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/chewer_prop.cc` & `cytosim-0.0.4/src/sim/hands/chewer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/chewer_prop.h` & `cytosim-0.0.4/src/sim/hands/chewer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/cutter.cc` & `cytosim-0.0.4/src/sim/hands/cutter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/cutter.h` & `cytosim-0.0.4/src/sim/hands/cutter.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/cutter_prop.cc` & `cytosim-0.0.4/src/sim/hands/cutter_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/cutter_prop.h` & `cytosim-0.0.4/src/sim/hands/cutter_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/digit.cc` & `cytosim-0.0.4/src/sim/hands/digit.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/digit.h` & `cytosim-0.0.4/src/sim/hands/digit.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/digit_prop.cc` & `cytosim-0.0.4/src/sim/hands/digit_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/digit_prop.h` & `cytosim-0.0.4/src/sim/hands/digit_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/dynein.cc` & `cytosim-0.0.4/src/sim/hands/dynein.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/dynein.h` & `cytosim-0.0.4/src/sim/hands/dynein.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/dynein_prop.cc` & `cytosim-0.0.4/src/sim/hands/dynein_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/dynein_prop.h` & `cytosim-0.0.4/src/sim/hands/dynein_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/kinesin.cc` & `cytosim-0.0.4/src/sim/hands/kinesin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/kinesin.h` & `cytosim-0.0.4/src/sim/hands/kinesin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/kinesin_prop.cc` & `cytosim-0.0.4/src/sim/hands/kinesin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/kinesin_prop.h` & `cytosim-0.0.4/src/sim/hands/kinesin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/mighty.cc` & `cytosim-0.0.4/src/sim/hands/mighty.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/mighty.h` & `cytosim-0.0.4/src/sim/hands/mighty.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/mighty_prop.cc` & `cytosim-0.0.4/src/sim/hands/mighty_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/mighty_prop.h` & `cytosim-0.0.4/src/sim/hands/mighty_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/motor.cc` & `cytosim-0.0.4/src/sim/hands/motor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/motor.h` & `cytosim-0.0.4/src/sim/hands/motor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/motor_prop.cc` & `cytosim-0.0.4/src/sim/hands/motor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/motor_prop.h` & `cytosim-0.0.4/src/sim/hands/motor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/myosin.cc` & `cytosim-0.0.4/src/sim/hands/myosin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/myosin.h` & `cytosim-0.0.4/src/sim/hands/myosin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/myosin_prop.cc` & `cytosim-0.0.4/src/sim/hands/myosin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/myosin_prop.h` & `cytosim-0.0.4/src/sim/hands/myosin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/nucleator.cc` & `cytosim-0.0.4/src/sim/hands/nucleator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/nucleator.h` & `cytosim-0.0.4/src/sim/hands/nucleator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/nucleator_prop.cc` & `cytosim-0.0.4/src/sim/hands/nucleator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/nucleator_prop.h` & `cytosim-0.0.4/src/sim/hands/nucleator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/regulator.cc` & `cytosim-0.0.4/src/sim/hands/regulator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/regulator.h` & `cytosim-0.0.4/src/sim/hands/regulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/regulator_prop.cc` & `cytosim-0.0.4/src/sim/hands/regulator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/regulator_prop.h` & `cytosim-0.0.4/src/sim/hands/regulator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/rescuer.cc` & `cytosim-0.0.4/src/sim/hands/rescuer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/rescuer.h` & `cytosim-0.0.4/src/sim/hands/rescuer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/rescuer_prop.cc` & `cytosim-0.0.4/src/sim/hands/rescuer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/rescuer_prop.h` & `cytosim-0.0.4/src/sim/hands/rescuer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/slider.cc` & `cytosim-0.0.4/src/sim/hands/slider.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/slider.h` & `cytosim-0.0.4/src/sim/hands/slider.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/slider_prop.cc` & `cytosim-0.0.4/src/sim/hands/slider_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/slider_prop.h` & `cytosim-0.0.4/src/sim/hands/slider_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/tracker.cc` & `cytosim-0.0.4/src/sim/hands/tracker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/tracker.h` & `cytosim-0.0.4/src/sim/hands/tracker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/tracker_prop.cc` & `cytosim-0.0.4/src/sim/hands/tracker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/tracker_prop.h` & `cytosim-0.0.4/src/sim/hands/tracker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/walker.cc` & `cytosim-0.0.4/src/sim/hands/walker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/walker.h` & `cytosim-0.0.4/src/sim/hands/walker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/walker_prop.cc` & `cytosim-0.0.4/src/sim/hands/walker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/hands/walker_prop.h` & `cytosim-0.0.4/src/sim/hands/walker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/interface.cc` & `cytosim-0.0.4/src/sim/interface.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/interface.h` & `cytosim-0.0.4/src/sim/interface.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/interpolation.cc` & `cytosim-0.0.4/src/sim/interpolation.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/interpolation.h` & `cytosim-0.0.4/src/sim/interpolation.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/interpolation4.cc` & `cytosim-0.0.4/src/sim/interpolation4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/interpolation4.h` & `cytosim-0.0.4/src/sim/interpolation4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/lattice.cc` & `cytosim-0.0.4/src/sim/lattice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/lattice.h` & `cytosim-0.0.4/src/sim/lattice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/makefile.inc` & `cytosim-0.0.4/src/sim/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/meca.cc` & `cytosim-0.0.4/src/sim/meca.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/meca.h` & `cytosim-0.0.4/src/sim/meca.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/meca1d.h` & `cytosim-0.0.4/src/sim/meca1d.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/meca_inter.cc` & `cytosim-0.0.4/src/sim/meca_inter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecable.cc` & `cytosim-0.0.4/src/sim/mecable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecable.h` & `cytosim-0.0.4/src/sim/mecable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecafil.cc` & `cytosim-0.0.4/src/sim/mecafil.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecafil.h` & `cytosim-0.0.4/src/sim/mecafil.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecafil_project.cc` & `cytosim-0.0.4/src/sim/mecafil_project.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecafil_projectmat.cc` & `cytosim-0.0.4/src/sim/mecafil_projectmat.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecapoint.cc` & `cytosim-0.0.4/src/sim/mecapoint.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/mecapoint.h` & `cytosim-0.0.4/src/sim/mecapoint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/modulo.cc` & `cytosim-0.0.4/src/sim/modulo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/modulo.h` & `cytosim-0.0.4/src/sim/modulo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/movable.cc` & `cytosim-0.0.4/src/sim/movable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/movable.h` & `cytosim-0.0.4/src/sim/movable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/object.cc` & `cytosim-0.0.4/src/sim/object.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/object.h` & `cytosim-0.0.4/src/sim/object.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/object_set.cc` & `cytosim-0.0.4/src/sim/object_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/object_set.h` & `cytosim-0.0.4/src/sim/object_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizer.cc` & `cytosim-0.0.4/src/sim/organizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizer.h` & `cytosim-0.0.4/src/sim/organizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizer_set.cc` & `cytosim-0.0.4/src/sim/organizer_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizer_set.h` & `cytosim-0.0.4/src/sim/organizer_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/aster.cc` & `cytosim-0.0.4/src/sim/organizers/aster.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/aster.h` & `cytosim-0.0.4/src/sim/organizers/aster.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/aster_prop.cc` & `cytosim-0.0.4/src/sim/organizers/aster_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/aster_prop.h` & `cytosim-0.0.4/src/sim/organizers/aster_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/bundle.cc` & `cytosim-0.0.4/src/sim/organizers/bundle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/bundle.h` & `cytosim-0.0.4/src/sim/organizers/bundle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/bundle_prop.cc` & `cytosim-0.0.4/src/sim/organizers/bundle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/bundle_prop.h` & `cytosim-0.0.4/src/sim/organizers/bundle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/fake.cc` & `cytosim-0.0.4/src/sim/organizers/fake.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/fake.h` & `cytosim-0.0.4/src/sim/organizers/fake.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/fake_prop.cc` & `cytosim-0.0.4/src/sim/organizers/fake_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/fake_prop.h` & `cytosim-0.0.4/src/sim/organizers/fake_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/nucleus.cc` & `cytosim-0.0.4/src/sim/organizers/nucleus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/nucleus.h` & `cytosim-0.0.4/src/sim/organizers/nucleus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/nucleus_prop.cc` & `cytosim-0.0.4/src/sim/organizers/nucleus_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/organizers/nucleus_prop.h` & `cytosim-0.0.4/src/sim/organizers/nucleus_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/parser.cc` & `cytosim-0.0.4/src/sim/parser.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/parser.h` & `cytosim-0.0.4/src/sim/parser.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/point_grid.cc` & `cytosim-0.0.4/src/sim/point_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/point_grid.h` & `cytosim-0.0.4/src/sim/point_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sim.cc` & `cytosim-0.0.4/src/sim/sim.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sim_thread.cc` & `cytosim-0.0.4/src/sim/sim_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sim_thread.h` & `cytosim-0.0.4/src/sim/sim_thread.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul.cc` & `cytosim-0.0.4/src/sim/simul.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul.h` & `cytosim-0.0.4/src/sim/simul.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul_custom.cc` & `cytosim-0.0.4/src/sim/simul_custom.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul_file.cc` & `cytosim-0.0.4/src/sim/simul_file.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul_prop.cc` & `cytosim-0.0.4/src/sim/simul_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul_report.cc` & `cytosim-0.0.4/src/sim/simul_report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul_solve.cc` & `cytosim-0.0.4/src/sim/simul_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/simul_step.cc` & `cytosim-0.0.4/src/sim/simul_step.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/single.cc` & `cytosim-0.0.4/src/sim/single.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/single.h` & `cytosim-0.0.4/src/sim/single.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/single_prop.cc` & `cytosim-0.0.4/src/sim/single_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/single_prop.h` & `cytosim-0.0.4/src/sim/single_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/single_set.cc` & `cytosim-0.0.4/src/sim/single_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/single_set.h` & `cytosim-0.0.4/src/sim/single_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/picket.cc` & `cytosim-0.0.4/src/sim/singles/picket.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/picket.h` & `cytosim-0.0.4/src/sim/singles/picket.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/picket_long.cc` & `cytosim-0.0.4/src/sim/singles/picket_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/picket_long.h` & `cytosim-0.0.4/src/sim/singles/picket_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/wrist.cc` & `cytosim-0.0.4/src/sim/singles/wrist.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/wrist.h` & `cytosim-0.0.4/src/sim/singles/wrist.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/wrist_long.cc` & `cytosim-0.0.4/src/sim/singles/wrist_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/singles/wrist_long.h` & `cytosim-0.0.4/src/sim/singles/wrist_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/solid.cc` & `cytosim-0.0.4/src/sim/solid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/solid.h` & `cytosim-0.0.4/src/sim/solid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/solid_prop.cc` & `cytosim-0.0.4/src/sim/solid_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/solid_prop.h` & `cytosim-0.0.4/src/sim/solid_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/solid_set.cc` & `cytosim-0.0.4/src/sim/solid_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/solid_set.h` & `cytosim-0.0.4/src/sim/solid_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/space.cc` & `cytosim-0.0.4/src/sim/space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/space.h` & `cytosim-0.0.4/src/sim/space.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/space_prop.cc` & `cytosim-0.0.4/src/sim/space_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/space_prop.h` & `cytosim-0.0.4/src/sim/space_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/space_set.cc` & `cytosim-0.0.4/src/sim/space_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/space_set.h` & `cytosim-0.0.4/src/sim/space_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_banana.cc` & `cytosim-0.0.4/src/sim/spaces/space_banana.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_banana.h` & `cytosim-0.0.4/src/sim/spaces/space_banana.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_capsule.cc` & `cytosim-0.0.4/src/sim/spaces/space_capsule.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_capsule.h` & `cytosim-0.0.4/src/sim/spaces/space_capsule.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_cylinder.cc` & `cytosim-0.0.4/src/sim/spaces/space_cylinder.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_cylinder.h` & `cytosim-0.0.4/src/sim/spaces/space_cylinder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_cylinderP.cc` & `cytosim-0.0.4/src/sim/spaces/space_cylinderP.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_cylinderP.h` & `cytosim-0.0.4/src/sim/spaces/space_cylinderP.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_cylinderZ.cc` & `cytosim-0.0.4/src/sim/spaces/space_cylinderZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_cylinderZ.h` & `cytosim-0.0.4/src/sim/spaces/space_cylinderZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_dice.cc` & `cytosim-0.0.4/src/sim/spaces/space_dice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_dice.h` & `cytosim-0.0.4/src/sim/spaces/space_dice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_ellipse.cc` & `cytosim-0.0.4/src/sim/spaces/space_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_ellipse.h` & `cytosim-0.0.4/src/sim/spaces/space_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_periodic.cc` & `cytosim-0.0.4/src/sim/spaces/space_periodic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_periodic.h` & `cytosim-0.0.4/src/sim/spaces/space_periodic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_polygon.cc` & `cytosim-0.0.4/src/sim/spaces/space_polygon.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_polygon.h` & `cytosim-0.0.4/src/sim/spaces/space_polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_polygonZ.cc` & `cytosim-0.0.4/src/sim/spaces/space_polygonZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_polygonZ.h` & `cytosim-0.0.4/src/sim/spaces/space_polygonZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_ring.cc` & `cytosim-0.0.4/src/sim/spaces/space_ring.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_ring.h` & `cytosim-0.0.4/src/sim/spaces/space_ring.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_sphere.cc` & `cytosim-0.0.4/src/sim/spaces/space_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_sphere.h` & `cytosim-0.0.4/src/sim/spaces/space_sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_square.cc` & `cytosim-0.0.4/src/sim/spaces/space_square.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_square.h` & `cytosim-0.0.4/src/sim/spaces/space_square.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_strip.cc` & `cytosim-0.0.4/src/sim/spaces/space_strip.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_strip.h` & `cytosim-0.0.4/src/sim/spaces/space_strip.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_torus.cc` & `cytosim-0.0.4/src/sim/spaces/space_torus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/spaces/space_torus.h` & `cytosim-0.0.4/src/sim/spaces/space_torus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sphere.cc` & `cytosim-0.0.4/src/sim/sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sphere.h` & `cytosim-0.0.4/src/sim/sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sphere_prop.cc` & `cytosim-0.0.4/src/sim/sphere_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sphere_prop.h` & `cytosim-0.0.4/src/sim/sphere_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sphere_set.cc` & `cytosim-0.0.4/src/sim/sphere_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/sphere_set.h` & `cytosim-0.0.4/src/sim/sphere_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/sim/splash.h` & `cytosim-0.0.4/src/sim/splash.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/CMakeLists.txt` & `cytosim-0.0.4/src/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/makefile.inc` & `cytosim-0.0.4/src/test/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test.cc` & `cytosim-0.0.4/src/test/test.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_blas.cc` & `cytosim-0.0.4/src/test/test_blas.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_code.cc` & `cytosim-0.0.4/src/test/test_code.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_cxx.cc` & `cytosim-0.0.4/src/test/test_cxx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_gillespie.cc` & `cytosim-0.0.4/src/test/test_gillespie.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_glapp.cc` & `cytosim-0.0.4/src/test/test_glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_glos.cc` & `cytosim-0.0.4/src/test/test_glos.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_glut.cc` & `cytosim-0.0.4/src/test/test_glut.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_glut3D.cc` & `cytosim-0.0.4/src/test/test_glut3D.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_grid.cc` & `cytosim-0.0.4/src/test/test_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_math.cc` & `cytosim-0.0.4/src/test/test_math.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_matrix.cc` & `cytosim-0.0.4/src/test/test_matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_omp.cc` & `cytosim-0.0.4/src/test/test_omp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_opengl.cc` & `cytosim-0.0.4/src/test/test_opengl.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_pipe.cc` & `cytosim-0.0.4/src/test/test_pipe.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_platonic.cc` & `cytosim-0.0.4/src/test/test_platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_quaternion.cc` & `cytosim-0.0.4/src/test/test_quaternion.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_random.cc` & `cytosim-0.0.4/src/test/test_random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_rasterizer.cc` & `cytosim-0.0.4/src/test/test_rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_signal.cc` & `cytosim-0.0.4/src/test/test_signal.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_simd.cc` & `cytosim-0.0.4/src/test/test_simd.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_sizeof.cc` & `cytosim-0.0.4/src/test/test_sizeof.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_solve.cc` & `cytosim-0.0.4/src/test/test_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_space.cc` & `cytosim-0.0.4/src/test/test_space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_sphere.cc` & `cytosim-0.0.4/src/test/test_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_thread.cc` & `cytosim-0.0.4/src/test/test_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/test/test_vbo.cc` & `cytosim-0.0.4/src/test/test_vbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/CMakeLists.txt` & `cytosim-0.0.4/src/tools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/cymart.cc` & `cytosim-0.0.4/src/tools/cymart.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/frametool.cc` & `cytosim-0.0.4/src/tools/frametool.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/makefile.inc` & `cytosim-0.0.4/src/tools/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/pycytoplay.cc` & `cytosim-0.0.4/src/tools/pycytoplay.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/pycytosim.cc` & `cytosim-0.0.4/src/tools/pycytosim.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/pycytosim.h` & `cytosim-0.0.4/src/tools/pycytosim.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/reader.cc` & `cytosim-0.0.4/src/tools/reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/report.cc` & `cytosim-0.0.4/src/tools/report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/reportF.cc` & `cytosim-0.0.4/src/tools/reportF.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.3/src/tools/sieve.cc` & `cytosim-0.0.4/src/tools/sieve.cc`

 * *Files identical despite different names*

