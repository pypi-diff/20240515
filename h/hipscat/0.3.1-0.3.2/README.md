# Comparing `tmp/hipscat-0.3.1.tar.gz` & `tmp/hipscat-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-0.3.1.tar", last modified: Wed May  8 17:53:53 2024, max compression
+gzip compressed data, was "hipscat-0.3.2.tar", last modified: Wed May 15 19:32:02 2024, max compression
```

## Comparing `hipscat-0.3.1.tar` & `hipscat-0.3.2.tar`

### file list

```diff
@@ -1,304 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.061213 hipscat-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-08 17:53:46.000000 hipscat-0.3.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 17:53:46.000000 hipscat-0.3.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 17:53:46.000000 hipscat-0.3.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.017213 hipscat-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.017213 hipscat-0.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/asv-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/asv-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/asv-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/publish-benchmarks-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 17:53:46.000000 hipscat-0.3.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 17:53:46.000000 hipscat-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-08 17:53:46.000000 hipscat-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-08 17:53:46.000000 hipscat-0.3.1/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 17:53:46.000000 hipscat-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-08 17:53:46.000000 hipscat-0.3.1/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 17:53:46.000000 hipscat-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-08 17:53:53.061213 hipscat-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-08 17:53:46.000000 hipscat-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:46.000000 hipscat-0.3.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-08 17:53:46.000000 hipscat-0.3.1/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-08 17:53:46.000000 hipscat-0.3.1/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/directory_scheme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/margin_cache_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/guide/pixel_math.md
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/notebooks/catalog_size_inspection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/notebooks/cone_search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 17:53:46.000000 hipscat-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-08 17:53:46.000000 hipscat-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:53:53.061213 hipscat-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.021213 hipscat-0.3.1/src/hipscat/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/association_catalog/partition_join_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/catalog_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/healpix_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/healpix_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/index/index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/index/index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.025213 hipscat-0.3.1/src/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/partition_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/source_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/catalog/source_catalog/source_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/inspection/visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/file_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/file_io/file_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/io/write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.029213 hipscat-0.3.1/src/hipscat/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/loaders/read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/src/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/box_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/cone_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/pixel_margins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/polygon_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_math/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/src/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/moc_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/negative_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    19339 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/pixel_alignment_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/pixel_tree/pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:46.000000 hipscat-0.3.1/src/hipscat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/src/hipscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-08 17:53:53.000000 hipscat-0.3.1/src/hipscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:53:52.000000 hipscat-0.3.1/src/hipscat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.033213 hipscat-0.3.1/tests/data/almanac/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/deprecated.yml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_order1.yml
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_order1_id_index.yml
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_order1_margin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_source.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_source_object_index.yml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac/small_sky_to_small_sky_order1.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/almanac_exception/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/association_missing_join.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/association_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/bad_catalog_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/bad_primary_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/bad_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/index_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/margin_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/almanac_exception/standalone_source_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/generate_data.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/info_only/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/dataset/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/index_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/index_catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.037213 hipscat-0.3.1/tests/data/info_only/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/info_only/margin_cache/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1_id_index/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1_id_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_id_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.041213 hipscat-0.3.1/tests/data/small_sky_order1_margin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_order1_margin/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_source/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_source/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_source/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.045213 hipscat-0.3.1/tests/data/small_sky_source/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.013213 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.049213 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.049213 hipscat-0.3.1/tests/data/small_sky_source_object_index/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.049213 hipscat-0.3.1/tests/data/small_sky_source_object_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_source_object_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/dataset/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/test_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/catalog/test_partition_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.053213 hipscat-0.3.1/tests/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/inspection/test_almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/inspection/test_almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/inspection/test_visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/file_io/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/file_io/test_file_pointers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/io/test_write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_math/test_pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:53:53.057213 hipscat-0.3.1/tests/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_moc_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-08 17:53:46.000000 hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.102580 hipscat-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 19:31:52.000000 hipscat-0.3.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:31:52.000000 hipscat-0.3.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 19:31:52.000000 hipscat-0.3.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.062579 hipscat-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.062579 hipscat-0.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.062579 hipscat-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/asv-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/asv-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/asv-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/publish-benchmarks-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-15 19:31:52.000000 hipscat-0.3.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 19:31:52.000000 hipscat-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-15 19:31:52.000000 hipscat-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 19:31:52.000000 hipscat-0.3.2/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 19:31:52.000000 hipscat-0.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-15 19:31:52.000000 hipscat-0.3.2/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 19:31:52.000000 hipscat-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-15 19:32:02.102580 hipscat-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-15 19:31:52.000000 hipscat-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.062579 hipscat-0.3.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:52.000000 hipscat-0.3.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-15 19:31:52.000000 hipscat-0.3.2/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-15 19:31:52.000000 hipscat-0.3.2/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.062579 hipscat-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.062579 hipscat-0.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.066580 hipscat-0.3.2/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/guide/directory_scheme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/guide/margin_cache_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/guide/pixel_math.md
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.066580 hipscat-0.3.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/notebooks/catalog_size_inspection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/notebooks/cone_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 19:31:52.000000 hipscat-0.3.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-15 19:31:52.000000 hipscat-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:32:02.102580 hipscat-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.066580 hipscat-0.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.066580 hipscat-0.3.2/src/hipscat/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 19:32:01.000000 hipscat-0.3.2/src/hipscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.066580 hipscat-0.3.2/src/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.066580 hipscat-0.3.2/src/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/association_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/association_catalog/association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/association_catalog/association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/association_catalog/partition_join_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/catalog_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/dataset/base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/dataset/catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/catalog/healpix_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/healpix_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/index/index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/index/index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/margin_cache/margin_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/partition_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/source_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/catalog/source_catalog/source_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/inspection/almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/inspection/almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/inspection/visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/file_io/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/file_io/file_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/io/write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.070580 hipscat-0.3.2/src/hipscat/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/loaders/read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.074580 hipscat-0.3.2/src/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/box_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/cone_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/pixel_margins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/polygon_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_math/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.074580 hipscat-0.3.2/src/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_tree/moc_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_tree/negative_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19695 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_tree/pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_tree/pixel_alignment_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/pixel_tree/pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:31:52.000000 hipscat-0.3.2/src/hipscat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/src/hipscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-15 19:32:01.000000 hipscat-0.3.2/src/hipscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-15 19:32:02.000000 hipscat-0.3.2/src/hipscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:32:01.000000 hipscat-0.3.2/src/hipscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 19:32:01.000000 hipscat-0.3.2/src/hipscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:32:01.000000 hipscat-0.3.2/src/hipscat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.074580 hipscat-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.074580 hipscat-0.3.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.078580 hipscat-0.3.2/tests/data/almanac/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/deprecated.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/small_sky.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/small_sky_order1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/small_sky_order1_id_index.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/small_sky_order1_margin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/small_sky_source.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/small_sky_source_object_index.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac/small_sky_to_small_sky_order1.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.078580 hipscat-0.3.2/tests/data/almanac_exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/association_missing_join.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/association_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/bad_catalog_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/bad_primary_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/bad_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/index_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/margin_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/almanac_exception/standalone_source_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/generate_data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.054580 hipscat-0.3.2/tests/data/info_only/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.078580 hipscat-0.3.2/tests/data/info_only/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/info_only/catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.078580 hipscat-0.3.2/tests/data/info_only/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/info_only/dataset/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.078580 hipscat-0.3.2/tests/data/info_only/index_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/info_only/index_catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.078580 hipscat-0.3.2/tests/data/info_only/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/info_only/margin_cache/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.082580 hipscat-0.3.2/tests/data/small_sky/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.054580 hipscat-0.3.2/tests/data/small_sky/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.082580 hipscat-0.3.2/tests/data/small_sky/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.082580 hipscat-0.3.2/tests/data/small_sky_order1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.054580 hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.082580 hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.082580 hipscat-0.3.2/tests/data/small_sky_order1_id_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_id_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_id_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_id_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.082580 hipscat-0.3.2/tests/data/small_sky_order1_id_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_id_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_id_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.086580 hipscat-0.3.2/tests/data/small_sky_order1_margin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.054580 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.086580 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.054580 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.086580 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_order1_margin/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.090580 hipscat-0.3.2/tests/data/small_sky_source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.058580 hipscat-0.3.2/tests/data/small_sky_source/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.090580 hipscat-0.3.2/tests/data/small_sky_source/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.058580 hipscat-0.3.2/tests/data/small_sky_source/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.090580 hipscat-0.3.2/tests/data/small_sky_source/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.058580 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.090580 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/data/small_sky_source_object_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source_object_index/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source_object_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source_object_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source_object_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/data/small_sky_source_object_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source_object_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_source_object_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/hipscat/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/association_catalog/test_association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/dataset/test_base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/dataset/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/index/test_index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/index/test_index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.094580 hipscat-0.3.2/tests/hipscat/catalog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/tests/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/tests/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/test_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/catalog/test_partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/tests/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/inspection/test_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/inspection/test_almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/inspection/test_visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/tests/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/io/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/tests/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/io/file_io/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/io/file_io/test_file_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/io/test_parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/io/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/io/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/io/test_write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/tests/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_math/test_healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_math/test_healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_math/test_hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_math/test_margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_math/test_partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:32:02.098580 hipscat-0.3.2/tests/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_tree/test_moc_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_tree/test_pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_tree/test_pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-15 19:31:52.000000 hipscat-0.3.2/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
```

### Comparing `hipscat-0.3.1/.copier-answers.yml` & `hipscat-0.3.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.gitattributes` & `hipscat-0.3.2/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat-0.3.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat-0.3.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/pull_request_template.md` & `hipscat-0.3.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/asv-main.yml` & `hipscat-0.3.2/.github/workflows/asv-main.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/asv-nightly.yml` & `hipscat-0.3.2/.github/workflows/asv-nightly.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/asv-pr.yml` & `hipscat-0.3.2/.github/workflows/asv-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/build-documentation.yml` & `hipscat-0.3.2/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/pre-commit-ci.yml` & `hipscat-0.3.2/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/publish-benchmarks-pr.yml` & `hipscat-0.3.2/.github/workflows/publish-benchmarks-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/publish-to-pypi.yml` & `hipscat-0.3.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/smoke-test.yml` & `hipscat-0.3.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.github/workflows/testing-and-coverage.yml` & `hipscat-0.3.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.gitignore` & `hipscat-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.pre-commit-config.yaml` & `hipscat-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.prepare_project.sh` & `hipscat-0.3.2/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/.setup_dev.sh` & `hipscat-0.3.2/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/LICENSE` & `hipscat-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/PKG-INFO` & `hipscat-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.3.1
+Version: 0.3.2
 Summary: Hierarchical Progressive Survey Catalog
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `hipscat-0.3.1/README.md` & `hipscat-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/benchmarks/asv.conf.json` & `hipscat-0.3.2/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/benchmarks/benchmarks.py` & `hipscat-0.3.2/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/Makefile` & `hipscat-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/conf.py` & `hipscat-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/guide/contributing.rst` & `hipscat-0.3.2/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/guide/directory_scheme.rst` & `hipscat-0.3.2/docs/guide/directory_scheme.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/guide/margin_cache_diagram.png` & `hipscat-0.3.2/docs/guide/margin_cache_diagram.png`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/guide/pixel_math.md` & `hipscat-0.3.2/docs/guide/pixel_math.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/index.rst` & `hipscat-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/notebooks/catalog_size_inspection.ipynb` & `hipscat-0.3.2/docs/notebooks/catalog_size_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/docs/notebooks/cone_search.ipynb` & `hipscat-0.3.2/docs/notebooks/cone_search.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/pyproject.toml` & `hipscat-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/.pylintrc` & `hipscat-0.3.2/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog.py` & `hipscat-0.3.2/src/hipscat/catalog/association_catalog/association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/association_catalog/association_catalog_info.py` & `hipscat-0.3.2/src/hipscat/catalog/association_catalog/association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/association_catalog/partition_join_info.py` & `hipscat-0.3.2/src/hipscat/catalog/association_catalog/partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/catalog.py` & `hipscat-0.3.2/src/hipscat/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/catalog_info.py` & `hipscat-0.3.2/src/hipscat/catalog/catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/dataset/base_catalog_info.py` & `hipscat-0.3.2/src/hipscat/catalog/dataset/base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/dataset/catalog_info_factory.py` & `hipscat-0.3.2/src/hipscat/catalog/dataset/catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/dataset/dataset.py` & `hipscat-0.3.2/src/hipscat/catalog/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/healpix_dataset/healpix_dataset.py` & `hipscat-0.3.2/src/hipscat/catalog/healpix_dataset/healpix_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,12 +166,10 @@
                 - "left" - use all pixels that appear in the left catalog and any overlapping from the right
                 - "right" - use all pixels that appear in the right catalog and any overlapping from the left
                 - "outer" - use all pixels from both catalogs
 
         Returns (PixelAlignment):
             A `PixelAlignment` object with the alignment from the two catalogs
         """
-        left_moc = self.moc if self.moc is not None else self.pixel_tree.to_moc()
-        right_moc = other_cat.moc if other_cat.moc is not None else other_cat.pixel_tree.to_moc()
         return align_with_mocs(
-            self.pixel_tree, other_cat.pixel_tree, left_moc, right_moc, alignment_type=alignment_type
+            self.pixel_tree, other_cat.pixel_tree, self.moc, other_cat.moc, alignment_type=alignment_type
         )
```

### Comparing `hipscat-0.3.1/src/hipscat/catalog/index/index_catalog.py` & `hipscat-0.3.2/src/hipscat/catalog/index/index_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/index/index_catalog_info.py` & `hipscat-0.3.2/src/hipscat/catalog/index/index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py` & `hipscat-0.3.2/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/margin_cache/margin_catalog.py` & `hipscat-0.3.2/src/hipscat/catalog/margin_cache/margin_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/partition_info.py` & `hipscat-0.3.2/src/hipscat/catalog/partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/catalog/source_catalog/source_catalog_info.py` & `hipscat-0.3.2/src/hipscat/catalog/source_catalog/source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/inspection/almanac.py` & `hipscat-0.3.2/src/hipscat/inspection/almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/inspection/almanac_info.py` & `hipscat-0.3.2/src/hipscat/inspection/almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/inspection/visualize_catalog.py` & `hipscat-0.3.2/src/hipscat/inspection/visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/__init__.py` & `hipscat-0.3.2/src/hipscat/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/file_io/__init__.py` & `hipscat-0.3.2/src/hipscat/io/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/file_io/file_io.py` & `hipscat-0.3.2/src/hipscat/io/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/file_io/file_pointer.py` & `hipscat-0.3.2/src/hipscat/io/file_io/file_pointer.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/parquet_metadata.py` & `hipscat-0.3.2/src/hipscat/io/parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/paths.py` & `hipscat-0.3.2/src/hipscat/io/paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/validation.py` & `hipscat-0.3.2/src/hipscat/io/validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/io/write_metadata.py` & `hipscat-0.3.2/src/hipscat/io/write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/loaders/read_from_hipscat.py` & `hipscat-0.3.2/src/hipscat/loaders/read_from_hipscat.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/__init__.py` & `hipscat-0.3.2/src/hipscat/pixel_math/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/box_filter.py` & `hipscat-0.3.2/src/hipscat/pixel_math/box_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/cone_filter.py` & `hipscat-0.3.2/src/hipscat/pixel_math/cone_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/filter.py` & `hipscat-0.3.2/src/hipscat/pixel_math/filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel.py` & `hipscat-0.3.2/src/hipscat/pixel_math/healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_convertor.py` & `hipscat-0.3.2/src/hipscat/pixel_math/healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/healpix_pixel_function.py` & `hipscat-0.3.2/src/hipscat/pixel_math/healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/hipscat_id.py` & `hipscat-0.3.2/src/hipscat/pixel_math/hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/margin_bounding.py` & `hipscat-0.3.2/src/hipscat/pixel_math/margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/partition_stats.py` & `hipscat-0.3.2/src/hipscat/pixel_math/partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/pixel_margins.py` & `hipscat-0.3.2/src/hipscat/pixel_math/pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/polygon_filter.py` & `hipscat-0.3.2/src/hipscat/pixel_math/polygon_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_math/validators.py` & `hipscat-0.3.2/src/hipscat/pixel_math/validators.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_tree/moc_filter.py` & `hipscat-0.3.2/src/hipscat/pixel_tree/moc_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_tree/negative_tree.py` & `hipscat-0.3.2/src/hipscat/pixel_tree/negative_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat/pixel_tree/pixel_alignment.py` & `hipscat-0.3.2/src/hipscat/pixel_tree/pixel_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Callable, Dict, List
 
 import numba
 import numpy as np
 import pandas as pd
 from mocpy import MOC
 from numba import njit
@@ -231,17 +233,20 @@
         matching_pix (int): The matching pixel from the side of the catalog that exists to map the new pixels
             to in the mapping
         is_left_pixel (int): Is the matching pixel from the left side of the alignment
         mapping (List[np.ndarray]): The List mapping left, right, and aligned pixels to add the new pixels to
     """
     while add_from < add_to:
         # maximum power of 4 that is a factor of add_from
-        max_p4_from = add_from & -add_from
-        if max_p4_from & 0xAAAAAAAAAAAAAAA:
-            max_p4_from = max_p4_from >> 1
+        # If add_from is 0, can add any power of 4, so use largest healpix order of 4**29
+        max_p4_from = 1 << 58
+        if add_from != 0:
+            max_p4_from = add_from & -add_from
+            if max_p4_from & 0xAAAAAAAAAAAAAAA:
+                max_p4_from = max_p4_from >> 1
 
         # maximum power of 4 less than or equal to (add_to - add_from)
         max_p4_to_log2 = np.int64(np.log2(add_to - add_from))
         max_p4_to = 1 << (max_p4_to_log2 - (max_p4_to_log2 & 1))
 
         pixel_size = min(max_p4_to, max_p4_from)
         pixel = np.array([add_from, add_from + pixel_size])
@@ -407,16 +412,16 @@
     new_tree = PixelTree(alignment.pixel_tree.tree[tree_mask], alignment.pixel_tree.tree_order)
     return PixelAlignment(new_tree, alignment.pixel_mapping.iloc[tree_mask], alignment.alignment_type)
 
 
 def align_with_mocs(
     left_tree: PixelTree,
     right_tree: PixelTree,
-    left_moc: MOC,
-    right_moc: MOC,
+    left_moc: MOC | None,
+    right_moc: MOC | None,
     alignment_type: PixelAlignmentType = PixelAlignmentType.INNER,
 ) -> PixelAlignment:
     """Aligns two pixel trees and mocs together, resulting in a pixel alignment with only aligned pixels that
     have coverage in the mocs.
 
     Args:
         left_tree (PixelTree): The left tree to align
@@ -430,14 +435,16 @@
                 - left - use all pixels that appear in the left catalog and any overlapping from the right
                 - right - use all pixels that appear in the right catalog and any overlapping from the left
                 - outer - use all pixels from both catalogs
 
     Returns:
         The PixelAlignment object with the aligned trees filtered by the coverage in the catalogs.
     """
+    left_moc = left_moc if left_moc is not None else left_tree.to_moc()
+    right_moc = right_moc if right_moc is not None else right_tree.to_moc()
     moc_intersection_methods: Dict[PixelAlignmentType, Callable[[MOC, MOC], MOC]] = {
         PixelAlignmentType.INNER: lambda l, r: l.intersection(r),
         PixelAlignmentType.LEFT: lambda l, r: l,
         PixelAlignmentType.RIGHT: lambda l, r: r,
         PixelAlignmentType.OUTER: lambda l, r: l.union(r),
     }
     filter_moc = moc_intersection_methods[alignment_type](left_moc, right_moc)
```

### Comparing `hipscat-0.3.1/src/hipscat/pixel_tree/pixel_tree.py` & `hipscat-0.3.2/src/hipscat/pixel_tree/pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/src/hipscat.egg-info/PKG-INFO` & `hipscat-0.3.2/src/hipscat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.3.1
+Version: 0.3.2
 Summary: Hierarchical Progressive Survey Catalog
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `hipscat-0.3.1/src/hipscat.egg-info/SOURCES.txt` & `hipscat-0.3.2/src/hipscat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/.pylintrc` & `hipscat-0.3.2/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/conftest.py` & `hipscat-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/generate_data.ipynb` & `hipscat-0.3.2/tests/data/generate_data.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-0.3.2/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky/_common_metadata` & `hipscat-0.3.2/tests/data/small_sky/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky/_metadata` & `hipscat-0.3.2/tests/data/small_sky/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky/point_map.fits` & `hipscat-0.3.2/tests/data/small_sky/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky/provenance_info.json` & `hipscat-0.3.2/tests/data/small_sky/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/README.md` & `hipscat-0.3.2/tests/data/small_sky_order1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/_common_metadata` & `hipscat-0.3.2/tests/data/small_sky_order1/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/_metadata` & `hipscat-0.3.2/tests/data/small_sky_order1/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/point_map.fits` & `hipscat-0.3.2/tests/data/small_sky_order1/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1/provenance_info.json` & `hipscat-0.3.2/tests/data/small_sky_order1/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_id_index/_common_metadata` & `hipscat-0.3.2/tests/data/small_sky_order1_id_index/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_id_index/_metadata` & `hipscat-0.3.2/tests/data/small_sky_order1_id_index/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_id_index/index/part.0.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1_id_index/index/part.0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_id_index/provenance_info.json` & `hipscat-0.3.2/tests/data/small_sky_order1_id_index/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/README.md` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/_common_metadata` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/_metadata` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_order1_margin/provenance_info.json` & `hipscat-0.3.2/tests/data/small_sky_order1_margin/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet` & `hipscat-0.3.2/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/_common_metadata` & `hipscat-0.3.2/tests/data/small_sky_source/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/_metadata` & `hipscat-0.3.2/tests/data/small_sky_source/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/point_map.fits` & `hipscat-0.3.2/tests/data/small_sky_source/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source/provenance_info.json` & `hipscat-0.3.2/tests/data/small_sky_source/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source_object_index/README.md` & `hipscat-0.3.2/tests/data/small_sky_source_object_index/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source_object_index/_common_metadata` & `hipscat-0.3.2/tests/data/small_sky_source_object_index/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source_object_index/_metadata` & `hipscat-0.3.2/tests/data/small_sky_source_object_index/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source_object_index/index/part.0.parquet` & `hipscat-0.3.2/tests/data/small_sky_source_object_index/index/part.0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_source_object_index/provenance_info.json` & `hipscat-0.3.2/tests/data/small_sky_source_object_index/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_common_metadata` & `hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/data/small_sky_to_small_sky_order1/_metadata` & `hipscat-0.3.2/tests/data/small_sky_to_small_sky_order1/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog.py` & `hipscat-0.3.2/tests/hipscat/catalog/association_catalog/test_association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/association_catalog/test_partition_join_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/association_catalog/test_partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/dataset/test_base_catalog_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/dataset/test_base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/dataset/test_catalog_info_factory.py` & `hipscat-0.3.2/tests/hipscat/catalog/dataset/test_catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/dataset/test_dataset.py` & `hipscat-0.3.2/tests/hipscat/catalog/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog.py` & `hipscat-0.3.2/tests/hipscat/catalog/index/test_index_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/index/test_index_catalog_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/index/test_index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/margin_cache/test_margin_catalog.py` & `hipscat-0.3.2/tests/hipscat/catalog/margin_cache/test_margin_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/test_catalog.py` & `hipscat-0.3.2/tests/hipscat/catalog/test_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/test_catalog_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/test_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/catalog/test_partition_info.py` & `hipscat-0.3.2/tests/hipscat/catalog/test_partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/conftest.py` & `hipscat-0.3.2/tests/hipscat/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/inspection/test_almanac.py` & `hipscat-0.3.2/tests/hipscat/inspection/test_almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/inspection/test_almanac_info.py` & `hipscat-0.3.2/tests/hipscat/inspection/test_almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/inspection/test_visualize_catalog.py` & `hipscat-0.3.2/tests/hipscat/inspection/test_visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/io/conftest.py` & `hipscat-0.3.2/tests/hipscat/io/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/io/file_io/test_file_io.py` & `hipscat-0.3.2/tests/hipscat/io/file_io/test_file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/io/file_io/test_file_pointers.py` & `hipscat-0.3.2/tests/hipscat/io/file_io/test_file_pointers.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/io/test_parquet_metadata.py` & `hipscat-0.3.2/tests/hipscat/io/test_parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/io/test_paths.py` & `hipscat-0.3.2/tests/hipscat/io/test_paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/io/test_validation.py` & `hipscat-0.3.2/tests/hipscat/io/test_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/io/test_write_metadata.py` & `hipscat-0.3.2/tests/hipscat/io/test_write_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel.py` & `hipscat-0.3.2/tests/hipscat/pixel_math/test_healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py` & `hipscat-0.3.2/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_math/test_healpix_pixel_function.py` & `hipscat-0.3.2/tests/hipscat/pixel_math/test_healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_math/test_hipscat_id.py` & `hipscat-0.3.2/tests/hipscat/pixel_math/test_hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_math/test_margin_bounding.py` & `hipscat-0.3.2/tests/hipscat/pixel_math/test_margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_math/test_partition_stats.py` & `hipscat-0.3.2/tests/hipscat/pixel_math/test_partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_math/test_pixel_margins.py` & `hipscat-0.3.2/tests/hipscat/pixel_math/test_pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_tree/conftest.py` & `hipscat-0.3.2/tests/hipscat/pixel_tree/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_tree/test_moc_filter.py` & `hipscat-0.3.2/tests/hipscat/pixel_tree/test_moc_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_alignment.py` & `hipscat-0.3.2/tests/hipscat/pixel_tree/test_pixel_alignment.py`

 * *Files 5% similar despite different names*

```diff
@@ -238,7 +238,18 @@
     assert_trees_equal(alignment.pixel_tree, right_moc_correct_tree)
     assert_mapping_matches_tree(alignment)
 
     both_moc_correct_tree = PixelTree.from_healpix(moc_pixels)
     alignment = left_cat_with_moc.align(right_cat_with_moc, alignment_type="outer")
     assert_trees_equal(alignment.pixel_tree, both_moc_correct_tree)
     assert_mapping_matches_tree(alignment)
+
+
+def test_outer_align_start_0():
+    left_tree = PixelTree.from_healpix([HealpixPixel(0, 0)])
+    right_tree = PixelTree.from_healpix([HealpixPixel(1, 1)])
+    alignment = align_trees(left_tree, right_tree, alignment_type="outer")
+    expected_tree = PixelTree.from_healpix(
+        [HealpixPixel(1, 0), HealpixPixel(1, 1), HealpixPixel(1, 2), HealpixPixel(1, 3)]
+    )
+    assert_trees_equal(alignment.pixel_tree, expected_tree)
+    assert_mapping_matches_tree(alignment)
```

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree.py` & `hipscat-0.3.2/tests/hipscat/pixel_tree/test_pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.1/tests/hipscat/pixel_tree/test_pixel_tree_builder.py` & `hipscat-0.3.2/tests/hipscat/pixel_tree/test_pixel_tree_builder.py`

 * *Files identical despite different names*

