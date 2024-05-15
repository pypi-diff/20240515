# Comparing `tmp/prtpy-0.8.2.tar.gz` & `tmp/prtpy-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prtpy-0.8.2.tar", last modified: Thu Jan 12 10:41:28 2023, max compression
+gzip compressed data, was "prtpy-0.8.3.tar", last modified: Wed May 15 10:57:14 2024, max compression
```

## Comparing `prtpy-0.8.2.tar` & `prtpy-0.8.3.tar`

### file list

```diff
@@ -1,127 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.130366 prtpy-0.8.2/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.020659 prtpy-0.8.2/.pytest_cache/
--rw-rw-rw-   0        0        0      310 2022-07-10 11:39:19.000000 prtpy-0.8.2/.pytest_cache/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.955793 prtpy-0.8.2/.venv310/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.956803 prtpy-0.8.2/.venv310/Lib/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.958785 prtpy-0.8.2/.venv310/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.022655 prtpy-0.8.2/.venv310/Lib/site-packages/experiments_csv/
--rw-rw-rw-   0        0        0        9 2022-07-12 07:43:23.000000 prtpy-0.8.2/.venv310/Lib/site-packages/experiments_csv/VERSION
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.959781 prtpy-0.8.2/.venv310/Lib/site-packages/scipy/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.960779 prtpy-0.8.2/.venv310/Lib/site-packages/scipy/fft/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.024647 prtpy-0.8.2/.venv310/Lib/site-packages/scipy/fft/_pocketfft/
--rw-rw-rw-   0        0        0     1498 2022-07-11 06:53:31.000000 prtpy-0.8.2/.venv310/Lib/site-packages/scipy/fft/_pocketfft/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.962773 prtpy-0.8.2/.venv38/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.963770 prtpy-0.8.2/.venv38/Lib/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.965818 prtpy-0.8.2/.venv38/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.026642 prtpy-0.8.2/.venv38/Lib/site-packages/prtpy/
--rw-rw-rw-   0        0        0        7 2022-07-10 12:29:11.000000 prtpy-0.8.2/.venv38/Lib/site-packages/prtpy/VERSION
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.965818 prtpy-0.8.2/.venv38/Lib/site-packages/scipy/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.966802 prtpy-0.8.2/.venv38/Lib/site-packages/scipy/fft/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.028636 prtpy-0.8.2/.venv38/Lib/site-packages/scipy/fft/_pocketfft/
--rw-rw-rw-   0        0        0     1498 2022-07-10 12:28:59.000000 prtpy-0.8.2/.venv38/Lib/site-packages/scipy/fft/_pocketfft/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.968797 prtpy-0.8.2/.venv38linux/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.969802 prtpy-0.8.2/.venv38linux/lib/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.970792 prtpy-0.8.2/.venv38linux/lib/python3.8/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.971804 prtpy-0.8.2/.venv38linux/lib/python3.8/site-packages/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.030631 prtpy-0.8.2/.venv38linux/lib/python3.8/site-packages/cylp/
--rw-rw-rw-   0        0        0        7 2022-02-15 15:32:40.000000 prtpy-0.8.2/.venv38linux/lib/python3.8/site-packages/cylp/VERSION
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.972786 prtpy-0.8.2/.venv38linux/lib/python3.8/site-packages/scipy/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.974780 prtpy-0.8.2/.venv38linux/lib/python3.8/site-packages/scipy/fft/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.032626 prtpy-0.8.2/.venv38linux/lib/python3.8/site-packages/scipy/fft/_pocketfft/
--rw-rw-rw-   0        0        0     1498 2022-02-15 15:32:28.000000 prtpy-0.8.2/.venv38linux/lib/python3.8/site-packages/scipy/fft/_pocketfft/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.975783 prtpy-0.8.2/.venv39/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.976776 prtpy-0.8.2/.venv39/Lib/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.997725 prtpy-0.8.2/.venv39/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.034621 prtpy-0.8.2/.venv39/Lib/site-packages/Markdown-3.3.6.dist-info/
--rw-rw-rw-   0        0        0     1645 2022-02-14 14:03:12.000000 prtpy-0.8.2/.venv39/Lib/site-packages/Markdown-3.3.6.dist-info/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.035618 prtpy-0.8.2/.venv39/Lib/site-packages/black-22.1.0.dist-info/
--rw-rw-rw-   0        0        0     7990 2022-02-14 12:30:10.000000 prtpy-0.8.2/.venv39/Lib/site-packages/black-22.1.0.dist-info/AUTHORS.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.037613 prtpy-0.8.2/.venv39/Lib/site-packages/cvxpy_leximin/
--rw-rw-rw-   0        0        0        7 2022-02-17 22:56:26.000000 prtpy-0.8.2/.venv39/Lib/site-packages/cvxpy_leximin/VERSION
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.039608 prtpy-0.8.2/.venv39/Lib/site-packages/cylp/
--rw-rw-rw-   0        0        0        7 2022-02-13 19:58:44.000000 prtpy-0.8.2/.venv39/Lib/site-packages/cylp/VERSION
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.982760 prtpy-0.8.2/.venv39/Lib/site-packages/debugpy/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.983775 prtpy-0.8.2/.venv39/Lib/site-packages/debugpy/_vendored/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.984754 prtpy-0.8.2/.venv39/Lib/site-packages/debugpy/_vendored/pydevd/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.985751 prtpy-0.8.2/.venv39/Lib/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.041604 prtpy-0.8.2/.venv39/Lib/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/
--rw-rw-rw-   0        0        0     1212 2022-02-14 14:03:03.000000 prtpy-0.8.2/.venv39/Lib/site-packages/debugpy/_vendored/pydevd/pydevd_plugins/extensions/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.043597 prtpy-0.8.2/.venv39/Lib/site-packages/ipykernel-6.9.0.dist-info/
--rw-rw-rw-   0        0        0     2835 2022-02-14 14:03:16.000000 prtpy-0.8.2/.venv39/Lib/site-packages/ipykernel-6.9.0.dist-info/COPYING.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.045592 prtpy-0.8.2/.venv39/Lib/site-packages/jupyter_client-7.1.2.dist-info/
--rw-rw-rw-   0        0        0     2885 2022-02-14 14:03:12.000000 prtpy-0.8.2/.venv39/Lib/site-packages/jupyter_client-7.1.2.dist-info/COPYING.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.047588 prtpy-0.8.2/.venv39/Lib/site-packages/jupyter_core-4.9.1.dist-info/
--rw-rw-rw-   0        0        0     2936 2022-02-14 14:03:07.000000 prtpy-0.8.2/.venv39/Lib/site-packages/jupyter_core-4.9.1.dist-info/COPYING.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.990741 prtpy-0.8.2/.venv39/Lib/site-packages/nbconvert/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.049581 prtpy-0.8.2/.venv39/Lib/site-packages/nbconvert/templates/
--rw-rw-rw-   0        0        0      318 2022-02-14 14:03:17.000000 prtpy-0.8.2/.venv39/Lib/site-packages/nbconvert/templates/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.051575 prtpy-0.8.2/.venv39/Lib/site-packages/nbconvert/templates/skeleton/
--rw-rw-rw-   0        0        0      513 2022-02-14 14:03:17.000000 prtpy-0.8.2/.venv39/Lib/site-packages/nbconvert/templates/skeleton/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.054567 prtpy-0.8.2/.venv39/Lib/site-packages/nbformat-5.1.3.dist-info/
--rw-rw-rw-   0        0        0     2888 2022-02-14 14:03:11.000000 prtpy-0.8.2/.venv39/Lib/site-packages/nbformat-5.1.3.dist-info/COPYING.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.056567 prtpy-0.8.2/.venv39/Lib/site-packages/pyzmq-22.3.0.dist-info/
--rw-rw-rw-   0        0        0     4915 2022-02-14 14:02:55.000000 prtpy-0.8.2/.venv39/Lib/site-packages/pyzmq-22.3.0.dist-info/AUTHORS.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.995725 prtpy-0.8.2/.venv39/Lib/site-packages/scipy/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:27.996727 prtpy-0.8.2/.venv39/Lib/site-packages/scipy/fft/
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.058558 prtpy-0.8.2/.venv39/Lib/site-packages/scipy/fft/_pocketfft/
--rw-rw-rw-   0        0        0     1498 2022-02-13 19:47:55.000000 prtpy-0.8.2/.venv39/Lib/site-packages/scipy/fft/_pocketfft/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.060553 prtpy-0.8.2/.venv39/Lib/site-packages/traitlets-5.1.1.dist-info/
--rw-rw-rw-   0        0        0     2957 2022-02-14 14:02:54.000000 prtpy-0.8.2/.venv39/Lib/site-packages/traitlets-5.1.1.dist-info/COPYING.md
--rw-rw-rw-   0        0        0      734 2022-10-24 13:53:11.000000 prtpy-0.8.2/INSTALL.md
--rw-rw-rw-   0        0        0     1055 2022-02-10 20:36:52.000000 prtpy-0.8.2/LICENSE
--rw-rw-rw-   0        0        0      107 2022-02-10 14:55:42.000000 prtpy-0.8.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4620 2023-01-12 10:41:28.129369 prtpy-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     4076 2022-07-12 07:40:04.000000 prtpy-0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.076508 prtpy-0.8.2/examples/
--rw-rw-rw-   0        0        0     1779 2022-07-10 22:29:50.000000 prtpy-0.8.2/examples/anytime_algorithm_demo.md
--rw-rw-rw-   0        0        0      941 2022-07-10 22:24:36.000000 prtpy-0.8.2/examples/covering_algorithms.md
--rw-rw-rw-   0        0        0     1179 2022-07-10 22:29:50.000000 prtpy-0.8.2/examples/input_formats.md
--rw-rw-rw-   0        0        0     4812 2022-07-10 22:24:41.000000 prtpy-0.8.2/examples/maximin_share_demo.md
--rw-rw-rw-   0        0        0     2680 2022-07-10 22:24:42.000000 prtpy-0.8.2/examples/objectives.md
--rw-rw-rw-   0        0        0     1332 2022-07-10 22:24:42.000000 prtpy-0.8.2/examples/output_formats.md
--rw-rw-rw-   0        0        0     1385 2022-07-10 22:24:43.000000 prtpy-0.8.2/examples/packing_algorithms.md
--rw-rw-rw-   0        0        0     4798 2022-07-10 22:30:14.000000 prtpy-0.8.2/examples/partitioning_algorithms.md
--rw-rw-rw-   0        0        0     2385 2022-07-11 06:37:32.000000 prtpy-0.8.2/examples/wmms_demo.md
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.086487 prtpy-0.8.2/prtpy/
--rw-rw-rw-   0        0        0        9 2023-01-12 10:39:56.000000 prtpy-0.8.2/prtpy/VERSION
--rw-rw-rw-   0        0        0     4300 2022-07-10 22:18:18.000000 prtpy-0.8.2/prtpy/__init__.py
--rw-rw-rw-   0        0        0    15249 2022-11-17 07:55:40.000000 prtpy-0.8.2/prtpy/binners.py
--rw-rw-rw-   0        0        0     3544 2022-07-01 08:25:19.000000 prtpy-0.8.2/prtpy/inclusion_exclusion_tree.py
--rw-rw-rw-   0        0        0     7963 2022-07-04 09:39:55.000000 prtpy-0.8.2/prtpy/objectives.py
--rw-rw-rw-   0        0        0     4341 2022-07-11 06:43:39.000000 prtpy-0.8.2/prtpy/outputtypes.py
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.105431 prtpy-0.8.2/prtpy/packing/
--rw-rw-rw-   0        0        0        0 2022-07-10 11:40:26.000000 prtpy-0.8.2/prtpy/packing/__init__.py
--rw-rw-rw-   0        0        0     3539 2022-07-10 21:47:13.000000 prtpy-0.8.2/prtpy/packing/adaptors.py
--rw-rw-rw-   0        0        0     2348 2022-07-10 22:40:33.000000 prtpy-0.8.2/prtpy/packing/best_fit.py
--rw-rw-rw-   0        0        0     9111 2022-07-10 22:43:13.000000 prtpy-0.8.2/prtpy/packing/bin_completion.py
--rw-rw-rw-   0        0        0    12837 2022-07-10 21:42:18.000000 prtpy-0.8.2/prtpy/packing/bin_completion_utils.py
--rw-rw-rw-   0        0        0     7431 2022-07-10 21:25:00.000000 prtpy-0.8.2/prtpy/packing/cflz_covering.py
--rw-rw-rw-   0        0        0     4450 2022-07-10 21:44:38.000000 prtpy-0.8.2/prtpy/packing/first_fit.py
--rw-rw-rw-   0        0        0     3147 2022-07-10 21:47:05.000000 prtpy-0.8.2/prtpy/packing/greedy_covering.py
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.126376 prtpy-0.8.2/prtpy/partitioning/
--rw-rw-rw-   0        0        0        0 2022-07-10 11:38:15.000000 prtpy-0.8.2/prtpy/partitioning/__init__.py
--rw-rw-rw-   0        0        0     7374 2022-07-12 08:28:00.000000 prtpy-0.8.2/prtpy/partitioning/adaptors.py
--rw-rw-rw-   0        0        0     1789 2022-07-10 18:39:24.000000 prtpy-0.8.2/prtpy/partitioning/balanced.py
--rw-rw-rw-   0        0        0     8707 2022-07-10 21:46:46.000000 prtpy-0.8.2/prtpy/partitioning/cbldm.py
--rw-rw-rw-   0        0        0    12752 2022-10-24 13:39:51.000000 prtpy-0.8.2/prtpy/partitioning/complete_greedy.py
--rw-rw-rw-   0        0        0     9257 2022-07-11 06:45:16.000000 prtpy-0.8.2/prtpy/partitioning/complete_karmarkar_karp_sy.py
--rw-rw-rw-   0        0        0     7416 2022-12-06 13:00:25.000000 prtpy-0.8.2/prtpy/partitioning/dynamic_programming.py
--rw-rw-rw-   0        0        0     2306 2022-07-10 20:23:34.000000 prtpy-0.8.2/prtpy/partitioning/greedy.py
--rw-rw-rw-   0        0        0     6684 2022-12-10 19:41:16.000000 prtpy-0.8.2/prtpy/partitioning/integer_programming.py
--rw-rw-rw-   0        0        0     5607 2022-07-10 21:46:20.000000 prtpy-0.8.2/prtpy/partitioning/karmarkar_karp_sy.py
--rw-rw-rw-   0        0        0     3580 2022-10-24 13:40:45.000000 prtpy-0.8.2/prtpy/partitioning/multifit.py
--rw-rw-rw-   0        0        0     7569 2022-07-10 21:38:17.000000 prtpy-0.8.2/prtpy/partitioning/recursive_number_partitioning_sy.py
--rw-rw-rw-   0        0        0     1632 2022-07-10 20:45:34.000000 prtpy-0.8.2/prtpy/partitioning/roundrobin.py
--rw-rw-rw-   0        0        0     6748 2022-07-10 21:43:01.000000 prtpy-0.8.2/prtpy/partitioning/sequential_number_partitioning_sy.py
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.092466 prtpy-0.8.2/prtpy.egg-info/
--rw-rw-rw-   0        0        0     4620 2023-01-12 10:41:21.000000 prtpy-0.8.2/prtpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2625 2023-01-12 10:41:27.000000 prtpy-0.8.2/prtpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 10:41:21.000000 prtpy-0.8.2/prtpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-01-12 10:41:21.000000 prtpy-0.8.2/prtpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-12 10:41:21.000000 prtpy-0.8.2/prtpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      331 2022-07-10 15:55:56.000000 prtpy-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-01 10:37:03.000000 prtpy-0.8.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-12 10:41:28.130366 prtpy-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1664 2022-07-12 07:39:51.000000 prtpy-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-12 10:41:28.128371 prtpy-0.8.2/simulations/
--rw-rw-rw-   0        0        0      186 2022-07-12 07:40:07.000000 prtpy-0.8.2/simulations/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.935709 prtpy-0.8.3/
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.783710 prtpy-0.8.3/.pytest_cache/
+-rw-rw-rw-   0        0        0      303 2023-01-16 19:04:48.000000 prtpy-0.8.3/.pytest_cache/README.md
+-rw-rw-rw-   0        0        0      734 2022-10-24 13:53:11.000000 prtpy-0.8.3/INSTALL.md
+-rw-rw-rw-   0        0        0     1055 2022-02-10 20:36:52.000000 prtpy-0.8.3/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-02-10 14:55:42.000000 prtpy-0.8.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4777 2024-05-15 10:57:14.935709 prtpy-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4073 2023-01-21 17:01:37.000000 prtpy-0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.874049 prtpy-0.8.3/examples/
+-rw-rw-rw-   0        0        0     1779 2022-07-10 22:29:50.000000 prtpy-0.8.3/examples/anytime_algorithm_demo.md
+-rw-rw-rw-   0        0        0      941 2022-07-10 22:24:36.000000 prtpy-0.8.3/examples/covering_algorithms.md
+-rw-rw-rw-   0        0        0     1179 2022-07-10 22:29:50.000000 prtpy-0.8.3/examples/input_formats.md
+-rw-rw-rw-   0        0        0     4812 2022-07-10 22:24:41.000000 prtpy-0.8.3/examples/maximin_share_demo.md
+-rw-rw-rw-   0        0        0     2680 2022-07-10 22:24:42.000000 prtpy-0.8.3/examples/objectives.md
+-rw-rw-rw-   0        0        0     1332 2022-07-10 22:24:42.000000 prtpy-0.8.3/examples/output_formats.md
+-rw-rw-rw-   0        0        0     1385 2022-07-10 22:24:43.000000 prtpy-0.8.3/examples/packing_algorithms.md
+-rw-rw-rw-   0        0        0     4798 2022-07-10 22:30:14.000000 prtpy-0.8.3/examples/partitioning_algorithms.md
+-rw-rw-rw-   0        0        0     2385 2022-07-11 06:37:32.000000 prtpy-0.8.3/examples/wmms_demo.md
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.881617 prtpy-0.8.3/prtpy/
+-rw-rw-rw-   0        0        0        7 2024-05-15 10:55:52.000000 prtpy-0.8.3/prtpy/VERSION
+-rw-rw-rw-   0        0        0     3240 2023-01-21 17:01:37.000000 prtpy-0.8.3/prtpy/__init__.py
+-rw-rw-rw-   0        0        0    15533 2024-05-15 10:45:20.000000 prtpy-0.8.3/prtpy/binners.py
+-rw-rw-rw-   0        0        0     3544 2022-07-01 08:25:19.000000 prtpy-0.8.3/prtpy/inclusion_exclusion_tree.py
+-rw-rw-rw-   0        0        0     9946 2024-05-15 10:50:38.000000 prtpy-0.8.3/prtpy/objectives.py
+-rw-rw-rw-   0        0        0     4341 2022-07-11 06:43:39.000000 prtpy-0.8.3/prtpy/outputtypes.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.910885 prtpy-0.8.3/prtpy/packing/
+-rw-rw-rw-   0        0        0        0 2022-07-10 11:40:26.000000 prtpy-0.8.3/prtpy/packing/__init__.py
+-rw-rw-rw-   0        0        0     3539 2022-07-10 21:47:13.000000 prtpy-0.8.3/prtpy/packing/adaptors.py
+-rw-rw-rw-   0        0        0     2348 2022-07-10 22:40:33.000000 prtpy-0.8.3/prtpy/packing/best_fit.py
+-rw-rw-rw-   0        0        0     9472 2023-02-01 13:55:27.000000 prtpy-0.8.3/prtpy/packing/bin_completion.py
+-rw-rw-rw-   0        0        0    12837 2022-07-10 21:42:18.000000 prtpy-0.8.3/prtpy/packing/bin_completion_utils.py
+-rw-rw-rw-   0        0        0     7431 2022-07-10 21:25:00.000000 prtpy-0.8.3/prtpy/packing/cflz_covering.py
+-rw-rw-rw-   0        0        0     4450 2022-07-10 21:44:38.000000 prtpy-0.8.3/prtpy/packing/first_fit.py
+-rw-rw-rw-   0        0        0     3147 2022-07-10 21:47:05.000000 prtpy-0.8.3/prtpy/packing/greedy_covering.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.922093 prtpy-0.8.3/prtpy/partitioning/
+-rw-rw-rw-   0        0        0     4231 2023-02-01 13:56:53.000000 prtpy-0.8.3/prtpy/partitioning/Horowitz_And_Sahni.py
+-rw-rw-rw-   0        0        0     2731 2023-02-01 13:57:03.000000 prtpy-0.8.3/prtpy/partitioning/Schroeppel_Shamir.py
+-rw-rw-rw-   0        0        0        0 2022-07-10 11:38:15.000000 prtpy-0.8.3/prtpy/partitioning/__init__.py
+-rw-rw-rw-   0        0        0     7374 2022-07-12 08:28:00.000000 prtpy-0.8.3/prtpy/partitioning/adaptors.py
+-rw-rw-rw-   0        0        0     1789 2022-07-10 18:39:24.000000 prtpy-0.8.3/prtpy/partitioning/balanced.py
+-rw-rw-rw-   0        0        0     8707 2022-07-10 21:46:46.000000 prtpy-0.8.3/prtpy/partitioning/cbldm.py
+-rw-rw-rw-   0        0        0    17608 2024-05-15 10:52:04.000000 prtpy-0.8.3/prtpy/partitioning/complete_greedy.py
+-rw-rw-rw-   0        0        0     9254 2023-01-21 17:01:37.000000 prtpy-0.8.3/prtpy/partitioning/complete_karmarkar_karp.py
+-rw-rw-rw-   0        0        0     7416 2022-12-06 13:00:25.000000 prtpy-0.8.3/prtpy/partitioning/dynamic_programming.py
+-rw-rw-rw-   0        0        0     2306 2022-07-10 20:23:34.000000 prtpy-0.8.3/prtpy/partitioning/greedy.py
+-rw-rw-rw-   0        0        0     8031 2023-08-31 14:51:38.000000 prtpy-0.8.3/prtpy/partitioning/integer_programming.py
+-rw-rw-rw-   0        0        0     6693 2024-05-15 10:55:48.000000 prtpy-0.8.3/prtpy/partitioning/integer_programming_avg.py
+-rw-rw-rw-   0        0        0     5607 2023-01-21 17:01:37.000000 prtpy-0.8.3/prtpy/partitioning/karmarkar_karp.py
+-rw-rw-rw-   0        0        0     3580 2022-10-24 13:40:45.000000 prtpy-0.8.3/prtpy/partitioning/multifit.py
+-rw-rw-rw-   0        0        0     7563 2023-01-21 17:01:37.000000 prtpy-0.8.3/prtpy/partitioning/recursive_number_partitioning_korf.py
+-rw-rw-rw-   0        0        0     7832 2023-02-01 13:55:27.000000 prtpy-0.8.3/prtpy/partitioning/recursive_number_partitioning_moffitt.py
+-rw-rw-rw-   0        0        0     1632 2022-07-10 20:45:34.000000 prtpy-0.8.3/prtpy/partitioning/roundrobin.py
+-rw-rw-rw-   0        0        0     6742 2023-01-21 17:01:37.000000 prtpy-0.8.3/prtpy/partitioning/sequential_number_partitioning.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.935709 prtpy-0.8.3/prtpy.egg-info/
+-rw-rw-rw-   0        0        0     4777 2024-05-15 10:57:14.000000 prtpy-0.8.3/prtpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2025 2024-05-15 10:57:14.000000 prtpy-0.8.3/prtpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 10:57:14.000000 prtpy-0.8.3/prtpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-05-15 10:57:14.000000 prtpy-0.8.3/prtpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 10:57:14.000000 prtpy-0.8.3/prtpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      331 2022-07-10 15:55:56.000000 prtpy-0.8.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-01 13:55:27.000000 prtpy-0.8.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 10:57:14.935709 prtpy-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1664 2023-10-11 10:12:11.000000 prtpy-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.923105 prtpy-0.8.3/simulations/
+-rw-rw-rw-   0        0        0      186 2022-07-12 07:40:07.000000 prtpy-0.8.3/simulations/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 10:57:14.935709 prtpy-0.8.3/tests/
+-rw-rw-rw-   0        0        0     4016 2022-07-10 22:44:40.000000 prtpy-0.8.3/tests/test_bin_completion.py
+-rw-rw-rw-   0        0        0     3850 2022-07-04 05:45:57.000000 prtpy-0.8.3/tests/test_cbldm_algorithm.py
+-rw-rw-rw-   0        0        0      675 2022-07-10 19:11:43.000000 prtpy-0.8.3/tests/test_complete_greedy.py
+-rw-rw-rw-   0        0        0      693 2022-07-12 08:21:06.000000 prtpy-0.8.3/tests/test_complete_karmarkar_karp.py
+-rw-rw-rw-   0        0        0     5666 2023-02-01 13:56:32.000000 prtpy-0.8.3/tests/test_horowitz_and_sahni.py
+-rw-rw-rw-   0        0        0     2809 2022-07-10 22:33:36.000000 prtpy-0.8.3/tests/test_packing_small_inputs.py
+-rw-rw-rw-   0        0        0     2114 2022-07-10 12:52:40.000000 prtpy-0.8.3/tests/test_partitioning_small_inputs.py
+-rw-rw-rw-   0        0        0     7489 2023-01-21 17:01:37.000000 prtpy-0.8.3/tests/test_recursive_number_partitioning.py
+-rw-rw-rw-   0        0        0     6252 2023-02-01 13:55:27.000000 prtpy-0.8.3/tests/test_recursive_number_partitioning_moffitt.py
+-rw-rw-rw-   0        0        0     6240 2023-02-01 13:56:32.000000 prtpy-0.8.3/tests/test_schroeppel_and_shamir.py
+-rw-rw-rw-   0        0        0     7694 2023-01-21 17:01:37.000000 prtpy-0.8.3/tests/test_sequential_number_partitioning.py
```

### Comparing `prtpy-0.8.2/INSTALL.md` & `prtpy-0.8.3/INSTALL.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/LICENSE` & `prtpy-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/PKG-INFO` & `prtpy-0.8.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: prtpy
-Version: 0.8.2
-Summary: Number partitioning in Python
-Home-page: https://github.com/erelsgl/prtpy
-Author: Erel Segal-Halevi
-Author-email: erelsgl@gmail.com
-License: MIT
-Project-URL: Bug Reports, https://github.com/erelsgl/prtpy/issues
-Project-URL: Source Code, https://github.com/erelsgl/prtpy
-Keywords: optimization,partition
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: simulations
-License-File: LICENSE
-
 # prtpy 
 
 ![Pytest result](https://github.com/erelsgl/prtpy/workflows/pytest/badge.svg)
 [![PyPI version](https://badge.fury.io/py/prtpy.svg)](https://badge.fury.io/py/prtpy)
 
 Python code for multiway number partitioning and bin packing algorithms.
 
@@ -87,13 +70,13 @@
 * `bins = binner.add_empty_bins(bins, numbins)` --- creates a new `bins` array with some additional empty bins at the end.
 * `bins = binner.remove_bins(bins, numbins)` --- creates a new `bins` array with some bins removed at the end.
 * `binner.valueof(item)` --- returns the value (size) of the given item.
 
 
 ## Related libraries
 
-* [numberpartitioning](https://github.com/fuglede/numberpartitioning) by SÃ¸ren Fuglede JÃ¸rgensen - the code for [complete_greedy](prtpy/partitioning/complete_greedy.py) and [complete_karmarkar_karp](prtpy/partitioning/complete_karmarkar_karp_sy.py)  was originally adapted from there.
+* [numberpartitioning](https://github.com/fuglede/numberpartitioning) by Søren Fuglede Jørgensen - the code for [complete_greedy](prtpy/partitioning/complete_greedy.py) and [complete_karmarkar_karp](prtpy/partitioning/complete_karmarkar_karp.py)  was originally adapted from there.
 * [binpacking](https://github.com/benmaier/binpacking) by Ben Maier.
 
 ## Limitations
 
 The package is tested on Python versions 3.8, 3.9 and 3.10. Other versions are not supported.
```

### Comparing `prtpy-0.8.2/README.md` & `prtpy-0.8.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: prtpy
+Version: 0.8.3
+Summary: Number partitioning in Python
+Home-page: https://github.com/erelsgl/prtpy
+Author: Erel Segal-Halevi
+Author-email: erelsgl@gmail.com
+License: MIT
+Project-URL: Bug Reports, https://github.com/erelsgl/prtpy/issues
+Project-URL: Source Code, https://github.com/erelsgl/prtpy
+Keywords: optimization,partition
+Classifier: Development Status :: 2 - Pre-Alpha
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.21.3
+Requires-Dist: scipy>=1.6.1
+Requires-Dist: mip>=1.13.0
+Provides-Extra: simulations
+Requires-Dist: experiments_csv[plotting]>=0.5.0; extra == "simulations"
+
 # prtpy 
 
 ![Pytest result](https://github.com/erelsgl/prtpy/workflows/pytest/badge.svg)
 [![PyPI version](https://badge.fury.io/py/prtpy.svg)](https://badge.fury.io/py/prtpy)
 
 Python code for multiway number partitioning and bin packing algorithms.
 
@@ -70,13 +91,13 @@
 * `bins = binner.add_empty_bins(bins, numbins)` --- creates a new `bins` array with some additional empty bins at the end.
 * `bins = binner.remove_bins(bins, numbins)` --- creates a new `bins` array with some bins removed at the end.
 * `binner.valueof(item)` --- returns the value (size) of the given item.
 
 
 ## Related libraries
 
-* [numberpartitioning](https://github.com/fuglede/numberpartitioning) by Søren Fuglede Jørgensen - the code for [complete_greedy](prtpy/partitioning/complete_greedy.py) and [complete_karmarkar_karp](prtpy/partitioning/complete_karmarkar_karp_sy.py)  was originally adapted from there.
+* [numberpartitioning](https://github.com/fuglede/numberpartitioning) by Sֳ¸ren Fuglede Jֳ¸rgensen - the code for [complete_greedy](prtpy/partitioning/complete_greedy.py) and [complete_karmarkar_karp](prtpy/partitioning/complete_karmarkar_karp.py)  was originally adapted from there.
 * [binpacking](https://github.com/benmaier/binpacking) by Ben Maier.
 
 ## Limitations
 
 The package is tested on Python versions 3.8, 3.9 and 3.10. Other versions are not supported.
```

### Comparing `prtpy-0.8.2/examples/anytime_algorithm_demo.md` & `prtpy-0.8.3/examples/anytime_algorithm_demo.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/covering_algorithms.md` & `prtpy-0.8.3/examples/covering_algorithms.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/input_formats.md` & `prtpy-0.8.3/examples/input_formats.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/maximin_share_demo.md` & `prtpy-0.8.3/examples/maximin_share_demo.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/objectives.md` & `prtpy-0.8.3/examples/objectives.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/output_formats.md` & `prtpy-0.8.3/examples/output_formats.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/packing_algorithms.md` & `prtpy-0.8.3/examples/packing_algorithms.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/partitioning_algorithms.md` & `prtpy-0.8.3/examples/partitioning_algorithms.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/examples/wmms_demo.md` & `prtpy-0.8.3/examples/wmms_demo.md`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/__init__.py` & `prtpy-0.8.3/prtpy/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,48 +25,36 @@
     from prtpy.partitioning.greedy import greedy as lpt
     from prtpy.partitioning.greedy import greedy as longest_processing_time
 
     from prtpy.partitioning.roundrobin import roundrobin
     from prtpy.partitioning.multifit import multifit as multifit
 
     # Samuel & Jonathan modules
-    from prtpy.partitioning.karmarkar_karp_sy import kk as karmarkar_karp_sy  
-    from prtpy.partitioning.karmarkar_karp_sy import kk as karmarkar_karp      # Default implementation
-    from prtpy.partitioning.karmarkar_karp_sy import kk as kk_sy
-    from prtpy.partitioning.karmarkar_karp_sy import kk as kk
-
-    from prtpy.partitioning.complete_karmarkar_karp_sy import optimal as complete_karmarkar_karp_sy
-    from prtpy.partitioning.complete_karmarkar_karp_sy import optimal as complete_karmarkar_karp     # Default implementation
-    from prtpy.partitioning.complete_karmarkar_karp_sy import optimal as ckk_sy
-    from prtpy.partitioning.complete_karmarkar_karp_sy import optimal as ckk
-
-    from prtpy.partitioning.sequential_number_partitioning_sy import snp as sequential_number_partitioning_sy
-    from prtpy.partitioning.sequential_number_partitioning_sy import snp as sequential_number_partitioning
-    from prtpy.partitioning.sequential_number_partitioning_sy import snp as snp_sy
-    from prtpy.partitioning.sequential_number_partitioning_sy import snp
-
-    from prtpy.partitioning.recursive_number_partitioning_sy import rnp as recursive_number_partitioning_sy
-    from prtpy.partitioning.recursive_number_partitioning_sy import rnp as rnp_sy
-    from prtpy.partitioning.recursive_number_partitioning_sy import rnp as recursive_number_partitioning # Default implementation
-    from prtpy.partitioning.recursive_number_partitioning_sy import rnp as rnp
+    from prtpy.partitioning.karmarkar_karp import kk as karmarkar_karp      # Default implementation
+    from prtpy.partitioning.karmarkar_karp import kk as kk
+
+    from prtpy.partitioning.complete_karmarkar_karp import optimal as complete_karmarkar_karp     # Default implementation
+    from prtpy.partitioning.complete_karmarkar_karp import optimal as ckk
+
+    from prtpy.partitioning.sequential_number_partitioning import snp as sequential_number_partitioning
+    from prtpy.partitioning.sequential_number_partitioning import snp
+
+    from prtpy.partitioning.recursive_number_partitioning_korf import rnp as recursive_number_partitioning  # Default implementation
+    from prtpy.partitioning.recursive_number_partitioning_korf import rnp as rnp
 
     # Eli Belkind module
     from prtpy.partitioning.cbldm import cbldm
 
     
 partitioning.complete_greedy.__name__ = "complete-greedy"
 partitioning.integer_programming.__name__ = "integer-programming"
 partitioning.dynamic_programming.__name__ = "dynamic-programming"
-partitioning.karmarkar_karp_sy.__name__ = "karmarkar-karp-sy"
 partitioning.karmarkar_karp.__name__ = "karmarkar-karp"
-partitioning.complete_karmarkar_karp_sy.__name__ = "complete-karmarkar-karp-sy"
 partitioning.complete_karmarkar_karp.__name__ = "complete-karmarkar-karp"
-partitioning.recursive_number_partitioning_sy.__name__ = "recursive-number-partitioning-sy"
 partitioning.recursive_number_partitioning.__name__ = "recursive-number-partitioning"
-partitioning.sequential_number_partitioning_sy.__name__ = "sequential-number-partitioning-sy"
 partitioning.sequential_number_partitioning.__name__ = "sequential-number-partitioning"
 
 class packing:
     from prtpy.packing.first_fit import online as first_fit, decreasing as first_fit_decreasing
     from prtpy.packing.first_fit import online as ff, decreasing as ffd
     from prtpy.packing.bin_completion import bin_completion
```

### Comparing `prtpy-0.8.2/prtpy/binners.py` & `prtpy-0.8.3/prtpy/binners.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,21 @@
     @abstractmethod
     def add_item_to_bin(self, bins:BinsArray, item: Any, bin_index: int)->BinsArray:
         """
         Add the given item to the given bin in the given array.
         Return the bins after the addition.
         """
         return bins
-
+        
+    def remove_item_from_bin(self, bins:BinsArray, bin_index: int, item_index: int)->BinsArray:
+        sums, lists = bins
+        value = lists[bin_index][item_index]
+        sums[bin_index] -= value
+        del lists[bin_index][item_index]
+        return bins
 
     @abstractmethod
     def sort_by_ascending_sum(self, bins:BinsArray):
         """
         Sort the bins by ascending order of sum. For consistency and testing.
         """
         pass
@@ -95,14 +101,16 @@
     @abstractmethod
     def numbins(self, bins: BinsArray) -> int:
         """
         Return the number of bins in the given bins-array.
         """
         return None
 
+
+    
     @abstractmethod
     def sums(self, bins: BinsArray) -> Tuple[float]:
         """
         Return only the current sums. 
         """
         return None
```

### Comparing `prtpy-0.8.2/prtpy/inclusion_exclusion_tree.py` & `prtpy-0.8.3/prtpy/inclusion_exclusion_tree.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/objectives.py` & `prtpy-0.8.3/prtpy/objectives.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Define various optimization objectives for a partition algorithm.
 
->>> objectives = [MaximizeSmallestSum, MaximizeKSmallestSums(2), MinimizeLargestSum, MinimizeKLargestSums(2), MinimizeDifference]
+>>> objectives = [MaximizeSmallestSum, MaximizeKSmallestSums(2), MinimizeLargestSum, MinimizeKLargestSums(2), MinimizeDifference, MinimizeDistAvg]
 >>> for o in objectives: print(o.value_to_minimize(sums=[1,2,3,4,5], are_sums_in_ascending_order=True))
 -1
 -3
 5
 9
 4
+3.0
 >>> objectives.append(MaximizeSmallestWeightedSum([1, 1, 1, 3, 4]))
 >>> for o in objectives: print(o.value_to_minimize(sums=[2,4,1,5,3]))
 -1
 -3
 5
 9
 4
+3.0
 -0.75
 """
 
 from typing import List
 from abc import ABC, abstractmethod
 import numpy as np
 
@@ -140,24 +142,65 @@
         """
         >>> MinimizeDifference.lower_bound([10,20,30,40,50], sum_of_remaining_items=5)
         35.0
         >>> MinimizeDifference.lower_bound([10,20,30,40,50], sum_of_remaining_items=20)
         25.0
         >>> MinimizeDifference.lower_bound([10,20,30,40,50], sum_of_remaining_items=45)
         15.0
-
         >>> MinimizeDifference.lower_bound([10,20,30,40,50], sum_of_remaining_items=200)
         0.0
         >>> MinimizeDifference.lower_bound([0,0,0,0,0], sum_of_remaining_items=54)
         1.0
         """
         return MaximizeSmallestSum.lower_bound(sums, sum_of_remaining_items, are_sums_in_ascending_order) \
              + MinimizeLargestSum.lower_bound(sums, sum_of_remaining_items, are_sums_in_ascending_order)
 MinimizeDifference = MinimizeTheDifference()
 
 
 
+class MinimizeTheDistanceFromAvg(Objective):
+    def value_to_minimize(self, sums:list, are_sums_in_ascending_order:bool=False)->float:
+        avg = sum(sums) / len(sums)
+        diff_from_avg = 0
+        for s in sums:
+            if (s > avg):
+                diff_from_avg = diff_from_avg + (s - avg)
+        return diff_from_avg
+    def __str__(self) -> str:
+        return "minimize-the-distance-from-avg"
+    def lower_bound(self, sums:list, sum_of_remaining_items:float, are_sums_in_ascending_order:bool=False)->float:
+        """
+        First we calculate the final avg including the remaining items.
+        We try to add values from the remaining sum to the bins that haven't reached the avg yet
+        (they don't contribute to our final difference because we only take the bins that are more than avg).
+        If at any point all bins are equal to avg then we just need to divide the remaining sum amongst all bins
+        and the residue will be given out to random bins (one each).
+        We calculate and return the difference.
+        >>> MinimizeDistAvg.lower_bound([10,20,30,40,50], sum_of_remaining_items=5)
+        28.0
+        >>> MinimizeDistAvg.lower_bound([10,20,30,40,50], sum_of_remaining_items=20)
+        22.0
+        >>> MinimizeDistAvg.lower_bound([10,20,30,40,50], sum_of_remaining_items=45)
+        12.0
+
+        >>> MinimizeDistAvg.lower_bound([10,20,30,40,50], sum_of_remaining_items=200)
+        0.0
+        >>> MinimizeDistAvg.lower_bound([0,0,0,0,0], sum_of_remaining_items=54)
+        0.8
+        """
+        remaining = sum_of_remaining_items
+        avg = (sum(sums) + remaining) / len(sums)
+        diff_from_avg = 0
+        for s in sums:
+            if (s < avg and remaining > 0):
+                remaining = remaining - min(remaining, int(avg - s))
+            if(s > avg):
+                diff_from_avg = diff_from_avg + (s - avg)
+        return diff_from_avg + ((remaining % len(sums)) / len(sums))
+
+MinimizeDistAvg = MinimizeTheDistanceFromAvg()
+
+
+
 if __name__ == "__main__":
     import doctest
-
-    (failures, tests) = doctest.testmod(report=True)
-    print("{} failures, {} tests".format(failures, tests))
+    print(doctest.testmod())
```

### Comparing `prtpy-0.8.2/prtpy/outputtypes.py` & `prtpy-0.8.3/prtpy/outputtypes.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/packing/adaptors.py` & `prtpy-0.8.3/prtpy/packing/adaptors.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/packing/best_fit.py` & `prtpy-0.8.3/prtpy/packing/best_fit.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/packing/bin_completion.py` & `prtpy-0.8.3/prtpy/packing/bin_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,20 @@
     Example 6: Article Example #3
     >>> printbins(bin_completion(BinnerKeepingContents(), binsize=100, items=[99, 97, 94, 93, 8, 5, 4, 2]))
     Bin #0: [99], sum=99.0
     Bin #1: [97, 2], sum=99.0
     Bin #2: [94, 5], sum=99.0
     Bin #3: [93, 4], sum=97.0
     Bin #4: [8], sum=8.0
+    
+    Example 7: Suggested here: https://github.com/erelsgl/prtpy/issues/15
+    >>> printbins(bin_completion(BinnerKeepingContents(), binsize=60, items=[44, 6, 24, 6, 24, 8, 22, 8, 17, 21]))
+    Bin #0: [44, 8, 8], sum=60.0
+    Bin #1: [24, 24, 6, 6], sum=60.0
+    Bin #2: [22, 21, 17], sum=60.0
     """
     # Test if there is an item with a value larger than binsize.
     for item in items:
         if binner.valueof(item) > binsize:
             raise ValueError(f"Item {item} is not valid: its value is {binner.valueof(item)} while the bin size is {binsize}.")
 
     # Remove zeros from items as they are irrelevant.
@@ -98,15 +104,17 @@
     main_branch = BinBranch(sorted_items, bins, bin_index=0)
     branches = [main_branch]
 
     while branches:
         # cb = current branch
         cb = branches.pop(0)
 
-        for x in cb.items:
+        # for x in cb.items:
+        while cb.items:
+            x = cb.items[0]
             # Add a new bin and add x to that bin
             cb.bins = binner.add_empty_bins(cb.bins, 1)
             binner.add_item_to_bin(cb.bins, x, cb.bin_index)
 
             # Now we consider all items except for x.
             # We generate all possible completions for the bin containing x, sorted by their sum in descending order.
             updated_list = cb.items[1:]
```

### Comparing `prtpy-0.8.2/prtpy/packing/bin_completion_utils.py` & `prtpy-0.8.3/prtpy/packing/bin_completion_utils.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/packing/cflz_covering.py` & `prtpy-0.8.3/prtpy/packing/cflz_covering.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/packing/first_fit.py` & `prtpy-0.8.3/prtpy/packing/first_fit.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/packing/greedy_covering.py` & `prtpy-0.8.3/prtpy/packing/greedy_covering.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/adaptors.py` & `prtpy-0.8.3/prtpy/partitioning/adaptors.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/balanced.py` & `prtpy-0.8.3/prtpy/partitioning/balanced.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/cbldm.py` & `prtpy-0.8.3/prtpy/partitioning/cbldm.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/complete_greedy.py` & `prtpy-0.8.3/prtpy/partitioning/complete_greedy.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,45 +6,53 @@
            https://github.com/fuglede/numberpartitioning/blob/master/src/numberpartitioning/greedy.py
 
     This stackoverflow question:
         https://stackoverflow.com/q/51635177/827927
     explains how to have a set with a custom key.
 
     Programmer: Erel Segal-Halevi
+    Eitan Lichtman added Minimize Distance from Avg Objective
 """
-
+import math
 from typing import List, Tuple, Callable, Iterator, Any
 import numpy as np
 import logging, time
+
 from prtpy import objectives as obj, Binner, BinsArray
 
 logger = logging.getLogger(__name__)
 
 
-
 def anytime(
-    binner: Binner, numbins: int, items: List[any],
+    binner: Binner, numbins: int, items: List[int], relative_value: List[int] = None,
     objective: obj.Objective = obj.MinimizeDifference,
-    use_lower_bound: bool = True,   # Prune branches whose lower bound (= optimistic value) is at least as large as the current minimum.
-    use_fast_lower_bound: bool = True,   # A faster lower bound, that does not create the branch at all. Useful for min-max and max-min objectives.
-    use_heuristic_3: bool = False,  # An improved stopping condition, applicable for min-max only. Not very useful in experiments.
-    use_set_of_seen_states: bool = True, 
+    use_lower_bound: bool = True,
+    # Prune branches whose lower bound (= optimistic value) is at least as large as the current minimum.
+    use_fast_lower_bound: bool = True,
+    # A faster lower bound, that does not create the branch at all. Useful for min-max max-min and min-dist-avg objectives.
+    use_heuristic_3: bool = False,
+    # An improved stopping condition, applicable for min-max only. Not very useful in experiments.
+    use_set_of_seen_states: bool = True,
     time_limit: float = np.inf,
 ) -> Iterator:
     """
     Finds a partition in which the largest sum is minimal, using the Complete Greedy algorithm.
 
     :param objective: represents the function that should be optimized. Default is minimizing the difference between bin sums.
     :param time_limit: determines how much time (in seconds) the function should run before it stops. Default is infinity.
 
     >>> from prtpy import BinnerKeepingContents, BinnerKeepingSums, printbins
     >>> printbins(anytime(BinnerKeepingContents(), 2, [4,5,6,7,8], objective=obj.MinimizeDifference))
     Bin #0: [6, 5, 4], sum=15.0
     Bin #1: [8, 7], sum=15.0
 
+    >>> printbins(anytime(BinnerKeepingContents(), 2, [4,5,6,7,8], [0.3,0.7], objective=obj.MinimizeDistAvg))
+    Bin #0: [5, 4], sum=9.0
+    Bin #1: [8, 7, 6], sum=21.0
+
     The following examples are based on:
         Walter (2013), 'Comparing the minimum completion times of two longest-first scheduling-heuristics'.
     >>> walter_numbers = [46, 39, 27, 26, 16, 13, 10]
     >>> printbins(anytime(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeDifference))
     Bin #0: [39, 16], sum=55.0
     Bin #1: [46, 13], sum=59.0
     Bin #2: [27, 26, 10], sum=63.0
@@ -52,14 +60,64 @@
     Bin #0: [27, 26], sum=53.0
     Bin #1: [39, 13, 10], sum=62.0
     Bin #2: [46, 16], sum=62.0
     >>> printbins(anytime(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MaximizeSmallestSum))
     Bin #0: [46, 10], sum=56.0
     Bin #1: [27, 16, 13], sum=56.0
     Bin #2: [39, 26], sum=65.0
+    >>> printbins(anytime(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeDistAvg))
+    Bin #0: [39, 16], sum=55.0
+    Bin #1: [46, 13], sum=59.0
+    Bin #2: [27, 26, 10], sum=63.0
+    >>> printbins(anytime(BinnerKeepingContents(), 3, walter_numbers,[0.2,0.4,0.4], objective=obj.MinimizeDistAvg))
+    Bin #0: [27, 10], sum=37.0
+    Bin #1: [39, 16, 13], sum=68.0
+    Bin #2: [46, 26], sum=72.0
+
+    >>> printbins(anytime(BinnerKeepingContents(), 5, [460000000, 390000000, 270000000, 260000000, 160000000, 130000000, 100000000],[0.2,0.4,0.1,0.15,0.15], objective=obj.MinimizeDistAvg))
+    Bin #0: [390000000], sum=390000000.0
+    Bin #1: [460000000, 130000000, 100000000], sum=690000000.0
+    Bin #2: [160000000], sum=160000000.0
+    Bin #3: [260000000], sum=260000000.0
+    Bin #4: [270000000], sum=270000000.0
+
+
+    >>> printbins(anytime(BinnerKeepingContents(), 10, [115268834, 22638149, 35260669, 68111031, 13376625, 20835125, 179398684, 69888000, 94462800, 5100340, 27184906, 305371, 272847, 545681, 1680746, 763835, 763835], [0.1,0.1,0.1,0.1,0.1,0.1,0.1,0.1,0.1,0.1], objective=obj.MinimizeDistAvg))
+    Bin #0: [13376625, 5100340, 1680746, 763835, 763835, 545681, 305371, 272847], sum=22809280.0
+    Bin #1: [20835125], sum=20835125.0
+    Bin #2: [22638149], sum=22638149.0
+    Bin #3: [27184906], sum=27184906.0
+    Bin #4: [35260669], sum=35260669.0
+    Bin #5: [68111031], sum=68111031.0
+    Bin #6: [69888000], sum=69888000.0
+    Bin #7: [94462800], sum=94462800.0
+    Bin #8: [115268834], sum=115268834.0
+    Bin #9: [179398684], sum=179398684.0
+
+
+    >>> printbins(anytime(BinnerKeepingContents(), 3, walter_numbers,[0.1,0.9,0], objective=obj.MinimizeDistAvg))
+    Bin #0: [16], sum=16.0
+    Bin #1: [46, 39, 27, 26, 13, 10], sum=161.0
+    Bin #2: [], sum=0.0
+
+
+    >>> printbins(anytime(BinnerKeepingContents(), 5, [2,2,5,5,5,5,9], objective=obj.MinimizeDistAvg))
+    Bin #0: [5], sum=5.0
+    Bin #1: [5], sum=5.0
+    Bin #2: [5, 2], sum=7.0
+    Bin #3: [5, 2], sum=7.0
+    Bin #4: [9], sum=9.0
+    >>> printbins(anytime(BinnerKeepingContents(), 3, [1,1,1,1], objective=obj.MinimizeDistAvg))
+    Bin #0: [1], sum=1.0
+    Bin #1: [1], sum=1.0
+    Bin #2: [1, 1], sum=2.0
+    >>> printbins(anytime(BinnerKeepingContents(), 3, [1,1,1,1,1], objective=obj.MinimizeDistAvg))
+    Bin #0: [1], sum=1.0
+    Bin #1: [1, 1], sum=2.0
+    Bin #2: [1, 1], sum=2.0
 
     Compare results with and without the lower bound:
     >>> random_numbers = np.random.randint(1, 2**48-1, 10, dtype=np.int64)
     >>> objective = obj.MinimizeDifference
     >>> bins1=anytime(BinnerKeepingSums(), 3, random_numbers, objective=objective, use_lower_bound=True)
     >>> bins2=anytime(BinnerKeepingSums(), 3, random_numbers, objective=objective, use_lower_bound=False)
     >>> objective.value_to_minimize(bins1)==objective.value_to_minimize(bins2)
@@ -91,32 +149,42 @@
     [16.0, 16.0]
     """
     numitems = len(items)
     start_time = time.perf_counter()
     end_time = start_time + time_limit
 
     sorted_items = sorted(items, key=binner.valueof, reverse=True)
-    sums_of_remaining_items = [sum(map(binner.valueof, sorted_items[i:])) for i in range(numitems)] + [0] # For Heuristic 3
+    sums_of_remaining_items = [sum(map(binner.valueof, sorted_items[i:])) for i in range(numitems)] + [
+        0]  # For Heuristic 3
+    from prtpy import BinnerKeepingContents, BinnerKeepingSums, printbins
     best_bins, best_objective_value = None, np.inf
 
-    global_lower_bound = objective.lower_bound(np.zeros(numbins), sums_of_remaining_items[0], are_sums_in_ascending_order=True)
 
-    logger.info("\nComplete Greedy %s Partitioning of %d items into %d parts. Lower bound: %s", objective, numitems, numbins, global_lower_bound)
+    global_lower_bound = objective.lower_bound(np.zeros(numbins), sums_of_remaining_items[0],
+                                               are_sums_in_ascending_order=True)
+
+    logger.info("\nComplete Greedy %s Partitioning of %d items into %d parts. Lower bound: %s", objective, numitems,
+                numbins, global_lower_bound)
 
     # Create a stack whose elements are a partition and the current depth.
     # Initially, it contains a single tuple: an empty partition with depth 0.
-    first_bins  = binner.new_bins(numbins)
+    # If the input has relative values for each bin -
+    # we add a sum to each bin in order to equal them out to the bin with the highest relative value
+    # (at the end of the algorithm we will remove these sums).
+    first_bins = binner.new_bins(numbins)
+    if (relative_value):
+        for i in range(numbins):
+            binner.add_item_to_bin(first_bins, (max(relative_value) * sum(items) - relative_value[i] * sum(items)), i)
     first_vertex = (first_bins, 0)
     stack: List[Tuple[BinsArray, int]] = [first_vertex]
     if use_set_of_seen_states:
         seen_states = set(tuple(binner.sums(first_bins)))
-
     # For logging and profiling:
-    complete_partitions_checked = 0      
-    intermediate_partitions_checked = 1  
+    complete_partitions_checked = 0
+    intermediate_partitions_checked = 1
 
     times_fast_lower_bound_activated = 0
     times_lower_bound_activated = 0
     times_heuristic_3_activated = 0
     times_seen_state_skipped = 0
 
     while len(stack) > 0:
@@ -130,112 +198,136 @@
         # If we have reached the leaves of the DFS tree, check if we have an improvement:
         if depth == numitems:
             complete_partitions_checked += 1
             new_objective_value = objective.value_to_minimize(current_sums)
             if new_objective_value < best_objective_value:
                 best_bins, best_objective_value = current_bins, new_objective_value
                 logger.info("  Found a better solution: %s, with value %s", current_bins, best_objective_value)
-                if new_objective_value<=global_lower_bound:
+                if new_objective_value <= global_lower_bound:
                     logger.info("    Solution matches global lower bound - stopping")
                     break
             continue
-
         # Heuristic 3: "If the sum of the remaining unassigned integers plus the smallest current subset sum is <= the largest subset sum, all remaining integers are assigned to the subset with the smallest sum, terminating that branch of the tree."
         # Note that this heuristic is valid only for the objective "minimize largest sum"!
-        if use_heuristic_3 and objective==obj.MinimizeLargestSum:
+        if use_heuristic_3 and objective == obj.MinimizeLargestSum:
             if sums_of_remaining_items[depth] + current_sums[0] <= current_sums[-1]:
                 new_bins = binner.copy_bins(current_bins)
-                for i in range(depth,numitems):
+                for i in range(depth, numitems):
                     binner.add_item_to_bin(new_bins, sorted_items[i], 0)
-                binner.sort_by_ascending_sum(new_bins)
+                    binner.sort_by_ascending_sum(new_bins)
                 new_depth = numitems
                 stack.append((new_bins, new_depth))
                 logger.debug("    Heuristic 3 activated")
-                times_heuristic_3_activated+=1
+                times_heuristic_3_activated += 1
                 continue
-
         next_item = sorted_items[depth]
-        sum_of_remaining_items = sums_of_remaining_items[depth+1]
+        sum_of_remaining_items = sums_of_remaining_items[depth + 1]
 
         previous_bin_sum = None
 
         # We want to insert the next item to the bin with the *smallest* sum first.
         # But, since we use a stack, we have to insert it to the bin with the *largest* sum first,
         # so that it is pushed deeper into the stack.
         # Therefore, we proceed in reverse, by *descending* order of sum.
-        for bin_index in reversed(range(numbins)):   
+        for bin_index in reversed(range(numbins)):
 
             # Heuristic 1: "If there are two subsets with the same sum, the current number is assigned to only one."
             current_bin_sum = current_sums[bin_index]
             if current_bin_sum == previous_bin_sum:
-                continue   
+                continue
             previous_bin_sum = current_bin_sum
 
             # Fast-lower-bound heuristic - before creating the new vertex.
-            # Currently implemented only for two objectives: min-max and max-min.
+            # Currently implemented only for two objectives: min-max, max-min and min-dist-avg
             if use_fast_lower_bound:
-                if objective==obj.MinimizeLargestSum:
+                if objective == obj.MinimizeLargestSum:
                     # "If an assignment to a subset creates a subset sum that equals or exceeds the largest subset sum in the best complete solution found so far, that branch is pruned from the tree."
                     fast_lower_bound = max(current_bin_sum + binner.valueof(next_item), current_sums[-1])
-                elif objective==obj.MaximizeSmallestSum:
+                elif objective == obj.MaximizeSmallestSum:
                     # An adaptation of the above heuristic to maximizing the smallest sum.
-                    if bin_index==0:
-                        new_smallest_sum = min(current_sums[0]+binner.valueof(next_item), current_sums[1])
+                    if bin_index == 0:
+                        new_smallest_sum = min(current_sums[0] + binner.valueof(next_item), current_sums[1])
                     else:
                         new_smallest_sum = current_sums[0]
-                    fast_lower_bound = -(new_smallest_sum+sum_of_remaining_items)
+                    fast_lower_bound = -(new_smallest_sum + sum_of_remaining_items)
+                elif objective == obj.MinimizeDistAvg:
+                    if relative_value:
+                        fast_lower_bound = 0
+                        for i in range (numbins):
+                            # For each bin: we take off the sum that we added in the beginning of the algorithm (max(relative_value) * sum(items) - relative_value[i] * sum(items))
+                            # Then we check if the difference between the bin's sum and the relative AVG for bin i: (sum(items)*relative_value[i])
+                            # is positive and contributes to our final difference or negative and we will not add anything to our difference.
+                            fast_lower_bound = fast_lower_bound + max((current_sums[i]-(max(relative_value) * sum(items) - relative_value[i] * sum(items)))-sum(items)*relative_value[i],0)
+                    else:
+                        fast_lower_bound = 0
+                        avg = sum(items) / numbins
+                        for i in range (numbins):
+                            fast_lower_bound = fast_lower_bound + max(current_sums[i]-avg,0)
                 else:
                     fast_lower_bound = -np.inf
                 if fast_lower_bound >= best_objective_value:
                     times_fast_lower_bound_activated += 1
                     continue
 
             new_bins = binner.add_item_to_bin(binner.copy_bins(current_bins), next_item, bin_index)
-            binner.sort_by_ascending_sum(new_bins)
+            if not relative_value:
+                binner.sort_by_ascending_sum(new_bins)
             new_sums = tuple(binner.sums(new_bins))
 
             # Lower-bound heuristic. 
             if use_lower_bound:
-                lower_bound = objective.lower_bound(new_sums, sum_of_remaining_items, are_sums_in_ascending_order=True)
+                lower_bound = objective.lower_bound(new_sums, sum_of_remaining_items, are_sums_in_ascending_order=False)
                 if lower_bound >= best_objective_value:
                     logger.debug("    Lower bound %f too large", lower_bound)
                     times_lower_bound_activated += 1
                     continue
-            if use_set_of_seen_states: 
+            if use_set_of_seen_states:
                 if new_sums in seen_states:
                     logger.debug("    State %s already seen", new_sums)
                     times_seen_state_skipped += 1
                     continue
-                seen_states.add(new_sums)   # should be after if use_lower_bound
+                seen_states.add(new_sums)  # should be after if use_lower_bound
 
             new_vertex = (new_bins, depth + 1)
             stack.append(new_vertex)
             intermediate_partitions_checked += 1
 
-    logger.info("Checked %d out of %d complete partitions, and %d intermediate partitions.", complete_partitions_checked, numbins**numitems, intermediate_partitions_checked)
-    logger.info("  Heuristics: fast lower bound = %d, lower bound = %d, seen state = %d, heuristic 3 = %d.", times_fast_lower_bound_activated, times_lower_bound_activated, times_seen_state_skipped, times_heuristic_3_activated)
+    logger.info("Checked %d out of %d complete partitions, and %d intermediate partitions.",
+                complete_partitions_checked, numbins ** numitems, intermediate_partitions_checked)
+    logger.info("  Heuristics: fast lower bound = %d, lower bound = %d, seen state = %d, heuristic 3 = %d.",
+                times_fast_lower_bound_activated, times_lower_bound_activated, times_seen_state_skipped,
+                times_heuristic_3_activated)
 
+
+    if (relative_value):
+        # For each bin we remove the value that we added in the beginning of the algorithm.
+        for i in range(numbins):
+            binner.remove_item_from_bin(best_bins, i, 0)
+
+    for i in range(numbins):
+        binner.sums(best_bins)[i] = math.floor(binner.sums(best_bins)[i])
     return best_bins
 
 
 if __name__ == "__main__":
     import doctest, sys
     (failures, tests) = doctest.testmod(report=True, optionflags=doctest.FAIL_FAST)
     print("{} failures, {} tests".format(failures, tests))
-    if failures>0: 
+    if failures > 0:
         sys.exit()
-
+    
     # DEMO
     logger.setLevel(logging.INFO)
     logger.addHandler(logging.StreamHandler())
 
     from prtpy import BinnerKeepingContents, BinnerKeepingSums
-    anytime(BinnerKeepingContents(), 2, [4,5,6,7,8], objective=obj.MinimizeLargestSum)
+
+    anytime(BinnerKeepingContents(), 2, [4, 5, 6, 7, 8], objective=obj.MinimizeLargestSum)
 
     walter_numbers = [46, 39, 27, 26, 16, 13, 10]
     anytime(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MaximizeSmallestSum)
     anytime(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeLargestSum)
 
-    random_numbers = np.random.randint(1, 2**16-1, 15, dtype=np.int64)
+    random_numbers = np.random.randint(1, 2 ** 16 - 1, 15, dtype=np.int64)
     anytime(BinnerKeepingSums(), 3, random_numbers, objective=obj.MaximizeSmallestSum)
     anytime(BinnerKeepingSums(), 3, random_numbers, objective=obj.MinimizeLargestSum)
     anytime(BinnerKeepingSums(), 3, random_numbers, objective=obj.MinimizeDifference)
```

### Comparing `prtpy-0.8.2/prtpy/partitioning/complete_karmarkar_karp_sy.py` & `prtpy-0.8.3/prtpy/partitioning/complete_karmarkar_karp.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Date:    2022-03
 """
 
 from typing import Iterator, List, Tuple, Callable, List, Any
 from prtpy import outputtypes as out, objectives as obj, Binner, BinsArray
 import logging, numpy as np
 
-from prtpy.partitioning.karmarkar_karp_sy import BinsSortedByMaxDiff
+from prtpy.partitioning.karmarkar_karp import BinsSortedByMaxDiff
 
 
 logger = logging.getLogger(__name__)
 
 
 def _possible_partition_difference_lower_bound(current_heap: BinsSortedByMaxDiff, numbins: int) -> int:
     """
```

### Comparing `prtpy-0.8.2/prtpy/partitioning/dynamic_programming.py` & `prtpy-0.8.3/prtpy/partitioning/dynamic_programming.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/greedy.py` & `prtpy-0.8.3/prtpy/partitioning/greedy.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/integer_programming.py` & `prtpy-0.8.3/prtpy/partitioning/integer_programming.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,80 +7,89 @@
 Credit: Rob Pratt, https://or.stackexchange.com/a/6115/2576
 """
 
 from typing import List, Callable, Any
 from numbers import Number
 from prtpy import objectives as obj, outputtypes as out, Binner, printbins
 from math import inf
+import logging
+
+logger = logging.getLogger(__name__)
 
 import mip
 
 
 def optimal(
     binner: Binner, numbins: int, items: List[any],
     objective: obj.Objective = obj.MinimizeDifference,
     copies=1,
     time_limit=inf,
     additional_constraints:Callable=lambda sums:[],
     weights:List[float]=None,
     verbose=0,
-    solver_name = mip.CBC # passed to MIP. See https://docs.python-mip.com/en/latest/quickstart.html#creating-models
+    solver_name = mip.CBC, # passed to MIP. See https://docs.python-mip.com/en/latest/quickstart.html#creating-models. 
+    # solver_name = mip.GRB, # passed to MIP. See https://docs.python-mip.com/en/latest/quickstart.html#creating-models. 
+    model_filename = None,  
+    solution_filename = None,  
 ):
     """
     Produce a partition that minimizes the given objective, by solving an integer linear program (ILP).
 
     :param numbins: number of bins.
     :param items: list of items.
     :param valueof: a function that maps an item from the list `items` to a number representing its value.
     :param objective: whether to maximize the smallest sum, minimize the largest sum, etc.
     :param outputtype: whether to return the entire partition, or just the sums, etc.
     :param copies: how many copies there are of each item. Default: 1.
     :param time_limit: stop the computation after this number of seconds have passed.
     :param additional_constraints: a function that accepts the list of sums in ascending order, and returns a list of possible additional constraints on the sums.
     :param weights: if given, must be of size bins.num. Divides each sum by its weight before applying the objective function.
+    :param solver_name: passed to MIP. See https://docs.python-mip.com/en/latest/quickstart.html#creating-models
+    :param model_filename: if not None, the MIP model will be written into this file, for debugging. NOTE: The extension should be either ".lp" or ".mps" (it indicates the output format)
+    :param solution_filename: if not None, the solution will be written into this file, for debugging.
 
     >>> from prtpy import BinnerKeepingContents, BinnerKeepingSums
     >>> optimal(BinnerKeepingSums(), 2, [11.1,11,11,11,22], objective=obj.MaximizeSmallestSum)
     array([33. , 33.1])
     >>> optimal(BinnerKeepingSums(), 2, [11,11,11,11,22], objective=obj.MaximizeSmallestSum)
     array([33., 33.])
 
     The following examples are based on:
         Walter (2013), 'Comparing the minimum completion times of two longest-first scheduling-heuristics'.
     >>> walter_numbers = [46, 39, 27, 26, 16, 13, 10]
     >>> printbins(optimal(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeDifference))
     Bin #0: [39, 16], sum=55.0
     Bin #1: [46, 13], sum=59.0
     Bin #2: [27, 26, 10], sum=63.0
-    >>> printbins(optimal(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeLargestSum))
+    >>> printbins(optimal(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeLargestSum)) #doctest: +ELLIPSIS
     Bin #0: [27, 26], sum=53.0
-    Bin #1: [46, 16], sum=62.0
-    Bin #2: [39, 13, 10], sum=62.0
-    >>> printbins(optimal(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MaximizeSmallestSum))
-    Bin #0: [46, 10], sum=56.0
-    Bin #1: [27, 16, 13], sum=56.0
+    Bin #1: [...], sum=62.0
+    Bin #2: [...], sum=62.0
+    >>> printbins(optimal(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MaximizeSmallestSum)) #doctest: +ELLIPSIS
+    Bin #0: [...], sum=56.0
+    Bin #1: [...], sum=56.0
     Bin #2: [39, 26], sum=65.0
-    >>> printbins(optimal(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeLargestSum, additional_constraints=lambda sums: [sums[0]==0]))
+    >>> printbins(optimal(BinnerKeepingContents(), 3, walter_numbers, objective=obj.MinimizeLargestSum, additional_constraints=lambda sums: [sums[0]==0])) #doctest: +ELLIPSIS
     Bin #0: [], sum=0.0
-    Bin #1: [39, 26, 13, 10], sum=88.0
-    Bin #2: [46, 27, 16], sum=89.0
+    Bin #1: [...], sum=88.0
+    Bin #2: [...], sum=89.0
     >>> optimal(BinnerKeepingSums(), 3, walter_numbers, objective=obj.MaximizeSmallestSum)
     array([56., 56., 65.])
 
     >>> items = [11.1, 11, 11, 11, 22]
     >>> optimal(BinnerKeepingSums(), 2, items, objective=obj.MaximizeSmallestSum, weights=[1,1])
     array([33. , 33.1])
     >>> optimal(BinnerKeepingSums(), 2, items, objective=obj.MaximizeSmallestSum, weights=[1,2])
     array([22. , 44.1])
     >>> optimal(BinnerKeepingSums(), 2, items, objective=obj.MaximizeSmallestSum, weights=[10,2])
     array([11.1, 55. ])
 
     >>> from prtpy import partition
-    >>> partition(algorithm=optimal, numbins=3, items={"a":1, "b":2, "c":3, "d":3, "e":5, "f":9, "g":9})
-    [['a', 'g'], ['c', 'd', 'e'], ['b', 'f']]
+    >>> partition(algorithm=optimal, numbins=3, items={"a":1, "b":2, "c":3, "d":3, "e":5, "f":9, "g":9}) #doctest: +ELLIPSIS
+    [['a', 'g'], [...], [...]]
     >>> partition(algorithm=optimal, numbins=2, items={"a":1, "b":2, "c":3, "d":3, "e":5, "f":9, "g":9}, outputtype=out.Sums)
     [16.0, 16.0]
 
     >>> traversc_example = [18, 12, 22, 22]
     >>> print(partition(algorithm=optimal, numbins=2, items=traversc_example, outputtype=out.PartitionAndSums))
     Bin #0: [12, 22], sum=34.0
     Bin #1: [18, 22], sum=40.0
@@ -100,15 +109,15 @@
     if isinstance(copies, Number):
         copies = {iitem: copies for iitem in iitems}
     if weights is None:
         weights = numbins*[1]
 
     model = mip.Model(name = '', solver_name=solver_name)
     counts: dict = {
-        iitem: [model.add_var(var_type=mip.INTEGER) for ibin in ibins] 
+        iitem: [model.add_var(var_type=mip.INTEGER, name=f'item{iitem}_in_bin{ibin}') for ibin in ibins] 
         for iitem in iitems
     }  # counts[i][j] is a variable that represents how many times item i appears in bin j.
     bin_sums = [
         sum([counts[iitem][ibin] * binner.valueof(items[iitem]) for iitem in iitems])/weights[ibin] 
         for ibin in ibins
     ]  # bin_sums[j] is a variable-expression that represents the sum of values in bin j.
 
@@ -125,26 +134,39 @@
         bin_sums[ibin + 1] >= bin_sums[ibin] for ibin in range(numbins - 1)
     ]
     constraints = counts_are_non_negative + each_item_in_one_bin + bin_sums_in_ascending_order + additional_constraints(bin_sums)
     for constraint in constraints: model += constraint
 
     # Solve the ILP:
     model.verbose = verbose
+    if  model_filename is not None:
+        model.write(model_filename)
+    # logger.info("MIP model: %s", model)
     status = model.optimize(max_seconds=time_limit)
     if status != mip.OptimizationStatus.OPTIMAL:
         raise ValueError(f"Problem status is not optimal - it is {status}.")
 
     # Construct the output:
     output = binner.new_bins(numbins)
     for ibin in ibins:
         for iitem in iitems:
             count_item_in_bin = int(counts[iitem][ibin].x)
             for _ in range(count_item_in_bin):
                 binner.add_item_to_bin(output, items[iitem], ibin)
     binner.sort_by_ascending_sum(output)
+
+    if solution_filename is not None:
+        with open(solution_filename,"w") as solution_file:
+            for ibin in ibins:
+                for iitem in iitems:
+                    count_item_in_bin = int(counts[iitem][ibin].x)
+                    # solution_file.write(f'item{binner.valueof(items[iitem]):05d}_in_bin{ibin} = {count_item_in_bin}\n')
+                    solution_file.write(f'item{iitem}_in_bin{ibin} = {count_item_in_bin}\n')
     return output
 
 
 if __name__ == "__main__":
     import doctest, logging
+    logger.setLevel(logging.DEBUG)
+    logger.addHandler(logging.StreamHandler())
     (failures, tests) = doctest.testmod(report=True, optionflags=doctest.FAIL_FAST)
     print("{} failures, {} tests".format(failures, tests))
```

### Comparing `prtpy-0.8.2/prtpy/partitioning/karmarkar_karp_sy.py` & `prtpy-0.8.3/prtpy/partitioning/karmarkar_karp.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/multifit.py` & `prtpy-0.8.3/prtpy/partitioning/multifit.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/recursive_number_partitioning_sy.py` & `prtpy-0.8.3/prtpy/partitioning/recursive_number_partitioning_korf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 Authors: Jonathan Escojido & Samuel Harroch
 Date:    03-2022
 """
 
 from typing import Callable, List
 from prtpy import outputtypes as out, objectives as obj, Binner, BinnerKeepingContents, BinsArray, printbins
-from prtpy.partitioning.karmarkar_karp_sy import kk
+from prtpy.partitioning.karmarkar_karp import kk
 import numpy as np, logging
 from prtpy import partition
-from prtpy.partitioning.complete_karmarkar_karp_sy import optimal as ckk_optimal, generator as ckk_generator
+from prtpy.partitioning.complete_karmarkar_karp import optimal as ckk_optimal, generator as ckk_generator
 from prtpy.inclusion_exclusion_tree import InExclusionBinTree
 
 logger = logging.getLogger(__name__)
 
 def find_diff(l1: List, l2: List):
     from collections import Counter
     c1 = Counter(l1)
```

### Comparing `prtpy-0.8.2/prtpy/partitioning/roundrobin.py` & `prtpy-0.8.3/prtpy/partitioning/roundrobin.py`

 * *Files identical despite different names*

### Comparing `prtpy-0.8.2/prtpy/partitioning/sequential_number_partitioning_sy.py` & `prtpy-0.8.3/prtpy/partitioning/sequential_number_partitioning.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 Programmers: Jonathan Escojido & Samuel Harroch
 Since: 03-2022
 """
 
 from typing import Callable, List
 from prtpy import outputtypes as out, objectives as obj, Binner, BinsArray, printbins
-from prtpy.partitioning.karmarkar_karp_sy import kk
-from prtpy.partitioning.complete_karmarkar_karp_sy import optimal as ckk_optimal
+from prtpy.partitioning.karmarkar_karp import kk
+from prtpy.partitioning.complete_karmarkar_karp import optimal as ckk_optimal
 import numpy as np, logging
 from prtpy import partition
 from prtpy.inclusion_exclusion_tree import InExclusionBinTree
 
 
 def find_diff(l1: List, l2: List):
     from collections import Counter
```

### Comparing `prtpy-0.8.2/prtpy.egg-info/PKG-INFO` & `prtpy-0.8.3/prtpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: prtpy
-Version: 0.8.2
+Version: 0.8.3
 Summary: Number partitioning in Python
 Home-page: https://github.com/erelsgl/prtpy
 Author: Erel Segal-Halevi
 Author-email: erelsgl@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/erelsgl/prtpy/issues
 Project-URL: Source Code, https://github.com/erelsgl/prtpy
 Keywords: optimization,partition
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: simulations
 License-File: LICENSE
+Requires-Dist: numpy>=1.21.3
+Requires-Dist: scipy>=1.6.1
+Requires-Dist: mip>=1.13.0
+Provides-Extra: simulations
+Requires-Dist: experiments_csv[plotting]>=0.5.0; extra == "simulations"
 
 # prtpy 
 
 ![Pytest result](https://github.com/erelsgl/prtpy/workflows/pytest/badge.svg)
 [![PyPI version](https://badge.fury.io/py/prtpy.svg)](https://badge.fury.io/py/prtpy)
 
 Python code for multiway number partitioning and bin packing algorithms.
@@ -87,13 +91,13 @@
 * `bins = binner.add_empty_bins(bins, numbins)` --- creates a new `bins` array with some additional empty bins at the end.
 * `bins = binner.remove_bins(bins, numbins)` --- creates a new `bins` array with some bins removed at the end.
 * `binner.valueof(item)` --- returns the value (size) of the given item.
 
 
 ## Related libraries
 
-* [numberpartitioning](https://github.com/fuglede/numberpartitioning) by SÃ¸ren Fuglede JÃ¸rgensen - the code for [complete_greedy](prtpy/partitioning/complete_greedy.py) and [complete_karmarkar_karp](prtpy/partitioning/complete_karmarkar_karp_sy.py)  was originally adapted from there.
+* [numberpartitioning](https://github.com/fuglede/numberpartitioning) by Sֳ¸ren Fuglede Jֳ¸rgensen - the code for [complete_greedy](prtpy/partitioning/complete_greedy.py) and [complete_karmarkar_karp](prtpy/partitioning/complete_karmarkar_karp.py)  was originally adapted from there.
 * [binpacking](https://github.com/benmaier/binpacking) by Ben Maier.
 
 ## Limitations
 
 The package is tested on Python versions 3.8, 3.9 and 3.10. Other versions are not supported.
```

### Comparing `prtpy-0.8.2/setup.py` & `prtpy-0.8.3/setup.py`

 * *Files identical despite different names*

