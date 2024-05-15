# Comparing `tmp/Wake-T-0.7.1.tar.gz` & `tmp/wake_t-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wake-T-0.7.1.tar", last modified: Tue Oct 17 13:17:26 2023, max compression
+gzip compressed data, was "wake_t-0.8.0.tar", last modified: Wed May 15 15:38:30 2024, max compression
```

## Comparing `Wake-T-0.7.1.tar` & `wake_t-0.8.0.tar`

### file list

```diff
@@ -1,114 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.221291 Wake-T-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-10-17 13:17:15.000000 Wake-T-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-10-17 13:17:26.221291 Wake-T-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-10-17 13:17:15.000000 Wake-T-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.185290 Wake-T-0.7.1/Wake_T.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-10-17 13:17:26.000000 Wake-T-0.7.1/Wake_T.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2023-10-17 13:17:26.000000 Wake-T-0.7.1/Wake_T.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 13:17:26.000000 Wake-T-0.7.1/Wake_T.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-10-17 13:17:26.000000 Wake-T-0.7.1/Wake_T.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-17 13:17:26.000000 Wake-T-0.7.1/Wake_T.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-17 13:17:15.000000 Wake-T-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-10-17 13:17:26.221291 Wake-T-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-17 13:17:15.000000 Wake-T-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.193290 Wake-T-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_active_plasma_lens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_beam_deposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_beamline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_bunch_read_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_custom_blowout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_field_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_field_gathering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_fluid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_laser_envelope_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_laser_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_multibunch.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_no_bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_openpmd_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_parabolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_particle_bunch_species.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_plasma_beamline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_plasma_deposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_ramps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_sc_baxevanis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2023-10-17 13:17:15.000000 Wake-T-0.7.1/tests/test_simple_blowout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.193290 Wake-T-0.7.1/wake_t/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.193290 Wake-T-0.7.1/wake_t/beamline_elements/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/beamline_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/beamline_elements/active_plasma_lens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/beamline_elements/beamline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/beamline_elements/field_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/beamline_elements/plasma_ramp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/beamline_elements/plasma_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16114 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/beamline_elements/tm_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.197290 Wake-T-0.7.1/wake_t/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/diagnostics/bunch_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/diagnostics/openpmd_diag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.197290 Wake-T-0.7.1/wake_t/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/fields/analytical_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/fields/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/fields/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/fields/numerical_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/fields/rz_wakefield.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.201290 Wake-T-0.7.1/wake_t/particles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/deposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/particle_bunch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.201290 Wake-T-0.7.1/wake_t/particles/push/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/push/boris_pusher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/push/runge_kutta_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/particles/push/transfer_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.201290 Wake-T-0.7.1/wake_t/physics_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.205290 Wake-T-0.7.1/wake_t/physics_models/beam_optics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/beam_optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/beam_optics/transfer_matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.205290 Wake-T-0.7.1/wake_t/physics_models/collective_effects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/collective_effects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15619 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/collective_effects/csr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.205290 Wake-T-0.7.1/wake_t/physics_models/em_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/em_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/em_fields/linear_b_theta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.209291 Wake-T-0.7.1/wake_t/physics_models/laser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/laser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/laser/envelope_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/laser/envelope_solver_non_centered.py
--rw-r--r--   0 runner    (1001) docker     (127)    25873 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/laser/laser_pulse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/laser/tdma.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.209291 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/custom_blowout.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/focusing_blowout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/from_pic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.213291 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15900 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.217290 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)    19861 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/simple_blowout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.217290 Wake-T-0.7.1/wake_t/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/tracking/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/tracking/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:26.221291 Wake-T-0.7.1/wake_t/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/utilities/bunch_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/utilities/bunch_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/utilities/bunch_saving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/utilities/numba.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2023-10-17 13:17:15.000000 Wake-T-0.7.1/wake_t/utilities/other.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.452384 wake_t-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-15 15:38:26.000000 wake_t-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-15 15:38:30.452384 wake_t-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-15 15:38:26.000000 wake_t-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.452384 wake_t-0.8.0/Wake_T.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-15 15:38:30.000000 wake_t-0.8.0/Wake_T.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-15 15:38:30.000000 wake_t-0.8.0/Wake_T.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:38:30.000000 wake_t-0.8.0/Wake_T.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 15:38:30.000000 wake_t-0.8.0/Wake_T.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:38:30.000000 wake_t-0.8.0/Wake_T.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 15:38:26.000000 wake_t-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 15:38:30.456384 wake_t-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 15:38:26.000000 wake_t-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.440384 wake_t-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_active_plasma_lens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_beam_deposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_beamline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_bunch_read_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_custom_blowout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_field_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_field_gathering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_field_quadrupole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_fluid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_laser_envelope_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_laser_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_multibunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_no_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_openpmd_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_parabolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_particle_bunch_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_plasma_beamline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_plasma_deposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_ramps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_sc_baxevanis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-15 15:38:26.000000 wake_t-0.8.0/tests/test_simple_blowout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.440384 wake_t-0.8.0/wake_t/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.444383 wake_t-0.8.0/wake_t/beamline_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/active_plasma_lens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/beamline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/field_element.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2685 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/field_quadrupole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/plasma_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/plasma_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/beamline_elements/tm_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.444383 wake_t-0.8.0/wake_t/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/diagnostics/bunch_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/diagnostics/openpmd_diag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.444383 wake_t-0.8.0/wake_t/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/fields/analytical_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/fields/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/fields/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/fields/numerical_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/fields/rz_wakefield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.444383 wake_t-0.8.0/wake_t/particles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/deposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/particle_bunch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.444383 wake_t-0.8.0/wake_t/particles/push/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/push/boris_pusher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/push/runge_kutta_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/particles/push/transfer_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.448383 wake_t-0.8.0/wake_t/physics_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.448383 wake_t-0.8.0/wake_t/physics_models/beam_optics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/beam_optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/beam_optics/transfer_matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.448383 wake_t-0.8.0/wake_t/physics_models/collective_effects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/collective_effects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/collective_effects/csr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.448383 wake_t-0.8.0/wake_t/physics_models/em_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/em_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/em_fields/linear_b_theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/em_fields/quadrupole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.448383 wake_t-0.8.0/wake_t/physics_models/laser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/laser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/laser/envelope_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/laser/envelope_solver_non_centered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25873 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/laser/laser_pulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/laser/tdma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/laser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.448383 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/custom_blowout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/focusing_blowout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.452384 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.452384 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19861 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/simple_blowout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.452384 wake_t-0.8.0/wake_t/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/tracking/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/tracking/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:30.452384 wake_t-0.8.0/wake_t/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/utilities/bunch_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/utilities/bunch_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/utilities/bunch_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/utilities/numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-15 15:38:26.000000 wake_t-0.8.0/wake_t/utilities/other.py
```

### Comparing `Wake-T-0.7.1/LICENSE` & `wake_t-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/PKG-INFO` & `wake_t-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wake-T
-Version: 0.7.1
+Version: 0.8.0
 Summary: A fast particle tracking code for plasma accelerators.
 Home-page: https://github.com/AngelFP/Wake-T
 Author: Angel Ferran Pousa
 Author-email: angel.ferran.pousa@desy.de,
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Wake-T-0.7.1/README.md` & `wake_t-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/Wake_T.egg-info/PKG-INFO` & `wake_t-0.8.0/Wake_T.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wake-T
-Version: 0.7.1
+Version: 0.8.0
 Summary: A fast particle tracking code for plasma accelerators.
 Home-page: https://github.com/AngelFP/Wake-T
 Author: Angel Ferran Pousa
 Author-email: angel.ferran.pousa@desy.de,
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Wake-T-0.7.1/Wake_T.egg-info/SOURCES.txt` & `wake_t-0.8.0/Wake_T.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 tests/test_active_plasma_lens.py
 tests/test_beam_deposition.py
 tests/test_beamline.py
 tests/test_bunch_read_save.py
 tests/test_custom_blowout.py
 tests/test_field_element.py
 tests/test_field_gathering.py
+tests/test_field_quadrupole.py
 tests/test_fluid_model.py
 tests/test_interpolation.py
 tests/test_laser_envelope_model.py
 tests/test_laser_initialization.py
 tests/test_multibunch.py
 tests/test_no_bunch.py
 tests/test_openpmd_viewer.py
@@ -30,14 +31,15 @@
 tests/test_sc_baxevanis.py
 tests/test_simple_blowout.py
 wake_t/__init__.py
 wake_t/beamline_elements/__init__.py
 wake_t/beamline_elements/active_plasma_lens.py
 wake_t/beamline_elements/beamline.py
 wake_t/beamline_elements/field_element.py
+wake_t/beamline_elements/field_quadrupole.py
 wake_t/beamline_elements/plasma_ramp.py
 wake_t/beamline_elements/plasma_stage.py
 wake_t/beamline_elements/tm_elements.py
 wake_t/diagnostics/__init__.py
 wake_t/diagnostics/bunch_analysis.py
 wake_t/diagnostics/openpmd_diag.py
 wake_t/fields/__init__.py
@@ -58,23 +60,24 @@
 wake_t/physics_models/__init__.py
 wake_t/physics_models/beam_optics/__init__.py
 wake_t/physics_models/beam_optics/transfer_matrices.py
 wake_t/physics_models/collective_effects/__init__.py
 wake_t/physics_models/collective_effects/csr.py
 wake_t/physics_models/em_fields/__init__.py
 wake_t/physics_models/em_fields/linear_b_theta.py
+wake_t/physics_models/em_fields/quadrupole.py
 wake_t/physics_models/laser/__init__.py
 wake_t/physics_models/laser/envelope_solver.py
 wake_t/physics_models/laser/envelope_solver_non_centered.py
 wake_t/physics_models/laser/laser_pulse.py
 wake_t/physics_models/laser/tdma.py
+wake_t/physics_models/laser/utils.py
 wake_t/physics_models/plasma_wakefields/__init__.py
 wake_t/physics_models/plasma_wakefields/custom_blowout.py
 wake_t/physics_models/plasma_wakefields/focusing_blowout.py
-wake_t/physics_models/plasma_wakefields/from_pic.py
 wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py
 wake_t/physics_models/plasma_wakefields/simple_blowout.py
 wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/__init__.py
 wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py
 wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py
 wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py
 wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py
```

### Comparing `Wake-T-0.7.1/setup.cfg` & `wake_t-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_active_plasma_lens.py` & `wake_t-0.8.0/tests/test_active_plasma_lens.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         en_x=en, en_y=en, a_x=alpha, a_y=alpha, b_x=beta, b_y=beta, ene=ene,
         ene_sp=ene_sp, s_t=s_t, xi_c=0e-6, q_tot=10, n_part=1e5)
     apl = ActivePlasmaLens(1e-2, 1000, wakefields=False, n_out=3)
 
     apl.track(bunch)
     bunch_params = analyze_bunch(bunch)
     gamma_x = bunch_params['gamma_x']
-    assert approx(gamma_x, rel=1e-10) == 92.38646379897074
+    assert approx(gamma_x, rel=1e-10) == 92.38407675999406
 
 
 def test_active_plasma_lens_with_wakefields():
     """
     Check that the beam propagation through an active plasma lens with
     wakefields is accurate.
     """
@@ -60,13 +60,13 @@
 
     # Do tracking.
     apl.track(bunch)
 
     # Analyze and check results.
     bunch_params = analyze_bunch(bunch)
     gamma_x = bunch_params['gamma_x']
-    assert approx(gamma_x, rel=1e-10) == 77.31995824746237
+    assert approx(gamma_x, rel=1e-10) == 77.32021188373825
 
 
 if __name__ == '__main__':
     test_active_plasma_lens()
     test_active_plasma_lens_with_wakefields()
```

### Comparing `Wake-T-0.7.1/tests/test_beam_deposition.py` & `wake_t-0.8.0/tests/test_beam_deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_beamline.py` & `wake_t-0.8.0/tests/test_beamline.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,20 @@
         xi_min=-20e-6, xi_max=20e-6, r_max=50e-6, n_xi=80, n_r=100,
         dz_fields=0.5e-3)
 
     # Define single-element beamline
     bl = Beamline([deepcopy(plasma)])
 
     # Track plasma.
-    bunch_1 = deepcopy(bunch)
+    bunch_1 = bunch.copy()
     out_dir_1 = os.path.join(output_folder, 'plasma_diags')
     plasma.track(bunch_1, opmd_diag=True, diag_dir=out_dir_1)
 
     # Track beamline.
-    bunch_2 = deepcopy(bunch)
+    bunch_2 = bunch.copy()
     out_dir_2 = os.path.join(output_folder, 'bl_diags')
     bl.track(bunch_2, opmd_diag=True, diag_dir=out_dir_2)
 
     # Check that final beams are identical.
     assert_array_equal(bunch_2.x, bunch_1.x)
     assert_array_equal(bunch_2.y, bunch_1.y)
     assert_array_equal(bunch_2.xi, bunch_1.xi)
@@ -77,24 +77,24 @@
         xi_min=-20e-6, xi_max=20e-6, r_max=50e-6, n_xi=80, n_r=100,
         dz_fields=0.5e-3)
 
     # Define single-element beamline
     bl = Beamline([deepcopy(d1), deepcopy(plasma), deepcopy(d2)])
 
     # Track elements individually.
-    bunch_1 = deepcopy(bunch)
+    bunch_1 = bunch.copy()
     out_dir_d1 = os.path.join(output_folder, 'd1_diags')
     out_dir_plasma = os.path.join(output_folder, 'plasma_diags')
     out_dir_d2 = os.path.join(output_folder, 'd2_diags')
     d1.track(bunch_1, opmd_diag=True, diag_dir=out_dir_d1)
     plasma.track(bunch_1, opmd_diag=True, diag_dir=out_dir_plasma)
     d2.track(bunch_1, opmd_diag=True, diag_dir=out_dir_d2)
 
     # Track beamline.
-    bunch_2 = deepcopy(bunch)
+    bunch_2 = bunch.copy()
     out_dir_bl = os.path.join(output_folder, 'bl_diags')
     bl.track(bunch_2, opmd_diag=True, diag_dir=out_dir_bl)
 
     # Check that final beams are identical.
     assert_array_equal(bunch_2.x, bunch_1.x)
     assert_array_equal(bunch_2.y, bunch_1.y)
     assert_array_equal(bunch_2.xi, bunch_1.xi)
```

### Comparing `Wake-T-0.7.1/tests/test_bunch_read_save.py` & `wake_t-0.8.0/tests/test_bunch_read_save.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_custom_blowout.py` & `wake_t-0.8.0/tests/test_custom_blowout.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         xi_fields=xi_c, n_out=50, bunch_pusher='boris')
 
     # Do tracking.
     bunch_list = plasma.track(bunch)
 
     bunch_params = analyze_bunch(bunch)
     rel_ene_sp = bunch_params['rel_ene_spread']
-    assert approx(rel_ene_sp, rel=1e-10) == 0.21192488237458038
+    assert approx(rel_ene_sp, rel=1e-10) == 0.21192494153185745
 
     if make_plots:
         # Analyze bunch evolution.
         params_evolution = analyze_bunch_list(bunch_list)
 
 
         # Quick plot of results.
```

### Comparing `Wake-T-0.7.1/tests/test_field_element.py` & `wake_t-0.8.0/tests/test_field_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,14 @@
     )
 
     # Check that an error is raised because the number of `dt_bunch` does
     # not agree with the number of bunches.
     with raises(ValueError) as e_info:
         element.track(bunch, opmd_diag=False)
     # This one should instead work.
-    element.track([bunch, copy.deepcopy(bunch)], opmd_diag=False)
+    element.track([bunch, bunch.copy()], opmd_diag=False)
 
 
 
 if __name__ == '__main__':
     test_field_element_tracking()
     test_field_element_error()
```

### Comparing `Wake-T-0.7.1/tests/test_field_gathering.py` & `wake_t-0.8.0/tests/test_field_gathering.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_fluid_model.py` & `wake_t-0.8.0/tests/test_fluid_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     bunch_list = plasma.track(bunch)
 
     # Analyze bunch evolution.
     params_evolution = analyze_bunch_list(bunch_list)
 
     # Check final parameters.
     ene_sp = params_evolution['rel_ene_spread'][-1]
-    assert approx(ene_sp, rel=1e-10) == 0.024179998095119972
+    assert approx(ene_sp, rel=1e-10) == 0.024157374564016194
 
     # Quick plot of results.
     if plot:
         z = params_evolution['prop_dist'] * 1e2
         fig_1 = plt.figure()
         plt.subplot(411)
         plt.plot(z, params_evolution['beta_x']*1e3)
```

### Comparing `Wake-T-0.7.1/tests/test_interpolation.py` & `wake_t-0.8.0/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_laser_envelope_model.py` & `wake_t-0.8.0/tests/test_laser_envelope_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from numpy.testing import assert_almost_equal
 import scipy.constants as ct
 import matplotlib.pyplot as plt
 from wake_t.physics_models.laser.laser_pulse import GaussianPulse
+from wake_t.physics_models.laser.utils import unwrap
 
 
 def test_gaussian_laser_in_vacuum(plot=False):
     """Test evolution of Gaussian laser pulse in vacuum.
 
     This test evolves a Gaussian laser pulse over a 1cm vacuum. It checks
     that the evolution is in agreement with the analytical expectation and that
@@ -186,14 +187,23 @@
         plt.figure()
         plt.plot(z, laser_a)
         plt.plot(z, laser_a_an)
 
         plt.show()
 
 
+def test_unwrap():
+    """Test that the custom function for phase unwrapping implemented for
+    numba agrees with the numpy version.
+    """
+    phase = np.linspace(0, np.pi, num=5)
+    phase[3:] += np.pi
+    np.testing.assert_allclose(np.unwrap(phase), unwrap(phase))
+
+
 def calculate_spot_size(a_env, dr):
     # Project envelope to r
     a_proj = np.sum(np.abs(a_env), axis=0)
 
     # Maximum is on axis
     a_max = a_proj[0]
 
@@ -226,7 +236,8 @@
     a0 = np.max(a_mod)
     return a0
 
 
 if __name__ == "__main__":
     test_gaussian_laser_in_vacuum(plot=True)
     test_gaussian_laser_in_vacuum_with_subgrid(plot=True)
+    test_unwrap()
```

### Comparing `Wake-T-0.7.1/tests/test_laser_initialization.py` & `wake_t-0.8.0/tests/test_laser_initialization.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_multibunch.py` & `wake_t-0.8.0/tests/test_multibunch.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     # Analyze evolution.
     driver_params = analyze_bunch_list(output[0])
     witness_params = analyze_bunch_list(output[1])
 
     # Assert final parameters are correct.
     final_energy_driver = driver_params['avg_ene'][-1]
     final_energy_witness = witness_params['avg_ene'][-1]
-    assert approx(final_energy_driver, rel=1e-10) == 1700.3927190416732
-    assert approx(final_energy_witness, rel=1e-10) == 636.330857261392
+    assert approx(final_energy_driver, rel=1e-10) == 1700.3843657635728
+    assert approx(final_energy_witness, rel=1e-10) == 636.3260426124102
 
     if plot:
         z = driver_params['prop_dist'] * 1e2
         plt.subplot(311)
         plt.plot(z, driver_params['emitt_x']*1e6, label='Driver',
                  color='tab:blue')
         plt.plot(z, witness_params['emitt_x']*1e6, label='Witness',
```

### Comparing `Wake-T-0.7.1/tests/test_no_bunch.py` & `wake_t-0.8.0/tests/test_no_bunch.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_openpmd_viewer.py` & `wake_t-0.8.0/tests/test_openpmd_viewer.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_parabolic_profile.py` & `wake_t-0.8.0/tests/test_parabolic_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     laser = GaussianPulse(-50e-6, a0, w0, tau, z_foc=0., l_0=l0)
     laser_1 = deepcopy(laser)
     laser_2 = deepcopy(laser)
 
     # Create identical bunches for each case.
     bunch = get_matched_bunch(
         1e-6, 1e-6, 200, 1, 3, laser.xi_c - 30e-6, 1e-6, 1e4, n_p=n_p)
-    bunch_1 = deepcopy(bunch)
-    bunch_2 = deepcopy(bunch)
+    bunch_1 = bunch.copy()
+    bunch_2 = bunch.copy()
 
     # Create single plasma stage (containing all sections).
     plasma_single = PlasmaStage(
         np.sum(L_stretches), n_p, wakefield_model='quasistatic_2d', n_out=10,
         xi_min=xi_min, xi_max=xi_max, r_max=r_max, r_max_plasma=r_max,
         laser=laser_1, laser_evolution=True, n_r=Nr, n_xi=Nxi, ppc=2,
         dz_fields=dz_fields, parabolic_coefficient=parabolic_coefficient)
```

### Comparing `Wake-T-0.7.1/tests/test_particle_bunch_species.py` & `wake_t-0.8.0/tests/test_particle_bunch_species.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_plasma_beamline.py` & `wake_t-0.8.0/tests/test_plasma_beamline.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_plasma_deposition.py` & `wake_t-0.8.0/tests/test_plasma_deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_ramps.py` & `wake_t-0.8.0/tests/test_ramps.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         1e-2, ramp_type='downramp', profile='inverse_square',
         plasma_dens_top=1e23, plasma_dens_down=1e21,
         wakefield_model='focusing_blowout', n_out=3)
 
     downramp.track(bunch)
     bunch_params = analyze_bunch(bunch)
     beta_x = bunch_params['beta_x']
-    assert beta_x == 0.009750309290619276
+    assert beta_x == 0.009750308724018872
 
 
 def test_upramp():
     """
     Test that a plasma upramp changes the beta function of an initial beam
     as expected. The simplest `focusing_blowout` wakefield model is used in
     order to have a fast test.
@@ -60,13 +60,13 @@
         1e-2, ramp_type='upramp', profile='inverse_square',
         plasma_dens_top=1e23, plasma_dens_down=1e21,
         wakefield_model='focusing_blowout', n_out=3)
 
     downramp.track(bunch)
     bunch_params = analyze_bunch(bunch)
     beta_x = bunch_params['beta_x']
-    assert beta_x == 0.0007631600676104024
+    assert beta_x == 0.000763155045965493
 
 
 if __name__ == '__main__':
     test_downramp()
     test_upramp()
```

### Comparing `Wake-T-0.7.1/tests/test_sc_baxevanis.py` & `wake_t-0.8.0/tests/test_sc_baxevanis.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/tests/test_simple_blowout.py` & `wake_t-0.8.0/tests/test_simple_blowout.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         bunch_pusher='boris')
 
     # Do tracking.
     bunch_list = plasma.track(bunch)
 
     bunch_params = analyze_bunch(bunch)
     rel_ene_sp = bunch_params['rel_ene_spread']
-    assert approx(rel_ene_sp, rel=1e-10) == 0.3637648484576557
+    assert approx(rel_ene_sp, rel=1e-10) == 0.3637651769109033
 
     if make_plots:
         # Analyze bunch evolution.
         params_evolution = analyze_bunch_list(bunch_list)
 
 
         # Quick plot of results.
```

### Comparing `Wake-T-0.7.1/wake_t/__init__.py` & `wake_t-0.8.0/wake_t/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7.1'
+__version__ = '0.8.0'
 
 
 from .beamline_elements import (PlasmaStage, PlasmaRamp, ActivePlasmaLens,
                                 Drift, Dipole, Quadrupole, Sextupole, Beamline)
 from .physics_models.collective_effects.csr import set_csr_settings
 from .physics_models.laser.laser_pulse import (
     GaussianPulse, LaguerreGaussPulse, FlattenedGaussianPulse)
```

### Comparing `Wake-T-0.7.1/wake_t/beamline_elements/active_plasma_lens.py` & `wake_t-0.8.0/wake_t/beamline_elements/active_plasma_lens.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,14 +47,28 @@
         be automatically set to :math:`dt = T/(10*2*pi)`, where T is the
         smallest expected betatron period of the bunch along the plasma lens
         (T is calculated from `foc_strength` if `wakefields=False`,
         otherwise the focusing strength of a blowout is used).
         A list of values can also be provided. In this case, the list
         should have the same order as the list of bunches given to the
         ``track`` method.
+    push_bunches_before_diags : bool, optional
+        Whether to push the bunches before saving them to the diagnostics.
+        Since the time step of the diagnostics can be different from that
+        of the bunches, it could happen that the bunches appear in the
+        diagnostics as they were at the last push, but not at the actual
+        time of the diagnostics. Setting this parameter to ``True``
+        (default) ensures that an additional push is given to all bunches
+        to evolve them to the diagnostics time before saving.
+        This additional push will always have a time step smaller than
+        the the time step of the bunch, so it has no detrimental impact
+        on the accuracy of the simulation. However, it could make
+        convergence studies more difficult to interpret,
+        since the number of pushes will depend on `n_diags`. Therefore,
+        it is exposed as an option so that it can be disabled if needed.
     n_out : int
         Number of times along the lens in which the particle distribution
         should be returned (A list with all output bunches is returned
         after tracking).
     name : str
         Name of the plasma lens. This is only used for displaying the
         progress bar during tracking. By default, ``'Active plasma lens'``.
@@ -74,14 +88,15 @@
         length: float,
         foc_strength: float,
         wakefields: bool = False,
         density: Optional[Union[float, Callable[[float], float]]] = None,
         wakefield_model: Optional[str] = 'quasistatic_2d',
         bunch_pusher: Optional[Literal['boris', 'rk4']] = 'boris',
         dt_bunch: Optional[DtBunchType] = 'auto',
+        push_bunches_before_diags: Optional[bool] = True,
         n_out: Optional[int] = 1,
         name: Optional[str] = 'Active plasma lens',
         **model_params
     ) -> None:
         self.foc_strength = foc_strength
         self.wakefields = wakefields
         if not self.wakefields:
@@ -96,14 +111,15 @@
         self.apl_field = LinearBThetaField(-self.foc_strength)
         super().__init__(
             length=length,
             density=density,
             wakefield_model=wakefield_model,
             bunch_pusher=bunch_pusher,
             dt_bunch=dt_bunch,
+            push_bunches_before_diags=push_bunches_before_diags,
             n_out=n_out,
             name=name,
             external_fields=[self.apl_field],
             **model_params
         )
 
     def _get_optimized_dt(self, beam):
```

### Comparing `Wake-T-0.7.1/wake_t/beamline_elements/beamline.py` & `wake_t-0.8.0/wake_t/beamline_elements/beamline.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     ) -> None:
         self.elements = elements
 
     def track(
         self,
         bunches: Optional[Union[ParticleBunch, List[ParticleBunch]]] = [],
         opmd_diag: Optional[bool] = False,
-        diag_dir: Optional[str] = None
+        diag_dir: Optional[str] = None,
+        show_progress_bar: Optional[bool] = True,
     ) -> Union[List[ParticleBunch], List[List[ParticleBunch]]]:
         """
         Track bunch through beamline.
 
         Parameters
         ----------
         bunches : ParticleBunch or list of ParticleBunch
@@ -36,19 +37,28 @@
             per beamline element is determined by its `n_out` value. It is also
             possible to provide an already existing OpenPMDDiagnostics
             instance instead of a boolean value.
         diag_dir : str
             Directory into which the openPMD output will be written. By default
             this is a 'diags' folder in the current directory. Only needed if
             `opmd_diag=True`.
+        show_progress_bar : bool, optional
+            Whether to show a progress bar of the tracking through each
+            element. By default ``True``.
 
         Returns
         -------
         A list of size 'n_out' containing the bunch distribution at each step.
 
         """
         bunch_list = []
         if type(opmd_diag) is not OpenPMDDiagnostics and opmd_diag:
             opmd_diag = OpenPMDDiagnostics(write_dir=diag_dir)
         for element in self.elements:
-            bunch_list.extend(element.track(bunches, opmd_diag=opmd_diag))
+            bunch_list.extend(
+                element.track(
+                    bunches,
+                    opmd_diag=opmd_diag,
+                    show_progress_bar=show_progress_bar,
+                )
+            )
         return bunch_list
```

### Comparing `Wake-T-0.7.1/wake_t/beamline_elements/field_element.py` & `wake_t-0.8.0/wake_t/beamline_elements/field_element.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,40 +35,57 @@
         progress bar during tracking. By default, ``'field element'``.
     fields : list
         List of Fields that will be applied to the particle bunches.
     auto_dt_bunch : callable, optional
         Function used to determine the adaptive time step for bunches in
         which the time step is set to ``'auto'``. The function should take
         solely a ``ParticleBunch`` as argument.
+    push_bunches_before_diags : bool, optional
+        Whether to push the bunches before saving them to the diagnostics.
+        Since the time step of the diagnostics can be different from that
+        of the bunches, it could happen that the bunches appear in the
+        diagnostics as they were at the last push, but not at the actual
+        time of the diagnostics. Setting this parameter to ``True``
+        (default) ensures that an additional push is given to all bunches
+        to evolve them to the diagnostics time before saving.
+        This additional push will always have a time step smaller than
+        the the time step of the bunch, so it has no detrimental impact
+        on the accuracy of the simulation. However, it could make
+        convergence studies more difficult to interpret,
+        since the number of pushes will depend on `n_diags`. Therefore,
+        it is exposed as an option so that it can be disabled if needed.
 
     """
 
     def __init__(
         self,
         length: float,
         dt_bunch: Union[float, str, List[Union[float, str]]],
         bunch_pusher: Optional[Literal['boris', 'rk4']] = 'boris',
         n_out: Optional[int] = 1,
         name: Optional[str] = 'field element',
         fields: Optional[List[Field]] = [],
-        auto_dt_bunch: Optional[str] = None
+        auto_dt_bunch: Optional[str] = None,
+        push_bunches_before_diags: Optional[bool] = True,
     ) -> None:
         self.length = length
         self.bunch_pusher = bunch_pusher
         self.dt_bunch = dt_bunch
         self.n_out = n_out
         self.name = name
         self.fields = fields
         self.auto_dt_bunch = auto_dt_bunch
+        self.push_bunches_before_diags = push_bunches_before_diags
 
     def track(
         self,
         bunches: Optional[Union[ParticleBunch, List[ParticleBunch]]] = [],
         opmd_diag: Optional[Union[bool, OpenPMDDiagnostics]] = False,
-        diag_dir: Optional[str] = None
+        diag_dir: Optional[str] = None,
+        show_progress_bar: Optional[bool] = True,
     ) -> Union[List[ParticleBunch], List[List[ParticleBunch]]]:
         """
         Track bunch through element.
 
         Parameters
         ----------
         bunches : ParticleBunch or list of ParticleBunch
@@ -79,14 +96,17 @@
             HDF5 files following the openPMD standard. The number of outputs
             the `n_out` value. It is also possible to provide an already
             existing OpenPMDDiagnostics instance instead of a boolean value.
         diag_dir : str
             Directory into which the openPMD output will be written. By default
             this is a 'diags' folder in the current directory. Only needed if
             `opmd_diag=True`.
+        show_progress_bar : bool, optional
+            Whether to show a progress bar of the tracking. By default
+            ``True``.
 
         Returns
         -------
         A list of size 'n_out' containing the bunch distribution at each step.
 
         """
         # Make sure `bunches` and `dt_bunch` are lists.
@@ -115,14 +135,16 @@
             bunches=bunches,
             dt_bunches=dt_bunch,
             fields=self.fields,
             n_diags=self.n_out,
             opmd_diags=opmd_diag,
             bunch_pusher=self.bunch_pusher,
             auto_dt_bunch_f=self.auto_dt_bunch,
+            push_bunches_before_diags=self.push_bunches_before_diags,
+            show_progress_bar=show_progress_bar,
             section_name=self.name
         )
 
         # Do tracking.
         bunch_list = tracker.do_tracking()
 
         # If only tracking one bunch, do not return list of lists.
```

### Comparing `Wake-T-0.7.1/wake_t/beamline_elements/plasma_ramp.py` & `wake_t-0.8.0/wake_t/beamline_elements/plasma_ramp.py`

 * *Files 11% similar despite different names*

```diff
@@ -92,14 +92,28 @@
     dt_bunch : float
         The time step for evolving the particle bunches. If ``None``, it will
         be automatically set to :math:`dt = T/(10*2*pi)`, where T is the
         smallest expected betatron period of the bunch along the plasma stage.
         A list of values can also be provided. In this case, the list
         should have the same order as the list of bunches given to the
         ``track`` method.
+    push_bunches_before_diags : bool, optional
+        Whether to push the bunches before saving them to the diagnostics.
+        Since the time step of the diagnostics can be different from that
+        of the bunches, it could happen that the bunches appear in the
+        diagnostics as they were at the last push, but not at the actual
+        time of the diagnostics. Setting this parameter to ``True``
+        (default) ensures that an additional push is given to all bunches
+        to evolve them to the diagnostics time before saving.
+        This additional push will always have a time step smaller than
+        the the time step of the bunch, so it has no detrimental impact
+        on the accuracy of the simulation. However, it could make
+        convergence studies more difficult to interpret,
+        since the number of pushes will depend on `n_diags`. Therefore,
+        it is exposed as an option so that it can be disabled if needed.
     n_out : int
         Number of times along the stage in which the particle distribution
         should be returned (A list with all output bunches is returned
         after tracking).
     name : str
         Name of the plasma ramp. This is only used for displaying the
         progress bar during tracking. By default, ``'Plasma ramp'``.
@@ -122,14 +136,15 @@
         wakefield_model: Optional[str] = 'focusing_blowout',
         decay_length: Optional[float] = None,
         plasma_dens_top: Optional[float] = None,
         plasma_dens_down: Optional[float] = None,
         position_down: Optional[float] = None,
         bunch_pusher: Optional[Literal['boris', 'rk4']] = 'boris',
         dt_bunch: Optional[DtBunchType] = 'auto',
+        push_bunches_before_diags: Optional[bool] = True,
         n_out: Optional[int] = 1,
         name: Optional[str] = 'Plasma ramp',
         **model_params
     ) -> None:
         self.ramp_type = ramp_type
         if position_down is None:
             position_down = length
@@ -147,14 +162,15 @@
         self.profile = profile
         super().__init__(
             length=length,
             density=self.ramp_profile,
             wakefield_model=wakefield_model,
             bunch_pusher=bunch_pusher,
             dt_bunch=dt_bunch,
+            push_bunches_before_diags=push_bunches_before_diags,
             n_out=n_out,
             name=name,
             **model_params
         )
 
     def ramp_profile(self, z):
         """ Return the density value at a certain z location. """
```

### Comparing `Wake-T-0.7.1/wake_t/beamline_elements/tm_elements.py` & `wake_t-0.8.0/wake_t/beamline_elements/tm_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """ Contains the classes of all elements tracked using transfer matrices. """
 from typing import Optional, Union, List
 import time
-from copy import deepcopy
 
 import numpy as np
 import scipy.constants as ct
 
 from wake_t.particles.push.transfer_matrix import track_with_transfer_map
 from wake_t.particles.particle_bunch import ParticleBunch
 from wake_t.utilities.other import print_progress_bar
@@ -73,15 +72,16 @@
 
     def track(
         self,
         bunch: ParticleBunch,
         backtrack: Optional[bool] = False,
         out_initial: Optional[bool] = False,
         opmd_diag: Optional[Union[bool, OpenPMDDiagnostics]] = False,
-        diag_dir: Optional[str] = None
+        diag_dir: Optional[str] = None,
+        show_progress_bar: Optional[bool] = True,
     ) -> List[ParticleBunch]:
         """
         Track bunch through element.
 
         Parameters
         ----------
         bunch : ParticleBunch
@@ -96,14 +96,17 @@
             HDF5 files following the openPMD standard. The number of outputs
             the `n_out` value. It is also possible to provide an already
             existing OpenPMDDiagnostics instance instead of a boolean value.
         diag_dir : str
             Directory into which the openPMD output will be written. By default
             this is a 'diags' folder in the current directory. Only needed if
             `opmd_diag=True`.
+        show_progress_bar : bool, optional
+            Whether to show a progress bar of the tracking. By default
+            ``True``.
 
         Returns
         -------
         A list of size 'n_out' containing the bunch distribution at each step.
 
         """
         # Convert bunch to ocelot units and reference frame
@@ -122,34 +125,36 @@
         # Create diagnostics if needed
         if type(opmd_diag) is not OpenPMDDiagnostics and opmd_diag:
             opmd_diag = OpenPMDDiagnostics(write_dir=diag_dir)
         elif not opmd_diag:
             opmd_diag = None
 
         # Print output header
-        print('')
-        print(self.element_name.capitalize())
-        print('-'*len(self.element_name))
-        self._print_element_properties()
-        csr_string = 'on' if self.csr_on else 'off'
-        print('CSR {}.'.format(csr_string))
-        print('')
-        n_steps = len(track_steps)
-        st_0 = 'Tracking in {} step(s)... '.format(n_steps)
+        if show_progress_bar:
+            print('')
+            print(self.element_name.capitalize())
+            print('-'*len(self.element_name))
+            self._print_element_properties()
+            csr_string = 'on' if self.csr_on else 'off'
+            print('CSR {}.'.format(csr_string))
+            print('')
+            n_steps = len(track_steps)
+            st_0 = 'Tracking in {} step(s)... '.format(n_steps)
 
         # Start tracking
         start_time = time.time()
         output_bunch_list = list()
         if out_initial:
-            output_bunch_list.append(deepcopy(bunch))
+            output_bunch_list.append(bunch.copy())
             if opmd_diag is not None:
                 opmd_diag.write_diagnostics(
                     0., l_step/ct.c, [output_bunch_list[-1]])
         for i in track_steps:
-            print_progress_bar(st_0, i+1, n_steps)
+            if show_progress_bar:
+                print_progress_bar(st_0, i+1, n_steps)
             l_curr = (i+1) * l_step * (1-2*backtrack)
             # Track with transfer matrix
             bunch_mat = track_with_transfer_map(
                 bunch_mat, l_step, self.length, -self.theta, self.k1, self.k2,
                 self.gamma_ref, order=self.order)
             # Apply CSR
             if self.csr_on:
@@ -170,17 +175,18 @@
         self._update_input_bunch(bunch, bunch_mat, output_bunch_list)
 
         # Add element length to diagnostics position
         if opmd_diag is not None:
             opmd_diag.increase_z_pos(self.length)
 
         # Finalize
-        tracking_time = time.time() - start_time
-        print('Done ({} s).'.format(tracking_time))
-        print('-'*80)
+        if show_progress_bar:
+            tracking_time = time.time() - start_time
+            print('Done ({} s).'.format(tracking_time))
+            print('-'*80)
         return output_bunch_list
 
     def _get_beam_matrix_for_tracking(self, bunch):
         bunch_mat = bunch.get_6D_matrix()
         # obtain with respect to reference displacement
         bunch_mat[0] -= bunch.x_ref
         # rotate by the reference angle so that it enters normal to the element
@@ -215,15 +221,15 @@
     def _update_input_bunch(self, bunch, bunch_mat, output_bunch_list):
         if len(output_bunch_list) == 0:
             new_bunch_mat = convert_from_ocelot_matrix(
                 bunch_mat, self.gamma_ref)
             last_bunch = self._create_new_bunch(bunch, new_bunch_mat,
                                                 self.length)
         else:
-            last_bunch = deepcopy(output_bunch_list[-1])
+            last_bunch = output_bunch_list[-1].copy()
         bunch.set_phase_space(last_bunch.x, last_bunch.y, last_bunch.xi,
                               last_bunch.px, last_bunch.py, last_bunch.pz)
         bunch.prop_distance = last_bunch.prop_distance
         bunch.theta_ref = last_bunch.theta_ref
         bunch.x_ref = last_bunch.x_ref
 
     def _create_new_bunch(self, old_bunch, new_bunch_mat, prop_dist):
```

### Comparing `Wake-T-0.7.1/wake_t/diagnostics/bunch_analysis.py` & `wake_t-0.8.0/wake_t/diagnostics/bunch_analysis.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/diagnostics/openpmd_diag.py` & `wake_t-0.8.0/wake_t/diagnostics/openpmd_diag.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/fields/analytical_field.py` & `wake_t-0.8.0/wake_t/fields/analytical_field.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/fields/base.py` & `wake_t-0.8.0/wake_t/fields/base.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/fields/gather.py` & `wake_t-0.8.0/wake_t/fields/gather.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/fields/interpolation.py` & `wake_t-0.8.0/wake_t/fields/interpolation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/fields/numerical_field.py` & `wake_t-0.8.0/wake_t/fields/numerical_field.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/fields/rz_wakefield.py` & `wake_t-0.8.0/wake_t/fields/rz_wakefield.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/particles/deposition.py` & `wake_t-0.8.0/wake_t/particles/deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/particles/interpolation.py` & `wake_t-0.8.0/wake_t/particles/interpolation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/particles/particle_bunch.py` & `wake_t-0.8.0/wake_t/particles/particle_bunch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 This module contains the class defining a particle bunch.
 """
 # TODO: clean methods to set and get bunch matrix
+from __future__ import annotations
+from copy import deepcopy
 from typing import Optional
 
 import numpy as np
 import scipy.constants as ct
 from aptools.plotting.quick_diagnostics import full_phase_space
 
 from .push.runge_kutta_4 import apply_rk4_pusher
@@ -291,14 +293,37 @@
         else:
             raise ValueError(
                 f"Bunch pusher '{pusher}' not recognized. "
                 "Possible values are 'boris' and 'rk4'"
             )
         self.prop_distance += dt * ct.c
 
+    def copy(self) -> ParticleBunch:
+        """Return a copy of the bunch.
+
+        To improve performance, this copy won't contain copies of auxiliary
+        arrays, only of the particle coordinates and properties.
+        """
+        bunch_copy = ParticleBunch(
+            w=deepcopy(self.w),
+            x=deepcopy(self.x),
+            y=deepcopy(self.y),
+            xi=deepcopy(self.xi),
+            px=deepcopy(self.px),
+            py=deepcopy(self.py),
+            pz=deepcopy(self.pz),
+            prop_distance=deepcopy(self.prop_distance),
+            name=deepcopy(self.name),
+            q_species=deepcopy(self.q_species),
+            m_species=deepcopy(self.m_species)
+        )
+        bunch_copy.x_ref = self.x_ref
+        bunch_copy.theta_ref = self.theta_ref
+        return bunch_copy
+
     def get_field_arrays(self):
         """Get the arrays where the gathered fields will be stored."""
         if not self.__field_arrays_allocated:
             self.__preallocate_field_arrays()
         return (
             self.__e_x, self.__e_y, self.__e_z,
             self.__b_x, self.__b_y, self.__b_z
```

### Comparing `Wake-T-0.7.1/wake_t/particles/push/boris_pusher.py` & `wake_t-0.8.0/wake_t/particles/push/boris_pusher.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/particles/push/runge_kutta_4.py` & `wake_t-0.8.0/wake_t/particles/push/runge_kutta_4.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/particles/push/transfer_matrix.py` & `wake_t-0.8.0/wake_t/particles/push/transfer_matrix.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/beam_optics/transfer_matrices.py` & `wake_t-0.8.0/wake_t/physics_models/beam_optics/transfer_matrices.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/collective_effects/csr.py` & `wake_t-0.8.0/wake_t/physics_models/collective_effects/csr.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/em_fields/linear_b_theta.py` & `wake_t-0.8.0/wake_t/physics_models/em_fields/linear_b_theta.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/laser/envelope_solver.py` & `wake_t-0.8.0/wake_t/physics_models/laser/envelope_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 import numpy as np
 import scipy.constants as ct
 
 from wake_t.utilities.numba import njit_serial
 from .tdma import TDMA
+from .utils import unwrap
 
 
 @njit_serial(fastmath=True)
 def evolve_envelope(
         a, a_old, chi, k0, kp, zmin, zmax, nz, rmax, nr, dt, nt,
         use_phase=True):
     """
@@ -87,34 +88,24 @@
     for n in range(nt):
         # a_new_jp1 is equivalent to a_new[j+1] and a_new_jp2 to a_new[j+2].
         a_new_jp1 = np.zeros(nr, dtype=np.complex128)
         a_new_jp2 = np.zeros(nr, dtype=np.complex128)
 
         # Getting the phase of the envelope on axis.
         if use_phase:
-            phases = np.angle(a[:, 0])
+            phases = unwrap(np.angle(a[:, 0]))
 
         # Loop over z.
         for j in range(nz - 1, -1, -1):
 
             # Calculate phase differences between adjacent points.
             if use_phase:
                 d_theta1 = phases[j + 1] - phases[j]
                 d_theta2 = phases[j + 2] - phases[j + 1]
 
-                # Prevent phase jumps bigger than 1.5*pi.
-                if d_theta1 < -1.5 * np.pi:
-                    d_theta1 += 2 * np.pi
-                if d_theta2 < -1.5 * np.pi:
-                    d_theta2 += 2 * np.pi
-                if d_theta1 > 1.5 * np.pi:
-                    d_theta1 -= 2 * np.pi
-                if d_theta2 > 1.5 * np.pi:
-                    d_theta2 -= 2 * np.pi
-
             # Calculate D factor [Eq. (6)].
             D_jkn = (1.5 * d_theta1 - 0.5 * d_theta2) * inv_dz
 
             # Calculate right-hand side of Eq (7).
             for k in range(nr):
                 rhs_k = (
                     - 2 * inv_dt ** 2 * a[j, k]
```

### Comparing `Wake-T-0.7.1/wake_t/physics_models/laser/envelope_solver_non_centered.py` & `wake_t-0.8.0/wake_t/physics_models/laser/envelope_solver_non_centered.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 import numpy as np
 import scipy.constants as ct
 
 from wake_t.utilities.numba import njit_serial
 from .tdma import TDMA
+from .utils import unwrap
 
 
 @njit_serial(fastmath=True)
 def evolve_envelope_non_centered(
         a, a_old, chi, k0, kp, zmin, zmax, nz, rmax, nr, dt, nt,
         use_phase=True):
     """
@@ -87,34 +88,24 @@
     for n in range(nt):
         # a_new_jp1 is equivalent to a_new[j+1] and a_new_jp2 to a_new[j+2].
         a_new_jp1 = np.zeros(nr, dtype=np.complex128)
         a_new_jp2 = np.zeros(nr, dtype=np.complex128)
 
         # Getting the phase of the envelope on axis.
         if use_phase:
-            phases = np.angle(a[:, 0])
+            phases = unwrap(np.angle(a[:, 0]))
 
         # Loop over z.
         for j in range(nz - 1, -1, -1):
 
             # Calculate phase differences between adjacent points.
             if use_phase:
                 d_theta1 = phases[j + 1] - phases[j]
                 d_theta2 = phases[j + 2] - phases[j + 1]
 
-                # Prevent phase jumps bigger than 1.5*pi.
-                if d_theta1 < -1.5 * np.pi:
-                    d_theta1 += 2 * np.pi
-                if d_theta2 < -1.5 * np.pi:
-                    d_theta2 += 2 * np.pi
-                if d_theta1 > 1.5 * np.pi:
-                    d_theta1 -= 2 * np.pi
-                if d_theta2 > 1.5 * np.pi:
-                    d_theta2 -= 2 * np.pi
-
             # Calculate D factor [Eq. (6)].
             D_jkn = (1.5 * d_theta1 - 0.5 * d_theta2) * inv_dz
 
             # Calculate right-hand side of Eq (7).
             for k in range(nr):
                 rhs_k = (
                     - (C_minus - chi[j, k] * 0.5 - 2j * inv_dt * D_jkn)
```

### Comparing `Wake-T-0.7.1/wake_t/physics_models/laser/laser_pulse.py` & `wake_t-0.8.0/wake_t/physics_models/laser/laser_pulse.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/laser/tdma.py` & `wake_t-0.8.0/wake_t/physics_models/laser/tdma.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/custom_blowout.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/custom_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/focusing_blowout.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/focusing_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/physics_models/plasma_wakefields/simple_blowout.py` & `wake_t-0.8.0/wake_t/physics_models/plasma_wakefields/simple_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/tracking/progress_bar.py` & `wake_t-0.8.0/wake_t/tracking/progress_bar.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,31 +6,34 @@
 from tqdm import tqdm
 
 
 # Avoid showing clamping warnings from the progress bar.
 warnings.filterwarnings('ignore', '.*clamping.*', )
 
 
-def get_progress_bar(description, total_length):
+def get_progress_bar(description, total_length, disable):
     """Get progress bar for the tracker.
 
     Parameters
     ----------
     description : str
         Description to be appended to start of the progress bar.
     total_length : float
         Total length in metres of the stage to be tracked.
+    disable : bool
+        Whether to disable (not show) the progress bar.
 
     Returns
     -------
     A tqdm progress bar.
     """
     l_bar = "{desc}: {percentage:3.0f}%|"
     r_bar = "| {n:.6f}/{total:.6f} {unit} [{elapsed}]"
     progress_bar = tqdm(
         desc=description,
         total=total_length,
         unit='m',
         bar_format=l_bar + "{bar}" + r_bar,
-        file=sys.stdout
+        file=sys.stdout,
+        disable=disable
     )
     return progress_bar
```

### Comparing `Wake-T-0.7.1/wake_t/tracking/tracker.py` & `wake_t-0.8.0/wake_t/tracking/tracker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ This module contains the Tracker class. """
 from typing import Optional, Callable, List, Literal
-from copy import deepcopy
 
 import numpy as np
 import scipy.constants as ct
 
 from wake_t.particles.particle_bunch import ParticleBunch
 from wake_t.fields.base import Field
 from wake_t.fields.analytical_field import AnalyticalField
@@ -58,14 +57,30 @@
     auto_dt_bunch_f : callable, optional
         Function used to determine the adaptive time step for bunches in
         which the time step is set to `'auto'`. The function should take
         solely a `ParticleBunch` as argument.
     bunch_pusher : str, optional
         The particle pusher used to evolve the bunches. Possible values
         are `'boris'` or `'rk4'`.
+    push_bunches_before_diags : bool, optional
+        Whether to push the bunches before saving them to the diagnostics.
+        Since the time step of the diagnostics can be different from that
+        of the bunches, it could happen that the bunches appear in the
+        diagnostics as they were at the last push, but not at the actual
+        time of the diagnostics. Setting this parameter to ``True``
+        (default) ensures that an additional push is given to all bunches
+        to evolve them to the diagnostics time before saving.
+        This additional push will always have a time step smaller than
+        the the time step of the bunch, so it has no detrimental impact
+        on the accuracy of the simulation. However, it could make
+        convergence studies more difficult to interpret,
+        since the number of pushes will depend on `n_diags`. Therefore,
+        it is exposed as an option so that it can be disabled if needed.
+    show_progress_bar : bool, optional
+        Whether to show a progress bar of the tracking. By default ``True``.
     section_name : str, optional
         Name of the section to be tracked. This will be appended to the
         beginning of the progress bar.
 
     """
 
     def __init__(
@@ -74,24 +89,28 @@
         bunches: Optional[List[ParticleBunch]] = [],
         dt_bunches: Optional[List[float]] = [],
         fields: Optional[List[Field]] = [],
         n_diags: Optional[int] = 0,
         opmd_diags: Optional[OpenPMDDiagnostics] = None,
         auto_dt_bunch_f: Optional[Callable[[ParticleBunch], float]] = None,
         bunch_pusher: Optional[Literal['boris', 'rk4']] = 'boris',
+        push_bunches_before_diags: Optional[bool] = True,
+        show_progress_bar: Optional[bool] = True,
         section_name: Optional[str] = 'Simulation'
     ) -> None:
         self.t_final = t_final
         self.bunches = bunches
         self.dt_bunches = dt_bunches
         self.fields = fields if len(fields) > 0 else [AnalyticalField()]
         self.opmd_diags = opmd_diags
         self.n_diags = n_diags
         self.auto_dt_bunch_f = auto_dt_bunch_f
         self.bunch_pusher = bunch_pusher
+        self.push_bunches_before_diags = push_bunches_before_diags
+        self.show_progress_bar = show_progress_bar
         self.section_name = section_name
 
         # Get all numerical fields and their time steps.
         self.num_fields = [f for f in fields if isinstance(f, NumericalField)]
         for field in self.num_fields:
             field.adjust_dt(self.t_final)
         self.dt_fields = [f.dt_update for f in self.num_fields]
@@ -130,15 +149,19 @@
         """
         # Get current number of threads before setting it to the number
         # requested by Wake-T.
         num_threads_outside_waket = get_num_threads()
         set_num_threads(num_threads)
 
         # Initialize progress bar.
-        progress_bar = get_progress_bar(self.section_name, self.t_final*ct.c)
+        progress_bar = get_progress_bar(
+            description=self.section_name,
+            total_length=self.t_final*ct.c,
+            disable=not self.show_progress_bar,
+        )
 
         # Calculate fields at t=0.
         for field in self.num_fields:
             field.update(self.bunches)
 
         # Generate initial diagnostics.
         self.generate_diagnostics()
@@ -183,35 +206,43 @@
                 break
 
             # Advance tracking time.
             self.t_tracking = t_next
 
             # If next object is a ParticleBunch, update it.
             if isinstance(obj_next, ParticleBunch):
-                obj_next.evolve(
-                    self.fields, t_current, dt_next, self.bunch_pusher)
-                # Update the time step if set to `'auto'`.
-                if obj_next in self.auto_dt_bunches:
-                    dt_objects[i_next] = self.auto_dt_bunch_f(obj_next)
-                # Determine if this was the last push.
-                final_push = np.float32(t_next) == np.float32(self.t_final)
-                # Determine if next push brings the bunch beyond `t_final`.
-                next_push_beyond_final_time = (
-                    t_next + dt_objects[i_next] > self.t_final)
-                # Make sure the last push of the bunch advances it to exactly
-                # `t_final`.
-                if not final_push and next_push_beyond_final_time:
-                    dt_objects[i_next] = self.t_final - t_next
+                self.evolve_bunch(
+                    bunch=obj_next,
+                    t_current=t_current,
+                    t_next=t_next,
+                    dt_next=dt_next,
+                    i_next=i_next,
+                    dt_objects=dt_objects,
+                )
 
             # If next object is a NumericalField, update it.
             elif isinstance(obj_next, NumericalField):
                 obj_next.update(self.bunches)
 
             # If next object are the diagnostics, generate them.
             elif obj_next == 'diags':
+                # Evolve all bunches to the diagnostics time.
+                if self.push_bunches_before_diags:
+                    for i, obj in enumerate(self.objects_to_track):
+                        if isinstance(obj, ParticleBunch):
+                            dt_bunch = t_next - t_objects[i]
+                            self.evolve_bunch(
+                                bunch=obj,
+                                t_current=t_objects[i],
+                                t_next=t_next,
+                                dt_next=dt_bunch,
+                                i_next=i,
+                                dt_objects=dt_objects,
+                            )
+                            t_objects[i] += dt_bunch
                 self.generate_diagnostics()
 
             # Advance current time of the update object.
             t_objects[i_next] += dt_next
 
             # Update progress bar.
             progress_bar.update(self.t_tracking*ct.c - progress_bar.n)
@@ -226,31 +257,57 @@
         # Reset the number of threads to the value outside of Wake-T.
         # This should help avoiding Wake-T to affect the behavior of other
         # applications that require a different number of threads.
         set_num_threads(num_threads_outside_waket)
 
         return self.bunch_list
 
+    def evolve_bunch(
+        self,
+        bunch: ParticleBunch,
+        t_current: float,
+        t_next: float,
+        dt_next: float,
+        i_next: int,
+        dt_objects: List,
+    ):
+        """Evolve particle bunch to next time step.
+
+        Parameters
+        ----------
+        bunch : ParticleBunch
+            The particle bunch to evolve.
+        t_current : float
+            The current time of the simulation.
+        t_next : float
+            The time of the next step.
+        dt_next : float
+            The time step by which to advance the bunch.
+        i_next : int
+            The index of the bunch in the list of objects to track.
+        dt_objects : List
+            The time steps of all objects to track.
+        """
+        bunch.evolve(self.fields, t_current, dt_next, self.bunch_pusher)
+        # Update the time step if set to `'auto'`.
+        if bunch in self.auto_dt_bunches:
+            dt_objects[i_next] = self.auto_dt_bunch_f(bunch)
+        # Determine if this was the last push.
+        final_push = np.float32(t_next) == np.float32(self.t_final)
+        # Determine if next push brings the bunch beyond `t_final`.
+        next_push_beyond_final_time = (
+            t_next + dt_objects[i_next] > self.t_final)
+        # Make sure the last push of the bunch advances it to exactly
+        # `t_final`.
+        if not final_push and next_push_beyond_final_time:
+            dt_objects[i_next] = self.t_final - t_next
+
     def generate_diagnostics(self) -> None:
         """Generate tracking diagnostics."""
         # Make copy of current bunches and store in output list.
         for i, bunch in enumerate(self.bunches):
-            self.bunch_list[i].append(
-                ParticleBunch(
-                    deepcopy(bunch.w),
-                    deepcopy(bunch.x),
-                    deepcopy(bunch.y),
-                    deepcopy(bunch.xi),
-                    deepcopy(bunch.px),
-                    deepcopy(bunch.py),
-                    deepcopy(bunch.pz),
-                    prop_distance=deepcopy(bunch.prop_distance),
-                    name=deepcopy(bunch.name),
-                    q_species=deepcopy(bunch.q_species),
-                    m_species=deepcopy(bunch.m_species)
-                )
-            )
+            self.bunch_list[i].append(bunch.copy())
 
         # If needed, write also the openPMD diagnostics.
         if self.opmd_diags is not None:
             self.opmd_diags.write_diagnostics(
                 self.t_tracking, self.dt_diags, self.bunches, self.fields)
```

### Comparing `Wake-T-0.7.1/wake_t/utilities/bunch_generation.py` & `wake_t-0.8.0/wake_t/utilities/bunch_generation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/utilities/bunch_manipulation.py` & `wake_t-0.8.0/wake_t/utilities/bunch_manipulation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/utilities/bunch_saving.py` & `wake_t-0.8.0/wake_t/utilities/bunch_saving.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/utilities/numba.py` & `wake_t-0.8.0/wake_t/utilities/numba.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.7.1/wake_t/utilities/other.py` & `wake_t-0.8.0/wake_t/utilities/other.py`

 * *Files identical despite different names*

