# Comparing `tmp/mongo_objects-1.2.2.tar.gz` & `tmp/mongo_objects-1.2.3.tar.gz`

## Comparing `mongo_objects-1.2.2.tar` & `mongo_objects-1.2.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/.buildinfo
--rw-r--r--   0        0        0    32726 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/MongoDictProxy.html
--rw-r--r--   0        0        0    37165 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/MongoListProxy.html
--rw-r--r--   0        0        0    34866 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/MongoSingleProxy.html
--rw-r--r--   0        0        0    86142 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/MongoUserDict.html
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/customization.html
--rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/genindex.html
--rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/index.html
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/objects.inv
--rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/proxy_overview.html
--rw-r--r--   0        0        0    15225 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/quickstart.html
--rw-r--r--   0        0        0    49234 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/sample.html
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/search.html
--rw-r--r--   0        0        0    37058 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/searchindex.js
--rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/add-feature.png
--rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/add-gift.png
--rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/add-ticket-type-1.png
--rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/add-ticket-type-2.png
--rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/add-ticket-type-3.png
--rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/add-venue.png
--rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/create-event.png
--rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/purchase-ticket.png
--rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_images/vip-ticket-detail-1.png
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/MongoDictProxy.rst.txt
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/MongoListProxy.rst.txt
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/MongoSingleProxy.rst.txt
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/MongoUserDict.rst.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/customization.rst.txt
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/index.rst.txt
--rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/proxy_overview.rst.txt
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/quickstart.rst.txt
--rw-r--r--   0        0        0    19506 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_sources/sample.rst.txt
--rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/add-feature.png
--rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/add-gift.png
--rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/add-ticket-type-1.png
--rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/add-ticket-type-2.png
--rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/add-ticket-type-3.png
--rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/add-venue.png
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/alabaster.css
--rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/basic.css
--rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/create-event.png
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/doctools.js
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/plus.png
--rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/purchase-ticket.png
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/docs/_static/vip-ticket-detail-1.png
--rw-r--r--   0        0        0    29582 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/mongo_objects_sample.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/requirements.txt
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/run-sample-app
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/static/base.css
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/admin-event-detail.jinja
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/admin-event-list.jinja
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/admin-ticket-detail.jinja
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/base.jinja
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/create-update-event.jinja
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/create-update-feature.jinja
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/create-update-gift.jinja
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/create-update-ticket-type.jinja
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/create-update-venue.jinja
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/customer-event-detail.jinja
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/customer-event-list.jinja
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/customer-purchase-ticket.jinja
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/form-tools.jinja
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/sample/templates/index.jinja
--rw-r--r--   0        0        0    63120 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/src/mongo_objects/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/requirements.txt
--rw-r--r--   0        0        0    36499 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_MongoDictProxy.py
--rw-r--r--   0        0        0    40045 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_MongoListProxy.py
--rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_MongoSingleProxy.py
--rw-r--r--   0        0        0    40926 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_MongoUserDict.py
--rw-r--r--   0        0        0    22162 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_PolymorphicMongoDictProxy.py
--rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_PolymorphicMongoListProxy.py
--rw-r--r--   0        0        0    20130 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_PolymorphicMongoSingleProxy.py
--rw-r--r--   0        0        0    24806 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_PolymorphicMongoUserDict.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/tests/test_proxy_combo.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/README.rst
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 mongo_objects-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/.buildinfo
+-rw-r--r--   0        0        0    32726 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/MongoDictProxy.html
+-rw-r--r--   0        0        0    37165 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/MongoListProxy.html
+-rw-r--r--   0        0        0    34866 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/MongoSingleProxy.html
+-rw-r--r--   0        0        0    86142 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/MongoUserDict.html
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/customization.html
+-rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/genindex.html
+-rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/index.html
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/objects.inv
+-rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/proxy_overview.html
+-rw-r--r--   0        0        0    15225 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/quickstart.html
+-rw-r--r--   0        0        0    49234 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/sample.html
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/search.html
+-rw-r--r--   0        0        0    37058 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/searchindex.js
+-rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/add-feature.png
+-rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/add-gift.png
+-rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/add-ticket-type-1.png
+-rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/add-ticket-type-2.png
+-rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/add-ticket-type-3.png
+-rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/add-venue.png
+-rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/create-event.png
+-rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/purchase-ticket.png
+-rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_images/vip-ticket-detail-1.png
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/MongoDictProxy.rst.txt
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/MongoListProxy.rst.txt
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/MongoSingleProxy.rst.txt
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/MongoUserDict.rst.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/customization.rst.txt
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/proxy_overview.rst.txt
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/quickstart.rst.txt
+-rw-r--r--   0        0        0    19506 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_sources/sample.rst.txt
+-rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/add-feature.png
+-rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/add-gift.png
+-rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/add-ticket-type-1.png
+-rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/add-ticket-type-2.png
+-rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/add-ticket-type-3.png
+-rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/add-venue.png
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/alabaster.css
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/basic.css
+-rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/create-event.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/doctools.js
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/plus.png
+-rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/purchase-ticket.png
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/docs/_static/vip-ticket-detail-1.png
+-rw-r--r--   0        0        0    29582 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/mongo_objects_sample.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/requirements.txt
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/run-sample-app
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/static/base.css
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/admin-event-detail.jinja
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/admin-event-list.jinja
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/admin-ticket-detail.jinja
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/base.jinja
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/create-update-event.jinja
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/create-update-feature.jinja
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/create-update-gift.jinja
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/create-update-ticket-type.jinja
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/create-update-venue.jinja
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/customer-event-detail.jinja
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/customer-event-list.jinja
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/customer-purchase-ticket.jinja
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/form-tools.jinja
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/sample/templates/index.jinja
+-rw-r--r--   0        0        0    63231 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/src/mongo_objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/conftest.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/requirements.txt
+-rw-r--r--   0        0        0    36499 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_MongoDictProxy.py
+-rw-r--r--   0        0        0    40045 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_MongoListProxy.py
+-rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_MongoSingleProxy.py
+-rw-r--r--   0        0        0    41904 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_MongoUserDict.py
+-rw-r--r--   0        0        0    22162 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_PolymorphicMongoDictProxy.py
+-rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_PolymorphicMongoListProxy.py
+-rw-r--r--   0        0        0    20130 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_PolymorphicMongoSingleProxy.py
+-rw-r--r--   0        0        0    24806 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_PolymorphicMongoUserDict.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/tests/test_proxy_combo.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/README.rst
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 mongo_objects-1.2.3/PKG-INFO
```

### Comparing `mongo_objects-1.2.2/docs/MongoDictProxy.html` & `mongo_objects-1.2.3/docs/MongoDictProxy.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoDictProxy &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>MongoDictProxy &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoListProxy" href="MongoListProxy.html" />
     <link rel="prev" title="Proxy Overview" href="proxy_overview.html" />
```

### Comparing `mongo_objects-1.2.2/docs/MongoListProxy.html` & `mongo_objects-1.2.3/docs/MongoListProxy.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoListProxy &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>MongoListProxy &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoSingleProxy" href="MongoSingleProxy.html" />
     <link rel="prev" title="MongoDictProxy" href="MongoDictProxy.html" />
```

### Comparing `mongo_objects-1.2.2/docs/MongoSingleProxy.html` & `mongo_objects-1.2.3/docs/MongoSingleProxy.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoSingleProxy &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>MongoSingleProxy &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="MongoListProxy" href="MongoListProxy.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `mongo_objects-1.2.2/docs/MongoUserDict.html` & `mongo_objects-1.2.3/docs/MongoUserDict.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoUserDict &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>MongoUserDict &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Proxy Overview" href="proxy_overview.html" />
     <link rel="prev" title="Sample Application" href="sample.html" />
```

### Comparing `mongo_objects-1.2.2/docs/customization.html` & `mongo_objects-1.2.3/docs/customization.html`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/genindex.html` & `mongo_objects-1.2.3/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>Index &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `mongo_objects-1.2.2/docs/index.html` & `mongo_objects-1.2.3/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Introduction To mongo_objects &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>Introduction To mongo_objects &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Quickstart" href="quickstart.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `mongo_objects-1.2.2/docs/objects.inv` & `mongo_objects-1.2.3/docs/objects.inv`

 * *Files 1% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: mongo_objects
-# Version: 1.2.0
+# Version: 1.2.3
 # The remainder of this file is compressed using zlib.
 
 mongo_objects.MongoDictProxy py:class 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.__init__ py:method 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.container_name py:attribute 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.create py:method 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.create_key py:method 1 MongoDictProxy.html#$ -
```

### Comparing `mongo_objects-1.2.2/docs/proxy_overview.html` & `mongo_objects-1.2.3/docs/proxy_overview.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Proxy Overview &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>Proxy Overview &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoDictProxy" href="MongoDictProxy.html" />
     <link rel="prev" title="MongoUserDict" href="MongoUserDict.html" />
```

### Comparing `mongo_objects-1.2.2/docs/quickstart.html` & `mongo_objects-1.2.3/docs/quickstart.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Quickstart &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>Quickstart &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Sample Application" href="sample.html" />
     <link rel="prev" title="Introduction To mongo_objects" href="index.html" />
```

### Comparing `mongo_objects-1.2.2/docs/sample.html` & `mongo_objects-1.2.3/docs/sample.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Sample Application &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>Sample Application &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoUserDict" href="MongoUserDict.html" />
     <link rel="prev" title="Quickstart" href="quickstart.html" />
```

### Comparing `mongo_objects-1.2.2/docs/search.html` & `mongo_objects-1.2.3/docs/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; mongo_objects 1.2.0 documentation</title>
+    <title>Search &#8212; mongo_objects 1.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     
-    <script src="_static/documentation_options.js?v=6efca38a"></script>
+    <script src="_static/documentation_options.js?v=590429e0"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
     <script src="searchindex.js" defer="defer"></script>
```

### Comparing `mongo_objects-1.2.2/docs/searchindex.js` & `mongo_objects-1.2.3/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/add-feature.png` & `mongo_objects-1.2.3/docs/_images/add-feature.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/add-gift.png` & `mongo_objects-1.2.3/docs/_images/add-gift.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/add-ticket-type-1.png` & `mongo_objects-1.2.3/docs/_images/add-ticket-type-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/add-ticket-type-2.png` & `mongo_objects-1.2.3/docs/_images/add-ticket-type-2.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/add-ticket-type-3.png` & `mongo_objects-1.2.3/docs/_images/add-ticket-type-3.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/add-venue.png` & `mongo_objects-1.2.3/docs/_images/add-venue.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/create-event.png` & `mongo_objects-1.2.3/docs/_images/create-event.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/purchase-ticket.png` & `mongo_objects-1.2.3/docs/_images/purchase-ticket.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_images/vip-ticket-detail-1.png` & `mongo_objects-1.2.3/docs/_images/vip-ticket-detail-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/MongoDictProxy.rst.txt` & `mongo_objects-1.2.3/docs/_sources/MongoDictProxy.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/MongoListProxy.rst.txt` & `mongo_objects-1.2.3/docs/_sources/MongoListProxy.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/MongoSingleProxy.rst.txt` & `mongo_objects-1.2.3/docs/_sources/MongoSingleProxy.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/MongoUserDict.rst.txt` & `mongo_objects-1.2.3/docs/_sources/MongoUserDict.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/index.rst.txt` & `mongo_objects-1.2.3/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/proxy_overview.rst.txt` & `mongo_objects-1.2.3/docs/_sources/proxy_overview.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/quickstart.rst.txt` & `mongo_objects-1.2.3/docs/_sources/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_sources/sample.rst.txt` & `mongo_objects-1.2.3/docs/_sources/sample.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/add-feature.png` & `mongo_objects-1.2.3/docs/_static/add-feature.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/add-gift.png` & `mongo_objects-1.2.3/docs/_static/add-gift.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/add-ticket-type-1.png` & `mongo_objects-1.2.3/docs/_static/add-ticket-type-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/add-ticket-type-2.png` & `mongo_objects-1.2.3/docs/_static/add-ticket-type-2.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/add-ticket-type-3.png` & `mongo_objects-1.2.3/docs/_static/add-ticket-type-3.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/add-venue.png` & `mongo_objects-1.2.3/docs/_static/add-venue.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/alabaster.css` & `mongo_objects-1.2.3/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/basic.css` & `mongo_objects-1.2.3/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/create-event.png` & `mongo_objects-1.2.3/docs/_static/create-event.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/doctools.js` & `mongo_objects-1.2.3/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/language_data.js` & `mongo_objects-1.2.3/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/purchase-ticket.png` & `mongo_objects-1.2.3/docs/_static/purchase-ticket.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/pygments.css` & `mongo_objects-1.2.3/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/searchtools.js` & `mongo_objects-1.2.3/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/sphinx_highlight.js` & `mongo_objects-1.2.3/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/docs/_static/vip-ticket-detail-1.png` & `mongo_objects-1.2.3/docs/_static/vip-ticket-detail-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/mongo_objects_sample.py` & `mongo_objects-1.2.3/sample/mongo_objects_sample.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/run-sample-app` & `mongo_objects-1.2.3/sample/run-sample-app`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/admin-event-detail.jinja` & `mongo_objects-1.2.3/sample/templates/admin-event-detail.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/admin-event-list.jinja` & `mongo_objects-1.2.3/sample/templates/admin-event-list.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/admin-ticket-detail.jinja` & `mongo_objects-1.2.3/sample/templates/admin-ticket-detail.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/base.jinja` & `mongo_objects-1.2.3/sample/templates/base.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/create-update-event.jinja` & `mongo_objects-1.2.3/sample/templates/create-update-event.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/create-update-feature.jinja` & `mongo_objects-1.2.3/sample/templates/create-update-feature.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/create-update-gift.jinja` & `mongo_objects-1.2.3/sample/templates/create-update-gift.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/create-update-ticket-type.jinja` & `mongo_objects-1.2.3/sample/templates/create-update-ticket-type.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/create-update-venue.jinja` & `mongo_objects-1.2.3/sample/templates/create-update-venue.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/customer-event-detail.jinja` & `mongo_objects-1.2.3/sample/templates/customer-event-detail.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/customer-event-list.jinja` & `mongo_objects-1.2.3/sample/templates/customer-event-list.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/customer-purchase-ticket.jinja` & `mongo_objects-1.2.3/sample/templates/customer-purchase-ticket.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/form-tools.jinja` & `mongo_objects-1.2.3/sample/templates/form-tools.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/sample/templates/index.jinja` & `mongo_objects-1.2.3/sample/templates/index.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/src/mongo_objects/__init__.py` & `mongo_objects-1.2.3/src/mongo_objects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,16 @@
         try:
             # if the document has never been written to the database, write it now and record the ID
             if '_id' not in self:
                 result = self.collection().insert_one( self.data )
                 self['_id'] = result.inserted_id
 
             # Force-save a document regardless of timestamp
-            elif force:
+            # An object without an _updated timestamp is considered a force save
+            elif force or '_updated' not in original:
                 result = self.collection().replace_one( { '_id' : self['_id'] }, self.data, upsert=True )
 
             # Otherwise, only update a document with the same updated timestamp as our in-memory object
             else:
                 result = self.collection().find_one_and_replace(
                     { '_id' : self['_id'], '_updated' : original['_updated'] },
                     self.data,
```

### Comparing `mongo_objects-1.2.2/tests/test_MongoDictProxy.py` & `mongo_objects-1.2.3/tests/test_MongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/tests/test_MongoListProxy.py` & `mongo_objects-1.2.3/tests/test_MongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/tests/test_MongoSingleProxy.py` & `mongo_objects-1.2.3/tests/test_MongoSingleProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/tests/test_MongoUserDict.py` & `mongo_objects-1.2.3/tests/test_MongoUserDict.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,17 +365,18 @@
         startTime = MMUD.utcnow()
 
         # manually assign an ObjectId
         # any object with an _id is assumed to have been saved already
         # and to have a valid _updated timestamp
         obj = MMUD( sampleData[1] )
         obj['_id'] = ObjectId()
+        obj['_updated'] = startTime
 
         # saving it should raise an exception as no existing object can be found
-        # in this case _updated starts as None but it could be anything
+        # with this timestamp
         original_updated = obj.get('_updated')
         with pytest.raises( Exception ):
             obj.save()
 
         # verify that nothing was saved
         assert MMUD.collection().count_documents( {} ) == count
 
@@ -387,14 +388,45 @@
 
         # verify that something was saved
         assert MMUD.collection().count_documents( {} ) == count+1
 
         # verify that timestamp has been updated
         assert obj['_updated'] >= startTime
 
+        # find document directly from database driver
+        doc = MMUD.collection().find_one( { '_id' : obj['_id'] } )
+
+        # verify database object _updated timestamp
+        assert doc['_updated'] == obj['_updated']
+
+
+    def test_save_force_backfill( self, getMMUDClass, sampleData ):
+        MMUD = getMMUDClass
+
+        # count documents
+        count =  MMUD.collection().count_documents( {} )
+
+        # record the current time
+        startTime = MMUD.utcnow()
+
+        # manually assign an ObjectId
+        # any object with an _id is assumed to have been saved already
+        # and to have a valid _updated timestamp
+        obj = MMUD( sampleData[1] )
+        obj['_id'] = ObjectId()
+
+        # saving will work but is treated as a force save
+        obj.save()
+
+        # verify that something was saved
+        assert MMUD.collection().count_documents( {} ) == count+1
+
+        # verify that timestamp has been updated
+        assert obj['_updated'] >= startTime
+
         # find document directly from database driver
         doc = MMUD.collection().find_one( { '_id' : obj['_id'] } )
 
         # verify database object _updated timestamp
         assert doc['_updated'] == obj['_updated']
```

### Comparing `mongo_objects-1.2.2/tests/test_PolymorphicMongoDictProxy.py` & `mongo_objects-1.2.3/tests/test_PolymorphicMongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/tests/test_PolymorphicMongoListProxy.py` & `mongo_objects-1.2.3/tests/test_PolymorphicMongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/tests/test_PolymorphicMongoSingleProxy.py` & `mongo_objects-1.2.3/tests/test_PolymorphicMongoSingleProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/tests/test_PolymorphicMongoUserDict.py` & `mongo_objects-1.2.3/tests/test_PolymorphicMongoUserDict.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/tests/test_proxy_combo.py` & `mongo_objects-1.2.3/tests/test_proxy_combo.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/LICENSE.txt` & `mongo_objects-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/README.rst` & `mongo_objects-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/pyproject.toml` & `mongo_objects-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.2/PKG-INFO` & `mongo_objects-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mongo_objects
-Version: 1.2.2
+Version: 1.2.3
 Summary: Access MongoDB documents and subdocuments through user-defined UserDict and proxy objects.
 Project-URL: Homepage, https://github.com/lindstrom-j/mongo_objects
 Project-URL: Documentation, https://mongo-objects.headwaters.com.sg/en/latest/
 Project-URL: Issues, https://github.com/lindstrom-j/mongo_objects/issues
 Author-email: Jonathan Lindstrom <lindstrom.j@headwaters.com.sg>
 License: MIT License
 License-File: LICENSE.txt
```

