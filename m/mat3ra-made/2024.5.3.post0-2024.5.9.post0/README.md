# Comparing `tmp/mat3ra_made-2024.5.3.post0.tar.gz` & `tmp/mat3ra_made-2024.5.9.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra_made-2024.5.3.post0.tar", last modified: Fri May  3 00:37:05 2024, max compression
+gzip compressed data, was "mat3ra_made-2024.5.9.post0.tar", last modified: Thu May  9 17:49:17 2024, max compression
```

## Comparing `mat3ra_made-2024.5.3.post0.tar` & `mat3ra_made-2024.5.9.post0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.934403 mat3ra_made-2024.5.3.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.906403 mat3ra_made-2024.5.3.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.914403 mat3ra_made-2024.5.3.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.914403 mat3ra_made-2024.5.3.post0/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.husky/post-checkout
--rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.husky/post-commit
--rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.husky/post-merge
--rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.husky/pre-commit
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.husky/pre-push
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-03 00:37:05.934403 mat3ra_made-2024.5.3.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   373142 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 00:37:05.934403 mat3ra_made-2024.5.3.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.910403 mat3ra_made-2024.5.3.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.914403 mat3ra_made-2024.5.3.post0/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.914403 mat3ra_made-2024.5.3.post0/src/js/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/abstract/array_with_ids.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/abstract/scalar_with_id.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.918403 mat3ra_made-2024.5.3.post0/src/js/basis/
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/basis/basis.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/basis/constrained_basis.ts
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/basis/types.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.918403 mat3ra_made-2024.5.3.post0/src/js/cell/
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/cell/cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/cell/conventional_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/cell/primitive_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/constants.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.918403 mat3ra_made-2024.5.3.post0/src/js/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/constraints/constraints.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.918403 mat3ra_made-2024.5.3.post0/src/js/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/lattice.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/lattice_bravais.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/lattice_vectors.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.918403 mat3ra_made-2024.5.3.post0/src/js/lattice/reciprocal/
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/reciprocal/lattice_reciprocal.js
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/reciprocal/paths.js
--rw-r--r--   0 runner    (1001) docker     (127)    24706 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/reciprocal/symmetry_points.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/types.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/lattice/unit_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/made.js
--rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/material.ts
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/math.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.918403 mat3ra_made-2024.5.3.post0/src/js/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/cif.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/errors.js
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/espresso.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/native_format_parsers.js
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/parsers.js
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/poscar.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/xyz.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/parsers/xyz_combinatorial_basis.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.918403 mat3ra_made-2024.5.3.post0/src/js/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/tools/basis.js
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/tools/cell.js
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/tools/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/tools/material.js
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/tools/supercell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/tools/surface.js
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/js/types.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.922403 mat3ra_made-2024.5.3.post0/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.922403 mat3ra_made-2024.5.3.post0/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.922403 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.922403 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.922403 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/build/
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/build/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/modify.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.930403 mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-03 00:37:05.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-03 00:37:05.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 00:37:05.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-03 00:37:05.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 00:37:05.000000 mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.922403 mat3ra_made-2024.5.3.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.926403 mat3ra_made-2024.5.3.post0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/AsGe-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/C2H4-translated.json
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/C2H4.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/FeLiSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/FeO.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Ge2-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Graphene.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Graphene.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/H2+H-final.json
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/H2+H-image.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/H2+H-initial.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/H2O.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/LiFeSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Na.json
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Na4Cl4-cartesian.json
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Na4Cl4.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Na4Cl4.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Ni-hex.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Ni-hex.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/OSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si-hex.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si-hex.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si-pwscf.in
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si-slab.json
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si-supercell.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si2-basis-repeated.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Si2-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Zr1H23Zr1H1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/Zr1H23Zr1H1.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/fixtures/atomic-constraints.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.926403 mat3ra_made-2024.5.3.post0/tests/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.926403 mat3ra_made-2024.5.3.post0/tests/js/basis/
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/basis/basis.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.926403 mat3ra_made-2024.5.3.post0/tests/js/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/cell/cell.js
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/cell/primitive_cell.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.926403 mat3ra_made-2024.5.3.post0/tests/js/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/constraints/constraints.js
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/enums.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.926403 mat3ra_made-2024.5.3.post0/tests/js/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/lattice/lattice.js
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/lattice/lattice_bravais.js
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/lattice/lattice_reciprocal.js
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/lattice/lattice_vectors.js
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/material.test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.930403 mat3ra_made-2024.5.3.post0/tests/js/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/parsers/espresso.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/parsers/native_formats.js
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/parsers/poscar.js
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/parsers/xyz.js
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/parsers/xyz_combinatorial_basis.js
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.930403 mat3ra_made-2024.5.3.post0/tests/js/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/tools/basis.js
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/tools/supercell.js
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/tools/surface.js
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/js/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.910403 mat3ra_made-2024.5.3.post0/tests/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:37:05.930403 mat3ra_made-2024.5.3.post0/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/test_material.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_build_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tests/py/unit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 00:36:44.000000 mat3ra_made-2024.5.3.post0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.824788 mat3ra_made-2024.5.9.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.796788 mat3ra_made-2024.5.9.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.800788 mat3ra_made-2024.5.9.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.800788 mat3ra_made-2024.5.9.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/post-checkout
+-rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/post-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/post-merge
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/pre-push
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-09 17:49:17.824788 mat3ra_made-2024.5.9.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   373142 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:49:17.824788 mat3ra_made-2024.5.9.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.796788 mat3ra_made-2024.5.9.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/abstract/array_with_ids.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/abstract/scalar_with_id.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/basis/basis.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/basis/constrained_basis.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/basis/types.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/cell/cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/cell/conventional_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/cell/primitive_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/constants.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/constraints/constraints.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/lattice.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_bravais.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_vectors.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/lattice_reciprocal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/paths.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24706 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/symmetry_points.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/types.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/unit_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/made.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/material.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/math.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/js/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/cif.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/errors.js
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/espresso.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/native_format_parsers.js
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/parsers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/poscar.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/xyz.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/xyz_combinatorial_basis.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/js/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/material.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/supercell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/surface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/types.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.812788 mat3ra_made-2024.5.9.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/AsGe-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4-translated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/FeLiSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/FeO.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Ge2-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Graphene.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Graphene.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-final.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-image.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-initial.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2O.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/LiFeSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4-cartesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Ni-hex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Ni-hex.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/OSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-hex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-hex.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-pwscf.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-slab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-supercell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si2-basis-repeated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si2-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/atomic-constraints.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/basis/basis.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/cell/cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/cell/primitive_cell.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/constraints/constraints.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/enums.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/js/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice.js
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_bravais.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_reciprocal.js
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_vectors.js
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/material.test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/js/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/espresso.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/native_formats.js
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/poscar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz_combinatorial_basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/js/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/tools/basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/tools/supercell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/tools/surface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.800788 mat3ra_made-2024.5.9.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_build_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tsconfig.json
```

### Comparing `mat3ra_made-2024.5.3.post0/.github/workflows/cicd.yml` & `mat3ra_made-2024.5.9.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/.gitignore` & `mat3ra_made-2024.5.9.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/.pre-commit-config.yaml` & `mat3ra_made-2024.5.9.post0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/LICENSE.md` & `mat3ra_made-2024.5.9.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/PKG-INFO` & `mat3ra_made-2024.5.9.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-made
-Version: 2024.5.3.post0
+Version: 2024.5.9.post0
 Summary: MAterials DEfinitions and/or MAterials DEsign library.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_made-2024.5.3.post0/README.md` & `mat3ra_made-2024.5.9.post0/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/package-lock.json` & `mat3ra_made-2024.5.9.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/package.json` & `mat3ra_made-2024.5.9.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/pyproject.toml` & `mat3ra_made-2024.5.9.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/abstract/array_with_ids.ts` & `mat3ra_made-2024.5.9.post0/src/js/abstract/array_with_ids.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/abstract/scalar_with_id.ts` & `mat3ra_made-2024.5.9.post0/src/js/abstract/scalar_with_id.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/basis/basis.ts` & `mat3ra_made-2024.5.9.post0/src/js/basis/basis.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/basis/constrained_basis.ts` & `mat3ra_made-2024.5.9.post0/src/js/basis/constrained_basis.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/cell/cell.ts` & `mat3ra_made-2024.5.9.post0/src/js/cell/cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/cell/conventional_cell.ts` & `mat3ra_made-2024.5.9.post0/src/js/cell/conventional_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/cell/primitive_cell.ts` & `mat3ra_made-2024.5.9.post0/src/js/cell/primitive_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/constraints/constraints.ts` & `mat3ra_made-2024.5.9.post0/src/js/constraints/constraints.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/lattice.ts` & `mat3ra_made-2024.5.9.post0/src/js/lattice/lattice.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/lattice_bravais.ts` & `mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_bravais.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/lattice_vectors.ts` & `mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_vectors.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/reciprocal/lattice_reciprocal.js` & `mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/lattice_reciprocal.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/reciprocal/paths.js` & `mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/paths.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/reciprocal/symmetry_points.ts` & `mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/symmetry_points.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/types.ts` & `mat3ra_made-2024.5.9.post0/src/js/lattice/types.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/lattice/unit_cell.ts` & `mat3ra_made-2024.5.9.post0/src/js/lattice/unit_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/made.js` & `mat3ra_made-2024.5.9.post0/src/js/made.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/material.ts` & `mat3ra_made-2024.5.9.post0/src/js/material.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/parsers/espresso.ts` & `mat3ra_made-2024.5.9.post0/src/js/parsers/espresso.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/parsers/native_format_parsers.js` & `mat3ra_made-2024.5.9.post0/src/js/parsers/native_format_parsers.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/parsers/poscar.ts` & `mat3ra_made-2024.5.9.post0/src/js/parsers/poscar.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/parsers/xyz.ts` & `mat3ra_made-2024.5.9.post0/src/js/parsers/xyz.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/parsers/xyz_combinatorial_basis.js` & `mat3ra_made-2024.5.9.post0/src/js/parsers/xyz_combinatorial_basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/tools/basis.js` & `mat3ra_made-2024.5.9.post0/src/js/tools/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/tools/cell.js` & `mat3ra_made-2024.5.9.post0/src/js/tools/cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/tools/material.js` & `mat3ra_made-2024.5.9.post0/src/js/tools/material.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/tools/supercell.ts` & `mat3ra_made-2024.5.9.post0/src/js/tools/supercell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/js/tools/surface.js` & `mat3ra_made-2024.5.9.post0/src/js/tools/surface.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/material.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/material.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/analyze.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/analyze.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/build/__init__.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from ...material import Material
-from .interface import InterfaceDataHolder
+from .interface import InterfaceDataHolder, CoherentInterfaceBuilder, TerminationType
 from .interface import InterfaceSettings as Settings
 from .interface import interface_init_zsl_builder, interface_patch_with_mean_abs_strain
 from ..convert import decorator_convert_material_args_kwargs_to_structure
 from ..modify import translate_to_bottom, wrap_to_unit_cell
 
 
 @decorator_convert_material_args_kwargs_to_structure
 def create_interfaces(
-    substrate: Material,
-    layer: Material,
-    settings: Settings,
+    substrate: Material = None,
+    layer: Material = None,
+    settings: Settings = None,
     sort_by_strain_and_size: bool = True,
     remove_duplicates: bool = True,
     is_logging_enabled: bool = True,
+    interface_builder: CoherentInterfaceBuilder = None,
+    termination: TerminationType = None,
 ) -> InterfaceDataHolder:
     """
     Create all interfaces between the substrate and layer structures using ZSL algorithm provided by pymatgen.
 
     Args:
         substrate (Material): The substrate structure.
         layer (Material): The layer structure.
         settings: The settings for the interface generation.
         sort_by_strain_and_size (bool): Whether to sort the interfaces by strain and size.
         remove_duplicates (bool): Whether to remove duplicate interfaces.
         is_logging_enabled (bool): Whether to enable debug print.
     Returns:
         InterfaceDataHolder.
     """
-    substrate = translate_to_bottom(substrate, settings["USE_CONVENTIONAL_CELL"])
-    layer = translate_to_bottom(layer, settings["USE_CONVENTIONAL_CELL"])
-
     if is_logging_enabled:
         print("Creating interfaces...")
 
-    builder = interface_init_zsl_builder(substrate, layer, settings)
+    builder = interface_builder or init_interface_builder(substrate, layer, settings)
     interfaces_data = InterfaceDataHolder()
 
+    if termination is not None:
+        builder.terminations = [termination]
+
     for termination in builder.terminations:
         all_interfaces_for_termination = builder.get_interfaces(
             termination,
             gap=settings["INTERFACE_PARAMETERS"]["DISTANCE_Z"],
             film_thickness=settings["LAYER_PARAMETERS"]["THICKNESS"],
             substrate_thickness=settings["SUBSTRATE_PARAMETERS"]["THICKNESS"],
             in_layers=True,
@@ -60,7 +62,18 @@
         )
 
     if is_logging_enabled:
         unique_str = "unique" if remove_duplicates else ""
         print(f"Found {len(interfaces_data.get_interfaces_for_termination(0))} {unique_str} interfaces.")
 
     return interfaces_data
+
+
+@decorator_convert_material_args_kwargs_to_structure
+def init_interface_builder(
+    substrate: Material,
+    layer: Material,
+    settings: Settings,
+) -> CoherentInterfaceBuilder:
+    substrate = translate_to_bottom(substrate, settings["USE_CONVENTIONAL_CELL"])
+    layer = translate_to_bottom(layer, settings["USE_CONVENTIONAL_CELL"])
+    return interface_init_zsl_builder(substrate, layer, settings)
```

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/build/interface.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/interface.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/calculate.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/calculate.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/convert.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/convert.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/modify.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/modify.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra/made/tools/utils.py` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/utils.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/PKG-INFO` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-made
-Version: 2024.5.3.post0
+Version: 2024.5.9.post0
 Summary: MAterials DEfinitions and/or MAterials DEsign library.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_made-2024.5.3.post0/src/py/mat3ra_made.egg-info/SOURCES.txt` & `mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/C2H4-translated.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4-translated.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/C2H4.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/FeO.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/FeO.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Graphene.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Graphene.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/H2+H-final.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-final.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/H2+H-image.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-image.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/H2+H-initial.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-initial.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Na.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Na.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Na4Cl4-cartesian.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4-cartesian.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Na4Cl4.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Na4Cl4.poscar` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Ni-hex.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Ni-hex.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Si-hex.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Si-hex.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Si-slab.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Si-slab.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Si-supercell.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Si-supercell.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Si.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Si.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Si2-basis-repeated.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Si2-basis-repeated.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Zr1H23Zr1H1.json` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/fixtures/Zr1H23Zr1H1.poscar` & `mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/basis/basis.js` & `mat3ra_made-2024.5.9.post0/tests/js/basis/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/cell/cell.js` & `mat3ra_made-2024.5.9.post0/tests/js/cell/cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/cell/primitive_cell.js` & `mat3ra_made-2024.5.9.post0/tests/js/cell/primitive_cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/constraints/constraints.js` & `mat3ra_made-2024.5.9.post0/tests/js/constraints/constraints.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/enums.js` & `mat3ra_made-2024.5.9.post0/tests/js/enums.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/lattice/lattice.js` & `mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/lattice/lattice_bravais.js` & `mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_bravais.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/lattice/lattice_reciprocal.js` & `mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_reciprocal.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/parsers/native_formats.js` & `mat3ra_made-2024.5.9.post0/tests/js/parsers/native_formats.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/parsers/poscar.js` & `mat3ra_made-2024.5.9.post0/tests/js/parsers/poscar.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/parsers/xyz.js` & `mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/parsers/xyz_combinatorial_basis.js` & `mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz_combinatorial_basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/tools/basis.js` & `mat3ra_made-2024.5.9.post0/tests/js/tools/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/js/tools/supercell.js` & `mat3ra_made-2024.5.9.post0/tests/js/tools/supercell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/py/unit/fixtures.py` & `mat3ra_made-2024.5.9.post0/tests/py/unit/fixtures.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_build.py` & `mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_build.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_build_interface.py` & `mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_build_interface.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_calculate.py` & `mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_calculate.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/py/unit/test_tools_convert.py` & `mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_convert.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.3.post0/tests/py/unit/utils.py` & `mat3ra_made-2024.5.9.post0/tests/py/unit/utils.py`

 * *Files identical despite different names*

