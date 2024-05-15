# Comparing `tmp/simpeg_drivers-0.1.0b4.tar.gz` & `tmp/simpeg_drivers-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpeg_drivers-0.1.0b4.tar", max compression
+gzip compressed data, was "simpeg_drivers-0.1.0b5.tar", max compression
```

## Comparing `simpeg_drivers-0.1.0b4.tar` & `simpeg_drivers-0.1.0b5.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 simpeg_drivers-0.1.0b4/LICENSE
--rw-r--r--   0        0        0     5304 2024-05-03 20:13:53.242114 simpeg_drivers-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0     5466 2024-04-29 02:02:58.449338 simpeg_drivers-0.1.0b4/README.rst
--rw-r--r--   0        0        0     3604 2024-05-03 19:13:21.827160 simpeg_drivers-0.1.0b4/simpeg_drivers/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-29 02:02:58.454666 simpeg_drivers-0.1.0b4/simpeg_drivers/components/__init__.py
--rw-r--r--   0        0        0    20469 2024-05-03 20:13:32.764456 simpeg_drivers-0.1.0b4/simpeg_drivers/components/data.py
--rw-r--r--   0        0        0     1231 2024-04-29 02:14:00.711152 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/__init__.py
--rw-r--r--   0        0        0     1462 2024-04-26 14:45:23.744035 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/abstract_factory.py
--rw-r--r--   0        0        0    21970 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/directives_factory.py
--rw-r--r--   0        0        0     4382 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/entity_factory.py
--rw-r--r--   0        0        0     5003 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/misfit_factory.py
--rw-r--r--   0        0        0     7519 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/receiver_factory.py
--rw-r--r--   0        0        0     3521 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simpeg_factory.py
--rw-r--r--   0        0        0     8146 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simulation_factory.py
--rw-r--r--   0        0        0     6194 2024-05-03 18:35:52.953133 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/source_factory.py
--rw-r--r--   0        0        0    17797 2024-05-03 18:35:52.953133 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/survey_factory.py
--rw-r--r--   0        0        0     6492 2024-05-03 18:35:52.954132 simpeg_drivers-0.1.0b4/simpeg_drivers/components/locations.py
--rw-r--r--   0        0        0     4797 2024-05-03 20:13:32.766267 simpeg_drivers-0.1.0b4/simpeg_drivers/components/meshes.py
--rw-r--r--   0        0        0    16890 2024-05-03 18:36:25.041051 simpeg_drivers-0.1.0b4/simpeg_drivers/components/models.py
--rw-r--r--   0        0        0     6144 2024-05-03 18:35:52.955183 simpeg_drivers-0.1.0b4/simpeg_drivers/components/topography.py
--rw-r--r--   0        0        0     1846 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b4/simpeg_drivers/components/utils.py
--rw-r--r--   0        0        0     4179 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b4/simpeg_drivers/components/windows.py
--rw-r--r--   0        0        0    14591 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b4/simpeg_drivers/constants.py
--rw-r--r--   0        0        0    18418 2024-05-03 19:13:59.671778 simpeg_drivers-0.1.0b4/simpeg_drivers/driver.py
--rw-r--r--   0        0        0     1112 2024-04-29 02:14:00.696694 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/__init__.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.755992 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/__init__.py
--rw-r--r--   0        0        0    10334 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py
--rw-r--r--   0        0        0     1506 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py
--rw-r--r--   0        0        0     2680 2024-04-26 14:45:23.758085 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py
--rw-r--r--   0        0        0      962 2024-04-29 02:14:00.601072 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py
--rw-r--r--   0        0        0     9075 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py
--rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py
--rw-r--r--   0        0        0     2808 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/params.py
--rw-r--r--   0        0        0      948 2024-05-03 20:13:32.768270 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py
--rw-r--r--   0        0        0    10879 2024-04-26 14:45:23.762303 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py
--rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py
--rw-r--r--   0        0        0     2646 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/params.py
--rw-r--r--   0        0        0     6677 2024-05-03 18:35:52.656394 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/driver.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.763466 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/__init__.py
--rw-r--r--   0        0        0    10754 2024-04-26 14:45:23.764555 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py
--rw-r--r--   0        0        0     1596 2024-04-26 14:45:23.765703 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py
--rw-r--r--   0        0        0     3031 2024-04-26 14:45:23.766703 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py
--rw-r--r--   0        0        0      968 2024-04-29 02:14:00.644863 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py
--rw-r--r--   0        0        0     9362 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py
--rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py
--rw-r--r--   0        0        0     3529 2024-04-26 14:45:23.768920 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py
--rw-r--r--   0        0        0      968 2024-04-29 02:14:00.616156 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py
--rw-r--r--   0        0        0    11193 2024-04-26 14:45:23.770003 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py
--rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.771008 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py
--rw-r--r--   0        0        0     3368 2024-04-26 14:45:23.771078 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py
--rw-r--r--   0        0        0     5508 2024-04-26 14:45:23.772174 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/params.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.773241 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/__init__.py
--rw-r--r--   0        0        0      978 2024-04-29 02:14:00.679279 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/__init__.py
--rw-r--r--   0        0        0     8022 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/constants.py
--rw-r--r--   0        0        0     1320 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/driver.py
--rw-r--r--   0        0        0     5676 2024-04-26 14:45:23.775408 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/params.py
--rw-r--r--   0        0        0      973 2024-04-29 02:14:00.668402 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/__init__.py
--rw-r--r--   0        0        0     9507 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/constants.py
--rw-r--r--   0        0        0     1300 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/driver.py
--rw-r--r--   0        0        0     6307 2024-04-26 14:45:23.777654 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/params.py
--rw-r--r--   0        0        0     3121 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/constants.py
--rw-r--r--   0        0        0     8452 2024-05-03 19:13:21.834695 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/driver.py
--rw-r--r--   0        0        0      965 2024-04-29 02:14:00.630255 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/__init__.py
--rw-r--r--   0        0        0     6884 2024-04-26 14:45:23.780891 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/constants.py
--rw-r--r--   0        0        0     9514 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/driver.py
--rw-r--r--   0        0        0     2789 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/params.py
--rw-r--r--   0        0        0      959 2024-04-29 02:14:00.702198 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/constants.py
--rw-r--r--   0        0        0     4940 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/driver.py
--rw-r--r--   0        0        0     2126 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/params.py
--rw-r--r--   0        0        0     3644 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/params.py
--rw-r--r--   0        0        0     8892 2024-04-26 14:45:23.786252 simpeg_drivers-0.1.0b4/simpeg_drivers/line_sweep/driver.py
--rw-r--r--   0        0        0     1007 2024-04-29 02:14:00.690154 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/__init__.py
--rw-r--r--   0        0        0      963 2024-04-29 02:14:00.673785 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/__init__.py
--rw-r--r--   0        0        0    17280 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/constants.py
--rw-r--r--   0        0        0     1260 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/driver.py
--rw-r--r--   0        0        0    10843 2024-04-26 14:45:23.789513 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/params.py
--rw-r--r--   0        0        0      953 2024-04-29 02:14:00.684640 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/__init__.py
--rw-r--r--   0        0        0    10148 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/constants.py
--rw-r--r--   0        0        0     1220 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/driver.py
--rw-r--r--   0        0        0     7359 2024-04-26 14:45:23.791658 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/params.py
--rw-r--r--   0        0        0    20664 2024-04-26 14:45:23.792706 simpeg_drivers-0.1.0b4/simpeg_drivers/params.py
--rw-r--r--   0        0        0     1078 2024-04-29 02:14:00.706667 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/__init__.py
--rw-r--r--   0        0        0      954 2024-04-29 02:14:00.716496 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/__init__.py
--rw-r--r--   0        0        0    18355 2024-04-26 14:45:23.793880 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/constants.py
--rw-r--r--   0        0        0     1224 2024-04-26 14:45:23.795051 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/driver.py
--rw-r--r--   0        0        0     9715 2024-04-26 14:45:23.796179 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/params.py
--rw-r--r--   0        0        0      961 2024-04-29 02:14:00.586879 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py
--rw-r--r--   0        0        0    19126 2024-04-26 14:45:23.797274 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/constants.py
--rw-r--r--   0        0        0     1252 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/driver.py
--rw-r--r--   0        0        0    11229 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/params.py
--rw-r--r--   0        0        0      961 2024-04-29 02:14:00.658721 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/__init__.py
--rw-r--r--   0        0        0    21697 2024-04-26 14:45:23.800544 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/constants.py
--rw-r--r--   0        0        0     2522 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/driver.py
--rw-r--r--   0        0        0    12279 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/params.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.802683 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/__init__.py
--rw-r--r--   0        0        0     6694 2024-05-03 18:35:52.901412 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/surveys.py
--rw-r--r--   0        0        0    17509 2024-04-26 14:45:23.804857 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/testing.py
--rw-r--r--   0        0        0    27865 2024-05-03 19:15:10.720720 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/utils.py
--rw-r--r--   0        0        0      944 2024-04-26 14:45:23.726759 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/__init__.py
--rw-r--r--   0        0        0      216 2024-04-24 21:13:56.506158 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/colortable.csv
--rw-r--r--   0        0        0  3108380 2024-04-24 21:13:58.874200 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/inversion_demo.geoh5
--rw-r--r--   0        0        0      109 2024-04-24 21:13:57.168793 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/time_channels.txt
--rw-r--r--   0        0        0     6006 2024-05-03 18:35:52.883963 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json
--rw-r--r--   0        0        0     4506 2024-05-03 18:35:52.885035 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json
--rw-r--r--   0        0        0     6054 2024-05-03 18:35:52.885035 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json
--rw-r--r--   0        0        0    14043 2024-05-03 18:35:52.886092 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json
--rw-r--r--   0        0        0    13496 2024-05-03 18:35:52.886092 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json
--rw-r--r--   0        0        0    14267 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json
--rw-r--r--   0        0        0     3790 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_forward.ui.json
--rw-r--r--   0        0        0    13431 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_inversion.ui.json
--rw-r--r--   0        0        0     6269 2024-05-03 18:35:52.888305 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_forward.ui.json
--rw-r--r--   0        0        0    20667 2024-05-03 18:35:52.888305 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_inversion.ui.json
--rw-r--r--   0        0        0     6085 2024-05-03 18:35:52.889361 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json
--rw-r--r--   0        0        0     4917 2024-05-03 18:35:52.889361 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json
--rw-r--r--   0        0        0     6372 2024-05-03 18:35:52.890482 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json
--rw-r--r--   0        0        0    14303 2024-05-03 18:35:52.891560 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json
--rw-r--r--   0        0        0    13914 2024-05-03 18:35:52.891560 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json
--rw-r--r--   0        0        0    14598 2024-05-03 18:35:52.892614 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json
--rw-r--r--   0        0        0    12640 2024-05-03 18:35:52.892614 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json
--rw-r--r--   0        0        0    12717 2024-05-03 18:35:52.893713 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json
--rw-r--r--   0        0        0     7077 2024-05-03 18:35:52.893713 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json
--rw-r--r--   0        0        0    21475 2024-05-03 18:35:52.894827 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json
--rw-r--r--   0        0        0     7898 2024-05-03 18:35:52.894827 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json
--rw-r--r--   0        0        0    23137 2024-05-03 18:35:52.895919 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json
--rw-r--r--   0        0        0     5968 2024-05-03 18:35:52.895919 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json
--rw-r--r--   0        0        0    19477 2024-05-03 18:35:52.897020 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json
--rw-r--r--   0        0        0     4264 2024-05-03 18:35:52.897020 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_forward.ui.json
--rw-r--r--   0        0        0    14383 2024-05-03 18:35:52.898158 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_inversion.ui.json
--rw-r--r--   0        0        0     5345 2024-05-03 18:35:52.898158 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_forward.ui.json
--rw-r--r--   0        0        0    16282 2024-05-03 18:35:52.899266 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_inversion.ui.json
--rw-r--r--   0        0        0      175 2024-04-24 21:13:57.169304 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/waveform.txt
--rw-r--r--   0        0        0      800 2024-04-23 22:37:27.593550 simpeg_drivers-0.1.0b4/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 simpeg_drivers-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 simpeg_drivers-0.1.0b5/LICENSE
+-rw-r--r--   0        0        0     5342 2024-05-15 15:52:33.874673 simpeg_drivers-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0     5466 2024-04-29 02:02:58.449338 simpeg_drivers-0.1.0b5/README.rst
+-rw-r--r--   0        0        0     3604 2024-05-11 04:24:04.327457 simpeg_drivers-0.1.0b5/simpeg_drivers/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-29 02:02:58.454666 simpeg_drivers-0.1.0b5/simpeg_drivers/components/__init__.py
+-rw-r--r--   0        0        0    20581 2024-05-09 21:52:32.962298 simpeg_drivers-0.1.0b5/simpeg_drivers/components/data.py
+-rw-r--r--   0        0        0     1231 2024-04-29 02:14:00.711152 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-26 14:45:23.744035 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/abstract_factory.py
+-rw-r--r--   0        0        0    21970 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/directives_factory.py
+-rw-r--r--   0        0        0     4382 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/entity_factory.py
+-rw-r--r--   0        0        0     5434 2024-05-11 04:24:03.542933 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/misfit_factory.py
+-rw-r--r--   0        0        0     7519 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/receiver_factory.py
+-rw-r--r--   0        0        0     3521 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/simpeg_factory.py
+-rw-r--r--   0        0        0     8146 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/simulation_factory.py
+-rw-r--r--   0        0        0     6194 2024-05-03 18:35:52.953133 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/source_factory.py
+-rw-r--r--   0        0        0    18163 2024-05-11 04:24:03.543932 simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/survey_factory.py
+-rw-r--r--   0        0        0     6492 2024-05-03 18:35:52.954132 simpeg_drivers-0.1.0b5/simpeg_drivers/components/locations.py
+-rw-r--r--   0        0        0     7834 2024-05-09 21:52:32.963297 simpeg_drivers-0.1.0b5/simpeg_drivers/components/meshes.py
+-rw-r--r--   0        0        0    16890 2024-05-03 18:36:25.041051 simpeg_drivers-0.1.0b5/simpeg_drivers/components/models.py
+-rw-r--r--   0        0        0     6144 2024-05-03 18:35:52.955183 simpeg_drivers-0.1.0b5/simpeg_drivers/components/topography.py
+-rw-r--r--   0        0        0     1846 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b5/simpeg_drivers/components/utils.py
+-rw-r--r--   0        0        0     4179 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b5/simpeg_drivers/components/windows.py
+-rw-r--r--   0        0        0    14591 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b5/simpeg_drivers/constants.py
+-rw-r--r--   0        0        0    18418 2024-05-03 19:13:59.671778 simpeg_drivers-0.1.0b5/simpeg_drivers/driver.py
+-rw-r--r--   0        0        0     1112 2024-04-29 02:14:00.696694 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.755992 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/__init__.py
+-rw-r--r--   0        0        0    10334 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py
+-rw-r--r--   0        0        0     1506 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py
+-rw-r--r--   0        0        0     2680 2024-04-26 14:45:23.758085 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py
+-rw-r--r--   0        0        0      962 2024-04-29 02:14:00.601072 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py
+-rw-r--r--   0        0        0     9075 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py
+-rw-r--r--   0        0        0     2808 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/params.py
+-rw-r--r--   0        0        0      962 2024-05-09 21:52:32.990814 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py
+-rw-r--r--   0        0        0    10879 2024-04-26 14:45:23.762303 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py
+-rw-r--r--   0        0        0     2646 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/params.py
+-rw-r--r--   0        0        0     6677 2024-05-03 18:35:52.656394 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/driver.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.763466 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/__init__.py
+-rw-r--r--   0        0        0    10754 2024-04-26 14:45:23.764555 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py
+-rw-r--r--   0        0        0     1596 2024-04-26 14:45:23.765703 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py
+-rw-r--r--   0        0        0     3031 2024-04-26 14:45:23.766703 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py
+-rw-r--r--   0        0        0      968 2024-04-29 02:14:00.644863 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py
+-rw-r--r--   0        0        0     9362 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py
+-rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py
+-rw-r--r--   0        0        0     3196 2024-05-09 21:52:32.991816 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py
+-rw-r--r--   0        0        0      968 2024-04-29 02:14:00.616156 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py
+-rw-r--r--   0        0        0    11193 2024-04-26 14:45:23.770003 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py
+-rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.771008 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py
+-rw-r--r--   0        0        0     3368 2024-04-26 14:45:23.771078 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py
+-rw-r--r--   0        0        0     5508 2024-04-26 14:45:23.772174 simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/params.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.773241 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/__init__.py
+-rw-r--r--   0        0        0      978 2024-04-29 02:14:00.679279 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/__init__.py
+-rw-r--r--   0        0        0     8022 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/constants.py
+-rw-r--r--   0        0        0     1320 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/driver.py
+-rw-r--r--   0        0        0     5676 2024-04-26 14:45:23.775408 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/params.py
+-rw-r--r--   0        0        0      973 2024-04-29 02:14:00.668402 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/time_domain/__init__.py
+-rw-r--r--   0        0        0     9507 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/time_domain/constants.py
+-rw-r--r--   0        0        0     3600 2024-05-11 04:24:03.544938 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/time_domain/driver.py
+-rw-r--r--   0        0        0     6307 2024-04-26 14:45:23.777654 simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/time_domain/params.py
+-rw-r--r--   0        0        0     3121 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/constants.py
+-rw-r--r--   0        0        0     8459 2024-05-15 15:43:47.928751 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/driver.py
+-rw-r--r--   0        0        0      965 2024-04-29 02:14:00.630255 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/__init__.py
+-rw-r--r--   0        0        0     6884 2024-04-26 14:45:23.780891 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/constants.py
+-rw-r--r--   0        0        0     9785 2024-05-15 15:43:47.931707 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/driver.py
+-rw-r--r--   0        0        0     2789 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/params.py
+-rw-r--r--   0        0        0      959 2024-04-29 02:14:00.702198 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/constants.py
+-rw-r--r--   0        0        0     4940 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/driver.py
+-rw-r--r--   0        0        0     2126 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/params.py
+-rw-r--r--   0        0        0     3644 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b5/simpeg_drivers/joint/params.py
+-rw-r--r--   0        0        0     8892 2024-04-26 14:45:23.786252 simpeg_drivers-0.1.0b5/simpeg_drivers/line_sweep/driver.py
+-rw-r--r--   0        0        0     1007 2024-04-29 02:14:00.690154 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-29 02:14:00.673785 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/__init__.py
+-rw-r--r--   0        0        0    17280 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/constants.py
+-rw-r--r--   0        0        0     1260 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/driver.py
+-rw-r--r--   0        0        0    10843 2024-04-26 14:45:23.789513 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/params.py
+-rw-r--r--   0        0        0      953 2024-04-29 02:14:00.684640 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/__init__.py
+-rw-r--r--   0        0        0    10148 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/constants.py
+-rw-r--r--   0        0        0     1220 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/driver.py
+-rw-r--r--   0        0        0     7359 2024-04-26 14:45:23.791658 simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/params.py
+-rw-r--r--   0        0        0    20664 2024-04-26 14:45:23.792706 simpeg_drivers-0.1.0b5/simpeg_drivers/params.py
+-rw-r--r--   0        0        0     1078 2024-04-29 02:14:00.706667 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/__init__.py
+-rw-r--r--   0        0        0      954 2024-04-29 02:14:00.716496 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/__init__.py
+-rw-r--r--   0        0        0    18355 2024-04-26 14:45:23.793880 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/constants.py
+-rw-r--r--   0        0        0     1224 2024-04-26 14:45:23.795051 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/driver.py
+-rw-r--r--   0        0        0     9715 2024-04-26 14:45:23.796179 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/params.py
+-rw-r--r--   0        0        0      961 2024-04-29 02:14:00.586879 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py
+-rw-r--r--   0        0        0    19126 2024-04-26 14:45:23.797274 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/constants.py
+-rw-r--r--   0        0        0     1252 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/driver.py
+-rw-r--r--   0        0        0    11229 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/params.py
+-rw-r--r--   0        0        0      961 2024-04-29 02:14:00.658721 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/__init__.py
+-rw-r--r--   0        0        0    21697 2024-04-26 14:45:23.800544 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/constants.py
+-rw-r--r--   0        0        0     2522 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/driver.py
+-rw-r--r--   0        0        0    12279 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/params.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.802683 simpeg_drivers-0.1.0b5/simpeg_drivers/utils/__init__.py
+-rw-r--r--   0        0        0     7210 2024-05-09 21:52:32.992815 simpeg_drivers-0.1.0b5/simpeg_drivers/utils/surveys.py
+-rw-r--r--   0        0        0    17509 2024-04-26 14:45:23.804857 simpeg_drivers-0.1.0b5/simpeg_drivers/utils/testing.py
+-rw-r--r--   0        0        0    27865 2024-05-03 19:15:10.720720 simpeg_drivers-0.1.0b5/simpeg_drivers/utils/utils.py
+-rw-r--r--   0        0        0      944 2024-04-26 14:45:23.726759 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-24 21:13:56.506158 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/colortable.csv
+-rw-r--r--   0        0        0  3108380 2024-04-24 21:13:58.874200 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/inversion_demo.geoh5
+-rw-r--r--   0        0        0      109 2024-04-24 21:13:57.168793 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/time_channels.txt
+-rw-r--r--   0        0        0     6006 2024-05-03 18:35:52.883963 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json
+-rw-r--r--   0        0        0     4506 2024-05-03 18:35:52.885035 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json
+-rw-r--r--   0        0        0     6054 2024-05-03 18:35:52.885035 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json
+-rw-r--r--   0        0        0    14043 2024-05-03 18:35:52.886092 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json
+-rw-r--r--   0        0        0    13496 2024-05-03 18:35:52.886092 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json
+-rw-r--r--   0        0        0    14267 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json
+-rw-r--r--   0        0        0     3790 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/fem_forward.ui.json
+-rw-r--r--   0        0        0    13431 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/fem_inversion.ui.json
+-rw-r--r--   0        0        0     6269 2024-05-03 18:35:52.888305 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/gravity_forward.ui.json
+-rw-r--r--   0        0        0    20667 2024-05-03 18:35:52.888305 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/gravity_inversion.ui.json
+-rw-r--r--   0        0        0     6085 2024-05-03 18:35:52.889361 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json
+-rw-r--r--   0        0        0     4917 2024-05-03 18:35:52.889361 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json
+-rw-r--r--   0        0        0     6372 2024-05-03 18:35:52.890482 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json
+-rw-r--r--   0        0        0    14303 2024-05-03 18:35:52.891560 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json
+-rw-r--r--   0        0        0    13914 2024-05-03 18:35:52.891560 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json
+-rw-r--r--   0        0        0    14598 2024-05-03 18:35:52.892614 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json
+-rw-r--r--   0        0        0    12622 2024-05-15 15:43:47.924183 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json
+-rw-r--r--   0        0        0    12717 2024-05-03 18:35:52.893713 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json
+-rw-r--r--   0        0        0     7077 2024-05-03 18:35:52.893713 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json
+-rw-r--r--   0        0        0    21474 2024-05-15 15:43:47.926191 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json
+-rw-r--r--   0        0        0     7898 2024-05-03 18:35:52.894827 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json
+-rw-r--r--   0        0        0    23137 2024-05-03 18:35:52.895919 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json
+-rw-r--r--   0        0        0     5968 2024-05-03 18:35:52.895919 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json
+-rw-r--r--   0        0        0    19477 2024-05-03 18:35:52.897020 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json
+-rw-r--r--   0        0        0     4264 2024-05-03 18:35:52.897020 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tdem_forward.ui.json
+-rw-r--r--   0        0        0    14383 2024-05-03 18:35:52.898158 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tdem_inversion.ui.json
+-rw-r--r--   0        0        0     5345 2024-05-10 14:55:31.090637 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tipper_forward.ui.json
+-rw-r--r--   0        0        0    16282 2024-05-03 18:35:52.899266 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tipper_inversion.ui.json
+-rw-r--r--   0        0        0      175 2024-04-24 21:13:57.169304 simpeg_drivers-0.1.0b5/simpeg_drivers-assets/waveform.txt
+-rw-r--r--   0        0        0      800 2024-04-23 22:37:27.593550 simpeg_drivers-0.1.0b5/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 simpeg_drivers-0.1.0b5/PKG-INFO
```

### Comparing `simpeg_drivers-0.1.0b4/LICENSE` & `simpeg_drivers-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/pyproject.toml` & `simpeg_drivers-0.1.0b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simpeg-drivers"
-version = "0.1.0-beta.4"
+version = "0.1.0-beta.5"
 description = "Application to run SimPEG inversions with geoh5 files from Geoscience Analyst."
 license = "MIT"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = [
     "Benjamin Kary <benjamink@mirageoscience.com>",
     "Dominique Fournier <dominiquef@mirageoscience.com>",
 ]
@@ -45,28 +45,29 @@
 #octree-creation-app = {url = "https://github.com/MiraGeoscience/octree-creation-app/archive/refs/heads/release/0.1.0.zip#sha256="}
 #octree-creation-app = {url = "http://localhost:8888/octree-creation-app.tar.gz#sha256="}
 
 geoapps-utils = {version = "~0.3.0rc1", source = "pypi", allow-prereleases = true}
 #geoapps-utils = {url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/release/0.3.0.zip#sha256="}
 #geoapps-utils = {url = "http://localhost:8888/geoapps-utils.tar.gz#sha256="}
 
-mira-simpeg = {version = ">=0.19.0.8rc1,<0.19.0.8.post999", source = "pypi", allow-prereleases = true}
+mira-simpeg = {version = ">=0.19.0.8rc3,<0.19.0.8.post999", source = "pypi", allow-prereleases = true}
 #mira-simpeg = {url = "https://github.com/MiraGeoscience/simpeg/archive/refs/heads/release/0.19.0.8.zip#sha256="}
 #mira-simpeg = {url = "http://localhost:8888/mira-simpeg.tar.gz#sha256="}
 
 param-sweeps = {version = "~0.1.7rc1", source = "pypi", allow-prereleases = true}
 #param-sweeps = {url = "https://github.com/MiraGeoscience/param-sweeps/archive/refs/heads/release/0.1.7.zip#sha256="}
 #param-sweeps = {url = "http://localhost:8888/param-sweeps.tar.gz#sha256="}
 
 ## indirect dependencies, forcing them here for installation through Conda not pip
 #---------------------------------------------------------------------------------
 Pillow = "~10.1.0"  # from geoh5py
 fsspec = "2022.*"  # from simpeg[dask]
 geoana = "~0.4.0"  # from simpeg
 h5py = "^3.2.1"  # from geoh5py
+matplotlib = "~3.7.1"  # from simpeg
 mkl = "2022.1.*"  # from simpeg
 pandas = "~2.2.1"  # from SimPEG, also used by targeting-workflow, petro-lingo
 pydantic = "~2.5.2"  # from geoapps-utils
 pydiso = "~0.0.3"  # from simpeg
 pymatsolver = "~0.2.0"  # from simpeg
 scikit-learn = "~1.4.0"  # from SimPEG, also used by geo-unsup-mapper, petro-lingo
 tqdm = "^4.66.1"  # from simpeg
```

### Comparing `simpeg_drivers-0.1.0b4/README.rst` & `simpeg_drivers-0.1.0b5/README.rst`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 # pylint: disable=unused-import
 # flake8: noqa
 
 from __future__ import annotations
 
-__version__ = "0.1.0-beta.4"
+__version__ = "0.1.0-beta.5"
 
 from pathlib import Path
 
 from SimPEG import dask
 
 from simpeg_drivers.constants import default_ui_json
 from simpeg_drivers.params import InversionBaseParams
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/data.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,16 +359,19 @@
                     offsets = self.params.tx_offsets
                     offsets = {
                         k: v * np.ones(len(self.locations)) for k, v in offsets.items()
                     }
                     normalizations[chan][comp] = (
                         mu0 * (-1 / offsets[chan] ** 3 / (4 * np.pi)) / 1e6
                     )
-                elif self.params.inversion_type in ["tdem"]:
-                    if comp in ["x", "z"]:
+                elif (
+                    self.params.inversion_type in ["tdem"]
+                    and self.params.data_units == "dB/dt (T/s)"
+                ):
+                    if comp in ["x", "y", "z"]:
                         normalizations[chan][comp] = -1
                     normalizations[chan][comp] *= np.ones(self.mask.sum())
 
         return normalizations
 
     def create_survey(
         self,
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/abstract_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/abstract_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/directives_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/directives_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/entity_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/entity_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/misfit_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/misfit_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,23 +69,26 @@
             channels = np.unique([list(v) for v in inversion_data.observed.values()])
         else:
             channels = [None]
 
         local_misfits = []
         self.sorting = []
         self.ordering = []
-        padding_cells = 8 if self.factory_type in ["fem", "tdem"] else 6
+        padding_cells = 4 if self.factory_type in ["fem", "tdem"] else 6
 
         # Keep whole mesh for 1 tile
         if len(tiles) == 1:
             padding_cells = 100
 
         tile_num = 0
         data_count = 0
         for local_index in tiles:
+            if len(local_index) == 0:
+                continue
+
             for count, channel in enumerate(channels):
                 survey, local_index, ordering = inversion_data.create_survey(
                     mesh=mesh, local_index=local_index, channel=channel
                 )
 
                 if count == 0:
                     if self.factory_type in ["fem", "tdem"]:
@@ -104,14 +107,22 @@
                     mesh,
                     active_cells,
                     survey,
                     self.models,
                     tile_id=tile_num,
                     padding_cells=padding_cells,
                 )
+
+                # TODO add option to export tile meshes
+                # from octree_creation_app.utils import treemesh_2_octree
+                # from geoh5py.shared.utils import fetch_active_workspace
+                #
+                # with fetch_active_workspace(self.params.geoh5) as ws:
+                #     treemesh_2_octree(ws, local_sim.mesh)
+
                 # TODO Parse workers to simulations
                 local_sim.workers = self.params.distributed_workers
                 local_data = data.Data(survey)
 
                 if self.params.forward_only:
                     lmisfit = data_misfit.L2DataMisfit(
                         local_data, local_sim, model_map=local_map
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/receiver_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/receiver_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simpeg_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/simpeg_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simulation_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/simulation_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/source_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/survey_factory.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/factories/survey_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,23 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from geoapps_utils.driver.params import BaseParams
 
 import numpy as np
 import SimPEG.electromagnetics.time_domain as tdem
+from geoh5py.objects.surveys.electromagnetics.ground_tem import (
+    LargeLoopGroundTEMTransmitters,
+)
 from scipy.interpolate import interp1d
 
 from simpeg_drivers.components.factories.receiver_factory import ReceiversFactory
 from simpeg_drivers.components.factories.simpeg_factory import SimPEGFactory
 from simpeg_drivers.components.factories.source_factory import SourcesFactory
+from simpeg_drivers.utils.surveys import counter_clockwise_sort
 
 
 def receiver_group(txi, potential_electrodes):
     """
     Group receivers by common transmitter id.
 
     :param: txi : transmitter index number.
@@ -324,33 +328,38 @@
         self.local_index = np.hstack(self.local_index)
 
         return [sources]
 
     def _tdem_arguments(self, data=None, local_index=None, mesh=None):
         receivers = data.entity
         transmitters = receivers.transmitters
-        transmitter_id = receivers.get_data("Transmitter ID")
 
-        if transmitter_id:
-            tx_rx = transmitter_id[0].values
+        if isinstance(transmitters, LargeLoopGroundTEMTransmitters):
+
+            if receivers.tx_id_property is None:
+                raise ValueError(
+                    "Transmitter ID property required for LargeLoopGroundTEMReceivers"
+                )
+
+            tx_rx = receivers.tx_id_property.values[self.local_index]
             tx_ids = transmitters.get_data("Transmitter ID")[0].values
-            rx_lookup = {}
-            tx_locs_lookup = {}
-            for k in np.unique(tx_rx[self.local_index]):
-                rx_lookup[k] = np.where(tx_rx == k)[0]
-                tx_ind = tx_ids == k
+            rx_lookup = []
+            tx_locs = []
+            for tx_id in np.unique(tx_rx):
+                rx_lookup.append(self.local_index[tx_rx == tx_id])
+                tx_ind = tx_ids == tx_id
                 loop_cells = transmitters.cells[
                     np.all(tx_ind[transmitters.cells], axis=1), :
                 ]
+                loop_cells = counter_clockwise_sort(loop_cells, transmitters.vertices)
                 loop_ind = np.r_[loop_cells[:, 0], loop_cells[-1, 1]]
-                tx_locs = transmitters.vertices[loop_ind, :]
-                tx_locs_lookup[k] = tx_locs
+                tx_locs.append(transmitters.vertices[loop_ind, :])
         else:
-            rx_lookup = {k: [k] for k in self.local_index}
-            tx_locs_lookup = {k: transmitters.vertices[k, :] for k in self.local_index}
+            rx_lookup = self.local_index[:, np.newaxis].tolist()
+            tx_locs = [transmitters.vertices[k, :] for k in self.local_index]
 
         wave_function = interp1d(
             (receivers.waveform[:, 0] - receivers.timing_mark)
             * self.params.unit_conversion,
             receivers.waveform[:, 1],
             fill_value="extrapolate",
         )
@@ -359,15 +368,15 @@
             waveform_function=wave_function, offTime=0.0
         )
 
         self.ordering = []
         tx_list = []
         rx_factory = ReceiversFactory(self.params)
         tx_factory = SourcesFactory(self.params)
-        for tx_id, rx_ids in rx_lookup.items():
+        for tx_locs, rx_ids in zip(tx_locs, rx_lookup):
             locs = receivers.vertices[rx_ids, :]
 
             rx_list = []
             for component_id, component in enumerate(data.components):
                 rx_obj = rx_factory.build(
                     locations=locs,
                     local_index=self.local_index,
@@ -378,17 +387,15 @@
                 rx_list.append(rx_obj)
 
                 for time_id in range(len(receivers.channels)):
                     for rx_id in rx_ids:
                         self.ordering.append([time_id, component_id, rx_id])
 
             tx_list.append(
-                tx_factory.build(
-                    rx_list, locations=tx_locs_lookup[tx_id], waveform=waveform
-                )
+                tx_factory.build(rx_list, locations=tx_locs, waveform=waveform)
             )
 
         return [tx_list]
 
     def _fem_arguments(self, data=None, mesh=None, channel=None):
         channels = np.array(data.entity.channels)
         frequencies = channels if channel is None else [channel]
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/locations.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/locations.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/models.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/models.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/topography.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/topography.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/utils.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/utils.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/components/windows.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/components/windows.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 #  may be used, copied, transmitted, and stored only in accordance with
 #  the terms of such license and with the inclusion of the above copyright
 #  notice.  This software and information or any other copies thereof may
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
-from .params import DirectCurrent2DParams
+from .params import DirectCurrent2DParams  # noqa: F401
 
 __all__ = ["DirectCurrent2DParams"]
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/direct_current/two_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,54 +16,47 @@
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 
 from __future__ import annotations
 
 from copy import deepcopy
 
-from simpeg_drivers import InversionBaseParams
-
+from ...params import Base2DParams
 from .constants import (
     default_ui_json,
     forward_defaults,
     inversion_defaults,
     validations,
 )
 
 
-class InducedPolarization3DParams(InversionBaseParams):
+class InducedPolarization2DParams(Base2DParams):
     """
-    Parameter class for electrical-induced polarization (IP) inversion.
+    Parameter class for electrical->induced polarization (IP) inversion.
     """
 
     _physical_property = "chargeability"
 
     def __init__(self, input_file=None, forward_only=False, **kwargs):
         self._default_ui_json = deepcopy(default_ui_json)
         self._forward_defaults = deepcopy(forward_defaults)
         self._inversion_defaults = deepcopy(inversion_defaults)
-        self._inversion_type = "induced polarization 3d"
+        self._inversion_type = "induced polarization 2d"
         self._validations = validations
         self._chargeability_channel_bool = None
         self._chargeability_channel = None
         self._chargeability_uncertainty = None
+        self._line_object = None
+        self._line_id = None
         self._conductivity_model_object = None
         self._conductivity_model = None
 
         super().__init__(input_file=input_file, forward_only=forward_only, **kwargs)
 
     @property
-    def inversion_type(self):
-        return self._inversion_type
-
-    @inversion_type.setter
-    def inversion_type(self, val):
-        self.setter_validator("inversion_type", val)
-
-    @property
     def chargeability_channel_bool(self):
         return self._chargeability_channel_bool
 
     @chargeability_channel_bool.setter
     def chargeability_channel_bool(self, val):
         self.setter_validator("chargeability_channel_bool", val)
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,47 +16,53 @@
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 
 from __future__ import annotations
 
 from copy import deepcopy
 
-from ...params import Base2DParams
+from simpeg_drivers import InversionBaseParams
+
 from .constants import (
     default_ui_json,
     forward_defaults,
     inversion_defaults,
     validations,
 )
 
 
-class InducedPolarization2DParams(Base2DParams):
+class InducedPolarization3DParams(InversionBaseParams):
     """
-    Parameter class for electrical->induced polarization (IP) inversion.
+    Parameter class for electrical-induced polarization (IP) inversion.
     """
 
     _physical_property = "chargeability"
 
     def __init__(self, input_file=None, forward_only=False, **kwargs):
         self._default_ui_json = deepcopy(default_ui_json)
         self._forward_defaults = deepcopy(forward_defaults)
         self._inversion_defaults = deepcopy(inversion_defaults)
-        self._inversion_type = "induced polarization 2d"
+        self._inversion_type = "induced polarization 3d"
         self._validations = validations
         self._chargeability_channel_bool = None
         self._chargeability_channel = None
         self._chargeability_uncertainty = None
-        self._line_object = None
-        self._line_id = None
-        self._conductivity_model_object = None
         self._conductivity_model = None
 
         super().__init__(input_file=input_file, forward_only=forward_only, **kwargs)
 
     @property
+    def inversion_type(self):
+        return self._inversion_type
+
+    @inversion_type.setter
+    def inversion_type(self, val):
+        self.setter_validator("inversion_type", val)
+
+    @property
     def chargeability_channel_bool(self):
         return self._chargeability_channel_bool
 
     @chargeability_channel_bool.setter
     def chargeability_channel_bool(self, val):
         self.setter_validator("chargeability_channel_bool", val)
 
@@ -73,21 +79,13 @@
         return self._chargeability_uncertainty
 
     @chargeability_uncertainty.setter
     def chargeability_uncertainty(self, val):
         self.setter_validator("chargeability_uncertainty", val, fun=self._uuid_promoter)
 
     @property
-    def conductivity_model_object(self):
-        return self._conductivity_model_object
-
-    @conductivity_model_object.setter
-    def conductivity_model_object(self, val):
-        self.setter_validator("conductivity_model_object", val, fun=self._uuid_promoter)
-
-    @property
     def conductivity_model(self):
         return self._conductivity_model
 
     @conductivity_model.setter
     def conductivity_model(self, val):
         self.setter_validator("conductivity_model", val, fun=self._uuid_promoter)
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electricals/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/frequency_domain/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/time_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/time_domain/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,21 +12,11 @@
 #  the terms of such license and with the inclusion of the above copyright
 #  notice.  This software and information or any other copies thereof may
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 
-from __future__ import annotations
+from .params import JointCrossGradientParams
 
-from simpeg_drivers.driver import InversionDriver
-
-from .constants import validations
-from .params import TimeDomainElectromagneticsParams
-
-
-class TimeDomainElectromagneticsDriver(InversionDriver):
-    _params_class = TimeDomainElectromagneticsParams
-    _validations = validations
-
-    def __init__(self, params: TimeDomainElectromagneticsParams):
-        super().__init__(params)
+# pylint: disable=unused-import
+# flake8: noqa
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/electromagnetics/time_domain/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         if getattr(self, "_data_misfit", None) is None and self.drivers is not None:
             objective_functions = []
             multipliers = []
             for label, driver in zip("abc", self.drivers):
                 if driver.data_misfit is not None:
                     objective_functions += driver.data_misfit.objfcts
                     multipliers += [
-                        getattr(self.params, f"group_{label}_multiplier")
+                        getattr(self.params, f"group_{label}_multiplier") ** 2.0
                     ] * len(driver.data_misfit.objfcts)
 
             self._data_misfit = ComboObjectiveFunction(
                 objfcts=objective_functions, multipliers=multipliers
             )
 
         return self._data_misfit
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 #  the terms of such license and with the inclusion of the above copyright
 #  notice.  This software and information or any other copies thereof may
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 
-from .params import JointCrossGradientParams
+from .magnetotellurics import MagnetotelluricsParams
+from .tipper import TipperParams
 
 # pylint: disable=unused-import
 # flake8: noqa
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,19 +179,24 @@
                         self._mapping[driver_pairs[0], mapping_a],
                         self._mapping[driver_pairs[1], mapping_b],
                     ]
                     reg_list.append(
                         CrossGradient(
                             self.inversion_mesh.mesh,
                             wires,
+                            normalize=True,
                             active_cells=self.models.active_cells,
                         )
                     )
+                    base_multipier = (
+                        reg_list[-1].regularization_mesh.base_length ** 4.0
+                    )  # Account for cross of length scale square
                     multipliers.append(
                         getattr(self.params, f"cross_gradient_weight_{label}")
+                        * base_multipier
                     )
 
         return ComboObjectiveFunction(objfcts=reg_list, multipliers=multipliers)
 
     @property
     def wires(self):
         """Model projections"""
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_cross_gradient/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/joint_surveys/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/joint/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/line_sweep/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/line_sweep/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,12 +12,11 @@
 #  the terms of such license and with the inclusion of the above copyright
 #  notice.  This software and information or any other copies thereof may
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 
-from .magnetotellurics import MagnetotelluricsParams
-from .tipper import TipperParams
+from .params import MagnetotelluricsParams
 
 # pylint: disable=unused-import
 # flake8: noqa
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 #  the terms of such license and with the inclusion of the above copyright
 #  notice.  This software and information or any other copies thereof may
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 
-from .params import MagnetotelluricsParams
+from .params import MagneticVectorParams
 
 # pylint: disable=unused-import
 # flake8: noqa
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/magnetotellurics/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/natural_sources/tipper/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/gravity/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_scalar/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,13 +10,11 @@
 #  This software is furnished pursuant to a written license agreement and
 #  may be used, copied, transmitted, and stored only in accordance with
 #  the terms of such license and with the inclusion of the above copyright
 #  notice.  This software and information or any other copies thereof may
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
-
-
-from .params import MagneticVectorParams
-
-# pylint: disable=unused-import
-# flake8: noqa
+#
+#  This file is part of simpeg_drivers package.
+#
+#  All rights reserved.
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/constants.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/driver.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/params.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/potential_fields/magnetic_vector/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/__init__.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/surveys.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/utils/surveys.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,32 @@
 from geoapps_utils.numerical import traveling_salesman
 from geoh5py import Workspace
 from geoh5py.objects import PotentialElectrode
 from scipy.spatial import cKDTree
 from SimPEG.survey import BaseSurvey
 
 
+def counter_clockwise_sort(segments: np.ndarray, vertices: np.ndarray) -> np.ndarray:
+    """
+    Sort segments in counter-clockwise order.
+
+    :param segments: Array of segment indices.
+    :param vertices: Array of vertices.
+
+    :return: Sorted segments.
+    """
+    deltas = vertices[segments[:, 1], :2] - vertices[segments[:, 0], :2]
+    cross = np.cross(deltas[:-1], deltas[1:])
+
+    if np.sign(np.mean(cross[cross != 0])) < 0:
+        segments = segments[::-1, ::-1]
+
+    return segments
+
+
 def compute_alongline_distance(points: np.ndarray, ordered: bool = True):
     """
     Convert from cartesian (x, y, values) points to (distance, values) locations.
 
     :param: points: Cartesian coordinates of points lying either roughly within a
         plane or a line.
     """
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/testing.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/utils/testing.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/utils.py` & `simpeg_drivers-0.1.0b5/simpeg_drivers/utils/utils.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/inversion_demo.geoh5` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/inversion_demo.geoh5`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_forward.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/fem_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/fem_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_forward.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/gravity_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/gravity_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998478835978836%*

 * *Differences: {"'cross_gradient_weight_a_b'": "{'value': 1.0}",*

 * * "'cross_gradient_weight_c_a'": "{'value': 1.0}",*

 * * "'cross_gradient_weight_c_b'": "{'value': 1.0}"}*

```diff
@@ -74,37 +74,37 @@
     "cross_gradient_weight_a_b": {
         "group": "Joint",
         "label": "A x B Coupling Scale",
         "lineEdit": false,
         "main": true,
         "min": 0.0,
         "tooltip": "Weight applied to the cross gradient regularizations (1: equal weight with the standard Smallness and Smoothness terms.)",
-        "value": 1000000.0
+        "value": 1.0
     },
     "cross_gradient_weight_c_a": {
         "dependency": "group_c",
         "dependencyType": "enabled",
         "group": "Joint",
         "label": "A x C Coupling Scale",
         "lineEdit": false,
         "main": true,
         "min": 0.0,
         "tooltip": "Weight applied to the cross gradient regularizations (1: equal weight with the standard Smallness and Smoothness terms.)",
-        "value": 1000000.0
+        "value": 1.0
     },
     "cross_gradient_weight_c_b": {
         "dependency": "group_c",
         "dependencyType": "enabled",
         "group": "Joint",
         "label": "B x C Coupling Scale",
         "lineEdit": false,
         "main": true,
         "min": 0.0,
         "tooltip": "Weight applied to the cross gradient regularizations (1: equal weight with the standard Smallness and Smoothness terms.)",
-        "value": 1000000.0
+        "value": 1.0
     },
     "distributed_workers": "",
     "every_iteration_bool": {
         "group": "Update sensitivity weights directive",
         "label": "Every iteration",
         "tooltip": "Update weights at every iteration",
         "value": true,
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997387669801462%*

 * *Differences: {"'lower_bound'": "{'enabled': True}"}*

```diff
@@ -471,15 +471,15 @@
     },
     "lower_bound": {
         "association": [
             "Cell",
             "Vertex"
         ],
         "dataType": "Float",
-        "enabled": false,
+        "enabled": true,
         "group": "Mesh and models",
         "isValue": true,
         "label": "Lower bound (SI)",
         "main": true,
         "optional": true,
         "parent": "mesh",
         "property": "",
```

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_forward.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tdem_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tdem_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_forward.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tipper_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_inversion.ui.json` & `simpeg_drivers-0.1.0b5/simpeg_drivers-assets/uijson/tipper_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/THIRD_PARTY_SOFTWARE.rst` & `simpeg_drivers-0.1.0b5/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b4/PKG-INFO` & `simpeg_drivers-0.1.0b5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpeg-drivers
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Application to run SimPEG inversions with geoh5 files from Geoscience Analyst.
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Benjamin Kary
 Maintainer-email: benjamink@mirageoscience.com
@@ -17,15 +17,16 @@
 Requires-Dist: discretize (>=0.10.0,<0.11.0)
 Requires-Dist: distributed (==2022.10.*)
 Requires-Dist: fsspec (==2022.*)
 Requires-Dist: geoana (>=0.4.0,<0.5.0)
 Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
-Requires-Dist: mira-simpeg (>=0.19.0.8rc1,<0.19.0.8.post999)
+Requires-Dist: matplotlib (>=3.7.1,<3.8.0)
+Requires-Dist: mira-simpeg (>=0.19.0.8rc3,<0.19.0.8.post999)
 Requires-Dist: mkl (==2022.1.*)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: octree-creation-app (>=0.1.0rc2,<0.2.0)
 Requires-Dist: pandas (>=2.2.1,<2.3.0)
 Requires-Dist: param-sweeps (>=0.1.7rc1,<0.2.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
 Requires-Dist: pydiso (>=0.0.3,<0.1.0)
```

