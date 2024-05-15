# Comparing `tmp/autotuning_methodology-1.0.0b1.tar.gz` & `tmp/autotuning_methodology-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotuning_methodology-1.0.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "autotuning_methodology-1.0.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autotuning_methodology-1.0.0b1.tar` & `autotuning_methodology-1.0.0b2.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0      112 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.coveragerc
--rw-r--r--   0        0        0     1424 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.github/workflows/build-test-python-package.yml
--rw-r--r--   0        0        0      573 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.github/workflows/publish-documentation.yml
--rw-r--r--   0        0        0     1227 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.github/workflows/publish-package.yml
--rwxr-xr-x   0        0        0     3571 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.gitignore
--rw-r--r--   0        0        0      144 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.vscode/extensions.json
--rw-r--r--   0        0        0      605 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/.vscode/settings.json
--rw-r--r--   0        0        0     1077 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     7328 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/README.md
--rw-r--r--   0        0        0     2597 2024-05-13 15:37:26.555070 autotuning_methodology-1.0.0b1/UML/.$Sequence Diagram.drawio.bkp
--rw-r--r--   0        0        0   302745 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0     2585 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/Sequence Diagram.drawio
--rw-r--r--   0        0        0    26889 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/classes.pdf
--rw-r--r--   0        0        0   303637 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/flowchart/.$flowchart.drawio.bkp
--rw-r--r--   0        0        0   303637 2024-05-13 15:37:26.559070 autotuning_methodology-1.0.0b1/UML/flowchart/flowchart.drawio
--rw-r--r--   0        0        0   315705 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_output_generation.png
--rw-r--r--   0        0        0   267296 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_performance_curve_generation.png
--rw-r--r--   0        0        0   131133 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
--rw-r--r--   0        0        0    95756 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_individual.png
--rw-r--r--   0        0        0     1074 2024-05-13 15:37:26.563070 autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plots.py
--rw-r--r--   0        0        0    15114 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/UML/packages.pdf
--rw-r--r--   0        0        0     5736 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
--rw-r--r--   0        0        0      634 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/Makefile
--rw-r--r--   0        0        0     1722 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/autotuning_methodology.rst
--rw-r--r--   0        0        0     2487 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/conf.py
--rw-r--r--   0        0        0     1669 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/getting_started.rst
--rw-r--r--   0        0        0      827 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/make.bat
--rw-r--r--   0        0        0      128 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/modules.rst
--rw-r--r--   0        0        0   315705 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/flowchart_output_generation.png
--rw-r--r--   0        0        0   267296 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/flowchart_performance_curve_generation.png
--rw-r--r--   0        0        0     5034 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/logo_autotuning_methodology.svg
--rw-r--r--   0        0        0    36351 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/logo_kernel_dashboard.svg
--rw-r--r--   0        0        0    42513 2024-05-13 15:37:26.567070 autotuning_methodology-1.0.0b1/docs/source/logo_kernel_launcher.svg
--rw-r--r--   0        0        0    39816 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/docs/source/logo_kernel_tuner.svg
--rwxr-xr-x   0        0        0      983 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/bootstrap_hyperparams.json
--rw-r--r--   0        0        0     1625 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/example_visualizations.json
--rw-r--r--   0        0        0     1971 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/methodology_paper_evaluation.json
--rw-r--r--   0        0        0     1647 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/milo_hotspot.json
--rw-r--r--   0        0        0     1403 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/presentation_comparison.json
--rw-r--r--   0        0        0     2364 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/simple_example.json
--rw-r--r--   0        0        0     1745 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/test_random_calculated.json
--rw-r--r--   0        0        0     1409 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/test_scatter.json
--rwxr-xr-x   0        0        0     2275 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/experiment_files/test_searchspace_algorithms.json
--rw-r--r--   0        0        0      132 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/.vscode/settings.json
--rwxr-xr-x   0        0        0    18897 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/bootstrap_hyperparams_visualizer.py
--rwxr-xr-x   0        0        0    19811 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/experiments_strategies.py
--rwxr-xr-x   0        0        0   119690 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/experiments_strategies_hyperparamtuning.py
--rwxr-xr-x   0        0        0     7475 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/generate_cachefile.py
--rw-r--r--   0        0        0    20608 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/max_draw_k_from_n.py
--rw-r--r--   0        0        0     3259 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/speedtest_index_performance.py
--rw-r--r--   0        0        0     1174 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/speedtest_python_reversed_nan_sort.py
--rwxr-xr-x   0        0        0     2545 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/try_BOtorch.py
--rwxr-xr-x   0        0        0     8426 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/try_GPytorch.py
--rw-r--r--   0        0        0    20822 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/extra/try_isotonic_regression.py
--rwxr-xr-x   0        0        0      435 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/mypy.ini
--rw-r--r--   0        0        0     1089 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/noxfile.py
--rwxr-xr-x   0        0        0       17 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/profilings/.gitignore
--rw-r--r--   0        0        0     2816 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0       42 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/__init__.py
--rw-r--r--   0        0        0    17647 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/baseline.py
--rwxr-xr-x   0        0        0     8418 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/caching.py
--rw-r--r--   0        0        0    51986 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/curves.py
--rwxr-xr-x   0        0        0     9764 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/experiments.py
--rwxr-xr-x   0        0        0    24377 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/runner.py
--rwxr-xr-x   0        0        0     4138 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/schema.json
--rw-r--r--   0        0        0    25701 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/searchspace_statistics.py
--rw-r--r--   0        0        0     1787 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/validators.py
--rwxr-xr-x   0        0        0    48490 2024-05-13 15:37:26.571071 autotuning_methodology-1.0.0b1/src/autotuning_methodology/visualize_experiments.py
--rw-r--r--   0        0        0  3269061 2024-05-13 15:37:26.579071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json
--rw-r--r--   0        0        0  3255846 2024-05-13 15:37:26.587071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json
--rw-r--r--   0        0        0  3483805 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
--rw-r--r--   0        0        0     2967 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
--rw-r--r--   0        0        0     1489 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test.json
--rw-r--r--   0        0        0     1476 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
--rw-r--r--   0        0        0     1465 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_cached.json
--rw-r--r--   0        0        0     1453 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json
--rw-r--r--   0        0        0     8913 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_run_experiment.py
--rw-r--r--   0        0        0     2934 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_visualization.py
--rw-r--r--   0        0        0     1978 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/release/test_toml_file.py
--rw-r--r--   0        0        0       34 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/unit/test_caching.py
--rw-r--r--   0        0        0     3464 2024-05-13 15:37:26.599071 autotuning_methodology-1.0.0b1/tests/autotuning_methodology/unit/test_curves.py
--rw-r--r--   0        0        0     9296 1970-01-01 00:00:00.000000 autotuning_methodology-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.coveragerc
+-rw-r--r--   0        0        0     1424 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.github/workflows/build-test-python-package.yml
+-rw-r--r--   0        0        0      658 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.github/workflows/publish-documentation.yml
+-rw-r--r--   0        0        0     1227 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.github/workflows/publish-package.yml
+-rwxr-xr-x   0        0        0     3571 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0      144 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.vscode/extensions.json
+-rw-r--r--   0        0        0      605 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/.vscode/settings.json
+-rw-r--r--   0        0        0     1077 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     7566 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/README.md
+-rw-r--r--   0        0        0     2597 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/.$Sequence Diagram.drawio.bkp
+-rw-r--r--   0        0        0   302745 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0     2585 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/Sequence Diagram.drawio
+-rw-r--r--   0        0        0    26889 2024-05-15 09:37:30.280802 autotuning_methodology-1.0.0b2/UML/classes.pdf
+-rw-r--r--   0        0        0   303637 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/.$flowchart.drawio.bkp
+-rw-r--r--   0        0        0   303637 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/flowchart.drawio
+-rw-r--r--   0        0        0   315705 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-15 09:37:30.284802 autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0   131133 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_aggregated.png
+-rw-r--r--   0        0        0    95756 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_individual.png
+-rw-r--r--   0        0        0     1074 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plots.py
+-rw-r--r--   0        0        0    15114 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/UML/packages.pdf
+-rw-r--r--   0        0        0     5736 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py
+-rw-r--r--   0        0        0      634 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/Makefile
+-rw-r--r--   0        0        0     1722 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/autotuning_methodology.rst
+-rw-r--r--   0        0        0     2541 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/conf.py
+-rw-r--r--   0        0        0     2225 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/contributing.rst
+-rw-r--r--   0        0        0     2409 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/getting_started.rst
+-rw-r--r--   0        0        0     1144 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-05-15 09:37:30.288802 autotuning_methodology-1.0.0b2/docs/make.bat
+-rw-r--r--   0        0        0   609663 2024-05-15 09:37:30.292802 autotuning_methodology-1.0.0b2/docs/source/example_aggregated.png
+-rw-r--r--   0        0        0   315705 2024-05-15 09:37:30.292802 autotuning_methodology-1.0.0b2/docs/source/flowchart_output_generation.png
+-rw-r--r--   0        0        0   267296 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/flowchart_performance_curve_generation.png
+-rw-r--r--   0        0        0     5034 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_autotuning_methodology.svg
+-rw-r--r--   0        0        0    36351 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_kernel_dashboard.svg
+-rw-r--r--   0        0        0    42513 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_kernel_launcher.svg
+-rw-r--r--   0        0        0    39816 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/docs/source/logo_kernel_tuner.svg
+-rwxr-xr-x   0        0        0      983 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/bootstrap_hyperparams.json
+-rw-r--r--   0        0        0     1625 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/example_visualizations.json
+-rw-r--r--   0        0        0     1971 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/methodology_paper_evaluation.json
+-rw-r--r--   0        0        0     1647 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/milo_hotspot.json
+-rw-r--r--   0        0        0     1403 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/presentation_comparison.json
+-rw-r--r--   0        0        0     2364 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/simple_example.json
+-rw-r--r--   0        0        0     1745 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/test_random_calculated.json
+-rw-r--r--   0        0        0     1409 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/test_scatter.json
+-rwxr-xr-x   0        0        0     2275 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/experiment_files/test_searchspace_algorithms.json
+-rw-r--r--   0        0        0      132 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/.vscode/settings.json
+-rwxr-xr-x   0        0        0    18897 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/bootstrap_hyperparams_visualizer.py
+-rwxr-xr-x   0        0        0    19811 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/experiments_strategies.py
+-rwxr-xr-x   0        0        0   119690 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/experiments_strategies_hyperparamtuning.py
+-rwxr-xr-x   0        0        0     7475 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/generate_cachefile.py
+-rw-r--r--   0        0        0    20608 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/max_draw_k_from_n.py
+-rw-r--r--   0        0        0     3259 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/speedtest_index_performance.py
+-rw-r--r--   0        0        0     1174 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/speedtest_python_reversed_nan_sort.py
+-rwxr-xr-x   0        0        0     2545 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/try_BOtorch.py
+-rwxr-xr-x   0        0        0     8426 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/try_GPytorch.py
+-rw-r--r--   0        0        0    20822 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/extra/try_isotonic_regression.py
+-rwxr-xr-x   0        0        0      435 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/mypy.ini
+-rw-r--r--   0        0        0     1089 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/noxfile.py
+-rwxr-xr-x   0        0        0       17 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/profilings/.gitignore
+-rw-r--r--   0        0        0     2816 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/__init__.py
+-rw-r--r--   0        0        0    17647 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/baseline.py
+-rwxr-xr-x   0        0        0     8418 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/caching.py
+-rw-r--r--   0        0        0    51986 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/curves.py
+-rwxr-xr-x   0        0        0     9764 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/experiments.py
+-rwxr-xr-x   0        0        0    24377 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/runner.py
+-rwxr-xr-x   0        0        0     4138 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/schema.json
+-rw-r--r--   0        0        0    25701 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/searchspace_statistics.py
+-rw-r--r--   0        0        0     1787 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/validators.py
+-rwxr-xr-x   0        0        0    48490 2024-05-15 09:37:30.296802 autotuning_methodology-1.0.0b2/src/autotuning_methodology/visualize_experiments.py
+-rw-r--r--   0        0        0  3269061 2024-05-15 09:37:30.308802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json
+-rw-r--r--   0        0        0  3255846 2024-05-15 09:37:30.312802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json
+-rw-r--r--   0        0        0  3483805 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json
+-rw-r--r--   0        0        0     2967 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py
+-rw-r--r--   0        0        0     1489 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test.json
+-rw-r--r--   0        0        0     1476 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json
+-rw-r--r--   0        0        0     1465 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_cached.json
+-rw-r--r--   0        0        0     1453 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json
+-rw-r--r--   0        0        0     8913 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_run_experiment.py
+-rw-r--r--   0        0        0     2934 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_visualization.py
+-rw-r--r--   0        0        0     1978 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/release/test_toml_file.py
+-rw-r--r--   0        0        0       34 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/unit/test_caching.py
+-rw-r--r--   0        0        0     3464 2024-05-15 09:37:30.324802 autotuning_methodology-1.0.0b2/tests/autotuning_methodology/unit/test_curves.py
+-rw-r--r--   0        0        0     9534 1970-01-01 00:00:00.000000 autotuning_methodology-1.0.0b2/PKG-INFO
```

### Comparing `autotuning_methodology-1.0.0b1/.github/workflows/build-test-python-package.yml` & `autotuning_methodology-1.0.0b2/.github/workflows/build-test-python-package.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/.github/workflows/publish-documentation.yml` & `autotuning_methodology-1.0.0b2/.github/workflows/publish-documentation.yml`

 * *Files 16% similar despite different names*

```diff
@@ -14,9 +14,11 @@
         environment:
             name: github-pages
             url: ${{ steps.deployment.outputs.page_url }}
         permissions:
             pages: write
             id-token: write
         steps:
+            - name: Setup Graphviz
+              uses: ts-graphviz/setup-graphviz@v2
             - id: deployment
               uses: sphinx-notes/pages@v3
```

### Comparing `autotuning_methodology-1.0.0b1/.github/workflows/publish-package.yml` & `autotuning_methodology-1.0.0b2/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/.gitignore` & `autotuning_methodology-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/.vscode/settings.json` & `autotuning_methodology-1.0.0b2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/LICENSE` & `autotuning_methodology-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/README.md` & `autotuning_methodology-1.0.0b2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 Plots outputted by this package are placed in a folder called `generated_plots` relative to the current working directory. 
 
 
 ## Pipeline
 The below schematics show the pipeline implemented by this tool as described in the paper. 
 
 <!-- <img width="100%" alt="flowchart performance curve generation" src="https://autotuningassociation.github.io/autotuning_methodology/_static/flowchart_performance_curve_generation.svg"> -->
-![flowchart performance curve generation](docs/source/flowchart_performance_curve_generation.png)
+![flowchart performance curve generation](https://github.com/AutoTuningAssociation/autotuning_methodology/blob/8af7773dea8a858f84a868b06c2695175e54fc05/docs/source/flowchart_performance_curve_generation.png?raw=true)
 The first flowchart shows the tranformation of raw, stochastic optimization algorithm data to a performance curve. 
 
 <!-- <img width="100%" alt="flowchart output generation" src="docs/source/flowchart_output_generation.svg"> -->
-![flowchart output generation](docs/source/flowchart_output_generation.png)
+![flowchart output generation](https://github.com/AutoTuningAssociation/autotuning_methodology/blob/8af7773dea8a858f84a868b06c2695175e54fc05/docs/source/flowchart_output_generation.png?raw=true)
 The second flowchart shows the adaption of performance curves of various optimization algorithms and search spaces to the desired output.
 
 
 ## Contributing
 
 ### Setup
 If you're looking to contribute to this package: welcome!
```

### Comparing `autotuning_methodology-1.0.0b1/UML/.$Sequence Diagram.drawio.bkp` & `autotuning_methodology-1.0.0b2/UML/.$Sequence Diagram.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b2/UML/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/Sequence Diagram.drawio` & `autotuning_methodology-1.0.0b2/UML/Sequence Diagram.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/classes.pdf` & `autotuning_methodology-1.0.0b2/UML/classes.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/flowchart/.$flowchart.drawio.bkp` & `autotuning_methodology-1.0.0b2/UML/flowchart/.$flowchart.drawio.bkp`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/flowchart/flowchart.drawio` & `autotuning_methodology-1.0.0b2/UML/flowchart/flowchart.drawio`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_output_generation.png` & `autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_output_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/flowchart/flowchart_performance_curve_generation.png` & `autotuning_methodology-1.0.0b2/UML/flowchart/flowchart_performance_curve_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_aggregated.png` & `autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_aggregated.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plot_individual.png` & `autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plot_individual.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/flowchart/mini_plots/flowchart_plots.py` & `autotuning_methodology-1.0.0b2/UML/flowchart/mini_plots/flowchart_plots.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/UML/packages.pdf` & `autotuning_methodology-1.0.0b2/UML/packages.pdf`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py` & `autotuning_methodology-1.0.0b2/cached_data_used/cachefiles/ktt_values_to_kerneltuner.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/Makefile` & `autotuning_methodology-1.0.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/autotuning_methodology.rst` & `autotuning_methodology-1.0.0b2/docs/autotuning_methodology.rst`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/conf.py` & `autotuning_methodology-1.0.0b2/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,45 +6,48 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
+import os
+import sys
 import time
 
 from sphinx_pyproject import SphinxConfig
 
-# sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, os.path.abspath(".."))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 # import data from pyproject.toml using https://github.com/sphinx-toolbox/sphinx-pyproject
 # additional data can be added with `[tool.sphinx-pyproject]` and retrieved with `config['']`.
 config = SphinxConfig("../pyproject.toml")  # add `, globalns=globals()` to directly insert in namespace
 year = time.strftime("%Y")
 
 project = "Autotuning Methodology"
 author = config.author
-copyright = f"{year}, {author}"
+copyright = f"2022-{year}, {author}"
 version = config.version  # major version (e.g. 2.6)
 release = config.version  # full version (e.g. 2.6rc1)
 
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.viewcode",
     "sphinx.ext.napoleon",
     "sphinx.ext.graphviz",
     "sphinx.ext.inheritance_diagram",
+    "sphinx.ext.githubpages",
 ]
 autosummary_generate = True  # Turn on sphinx.ext.autosummary
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 add_module_names = False
 toc_object_entries_show_parents = "hide"
```

### Comparing `autotuning_methodology-1.0.0b1/docs/make.bat` & `autotuning_methodology-1.0.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/source/flowchart_output_generation.png` & `autotuning_methodology-1.0.0b2/docs/source/flowchart_output_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/source/flowchart_performance_curve_generation.png` & `autotuning_methodology-1.0.0b2/docs/source/flowchart_performance_curve_generation.png`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/source/logo_autotuning_methodology.svg` & `autotuning_methodology-1.0.0b2/docs/source/logo_autotuning_methodology.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/source/logo_kernel_dashboard.svg` & `autotuning_methodology-1.0.0b2/docs/source/logo_kernel_dashboard.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/source/logo_kernel_launcher.svg` & `autotuning_methodology-1.0.0b2/docs/source/logo_kernel_launcher.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/docs/source/logo_kernel_tuner.svg` & `autotuning_methodology-1.0.0b2/docs/source/logo_kernel_tuner.svg`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/bootstrap_hyperparams.json` & `autotuning_methodology-1.0.0b2/experiment_files/bootstrap_hyperparams.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/example_visualizations.json` & `autotuning_methodology-1.0.0b2/experiment_files/example_visualizations.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/methodology_paper_evaluation.json` & `autotuning_methodology-1.0.0b2/experiment_files/methodology_paper_evaluation.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/milo_hotspot.json` & `autotuning_methodology-1.0.0b2/experiment_files/milo_hotspot.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/presentation_comparison.json` & `autotuning_methodology-1.0.0b2/experiment_files/presentation_comparison.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/simple_example.json` & `autotuning_methodology-1.0.0b2/experiment_files/simple_example.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/test_random_calculated.json` & `autotuning_methodology-1.0.0b2/experiment_files/test_random_calculated.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/test_scatter.json` & `autotuning_methodology-1.0.0b2/experiment_files/test_scatter.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/experiment_files/test_searchspace_algorithms.json` & `autotuning_methodology-1.0.0b2/experiment_files/test_searchspace_algorithms.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/bootstrap_hyperparams_visualizer.py` & `autotuning_methodology-1.0.0b2/extra/bootstrap_hyperparams_visualizer.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/experiments_strategies.py` & `autotuning_methodology-1.0.0b2/extra/experiments_strategies.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/experiments_strategies_hyperparamtuning.py` & `autotuning_methodology-1.0.0b2/extra/experiments_strategies_hyperparamtuning.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/generate_cachefile.py` & `autotuning_methodology-1.0.0b2/extra/generate_cachefile.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/max_draw_k_from_n.py` & `autotuning_methodology-1.0.0b2/extra/max_draw_k_from_n.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/speedtest_index_performance.py` & `autotuning_methodology-1.0.0b2/extra/speedtest_index_performance.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/speedtest_python_reversed_nan_sort.py` & `autotuning_methodology-1.0.0b2/extra/speedtest_python_reversed_nan_sort.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/try_BOtorch.py` & `autotuning_methodology-1.0.0b2/extra/try_BOtorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/try_GPytorch.py` & `autotuning_methodology-1.0.0b2/extra/try_GPytorch.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/extra/try_isotonic_regression.py` & `autotuning_methodology-1.0.0b2/extra/try_isotonic_regression.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/noxfile.py` & `autotuning_methodology-1.0.0b2/noxfile.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/pyproject.toml` & `autotuning_methodology-1.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project] # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 name = "autotuning_methodology"
-version = "1.0.0b1"
+version = "1.0.0b2"
 authors = [{ name = "Floris-Jan Willemsen", email = "fjwillemsen97@gmail.com" }]
-description = "Software package easing implementation of the guidelines of the 2023 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'."
+description = "Software package easing implementation of the guidelines of the 2024 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'."
 keywords = ["autotuning", "auto-tuning", "methodology", "scientific"]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -31,17 +31,17 @@
     "nonconformist >= 2.1.0",
     "kernel_tuner >= 1.0.0b5",
 ]
 
 [project.optional-dependencies]
 dev = ["pylint >=2.14.4", "black >= 23.3.0"]
 docs = [
-    "sphinx >= 6.2.1",
-    "sphinx_rtd_theme >= 1.2.0",
-    "sphinx-pyproject >= 0.1.0",
+    "sphinx >= 7.2.1",
+    "sphinx_rtd_theme >= 2.0.0",
+    "sphinx-pyproject >= 0.3.0",
 ]
 test = [
     "ruff >= 0.0.263",
     "pep440 >= 0.1.2",
     "pytest >= 7.3.1",
     "pytest-cov >= 4.0.0",
     "nox >= 2023.4.22",
```

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/baseline.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/baseline.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/caching.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/caching.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/curves.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/curves.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/experiments.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/experiments.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/runner.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/runner.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/schema.json` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/schema.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/searchspace_statistics.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/searchspace_statistics.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/validators.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/validators.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/src/autotuning_methodology/visualize_experiments.py` & `autotuning_methodology-1.0.0b2/src/autotuning_methodology/visualize_experiments.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~0.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/import_runs/t~'ktt'd~'mock_gpu'k~'mocktest_kernel_convolution's~'profile_searcher'r~1.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mock_gpu.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/mocktest_kernel_convolution.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test.json` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_bad_kernel_path.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_cached.json` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_cached.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/mockfiles/test_import_runs.json`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_run_experiment.py` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_run_experiment.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/integration/test_visualization.py` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/integration/test_visualization.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/release/test_toml_file.py` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/release/test_toml_file.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/tests/autotuning_methodology/unit/test_curves.py` & `autotuning_methodology-1.0.0b2/tests/autotuning_methodology/unit/test_curves.py`

 * *Files identical despite different names*

### Comparing `autotuning_methodology-1.0.0b1/PKG-INFO` & `autotuning_methodology-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: autotuning_methodology
-Version: 1.0.0b1
-Summary: Software package easing implementation of the guidelines of the 2023 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'.
+Version: 1.0.0b2
+Summary: Software package easing implementation of the guidelines of the 2024 paper 'A Methodology for Comparing Auto-Tuning Optimization Algorithms'.
 Keywords: autotuning,auto-tuning,methodology,scientific
 Author-email: Floris-Jan Willemsen <fjwillemsen97@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -20,17 +20,17 @@
 Requires-Dist: yappi >= 1.4.0
 Requires-Dist: progressbar2 >= 4.2.0
 Requires-Dist: jsonschema >= 4.17.3
 Requires-Dist: nonconformist >= 2.1.0
 Requires-Dist: kernel_tuner >= 1.0.0b5
 Requires-Dist: pylint >=2.14.4 ; extra == "dev"
 Requires-Dist: black >= 23.3.0 ; extra == "dev"
-Requires-Dist: sphinx >= 6.2.1 ; extra == "docs"
-Requires-Dist: sphinx_rtd_theme >= 1.2.0 ; extra == "docs"
-Requires-Dist: sphinx-pyproject >= 0.1.0 ; extra == "docs"
+Requires-Dist: sphinx >= 7.2.1 ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme >= 2.0.0 ; extra == "docs"
+Requires-Dist: sphinx-pyproject >= 0.3.0 ; extra == "docs"
 Requires-Dist: ruff >= 0.0.263 ; extra == "test"
 Requires-Dist: pep440 >= 0.1.2 ; extra == "test"
 Requires-Dist: pytest >= 7.3.1 ; extra == "test"
 Requires-Dist: pytest-cov >= 4.0.0 ; extra == "test"
 Requires-Dist: nox >= 2023.4.22 ; extra == "test"
 Requires-Dist: crepes >= 0.2.0 ; extra == "test"
 Requires-Dist: tomli >= 2.0.1 ; extra == "test"
@@ -91,19 +91,19 @@
 Plots outputted by this package are placed in a folder called `generated_plots` relative to the current working directory. 
 
 
 ## Pipeline
 The below schematics show the pipeline implemented by this tool as described in the paper. 
 
 <!-- <img width="100%" alt="flowchart performance curve generation" src="https://autotuningassociation.github.io/autotuning_methodology/_static/flowchart_performance_curve_generation.svg"> -->
-![flowchart performance curve generation](docs/source/flowchart_performance_curve_generation.png)
+![flowchart performance curve generation](https://github.com/AutoTuningAssociation/autotuning_methodology/blob/8af7773dea8a858f84a868b06c2695175e54fc05/docs/source/flowchart_performance_curve_generation.png?raw=true)
 The first flowchart shows the tranformation of raw, stochastic optimization algorithm data to a performance curve. 
 
 <!-- <img width="100%" alt="flowchart output generation" src="docs/source/flowchart_output_generation.svg"> -->
-![flowchart output generation](docs/source/flowchart_output_generation.png)
+![flowchart output generation](https://github.com/AutoTuningAssociation/autotuning_methodology/blob/8af7773dea8a858f84a868b06c2695175e54fc05/docs/source/flowchart_output_generation.png?raw=true)
 The second flowchart shows the adaption of performance curves of various optimization algorithms and search spaces to the desired output.
 
 
 ## Contributing
 
 ### Setup
 If you're looking to contribute to this package: welcome!
```

