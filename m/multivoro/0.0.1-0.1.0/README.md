# Comparing `tmp/multivoro-0.0.1.tar.gz` & `tmp/multivoro-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multivoro-0.0.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "multivoro-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `multivoro-0.0.1.tar` & `multivoro-0.1.0.tar`

### file list

```diff
@@ -1,254 +1,255 @@
--rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 multivoro-0.0.1/.github/workflows/run-tox.yml
--rw-r--r--   0        0        0     1591 2022-11-09 12:37:21.000000 multivoro-0.0.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 multivoro-0.0.1/.gitignore
--rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 multivoro-0.0.1/.gitmodules
--rw-r--r--   0        0        0     3515 2022-11-09 12:37:21.000000 multivoro-0.0.1/CMakeLists.txt
--rw-r--r--   0        0        0     2402 2022-11-09 12:37:21.000000 multivoro-0.0.1/LICENSE
--rw-r--r--   0        0        0     3066 2022-11-09 12:37:21.000000 multivoro-0.0.1/README.rst
--rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/.git
--rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/Makefile
--rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/basic/Makefile
--rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/basic/doe_diagram.cc
--rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/basic/doe_diagram.pov
--rw-r--r--   0        0        0     1249 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/basic/import_2d.cc
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/basic/random_points_2d.cc
--rw-r--r--   0        0        0      909 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/basic/single_cell_2d.cc
--rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/boundary/Makefile
--rw-r--r--   0        0        0     1225 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/boundary/annulus.cc
--rw-r--r--   0        0        0     1209 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/boundary/comb.cc
--rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/boundary/container_bd.cc
--rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/boundary/nonconvex_cell.cc
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/extra/Makefile
--rw-r--r--   0        0        0     1906 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/extra/intersect.cc
--rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/extra/lloyd.cc
--rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/extra/lloyd_movie.pl
--rw-r--r--   0        0        0     1251 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/timing/timing_test_2d.cc
--rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/walls/Makefile
--rw-r--r--   0        0        0     1339 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/walls/circle.cc
--rw-r--r--   0        0        0     1563 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/examples/walls/polygon.cc
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/scripts/network.pl
--rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/scripts/sum.pl
--rw-r--r--   0        0        0    72416 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/Doxyfile
--rw-r--r--   0        0        0      915 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/Makefile
--rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/Makefile.dep
--rw-r--r--   0        0        0     4829 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/c_loops_2d.cc
--rw-r--r--   0        0        0    12191 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/c_loops_2d.hh
--rw-r--r--   0        0        0    18628 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/cell_2d.cc
--rw-r--r--   0        0        0     7342 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/cell_2d.hh
--rw-r--r--   0        0        0     3669 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/cell_nc_2d.cc
--rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/cell_nc_2d.hh
--rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/common.cc
--rw-r--r--   0        0        0     1766 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/common.hh
--rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/config.hh
--rw-r--r--   0        0        0    20929 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/container_2d.cc
--rw-r--r--   0        0        0    30391 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/container_2d.hh
--rw-r--r--   0        0        0     8577 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/container_2d_old.hh
--rw-r--r--   0        0        0     1153 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/cq_test.cc
--rw-r--r--   0        0        0    21785 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/ctr_boundary_2d.cc
--rw-r--r--   0        0        0    16956 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/ctr_boundary_2d.hh
--rw-r--r--   0        0        0     7836 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/ctr_quad_2d.cc
--rw-r--r--   0        0        0     3489 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/ctr_quad_2d.hh
--rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/quad_march.cc
--rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/quad_march.hh
--rw-r--r--   0        0        0     7421 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/rad_option.hh
--rw-r--r--   0        0        0     4258 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/v_base_2d.cc
--rw-r--r--   0        0        0     3539 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/v_base_2d.hh
--rw-r--r--   0        0        0     8450 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/v_base_wl_2d.cc
--rw-r--r--   0        0        0    32528 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/v_compute_2d.cc
--rw-r--r--   0        0        0     5045 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/v_compute_2d.hh
--rw-r--r--   0        0        0    47351 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/v_connect.cc
--rw-r--r--   0        0        0    13078 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/v_connect.hh
--rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/voro++_2d.cc
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/voro++_2d.hh
--rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/wall_2d.cc
--rw-r--r--   0        0        0     2403 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/wall_2d.hh
--rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/worklist_2d.hh
--rwxr-xr-x   0        0        0     5908 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/2d/src/worklist_gen.pl
--rw-r--r--   0        0        0     3854 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/CMakeLists.txt
--rw-r--r--   0        0        0     2402 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/LICENSE
--rw-r--r--   0        0        0     2614 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/Makefile
--rw-r--r--   0        0        0    21372 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/NEWS
--rw-r--r--   0        0        0     7646 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/README
--rw-r--r--   0        0        0      599 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/config.mk
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/Makefile
--rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/README
--rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/Makefile
--rw-r--r--   0        0        0     2035 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/README
--rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/convex_test.cc
--rw-r--r--   0        0        0     1120 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/import.cc
--rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/import.pov
--rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/mthread.cc
--rw-r--r--   0        0        0    41471 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/pack_ten_cube
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/platonic.cc
--rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/random_points.cc
--rw-r--r--   0        0        0     1041 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/basic/single_cell.cc
--rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/Makefile
--rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/README
--rw-r--r--   0        0        0     1720 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/cell_statistics.cc
--rw-r--r--   0        0        0     1820 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/custom_output.cc
--rw-r--r--   0        0        0      705 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/custom_output.pl
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/custom_output.pov
--rw-r--r--   0        0        0     9281 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube
--rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube.pov
--rw-r--r--   0        0        0     8829 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube_poly
--rw-r--r--   0        0        0      827 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube_poly.pov
--rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/custom/radical.cc
--rw-r--r--   0        0        0      501 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/degenerate/Makefile
--rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/degenerate/README
--rw-r--r--   0        0        0     1216 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/degenerate/degenerate.cc
--rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/degenerate/degenerate.pov
--rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/degenerate/degenerate2.cc
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/degenerate/degenerate2.pov
--rw-r--r--   0        0        0      886 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/Makefile
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/README
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/box_cut.cc
--rw-r--r--   0        0        0     2405 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/cut_region.cc
--rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/irregular.cc
--rw-r--r--   0        0        0      674 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/irregular.pov
--rw-r--r--   0        0        0     2360 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/l_shape.cc
--rw-r--r--   0        0        0     2653 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/pack_irregular
--rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/superellipsoid.cc
--rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/extra/superellipsoid.pov
--rw-r--r--   0        0        0      665 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/Makefile
--rw-r--r--   0        0        0     3055 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/README
--rw-r--r--   0        0        0     3168 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/find_voro_cell.cc
--rw-r--r--   0        0        0     2783 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/loops.cc
--rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/loops.pov
--rw-r--r--   0        0        0     1589 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/odd_even.cc
--rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/odd_even.pov
--rw-r--r--   0        0        0     9281 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/pack_six_cube
--rw-r--r--   0        0        0     3091 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/polygons.cc
--rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/polygons4.pov
--rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/polygons5.pov
--rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/interface/polygons6.pov
--rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/Makefile
--rw-r--r--   0        0        0     2510 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/cylinder_inv.cc
--rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/cylinder_inv.pov
--rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/ellipsoid.cc
--rw-r--r--   0        0        0     3066 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/finite_sys.cc
--rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/finite_sys.pov
--rw-r--r--   0        0        0     1810 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/ghost_test.cc
--rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/import_freeman.cc
--rw-r--r--   0        0        0     1159 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/import_nguyen.cc
--rw-r--r--   0        0        0     1170 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/import_rahman.cc
--rw-r--r--   0        0        0    24646 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/liq-900K.dat
--rw-r--r--   0        0        0     2347 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/lloyd_box.cc
--rw-r--r--   0        0        0     1498 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/minkowski.cc
--rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/neigh_test.cc
--rw-r--r--   0        0        0    59272 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/pack_semicircle
--rw-r--r--   0        0        0     1316 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/period.cc
--rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/polycry.gnuplot
--rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/polycrystal_rahman.cc
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/r_pts_interface.cc
--rw-r--r--   0        0        0     1582 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/rad_test.cc
--rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/rad_test.pl
--rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/rad_test.pov
--rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/random_points_10.cc
--rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/random_points_200.cc
--rw-r--r--   0        0        0      921 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/single_cell_2d.cc
--rw-r--r--   0        0        0     1295 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/sphere.cc
--rw-r--r--   0        0        0     5807 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/sphere_mesh.cc
--rw-r--r--   0        0        0     1118 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/split_cell.cc
--rw-r--r--   0        0        0     2230 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/tri_mesh.cc
--rw-r--r--   0        0        0     2908 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/no_release/voro_lf.cc
--rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/timing/Makefile
--rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/timing/README
--rw-r--r--   0        0        0     3255 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/timing/timing_test.cc
--rw-r--r--   0        0        0      714 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/Makefile
--rw-r--r--   0        0        0     2440 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/README
--rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/cylinder.cc
--rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/cylinder.pov
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/frustum.cc
--rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/frustum.pov
--rw-r--r--   0        0        0   104419 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/pack_cylinder
--rw-r--r--   0        0        0    72457 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/pack_torus
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/tetrahedron.cc
--rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/tetrahedron.pov
--rw-r--r--   0        0        0     4114 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/torus.cc
--rw-r--r--   0        0        0     1005 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/examples/walls/torus.pov
--rw-r--r--   0        0        0    13768 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/man/voro++.1
--rw-r--r--   0        0        0      481 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/scripts/README
--rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/scripts/network.pl
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/scripts/random.pl
--rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/scripts/sum.pl
--rw-r--r--   0        0        0   115286 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/Doxyfile
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/Makefile
--rw-r--r--   0        0        0     2570 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/Makefile.dep
--rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/README
--rw-r--r--   0        0        0      662 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/c_info.hh
--rw-r--r--   0        0        0    21152 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/cell_2d.cc
--rw-r--r--   0        0        0     8339 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/cell_2d.hh
--rw-r--r--   0        0        0    94809 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/cell_3d.cc
--rw-r--r--   0        0        0    27943 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/cell_3d.hh
--rw-r--r--   0        0        0    26418 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/cmd_line.cc
--rw-r--r--   0        0        0     7844 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/common.cc
--rw-r--r--   0        0        0     1163 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/common.hh
--rw-r--r--   0        0        0     5202 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/config.hh
--rw-r--r--   0        0        0    32044 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/container_2d.cc
--rw-r--r--   0        0        0    22210 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/container_2d.hh
--rw-r--r--   0        0        0    35322 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/container_3d.cc
--rw-r--r--   0        0        0    25856 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/container_3d.hh
--rw-r--r--   0        0        0    43736 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/container_tri.cc
--rw-r--r--   0        0        0    27367 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/container_tri.hh
--rw-r--r--   0        0        0    27551 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/iter_2d.cc
--rw-r--r--   0        0        0    17573 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/iter_2d.hh
--rw-r--r--   0        0        0    42836 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/iter_3d.cc
--rw-r--r--   0        0        0    24863 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/iter_3d.hh
--rw-r--r--   0        0        0    10181 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/particle_list.cc
--rw-r--r--   0        0        0     5326 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/particle_list.hh
--rw-r--r--   0        0        0     2835 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/particle_order.hh
--rw-r--r--   0        0        0    11585 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/rad_option.hh
--rw-r--r--   0        0        0     9853 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/unitcell.cc
--rw-r--r--   0        0        0     2691 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/unitcell.hh
--rw-r--r--   0        0        0     3668 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_base_2d.cc
--rw-r--r--   0        0        0     3148 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_base_2d.hh
--rw-r--r--   0        0        0     4501 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_base_3d.cc
--rw-r--r--   0        0        0     3651 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_base_3d.hh
--rw-r--r--   0        0        0     8450 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_base_wl_2d.cc
--rw-r--r--   0        0        0    40357 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_base_wl_3d.cc
--rw-r--r--   0        0        0    32615 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_compute_2d.cc
--rw-r--r--   0        0        0     5044 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_compute_2d.hh
--rw-r--r--   0        0        0    47042 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_compute_3d.cc
--rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/v_compute_3d.hh
--rw-r--r--   0        0        0      587 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/voro++.cc
--rw-r--r--   0        0        0    19971 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/voro++.hh
--rw-r--r--   0        0        0     2672 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/wall.cc
--rw-r--r--   0        0        0     6549 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/wall.hh
--rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/wall_2d.cc
--rw-r--r--   0        0        0     2403 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/wall_2d.hh
--rw-r--r--   0        0        0     5351 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/wall_3d.cc
--rw-r--r--   0        0        0     5061 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/wall_3d.hh
--rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/worklist_2d.hh
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/worklist_3d.hh
--rwxr-xr-x   0        0        0     5930 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/worklist_gen_2d.pl
--rwxr-xr-x   0        0        0     6968 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/src/worklist_gen_3d.pl
--rw-r--r--   0        0        0      765 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/Makefile
--rw-r--r--   0        0        0     1113 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/cp_test.cc
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/cp_test.gnuplot
--rw-r--r--   0        0        0     6089 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/AFX.v1
--rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/BIK.v1
--rw-r--r--   0        0        0      590 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/EDI.v1
--rw-r--r--   0        0        0    11947 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/EMT.v1
--rw-r--r--   0        0        0     4452 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/HEU.v1
--rw-r--r--   0        0        0     4451 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/HV.v1
--rw-r--r--   0        0        0     3945 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/IFR.v1
--rw-r--r--   0        0        0      866 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/JBW.v1
--rw-r--r--   0        0        0     3437 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/P1.v1
--rw-r--r--   0        0        0    11864 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/P2.v1
--rw-r--r--   0        0        0    13418 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/P3.v1
--rw-r--r--   0        0        0    11966 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/P4.v1
--rw-r--r--   0        0        0     1632 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/YUG.v1
--rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/examples/test.v1
--rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/images.cc
--rw-r--r--   0        0        0     5775 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/network.cc
--rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/r_table.cc
--rw-r--r--   0        0        0    17616 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/v_network.cc
--rw-r--r--   0        0        0     3531 2022-11-09 12:37:21.000000 multivoro-0.0.1/ext/voro/zeo/v_network.hh
--rw-r--r--   0        0        0   343881 2022-11-09 12:37:21.000000 multivoro-0.0.1/logo.png
--rw-r--r--   0        0        0     2579 2022-11-09 12:37:21.000000 multivoro-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2801 2022-11-09 12:37:21.000000 multivoro-0.0.1/src/multivoro/__init__.py
--rw-r--r--   0        0        0       99 2022-11-09 12:37:21.000000 multivoro-0.0.1/src/multivoro/exceptions.py
--rw-r--r--   0        0        0     4359 2022-11-09 12:37:21.000000 multivoro-0.0.1/src/multivoro.cpp
--rw-r--r--   0        0        0     1872 2022-11-09 12:37:21.000000 multivoro-0.0.1/tests/test_compute_voronoi.py
--rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 multivoro-0.0.1/tox.ini
--rw-r--r--   0        0        0     3877 2022-11-09 12:37:21.000000 multivoro-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      990 2022-11-09 12:37:21.000000 multivoro-0.1.0/.github/workflows/tox.yml
+-rw-r--r--   0        0        0     1610 2022-11-09 12:37:21.000000 multivoro-0.1.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 multivoro-0.1.0/.gitignore
+-rw-r--r--   0        0        0      215 2022-11-09 12:37:21.000000 multivoro-0.1.0/.gitmodules
+-rw-r--r--   0        0        0     3739 2022-11-09 12:37:21.000000 multivoro-0.1.0/CMakeLists.txt
+-rw-r--r--   0        0        0     2402 2022-11-09 12:37:21.000000 multivoro-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3491 2022-11-09 12:37:21.000000 multivoro-0.1.0/README.rst
+-rwxr-xr-x   0        0        0      435 2022-11-09 12:37:21.000000 multivoro-0.1.0/ci/build_libomp.sh
+-rw-r--r--   0        0        0       36 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/.git
+-rw-r--r--   0        0        0      473 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/Makefile
+-rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/basic/Makefile
+-rw-r--r--   0        0        0      551 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/basic/doe_diagram.cc
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/basic/doe_diagram.pov
+-rw-r--r--   0        0        0     1249 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/basic/import_2d.cc
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/basic/random_points_2d.cc
+-rw-r--r--   0        0        0      909 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/basic/single_cell_2d.cc
+-rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/boundary/Makefile
+-rw-r--r--   0        0        0     1225 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/boundary/annulus.cc
+-rw-r--r--   0        0        0     1209 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/boundary/comb.cc
+-rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/boundary/container_bd.cc
+-rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/boundary/nonconvex_cell.cc
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/extra/Makefile
+-rw-r--r--   0        0        0     1906 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/extra/intersect.cc
+-rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/extra/lloyd.cc
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/extra/lloyd_movie.pl
+-rw-r--r--   0        0        0     1251 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/timing/timing_test_2d.cc
+-rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/walls/Makefile
+-rw-r--r--   0        0        0     1339 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/walls/circle.cc
+-rw-r--r--   0        0        0     1563 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/examples/walls/polygon.cc
+-rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/scripts/network.pl
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/scripts/sum.pl
+-rw-r--r--   0        0        0    72416 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/Doxyfile
+-rw-r--r--   0        0        0      915 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/Makefile
+-rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/Makefile.dep
+-rw-r--r--   0        0        0     4829 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/c_loops_2d.cc
+-rw-r--r--   0        0        0    12191 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/c_loops_2d.hh
+-rw-r--r--   0        0        0    18628 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/cell_2d.cc
+-rw-r--r--   0        0        0     7342 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/cell_2d.hh
+-rw-r--r--   0        0        0     3669 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/cell_nc_2d.cc
+-rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/cell_nc_2d.hh
+-rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/common.cc
+-rw-r--r--   0        0        0     1766 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/common.hh
+-rw-r--r--   0        0        0     3150 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/config.hh
+-rw-r--r--   0        0        0    20929 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/container_2d.cc
+-rw-r--r--   0        0        0    30391 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/container_2d.hh
+-rw-r--r--   0        0        0     8577 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/container_2d_old.hh
+-rw-r--r--   0        0        0     1153 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/cq_test.cc
+-rw-r--r--   0        0        0    21785 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/ctr_boundary_2d.cc
+-rw-r--r--   0        0        0    16956 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/ctr_boundary_2d.hh
+-rw-r--r--   0        0        0     7836 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/ctr_quad_2d.cc
+-rw-r--r--   0        0        0     3489 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/ctr_quad_2d.hh
+-rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/quad_march.cc
+-rw-r--r--   0        0        0      631 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/quad_march.hh
+-rw-r--r--   0        0        0     7421 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/rad_option.hh
+-rw-r--r--   0        0        0     4258 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/v_base_2d.cc
+-rw-r--r--   0        0        0     3539 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/v_base_2d.hh
+-rw-r--r--   0        0        0     8450 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/v_base_wl_2d.cc
+-rw-r--r--   0        0        0    32528 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/v_compute_2d.cc
+-rw-r--r--   0        0        0     5045 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/v_compute_2d.hh
+-rw-r--r--   0        0        0    47351 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/v_connect.cc
+-rw-r--r--   0        0        0    13078 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/v_connect.hh
+-rw-r--r--   0        0        0      223 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/voro++_2d.cc
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/voro++_2d.hh
+-rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/wall_2d.cc
+-rw-r--r--   0        0        0     2403 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/wall_2d.hh
+-rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/worklist_2d.hh
+-rwxr-xr-x   0        0        0     5908 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/2d/src/worklist_gen.pl
+-rw-r--r--   0        0        0     3854 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/CMakeLists.txt
+-rw-r--r--   0        0        0     2402 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/LICENSE
+-rw-r--r--   0        0        0     2614 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/Makefile
+-rw-r--r--   0        0        0    21372 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/NEWS
+-rw-r--r--   0        0        0     7646 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/README
+-rw-r--r--   0        0        0      599 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/config.mk
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/Makefile
+-rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/README
+-rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/Makefile
+-rw-r--r--   0        0        0     2035 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/README
+-rw-r--r--   0        0        0      808 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/convex_test.cc
+-rw-r--r--   0        0        0     1120 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/import.cc
+-rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/import.pov
+-rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/mthread.cc
+-rw-r--r--   0        0        0    41471 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/pack_ten_cube
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/platonic.cc
+-rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/random_points.cc
+-rw-r--r--   0        0        0     1041 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/basic/single_cell.cc
+-rw-r--r--   0        0        0      604 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/Makefile
+-rw-r--r--   0        0        0     1416 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/README
+-rw-r--r--   0        0        0     1720 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/cell_statistics.cc
+-rw-r--r--   0        0        0     1820 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/custom_output.cc
+-rw-r--r--   0        0        0      705 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/custom_output.pl
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/custom_output.pov
+-rw-r--r--   0        0        0     9281 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube
+-rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube.pov
+-rw-r--r--   0        0        0     8829 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube_poly
+-rw-r--r--   0        0        0      827 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube_poly.pov
+-rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/custom/radical.cc
+-rw-r--r--   0        0        0      501 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/degenerate/Makefile
+-rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/degenerate/README
+-rw-r--r--   0        0        0     1216 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/degenerate/degenerate.cc
+-rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/degenerate/degenerate.pov
+-rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/degenerate/degenerate2.cc
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/degenerate/degenerate2.pov
+-rw-r--r--   0        0        0      886 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/Makefile
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/README
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/box_cut.cc
+-rw-r--r--   0        0        0     2405 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/cut_region.cc
+-rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/irregular.cc
+-rw-r--r--   0        0        0      674 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/irregular.pov
+-rw-r--r--   0        0        0     2360 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/l_shape.cc
+-rw-r--r--   0        0        0     2653 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/pack_irregular
+-rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/superellipsoid.cc
+-rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/extra/superellipsoid.pov
+-rw-r--r--   0        0        0      665 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/Makefile
+-rw-r--r--   0        0        0     3055 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/README
+-rw-r--r--   0        0        0     3168 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/find_voro_cell.cc
+-rw-r--r--   0        0        0     2783 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/loops.cc
+-rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/loops.pov
+-rw-r--r--   0        0        0     1589 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/odd_even.cc
+-rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/odd_even.pov
+-rw-r--r--   0        0        0     9281 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/pack_six_cube
+-rw-r--r--   0        0        0     3091 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/polygons.cc
+-rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/polygons4.pov
+-rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/polygons5.pov
+-rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/interface/polygons6.pov
+-rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/Makefile
+-rw-r--r--   0        0        0     2510 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/cylinder_inv.cc
+-rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/cylinder_inv.pov
+-rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/ellipsoid.cc
+-rw-r--r--   0        0        0     3066 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/finite_sys.cc
+-rw-r--r--   0        0        0      603 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/finite_sys.pov
+-rw-r--r--   0        0        0     1810 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/ghost_test.cc
+-rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/import_freeman.cc
+-rw-r--r--   0        0        0     1159 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/import_nguyen.cc
+-rw-r--r--   0        0        0     1170 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/import_rahman.cc
+-rw-r--r--   0        0        0    24646 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/liq-900K.dat
+-rw-r--r--   0        0        0     2347 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/lloyd_box.cc
+-rw-r--r--   0        0        0     1498 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/minkowski.cc
+-rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/neigh_test.cc
+-rw-r--r--   0        0        0    59272 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/pack_semicircle
+-rw-r--r--   0        0        0     1316 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/period.cc
+-rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/polycry.gnuplot
+-rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/polycrystal_rahman.cc
+-rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/r_pts_interface.cc
+-rw-r--r--   0        0        0     1582 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/rad_test.cc
+-rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/rad_test.pl
+-rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/rad_test.pov
+-rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/random_points_10.cc
+-rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/random_points_200.cc
+-rw-r--r--   0        0        0      921 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/single_cell_2d.cc
+-rw-r--r--   0        0        0     1295 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/sphere.cc
+-rw-r--r--   0        0        0     5807 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/sphere_mesh.cc
+-rw-r--r--   0        0        0     1118 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/split_cell.cc
+-rw-r--r--   0        0        0     2230 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/tri_mesh.cc
+-rw-r--r--   0        0        0     2908 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/no_release/voro_lf.cc
+-rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/timing/Makefile
+-rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/timing/README
+-rw-r--r--   0        0        0     3255 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/timing/timing_test.cc
+-rw-r--r--   0        0        0      714 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/Makefile
+-rw-r--r--   0        0        0     2440 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/README
+-rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/cylinder.cc
+-rw-r--r--   0        0        0      749 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/cylinder.pov
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/frustum.cc
+-rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/frustum.pov
+-rw-r--r--   0        0        0   104419 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/pack_cylinder
+-rw-r--r--   0        0        0    72457 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/pack_torus
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/tetrahedron.cc
+-rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/tetrahedron.pov
+-rw-r--r--   0        0        0     4114 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/torus.cc
+-rw-r--r--   0        0        0     1005 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/examples/walls/torus.pov
+-rw-r--r--   0        0        0    13768 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/man/voro++.1
+-rw-r--r--   0        0        0      481 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/scripts/README
+-rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/scripts/network.pl
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/scripts/random.pl
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/scripts/sum.pl
+-rw-r--r--   0        0        0   115286 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/Doxyfile
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/Makefile
+-rw-r--r--   0        0        0     2570 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/Makefile.dep
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/README
+-rw-r--r--   0        0        0      662 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/c_info.hh
+-rw-r--r--   0        0        0    21152 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/cell_2d.cc
+-rw-r--r--   0        0        0     8339 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/cell_2d.hh
+-rw-r--r--   0        0        0    94809 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/cell_3d.cc
+-rw-r--r--   0        0        0    27943 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/cell_3d.hh
+-rw-r--r--   0        0        0    26418 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/cmd_line.cc
+-rw-r--r--   0        0        0     7844 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/common.cc
+-rw-r--r--   0        0        0     1163 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/common.hh
+-rw-r--r--   0        0        0     5202 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/config.hh
+-rw-r--r--   0        0        0    32044 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/container_2d.cc
+-rw-r--r--   0        0        0    22210 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/container_2d.hh
+-rw-r--r--   0        0        0    35322 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/container_3d.cc
+-rw-r--r--   0        0        0    25856 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/container_3d.hh
+-rw-r--r--   0        0        0    43736 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/container_tri.cc
+-rw-r--r--   0        0        0    27367 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/container_tri.hh
+-rw-r--r--   0        0        0    27551 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/iter_2d.cc
+-rw-r--r--   0        0        0    17573 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/iter_2d.hh
+-rw-r--r--   0        0        0    42836 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/iter_3d.cc
+-rw-r--r--   0        0        0    24863 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/iter_3d.hh
+-rw-r--r--   0        0        0    10181 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/particle_list.cc
+-rw-r--r--   0        0        0     5326 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/particle_list.hh
+-rw-r--r--   0        0        0     2835 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/particle_order.hh
+-rw-r--r--   0        0        0    11585 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/rad_option.hh
+-rw-r--r--   0        0        0     9853 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/unitcell.cc
+-rw-r--r--   0        0        0     2691 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/unitcell.hh
+-rw-r--r--   0        0        0     3668 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_base_2d.cc
+-rw-r--r--   0        0        0     3148 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_base_2d.hh
+-rw-r--r--   0        0        0     4501 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_base_3d.cc
+-rw-r--r--   0        0        0     3651 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_base_3d.hh
+-rw-r--r--   0        0        0     8450 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_base_wl_2d.cc
+-rw-r--r--   0        0        0    40357 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_base_wl_3d.cc
+-rw-r--r--   0        0        0    32615 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_compute_2d.cc
+-rw-r--r--   0        0        0     5044 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_compute_2d.hh
+-rw-r--r--   0        0        0    47042 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_compute_3d.cc
+-rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/v_compute_3d.hh
+-rw-r--r--   0        0        0      587 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/voro++.cc
+-rw-r--r--   0        0        0    19971 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/voro++.hh
+-rw-r--r--   0        0        0     2672 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/wall.cc
+-rw-r--r--   0        0        0     6549 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/wall.hh
+-rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/wall_2d.cc
+-rw-r--r--   0        0        0     2403 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/wall_2d.hh
+-rw-r--r--   0        0        0     5351 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/wall_3d.cc
+-rw-r--r--   0        0        0     5061 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/wall_3d.hh
+-rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/worklist_2d.hh
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/worklist_3d.hh
+-rwxr-xr-x   0        0        0     5930 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/worklist_gen_2d.pl
+-rwxr-xr-x   0        0        0     6968 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/src/worklist_gen_3d.pl
+-rw-r--r--   0        0        0      765 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/Makefile
+-rw-r--r--   0        0        0     1113 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/cp_test.cc
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/cp_test.gnuplot
+-rw-r--r--   0        0        0     6089 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/AFX.v1
+-rw-r--r--   0        0        0     1606 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/BIK.v1
+-rw-r--r--   0        0        0      590 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/EDI.v1
+-rw-r--r--   0        0        0    11947 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/EMT.v1
+-rw-r--r--   0        0        0     4452 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/HEU.v1
+-rw-r--r--   0        0        0     4451 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/HV.v1
+-rw-r--r--   0        0        0     3945 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/IFR.v1
+-rw-r--r--   0        0        0      866 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/JBW.v1
+-rw-r--r--   0        0        0     3437 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/P1.v1
+-rw-r--r--   0        0        0    11864 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/P2.v1
+-rw-r--r--   0        0        0    13418 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/P3.v1
+-rw-r--r--   0        0        0    11966 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/P4.v1
+-rw-r--r--   0        0        0     1632 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/YUG.v1
+-rw-r--r--   0        0        0      101 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/examples/test.v1
+-rw-r--r--   0        0        0      638 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/images.cc
+-rw-r--r--   0        0        0     5775 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/network.cc
+-rw-r--r--   0        0        0      497 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/r_table.cc
+-rw-r--r--   0        0        0    17616 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/v_network.cc
+-rw-r--r--   0        0        0     3531 2022-11-09 12:37:21.000000 multivoro-0.1.0/ext/voro/zeo/v_network.hh
+-rw-r--r--   0        0        0   343881 2022-11-09 12:37:21.000000 multivoro-0.1.0/logo.png
+-rw-r--r--   0        0        0     2712 2022-11-09 12:37:21.000000 multivoro-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2801 2022-11-09 12:37:21.000000 multivoro-0.1.0/src/multivoro/__init__.py
+-rw-r--r--   0        0        0       99 2022-11-09 12:37:21.000000 multivoro-0.1.0/src/multivoro/exceptions.py
+-rw-r--r--   0        0        0     4316 2022-11-09 12:37:21.000000 multivoro-0.1.0/src/multivoro.cpp
+-rw-r--r--   0        0        0     6035 2022-11-09 12:37:21.000000 multivoro-0.1.0/tests/test_compute_voronoi.py
+-rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 multivoro-0.1.0/tox.ini
+-rw-r--r--   0        0        0     4302 2022-11-09 12:37:21.000000 multivoro-0.1.0/PKG-INFO
```

### Comparing `multivoro-0.0.1/.github/workflows/run-tox.yml` & `multivoro-0.1.0/.github/workflows/tox.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-name: Tox
+name: tox
 
 on:
   workflow_dispatch:
   pull_request:
   push:
     branches:
       - main
   release:
     types:
       - published
+  schedule:
+    - cron: '0 0 * * *'
 
 jobs:
-  tox_checks:
+  checks:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
+        openmp-mode: ['ON', 'OFF']
 
     steps:
 
     - uses: actions/checkout@v4
       with:
         submodules: true
 
@@ -32,7 +35,15 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox-gh-actions
 
     - name: Run tox
       run: tox
+      env:
+        USE_OpenMP: ${{ matrix.openmp-mode }}
+
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v4.0.1
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
+        slug: eleftherioszisis/multivoro
```

### Comparing `multivoro-0.0.1/.github/workflows/wheels.yml` & `multivoro-0.1.0/.github/workflows/wheels.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-name: Wheels
+name: wheels
 
 on:
   workflow_dispatch:
   pull_request:
   push:
     branches:
      - main
   release:
     types:
       - published
 
 jobs:
 
   build_wheels:
-    name: Wheels on ${{ matrix.os }}
+    name: wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-latest]
+        os: [ubuntu-20.04, macos-13, macos-14]
 
     steps:
     - uses: actions/checkout@v4
       with:
         submodules: true
 
     - uses: pypa/cibuildwheel@v2.17
@@ -34,15 +34,15 @@
     - name: Upload wheels
       uses: actions/upload-artifact@v4
       with:
         path: wheelhouse/*.whl
         name: cibw-wheels-${{ matrix.os }}-${{ strategy.job-index }}
 
   build_sdist:
-    name: Build SDist
+    name: build sdist
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
       with:
         submodules: true
 
     - name: Build SDist
```

### Comparing `multivoro-0.0.1/.gitignore` & `multivoro-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/CMakeLists.txt` & `multivoro-0.1.0/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,31 +31,35 @@
    $ pip install --no-build-isolation -ve .
   =====================================================================
   You may optionally add -Ceditable.rebuild=true to auto-rebuild when
   the package is imported. Otherwise, you need to rerun the above
   after editing C++ files.")
 endif()
 
+set(CMAKE_CXX_STANDARD 17)
+set(CMAKE_CXX_STANDARD_REQUIRED ON)
+
 # Try to import all Python components potentially needed by nanobind
 find_package(Python 3.8
   REQUIRED COMPONENTS Interpreter Development.Module
   OPTIONAL_COMPONENTS Development.SABIModule)
 
 # Import nanobind through CMake's find_package mechanism
 find_package(nanobind CONFIG REQUIRED)
 
-# Import OpenMP
-find_package(OpenMP)
+OPTION(USE_OpenMP "Use OpenMP" OFF)
 
-if (OPENMP_FOUND)
+if (USE_OpenMP)
+  find_package(OpenMP REQUIRED)
   set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
   set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
   set (CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} ${OpenMP_EXE_LINKER_FLAGS}")
+  message(WARNING "OpenMP option is enabled. Compilation will proceed with multihreading support.")
 else()
-  message(WARNING "OpenMP was not found. Compilation will proceed without multihreading support.")
+  message(WARNING "OpenMP option is disabled. Compilation will proceed without multihreading support.")
 endif()
 
 set(
     VORO_SOURCES
     ext/voro/src/cell_2d.cc
     ext/voro/src/cell_3d.cc
     ext/voro/src/common.cc
@@ -95,11 +99,13 @@
 
 target_include_directories(
     _multivoro
     PRIVATE
     ext/voro/src
 )
 
-target_link_libraries(_multivoro PRIVATE ${OpenMP_CXX_FLAGS})
+if (USE_OpenMP)
+  target_link_libraries(_multivoro PRIVATE ${OpenMP_CXX_FLAGS})
+endif()
 
 # Install directive for scikit-build-core
 install(TARGETS _multivoro LIBRARY DESTINATION multivoro)
```

### Comparing `multivoro-0.0.1/LICENSE` & `multivoro-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/README.rst` & `multivoro-0.1.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,70 @@
-.. image:: logo.png
+.. image:: https://github.com/eleftherioszisis/multivoro/blob/main/logo.png
 
 Parallel cell-based 3D voronoi tessellations
 --------------------------------------------
 
-
 multivoro is a python library that allows building 3D Voronoi/Laguerre tessellations with `voro++ <voro_site_>`_ exposed in python via the nanobind_ library.
 It leverages the latest `multi-threaded extension of Voro++ <voro_mthread_>`_ to allow computing the voronoi cells in parallel.
 
 Codebases
 ---------
 * `Voro++ <voro_repo_>`_
 * nanobind_
 
 Installation
 ------------
 
-If one is on a Linux platform, one should be able to use the compiled Python wheels.
-This is the recommended way.
+Wheels
+~~~~~~
+There are available pre-compiled wheels to pip install for Linux and macOS.
+However, note that these wheels are compiled without multithreading support.
+
+To install them in your system:
 
 .. code-block:: bash
 
   pip install multivoro
 
+Source
+~~~~~~
 To build multivoro from source in Ubuntu:
 
+Setup a python virtual environment:
+
 .. code-block:: bash
 
    # python versions to choose from: [python3.8-python3.12]
-   sudo apt install openmp python3.10-dev python3.10-venv
+   sudo apt install python3.10-dev python3.10-venv
+   python3.10 -mvenv venv
+   source ./venv/bin/activate
+
+Install openmp runtime and compile the wheel:
+
+.. code-block:: bash
+
+   sudo apt install libomp-dev
    git clone --recurse-submodules https://github.com/eleftherioszisis/multivoro.git
-   python3.10 -mvenv venv && source ./venv/bin/activate
-   cd multivoro && pip install .
+   cd multivoro
+   USE_OpenMP=ON pip install .
+
+USE_OpenMP environment variable is used as an option in multivoro cmake. By default it is set to 'OFF'.
 
 Usage
 -----
 
 .. code-block:: python
 
    from multivoro import compute_voronoi
 
    cells = compute_voronoi(
        points=[[-1.0, 0.0, 0.0], [1.0, 0.0, 0.0]],
        radii=[1.0, 1.0],
        limits=[[-2.0, -1.0, -1.0], [2.0, 1.0, 1.0]],
+       n_threads=6,
    )
 
    for cell in cells:
        print(cell.get_vertices())
        print(cell.get_neighbors())
        print(cell.get_face_vertices())
```

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/basic/Makefile` & `multivoro-0.1.0/ext/voro/2d/examples/basic/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/basic/doe_diagram.cc` & `multivoro-0.1.0/ext/voro/2d/examples/basic/doe_diagram.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/basic/doe_diagram.pov` & `multivoro-0.1.0/ext/voro/2d/examples/basic/doe_diagram.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/basic/import_2d.cc` & `multivoro-0.1.0/ext/voro/2d/examples/basic/import_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/basic/random_points_2d.cc` & `multivoro-0.1.0/ext/voro/2d/examples/basic/random_points_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/basic/single_cell_2d.cc` & `multivoro-0.1.0/ext/voro/2d/examples/basic/single_cell_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/boundary/Makefile` & `multivoro-0.1.0/ext/voro/2d/examples/boundary/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/boundary/annulus.cc` & `multivoro-0.1.0/ext/voro/2d/examples/boundary/annulus.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/boundary/comb.cc` & `multivoro-0.1.0/ext/voro/2d/examples/boundary/comb.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/boundary/container_bd.cc` & `multivoro-0.1.0/ext/voro/2d/examples/boundary/container_bd.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/boundary/nonconvex_cell.cc` & `multivoro-0.1.0/ext/voro/2d/examples/boundary/nonconvex_cell.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/extra/intersect.cc` & `multivoro-0.1.0/ext/voro/2d/examples/extra/intersect.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/extra/lloyd.cc` & `multivoro-0.1.0/ext/voro/2d/examples/extra/lloyd.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/timing/timing_test_2d.cc` & `multivoro-0.1.0/ext/voro/2d/examples/timing/timing_test_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/walls/circle.cc` & `multivoro-0.1.0/ext/voro/2d/examples/walls/circle.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/examples/walls/polygon.cc` & `multivoro-0.1.0/ext/voro/2d/examples/walls/polygon.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/scripts/network.pl` & `multivoro-0.1.0/ext/voro/2d/scripts/network.pl`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/Doxyfile` & `multivoro-0.1.0/ext/voro/2d/src/Doxyfile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/Makefile` & `multivoro-0.1.0/ext/voro/2d/src/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/Makefile.dep` & `multivoro-0.1.0/ext/voro/2d/src/Makefile.dep`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/c_loops_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/c_loops_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/c_loops_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/c_loops_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/cell_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/cell_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/cell_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/cell_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/cell_nc_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/cell_nc_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/cell_nc_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/cell_nc_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/common.cc` & `multivoro-0.1.0/ext/voro/2d/src/common.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/common.hh` & `multivoro-0.1.0/ext/voro/2d/src/common.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/config.hh` & `multivoro-0.1.0/ext/voro/2d/src/config.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/container_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/container_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/container_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/container_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/container_2d_old.hh` & `multivoro-0.1.0/ext/voro/2d/src/container_2d_old.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/cq_test.cc` & `multivoro-0.1.0/ext/voro/2d/src/cq_test.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/ctr_boundary_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/ctr_boundary_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/ctr_boundary_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/ctr_boundary_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/ctr_quad_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/ctr_quad_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/ctr_quad_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/ctr_quad_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/quad_march.cc` & `multivoro-0.1.0/ext/voro/2d/src/quad_march.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/quad_march.hh` & `multivoro-0.1.0/ext/voro/2d/src/quad_march.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/rad_option.hh` & `multivoro-0.1.0/ext/voro/2d/src/rad_option.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/v_base_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/v_base_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/v_base_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/v_base_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/v_base_wl_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/v_base_wl_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/v_compute_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/v_compute_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/v_compute_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/v_compute_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/v_connect.cc` & `multivoro-0.1.0/ext/voro/2d/src/v_connect.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/v_connect.hh` & `multivoro-0.1.0/ext/voro/2d/src/v_connect.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/wall_2d.cc` & `multivoro-0.1.0/ext/voro/2d/src/wall_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/wall_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/wall_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/worklist_2d.hh` & `multivoro-0.1.0/ext/voro/2d/src/worklist_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/2d/src/worklist_gen.pl` & `multivoro-0.1.0/ext/voro/2d/src/worklist_gen.pl`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/CMakeLists.txt` & `multivoro-0.1.0/ext/voro/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/LICENSE` & `multivoro-0.1.0/ext/voro/LICENSE`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/Makefile` & `multivoro-0.1.0/ext/voro/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/NEWS` & `multivoro-0.1.0/ext/voro/NEWS`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/README` & `multivoro-0.1.0/ext/voro/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/config.mk` & `multivoro-0.1.0/ext/voro/config.mk`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/Makefile` & `multivoro-0.1.0/ext/voro/examples/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/README` & `multivoro-0.1.0/ext/voro/examples/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/Makefile` & `multivoro-0.1.0/ext/voro/examples/basic/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/README` & `multivoro-0.1.0/ext/voro/examples/basic/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/convex_test.cc` & `multivoro-0.1.0/ext/voro/examples/basic/convex_test.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/import.cc` & `multivoro-0.1.0/ext/voro/examples/basic/import.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/import.pov` & `multivoro-0.1.0/ext/voro/examples/basic/import.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/mthread.cc` & `multivoro-0.1.0/ext/voro/examples/basic/mthread.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/pack_ten_cube` & `multivoro-0.1.0/ext/voro/examples/basic/pack_ten_cube`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/platonic.cc` & `multivoro-0.1.0/ext/voro/examples/basic/platonic.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/random_points.cc` & `multivoro-0.1.0/ext/voro/examples/basic/random_points.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/basic/single_cell.cc` & `multivoro-0.1.0/ext/voro/examples/basic/single_cell.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/Makefile` & `multivoro-0.1.0/ext/voro/examples/custom/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/README` & `multivoro-0.1.0/ext/voro/examples/custom/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/cell_statistics.cc` & `multivoro-0.1.0/ext/voro/examples/custom/cell_statistics.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/custom_output.cc` & `multivoro-0.1.0/ext/voro/examples/custom/custom_output.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/custom_output.pl` & `multivoro-0.1.0/ext/voro/examples/custom/custom_output.pl`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/custom_output.pov` & `multivoro-0.1.0/ext/voro/examples/custom/custom_output.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube` & `multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube.pov` & `multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube_poly` & `multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube_poly`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/pack_six_cube_poly.pov` & `multivoro-0.1.0/ext/voro/examples/custom/pack_six_cube_poly.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/custom/radical.cc` & `multivoro-0.1.0/ext/voro/examples/custom/radical.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/degenerate/README` & `multivoro-0.1.0/ext/voro/examples/degenerate/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/degenerate/degenerate.cc` & `multivoro-0.1.0/ext/voro/examples/degenerate/degenerate.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/degenerate/degenerate.pov` & `multivoro-0.1.0/ext/voro/examples/degenerate/degenerate.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/degenerate/degenerate2.cc` & `multivoro-0.1.0/ext/voro/examples/degenerate/degenerate2.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/degenerate/degenerate2.pov` & `multivoro-0.1.0/ext/voro/examples/degenerate/degenerate2.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/Makefile` & `multivoro-0.1.0/ext/voro/examples/extra/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/README` & `multivoro-0.1.0/ext/voro/examples/extra/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/box_cut.cc` & `multivoro-0.1.0/ext/voro/examples/extra/box_cut.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/cut_region.cc` & `multivoro-0.1.0/ext/voro/examples/extra/cut_region.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/irregular.cc` & `multivoro-0.1.0/ext/voro/examples/extra/irregular.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/irregular.pov` & `multivoro-0.1.0/ext/voro/examples/extra/irregular.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/l_shape.cc` & `multivoro-0.1.0/ext/voro/examples/extra/l_shape.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/pack_irregular` & `multivoro-0.1.0/ext/voro/examples/extra/pack_irregular`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/extra/superellipsoid.cc` & `multivoro-0.1.0/ext/voro/examples/extra/superellipsoid.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/Makefile` & `multivoro-0.1.0/ext/voro/examples/interface/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/README` & `multivoro-0.1.0/ext/voro/examples/interface/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/find_voro_cell.cc` & `multivoro-0.1.0/ext/voro/examples/interface/find_voro_cell.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/loops.cc` & `multivoro-0.1.0/ext/voro/examples/interface/loops.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/loops.pov` & `multivoro-0.1.0/ext/voro/examples/interface/loops.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/odd_even.cc` & `multivoro-0.1.0/ext/voro/examples/interface/odd_even.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/odd_even.pov` & `multivoro-0.1.0/ext/voro/examples/interface/odd_even.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/pack_six_cube` & `multivoro-0.1.0/ext/voro/examples/interface/pack_six_cube`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/polygons.cc` & `multivoro-0.1.0/ext/voro/examples/interface/polygons.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/polygons4.pov` & `multivoro-0.1.0/ext/voro/examples/interface/polygons4.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/polygons5.pov` & `multivoro-0.1.0/ext/voro/examples/interface/polygons5.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/interface/polygons6.pov` & `multivoro-0.1.0/ext/voro/examples/interface/polygons6.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/Makefile` & `multivoro-0.1.0/ext/voro/examples/no_release/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/cylinder_inv.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/cylinder_inv.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/cylinder_inv.pov` & `multivoro-0.1.0/ext/voro/examples/no_release/cylinder_inv.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/ellipsoid.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/ellipsoid.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/finite_sys.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/finite_sys.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/finite_sys.pov` & `multivoro-0.1.0/ext/voro/examples/no_release/finite_sys.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/ghost_test.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/ghost_test.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/import_freeman.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/import_freeman.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/import_nguyen.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/import_nguyen.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/import_rahman.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/import_rahman.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/liq-900K.dat` & `multivoro-0.1.0/ext/voro/examples/no_release/liq-900K.dat`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/lloyd_box.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/lloyd_box.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/minkowski.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/minkowski.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/neigh_test.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/neigh_test.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/pack_semicircle` & `multivoro-0.1.0/ext/voro/examples/no_release/pack_semicircle`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/period.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/period.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/polycrystal_rahman.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/polycrystal_rahman.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/r_pts_interface.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/r_pts_interface.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/rad_test.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/rad_test.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/rad_test.pov` & `multivoro-0.1.0/ext/voro/examples/no_release/rad_test.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/random_points_10.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/random_points_10.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/random_points_200.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/random_points_200.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/single_cell_2d.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/single_cell_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/sphere.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/sphere.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/sphere_mesh.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/sphere_mesh.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/split_cell.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/split_cell.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/tri_mesh.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/tri_mesh.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/no_release/voro_lf.cc` & `multivoro-0.1.0/ext/voro/examples/no_release/voro_lf.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/timing/README` & `multivoro-0.1.0/ext/voro/examples/timing/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/timing/timing_test.cc` & `multivoro-0.1.0/ext/voro/examples/timing/timing_test.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/Makefile` & `multivoro-0.1.0/ext/voro/examples/walls/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/README` & `multivoro-0.1.0/ext/voro/examples/walls/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/cylinder.cc` & `multivoro-0.1.0/ext/voro/examples/walls/cylinder.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/cylinder.pov` & `multivoro-0.1.0/ext/voro/examples/walls/cylinder.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/frustum.cc` & `multivoro-0.1.0/ext/voro/examples/walls/frustum.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/frustum.pov` & `multivoro-0.1.0/ext/voro/examples/walls/frustum.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/pack_cylinder` & `multivoro-0.1.0/ext/voro/examples/walls/pack_cylinder`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/pack_torus` & `multivoro-0.1.0/ext/voro/examples/walls/pack_torus`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/tetrahedron.cc` & `multivoro-0.1.0/ext/voro/examples/walls/tetrahedron.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/tetrahedron.pov` & `multivoro-0.1.0/ext/voro/examples/walls/tetrahedron.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/torus.cc` & `multivoro-0.1.0/ext/voro/examples/walls/torus.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/examples/walls/torus.pov` & `multivoro-0.1.0/ext/voro/examples/walls/torus.pov`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/man/voro++.1` & `multivoro-0.1.0/ext/voro/man/voro++.1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/scripts/network.pl` & `multivoro-0.1.0/ext/voro/scripts/network.pl`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/scripts/random.pl` & `multivoro-0.1.0/ext/voro/scripts/random.pl`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/Doxyfile` & `multivoro-0.1.0/ext/voro/src/Doxyfile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/Makefile` & `multivoro-0.1.0/ext/voro/src/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/Makefile.dep` & `multivoro-0.1.0/ext/voro/src/Makefile.dep`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/README` & `multivoro-0.1.0/ext/voro/src/README`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/c_info.hh` & `multivoro-0.1.0/ext/voro/src/c_info.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/cell_2d.cc` & `multivoro-0.1.0/ext/voro/src/cell_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/cell_2d.hh` & `multivoro-0.1.0/ext/voro/src/cell_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/cell_3d.cc` & `multivoro-0.1.0/ext/voro/src/cell_3d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/cell_3d.hh` & `multivoro-0.1.0/ext/voro/src/cell_3d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/cmd_line.cc` & `multivoro-0.1.0/ext/voro/src/cmd_line.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/common.cc` & `multivoro-0.1.0/ext/voro/src/common.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/common.hh` & `multivoro-0.1.0/ext/voro/src/common.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/config.hh` & `multivoro-0.1.0/ext/voro/src/config.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/container_2d.cc` & `multivoro-0.1.0/ext/voro/src/container_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/container_2d.hh` & `multivoro-0.1.0/ext/voro/src/container_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/container_3d.cc` & `multivoro-0.1.0/ext/voro/src/container_3d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/container_3d.hh` & `multivoro-0.1.0/ext/voro/src/container_3d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/container_tri.cc` & `multivoro-0.1.0/ext/voro/src/container_tri.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/container_tri.hh` & `multivoro-0.1.0/ext/voro/src/container_tri.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/iter_2d.cc` & `multivoro-0.1.0/ext/voro/src/iter_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/iter_2d.hh` & `multivoro-0.1.0/ext/voro/src/iter_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/iter_3d.cc` & `multivoro-0.1.0/ext/voro/src/iter_3d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/iter_3d.hh` & `multivoro-0.1.0/ext/voro/src/iter_3d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/particle_list.cc` & `multivoro-0.1.0/ext/voro/src/particle_list.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/particle_list.hh` & `multivoro-0.1.0/ext/voro/src/particle_list.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/particle_order.hh` & `multivoro-0.1.0/ext/voro/src/particle_order.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/rad_option.hh` & `multivoro-0.1.0/ext/voro/src/rad_option.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/unitcell.cc` & `multivoro-0.1.0/ext/voro/src/unitcell.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/unitcell.hh` & `multivoro-0.1.0/ext/voro/src/unitcell.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_base_2d.cc` & `multivoro-0.1.0/ext/voro/src/v_base_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_base_2d.hh` & `multivoro-0.1.0/ext/voro/src/v_base_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_base_3d.cc` & `multivoro-0.1.0/ext/voro/src/v_base_3d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_base_3d.hh` & `multivoro-0.1.0/ext/voro/src/v_base_3d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_base_wl_2d.cc` & `multivoro-0.1.0/ext/voro/src/v_base_wl_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_base_wl_3d.cc` & `multivoro-0.1.0/ext/voro/src/v_base_wl_3d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_compute_2d.cc` & `multivoro-0.1.0/ext/voro/src/v_compute_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_compute_2d.hh` & `multivoro-0.1.0/ext/voro/src/v_compute_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_compute_3d.cc` & `multivoro-0.1.0/ext/voro/src/v_compute_3d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/v_compute_3d.hh` & `multivoro-0.1.0/ext/voro/src/v_compute_3d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/voro++.cc` & `multivoro-0.1.0/ext/voro/src/voro++.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/voro++.hh` & `multivoro-0.1.0/ext/voro/src/voro++.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/wall.cc` & `multivoro-0.1.0/ext/voro/src/wall.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/wall.hh` & `multivoro-0.1.0/ext/voro/src/wall.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/wall_2d.cc` & `multivoro-0.1.0/ext/voro/src/wall_2d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/wall_2d.hh` & `multivoro-0.1.0/ext/voro/src/wall_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/wall_3d.cc` & `multivoro-0.1.0/ext/voro/src/wall_3d.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/wall_3d.hh` & `multivoro-0.1.0/ext/voro/src/wall_3d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/worklist_2d.hh` & `multivoro-0.1.0/ext/voro/src/worklist_2d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/worklist_3d.hh` & `multivoro-0.1.0/ext/voro/src/worklist_3d.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/worklist_gen_2d.pl` & `multivoro-0.1.0/ext/voro/src/worklist_gen_2d.pl`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/src/worklist_gen_3d.pl` & `multivoro-0.1.0/ext/voro/src/worklist_gen_3d.pl`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/Makefile` & `multivoro-0.1.0/ext/voro/zeo/Makefile`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/cp_test.cc` & `multivoro-0.1.0/ext/voro/zeo/cp_test.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/AFX.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/AFX.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/BIK.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/BIK.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/EDI.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/EDI.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/EMT.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/EMT.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/HEU.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/HEU.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/HV.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/HV.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/IFR.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/IFR.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/JBW.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/JBW.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/P1.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/P1.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/P2.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/P2.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/P3.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/P3.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/P4.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/P4.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/examples/YUG.v1` & `multivoro-0.1.0/ext/voro/zeo/examples/YUG.v1`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/images.cc` & `multivoro-0.1.0/ext/voro/zeo/images.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/network.cc` & `multivoro-0.1.0/ext/voro/zeo/network.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/v_network.cc` & `multivoro-0.1.0/ext/voro/zeo/v_network.cc`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/ext/voro/zeo/v_network.hh` & `multivoro-0.1.0/ext/voro/zeo/v_network.hh`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/logo.png` & `multivoro-0.1.0/logo.png`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/pyproject.toml` & `multivoro-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core>= 0.4.3", "nanobind>=1.3.2"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "multivoro"
-version = "0.0.1"
+version = "0.1.0"
 description = "Parallel cell-based 3D voronoi tessellations"
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
     { name = "Eleftherios Zisis", email = "elef.zisis@gmail.com" },
 ]
 dependencies=[
@@ -39,14 +39,20 @@
 
 # Setuptools-style build caching in a local directory
 build-dir = "build/{wheel_tag}"
 
 # Build stable ABI wheels for CPython 3.12+
 wheel.py-api = "cp312"
 
+# Specify build type
+cmake.build-type = "Release"
+
+[tool.scikit-build.cmake.define]
+USE_OpenMP = {env="USE_OpenMP", default="OFF"}
+
 [tool.cibuildwheel]
 # Necessary to see build output from the actual compilation
 build-verbosity = 1
 
 # Optional: run pytest to ensure that the package was correctly built
 test-command = "pytest {project}/tests"
 test-requires = "pytest"
@@ -55,14 +61,15 @@
 skip = ["pp*", "*musllinux*"]
 archs = ["auto64"]
 
 # Needed for full C++17 support on macOS
 [tool.cibuildwheel.macos.environment]
 MACOSX_DEPLOYMENT_TARGET = "10.14"
 
+
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 
 [tool.ruff.lint]
 select = [
     "A", # flake8-builtins
```

### Comparing `multivoro-0.0.1/src/multivoro/__init__.py` & `multivoro-0.1.0/src/multivoro/__init__.py`

 * *Files identical despite different names*

### Comparing `multivoro-0.0.1/src/multivoro.cpp` & `multivoro-0.1.0/src/multivoro.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #include <vector>
-#include <iostream>
 #include <sstream>
-#include <iterator>
 #include <nanobind/nanobind.h>
 #include <nanobind/ndarray.h>
 #include <nanobind/stl/vector.h>
 
 #include "voro++.hh"
 
 #ifdef _OPENMP
     #include <omp.h>
 #endif
 
 namespace nb = nanobind;
 
+
 using IntVector = std::vector<int>;
 using DoubleVector = std::vector<double>;
 
 struct Cell {
     IntVector neighbors;
     IntVector face_vertices;
     DoubleVector vertices;
@@ -62,15 +61,15 @@
 #endif
         );
 
     // populate container with points
     for (int i = 0; i < n_cells; ++i) {
 
         const bool is_inside_container = container.point_inside(v_points(i, 0), v_points(i, 1), v_points(i, 2));
-        if (not is_inside_container){
+        if (!is_inside_container){
             throw nb::value_error("Points outside container walls.");
         }
 
         container.put(i, v_points(i, 0), v_points(i, 1), v_points(i, 2), v_radii(i));
     }
 
     CellVector cells(n_cells);
@@ -103,15 +102,14 @@
         impl_cell.neighbors(cell.neighbors);
         impl_cell.face_vertices(cell.face_vertices);
     }
 
     return cells;
 }
 
-
 NB_MODULE(_multivoro, m) {
 
     nb::class_<Cell>(m, "Cell")
         .def(nb::init<>())
         .def(
             "get_vertices",
             [](Cell& self){
```

### Comparing `multivoro-0.0.1/tox.ini` & `multivoro-0.1.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -11,36 +11,49 @@
     lint
     docs
     coverage
     check-packaging
     py{38,39,310,311,312}
 
 [testenv]
-deps = {[base]testdeps}
-commands = pytest {posargs}
+passenv = USE_OpenMP
+deps =
+  {[base]testdeps}
+  pytest-cov
+commands = pytest \
+                --cov={envsitepackagesdir}/{[base]name} \
+                --cov-report term-missing \
+                --cov-fail-under=80 \
+                --cov-report=xml \
+                --no-cov-on-fail \
+                {posargs}
 
 [testenv:lint]
 deps =
     ruff
 commands =
-    ruff format --check {[base]path}
+    ruff format --check {[base]path} tests/
     ruff check {[base]path}
 
 [testenv:format]
 deps =
     ruff
 commands =
-    ruff check --fix --select I {[base]path}
-    ruff format {[base]path}
+    ruff check --fix --select I {[base]path} tests/
+    ruff format {[base]path} tests/
 
 [testenv:check-packaging]
 skip_install = true
 deps =
     build
     twine
 commands =
     python -m build -o {envtmpdir}/dist
     twine check {envtmpdir}/dist/*
 
 [gh-actions]
 python =
-  3.11: lint, check-packaging
+  3.8: py38
+  3.9: py39
+  3.10: py310, check-packaging
+  3.11: py311, lint
+  3.12: py312
```

### Comparing `multivoro-0.0.1/PKG-INFO` & `multivoro-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multivoro
-Version: 0.0.1
+Version: 0.1.0
 Summary: Parallel cell-based 3D voronoi tessellations
 Author-Email: Eleftherios Zisis <elef.zisis@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,59 +14,77 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Project-URL: Homepage, https://github.com/eleftherioszisis/multivoro
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Description-Content-Type: text/x-rst
 
-.. image:: logo.png
+.. image:: https://github.com/eleftherioszisis/multivoro/blob/main/logo.png
 
 Parallel cell-based 3D voronoi tessellations
 --------------------------------------------
 
-
 multivoro is a python library that allows building 3D Voronoi/Laguerre tessellations with `voro++ <voro_site_>`_ exposed in python via the nanobind_ library.
 It leverages the latest `multi-threaded extension of Voro++ <voro_mthread_>`_ to allow computing the voronoi cells in parallel.
 
 Codebases
 ---------
 * `Voro++ <voro_repo_>`_
 * nanobind_
 
 Installation
 ------------
 
-If one is on a Linux platform, one should be able to use the compiled Python wheels.
-This is the recommended way.
+Wheels
+~~~~~~
+There are available pre-compiled wheels to pip install for Linux and macOS.
+However, note that these wheels are compiled without multithreading support.
+
+To install them in your system:
 
 .. code-block:: bash
 
   pip install multivoro
 
+Source
+~~~~~~
 To build multivoro from source in Ubuntu:
 
+Setup a python virtual environment:
+
 .. code-block:: bash
 
    # python versions to choose from: [python3.8-python3.12]
-   sudo apt install openmp python3.10-dev python3.10-venv
+   sudo apt install python3.10-dev python3.10-venv
+   python3.10 -mvenv venv
+   source ./venv/bin/activate
+
+Install openmp runtime and compile the wheel:
+
+.. code-block:: bash
+
+   sudo apt install libomp-dev
    git clone --recurse-submodules https://github.com/eleftherioszisis/multivoro.git
-   python3.10 -mvenv venv && source ./venv/bin/activate
-   cd multivoro && pip install .
+   cd multivoro
+   USE_OpenMP=ON pip install .
+
+USE_OpenMP environment variable is used as an option in multivoro cmake. By default it is set to 'OFF'.
 
 Usage
 -----
 
 .. code-block:: python
 
    from multivoro import compute_voronoi
 
    cells = compute_voronoi(
        points=[[-1.0, 0.0, 0.0], [1.0, 0.0, 0.0]],
        radii=[1.0, 1.0],
        limits=[[-2.0, -1.0, -1.0], [2.0, 1.0, 1.0]],
+       n_threads=6,
    )
 
    for cell in cells:
        print(cell.get_vertices())
        print(cell.get_neighbors())
        print(cell.get_face_vertices())
```

