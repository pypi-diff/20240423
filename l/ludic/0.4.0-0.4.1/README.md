# Comparing `tmp/ludic-0.4.0.tar.gz` & `tmp/ludic-0.4.1.tar.gz`

## Comparing `ludic-0.4.0.tar` & `ludic-0.4.1.tar`

### file list

```diff
@@ -1,83 +1,82 @@
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.0/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.0/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/catalog.md
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/getting-started.md
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/README.md
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/__init__.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/click_to_load.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/infinite_scroll.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/lazy_loading.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/__init__.py
--rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/attrs.py
--rw-r--r--   0        0        0    10080 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/components.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/format.py
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/forms.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/headers.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/items.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/lists.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/loaders.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/tables.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/typography.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/collect.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/themes.py
--rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/types.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/__init__.py
--rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/parsers.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/responses.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_components.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/styles/test_styles.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.0/LICENCE
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.0/README.md
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 ludic-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 ludic-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.1/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.1/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/catalog.md
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/getting-started.md
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.1/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/click_to_load.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.1/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/__init__.py
+-rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/attrs.py
+-rw-r--r--   0        0        0    10080 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/components.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/format.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/headers.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/items.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/collect.py
+-rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/themes.py
+-rw-r--r--   0        0        0    22939 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/types.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/responses.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.4.1/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_components.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.1/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.1/LICENCE
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.1/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.1/PKG-INFO
```

### Comparing `ludic-0.4.0/.pre-commit-config.yaml` & `ludic-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/CONTRIBUTING.md` & `ludic-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/mkdocs.yaml` & `ludic-0.4.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/.github/workflows/publish.yaml` & `ludic-0.4.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/.github/workflows/test.yaml` & `ludic-0.4.1/.github/workflows/test.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         python -m pip install .[full,test]
 
     - name: Test with pytest
       run: |
         pytest --cov --cov-report xml:coverage.xml
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v4.2.0
+      uses: codecov/codecov-action@v4.3.0
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `ludic-0.4.0/docs/catalog.md` & `ludic-0.4.1/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/docs/components.md` & `ludic-0.4.1/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/docs/getting-started.md` & `ludic-0.4.1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/docs/htmx.md` & `ludic-0.4.1/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/docs/index.md` & `ludic-0.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/docs/styles.md` & `ludic-0.4.1/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/docs/web-framework.md` & `ludic-0.4.1/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/docs/assets/ludic.png` & `ludic-0.4.1/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/examples/README.md` & `ludic-0.4.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/examples/__init__.py` & `ludic-0.4.1/examples/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,11 +84,14 @@
         return HtmlPage(
             Head(
                 meta(charset="utf-8"),
                 meta(name="viewport", content="width=device-width, initial-scale=1.0"),
                 title="HTMX Examples",
             ),
             Body(
-                Center(Stack(*self.children), style={"padding": self.theme.sizes.xxl}),
+                Center(
+                    Stack(*self.children, id="content"),
+                    style={"padding": self.theme.sizes.xxl},
+                ),
                 htmx_version="1.9.10",
             ),
         )
```

### Comparing `ludic-0.4.0/examples/bulk_update.py` & `ludic-0.4.1/examples/bulk_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     id: str = "toast"
     target: str = f"#{id}"
     styles = style.use(
         lambda theme: {
             Toast.target: {
                 "background": theme.colors.success,
                 "padding": f"{theme.sizes.xxxxs} {theme.sizes.xxxs}",
-                "font-size": theme.fonts.size.scale(0.9),
+                "font-size": theme.fonts.size * 0.9,
                 "border-radius": "3px",
                 "opacity": "0",
                 "transition": "opacity 3s ease-out",
             },
             f"{Toast.target}.htmx-settling": {
                 "opacity": "100",
             },
```

### Comparing `ludic-0.4.0/examples/click_to_edit.py` & `ludic-0.4.1/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/examples/click_to_load.py` & `ludic-0.4.1/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/examples/delete_row.py` & `ludic-0.4.1/examples/delete_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/examples/edit_row.py` & `ludic-0.4.1/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/examples/infinite_scroll.py` & `ludic-0.4.1/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/examples/lazy_loading.py` & `ludic-0.4.1/examples/lazy_loading.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import asyncio
 
 from examples import Page
 
-from ludic.catalog.headers import H1, H2
+from ludic.catalog.headers import H1, H2, H3
+from ludic.catalog.layouts import Box
 from ludic.catalog.loaders import LazyLoader
 from ludic.catalog.quotes import Quote
-from ludic.html import svg
-from ludic.types import Safe
 from ludic.web import LudicApp, Request
 
 app = LudicApp(debug=True)
 
 
 @app.get("/")
 async def index(request: Request) -> Page:
@@ -22,21 +21,14 @@
         ),
         H2("Demo"),
         LazyLoader(load_url=request.url_for(load_svg, seconds=3)),
     )
 
 
 @app.get("/load/{seconds:int}")
-async def load_svg(seconds: int) -> svg:
+async def load_svg(seconds: int) -> Box:
     await asyncio.sleep(seconds)
-    return svg(
-        Safe(
-            '<rect width="100%" height="100%" fill="#eee" />\n'
-            '<text x="310" y="215" text-anchor="middle" fill="#555">'
-            "Content Loaded"
-            "</text>"
-        ),
-        version="1.1",
-        width="700",
-        height="400",
-        style={"font-size": "2em"},
+    return Box(
+        H3("Content Loaded!", classes=["text-align-center"]),
+        classes=["invert"],
+        style={"padding-top": "10rem", "padding-bottom": "10rem"},
     )
```

### Comparing `ludic-0.4.0/ludic/attrs.py` & `ludic-0.4.1/ludic/attrs.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/base.py` & `ludic-0.4.1/ludic/base.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/components.py` & `ludic-0.4.1/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/format.py` & `ludic-0.4.1/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/html.py` & `ludic-0.4.1/ludic/html.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/types.py` & `ludic-0.4.1/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/utils.py` & `ludic-0.4.1/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/catalog/buttons.py` & `ludic-0.4.1/ludic/catalog/buttons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,148 +1,186 @@
+from typing import override
+
 from ludic.attrs import ButtonAttrs
-from ludic.html import button, style
+from ludic.html import a, button, style
 from ludic.types import ComponentStrict, PrimitiveChildren
 
 
 class Button(ComponentStrict[PrimitiveChildren, ButtonAttrs]):
     """Simple component creating an HTML button.
 
     The component creates a button.
     """
 
     classes = ["btn"]
     styles = style.use(
         lambda theme: {
-            "button.btn": {
+            ".btn": {
                 "background-color": theme.colors.light,
                 "color": theme.colors.black,
                 "padding": f"{theme.sizes.xxs} {theme.sizes.s}",
-                "border": f"1px solid {theme.colors.light.darken(0.1)}",
+                "border": "none",
                 "border-radius": theme.rounding.normal,
                 "cursor": "pointer",
                 "font-size": theme.fonts.size,
                 "transition": "0.1s filter linear, 0.1s -webkit-filter linear",
             },
-            "button.btn:hover": {
+            ".btn:hover": {
                 "filter": "brightness(85%)",
             },
-            "button.btn.small": {
-                "font-size": theme.fonts.size.scale(0.9),
+            ".btn.small": {
+                "font-size": theme.fonts.size * 0.9,
                 "padding": f"{theme.sizes.xxxs} {theme.sizes.xs}",
             },
-            "button.btn.large": {
-                "font-size": theme.fonts.size.scale(1.2),
+            ".btn.large": {
+                "font-size": theme.fonts.size * 1.2,
                 "padding": f"{theme.sizes.xs} {theme.sizes.m}",
             },
+            ".box .btn": {
+                "background-color": theme.colors.dark,
+                "color": theme.colors.light,
+                "border-color": theme.colors.dark,
+            },
         }
     )
 
-    def render(self) -> button:
+    @override
+    def render(self) -> button | a:
         return button(self.children[0], **self.attrs)
 
 
 class ButtonPrimary(Button):
     """Simple component creating an HTML button.
 
     The component creates a button with the ``primary`` class.
     """
 
     classes = ["btn", "primary"]
     styles = style.use(
         lambda theme: {
-            "button.btn.primary": {
+            ".btn.primary": {
                 "color": theme.colors.primary.readable(),
                 "background-color": theme.colors.primary,
-                "border-color": theme.colors.primary.darken(0.05),
             }
         }
     )
 
 
 class ButtonSecondary(Button):
     """Simple component creating an HTML button.
 
     The component creates a button with the ``secondary`` class.
     """
 
     classes = ["btn", "secondary"]
     styles = style.use(
         lambda theme: {
-            "button.btn.secondary": {
+            ".btn.secondary": {
                 "color": theme.colors.secondary.readable(),
                 "background-color": theme.colors.secondary,
-                "border-color": theme.colors.secondary.darken(0.05),
             }
         }
     )
 
 
+class ButtonLink(Button):
+    """Simple component creating an HTML button.
+
+    The component creates a button with the ``secondary`` class.
+    """
+
+    classes = ["btn", "link"]
+    styles = style.use(
+        lambda theme: {
+            (".btn.link", ".box .btn.link"): {
+                "color": theme.colors.dark,
+                "background": "none",
+                "border": "none",
+                "text-decoration": "none",
+                "display": "inline-block",
+            },
+            (".btn.link.active", ".btn.link.active:hover"): {
+                "background-color": theme.colors.light,
+            },
+            (".box .btn.link.active", ".box .btn.link.active:hover"): {
+                "color": theme.colors.light,
+                "background-color": theme.colors.dark,
+            },
+            (".btn.link:hover", ".box .btn.link:hover"): {
+                "color": theme.colors.dark,
+                "background-color": theme.colors.light,
+                "text-decoration": "none",
+            },
+        }
+    )
+
+    @override
+    def render(self) -> a:
+        return a(self.children[0], **self.attrs)
+
+
 class ButtonSuccess(Button):
     """Simple component creating an HTML button.
 
     The component creates a button with the ``success`` class.
     """
 
     classes = ["btn", "success"]
     styles = style.use(
         lambda theme: {
-            "button.btn.success": {
+            ".btn.success": {
                 "color": theme.colors.success.readable(),
                 "background-color": theme.colors.success,
-                "border-color": theme.colors.success.darken(0.05),
             }
         }
     )
 
 
 class ButtonDanger(Button):
     """Simple component creating an HTML button.
 
     The component creates a button with the ``danger`` class.
     """
 
     classes = ["btn", "danger"]
     styles = style.use(
         lambda theme: {
-            "button.btn.danger": {
+            ".btn.danger": {
                 "color": theme.colors.danger.readable(),
                 "background-color": theme.colors.danger,
-                "border-color": theme.colors.danger.darken(0.05),
             }
         }
     )
 
 
 class ButtonWarning(Button):
     """Simple component creating an HTML button.
 
     The component creates a button with the ``warning`` class.
     """
 
     classes = ["btn", "warning"]
     styles = style.use(
         lambda theme: {
-            "button.btn.warning": {
+            ".btn.warning": {
                 "color": theme.colors.warning.readable(),
                 "background-color": theme.colors.warning,
-                "border-color": theme.colors.warning.darken(0.05),
             }
         }
     )
 
 
 class ButtonInfo(Button):
     """Simple component creating an HTML button.
 
     The component creates a button with the ``info`` class.
     """
 
     classes = ["btn", "info"]
     styles = style.use(
         lambda theme: {
-            "button.btn.info": {
+            ".btn.info": {
                 "color": theme.colors.info.readable(),
                 "background-color": theme.colors.info,
-                "border-color": theme.colors.info.darken(0.05),
             }
         }
     )
```

### Comparing `ludic-0.4.0/ludic/catalog/forms.py` & `ludic-0.4.1/ludic/catalog/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,20 +105,20 @@
             ".form-field": {
                 "label": {
                     "display": "block",
                     "font-weight": "bold",
                     "margin": f"{theme.sizes.xxxs} 0 {theme.sizes.xxs}",
                 },
                 "input": {
-                    "width": "100%",
-                    "padding": f"{theme.sizes.xs} {theme.sizes.xxxs}",
+                    "inline-size": "100%",
+                    "padding": f"{theme.sizes.xxxs} {theme.sizes.xs}",
                     "border": f"1px solid {theme.colors.light.darken(0.2)}",
-                    "border-radius": "4px",
+                    "border-radius": theme.rounding.normal,
                     "box-sizing": "border-box",
-                    "font-size": theme.fonts.size,
+                    "font-size": theme.fonts.size * 0.9,
                 },
             }
         }
     )
 
     def create_label(self, text: PrimitiveChildren, for_: str = "") -> label:
         if for_:
```

### Comparing `ludic-0.4.0/ludic/catalog/headers.py` & `ludic-0.4.1/ludic/catalog/headers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import override
 
-from ludic.attrs import Attrs
+from ludic.attrs import Attrs, GlobalAttrs
 from ludic.html import a, div, h1, h2, h3, h4, style
 from ludic.types import Component, ComponentStrict
 
 from .utils import text_to_kebab
 
 
 class AnchorAttrs(Attrs):
@@ -15,16 +15,16 @@
     """Component representing a clickable anchor."""
 
     classes = ["anchor"]
     styles = style.use(
         lambda theme: {
             "a.anchor": {
                 "font-family": theme.fonts.serif,
-                "font-size": theme.fonts.size.scale(2.5),
-                "color": theme.colors.dark.lighten(0.5),
+                "font-size": theme.fonts.size * 2.5,
+                "color": theme.colors.light.darken(0.1),
                 "text-decoration": "none",
             },
             "a.anchor:hover": {
                 "color": theme.colors.dark,
                 "text-decoration": "none",
             },
         }
@@ -33,19 +33,19 @@
     @override
     def render(self) -> a:
         return a(
             self.children[0] if self.children else "#", href=f"#{self.attrs["target"]}"
         )
 
 
-class WitchAnchorAttrs(Attrs, total=False):
+class WithAnchorAttrs(GlobalAttrs, total=False):
     anchor: Anchor
 
 
-class WithAnchor(ComponentStrict[h1 | h2 | h3 | h4 | str, WitchAnchorAttrs]):
+class WithAnchor(ComponentStrict[h1 | h2 | h3 | h4 | str, WithAnchorAttrs]):
     """Component which renders its content (header) with a clickable anchor."""
 
     classes = ["with-anchor"]
     styles = style.use(
         lambda theme: {
             ".with-anchor": {
                 "display": "flex",
@@ -58,73 +58,74 @@
         }
     )
 
     @override
     def render(self) -> div:
         element: h1 | h2 | h3 | h4
         if isinstance(self.children[0], str):
-            element = h1(self.children[0], id=text_to_kebab(self.children[0]))
+            element = h1(self.children[0])
         else:
             element = self.children[0]
 
-        id = element.attrs.get("id", text_to_kebab(element.text))
+        element.attrs.setdefault("id", text_to_kebab(element.text))
+        id = element.attrs["id"]
 
         return div(
             element,
             (self.attrs["anchor"] if "anchor" in self.attrs else Anchor(target=id)),
         )
 
 
-class H1(ComponentStrict[str, WitchAnchorAttrs]):
+class H1(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h1 with an optional clickable anchor."""
 
     @override
     def render(self) -> h1 | WithAnchor:
-        header = h1(self.children[0], style={"font-family": self.theme.fonts.serif})
+        header = h1(self.children[0], **self.attrs_for(h1))
         if anchor := self.attrs.get("anchor"):
             return WithAnchor(header, anchor=anchor)
         elif self.theme.headers.h1.anchor:
             return WithAnchor(header)
         else:
             return header
 
 
-class H2(ComponentStrict[str, WitchAnchorAttrs]):
+class H2(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h2 with an optional clickable anchor."""
 
     @override
     def render(self) -> h2 | WithAnchor:
-        header = h2(self.children[0], style={"font-family": self.theme.fonts.serif})
+        header = h2(self.children[0], **self.attrs_for(h2))
         if anchor := self.attrs.get("anchor"):
             return WithAnchor(header, anchor=anchor)
         elif self.theme.headers.h2.anchor:
             return WithAnchor(header)
         else:
             return header
 
 
-class H3(ComponentStrict[str, WitchAnchorAttrs]):
+class H3(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h3 with an optional clickable anchor."""
 
     @override
     def render(self) -> h3 | WithAnchor:
-        header = h3(self.children[0], style={"font-family": self.theme.fonts.serif})
+        header = h3(self.children[0], **self.attrs_for(h3))
         if anchor := self.attrs.get("anchor"):
             return WithAnchor(header, anchor=anchor)
         elif self.theme.headers.h3.anchor:
             return WithAnchor(header)
         else:
             return header
 
 
-class H4(ComponentStrict[str, WitchAnchorAttrs]):
+class H4(ComponentStrict[str, WithAnchorAttrs]):
     """Component rendering as h4 with an optional clickable anchor."""
 
     @override
     def render(self) -> h4 | WithAnchor:
-        header = h4(self.children[0], style={"font-family": self.theme.fonts.serif})
+        header = h4(self.children[0], **self.attrs_for(h4))
         if anchor := self.attrs.get("anchor"):
             return WithAnchor(header, anchor=anchor)
         elif self.theme.headers.h4.anchor:
             return WithAnchor(header)
         else:
             return header
```

### Comparing `ludic-0.4.0/ludic/catalog/items.py` & `ludic-0.4.1/ludic/catalog/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     Or alternatively:
 
         Pairs(
             items={"name": "John", "age": 42}.items(),
         )
     """
 
-    classes = ["stack", "stack-small"]
+    classes = ["stack", "small"]
     styles = style.use(
         lambda theme: {
-            ".stack.stack-small > dt + dd": {
+            ".stack.small > dt + dd": {
                 "margin-block-start": theme.sizes.xxxxs,
             },
         }
     )
 
     @override
     def render(self) -> dl:
```

### Comparing `ludic-0.4.0/ludic/catalog/loaders.py` & `ludic-0.4.1/ludic/catalog/loaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,12 +90,11 @@
         LazyLoader(
             load_url="https://example.com/svg-file"
         )
     """
 
     @override
     def render(self) -> div:
-        return div(
-            self.attrs.get("placeholder", Loading()),
-            hx_get=self.attrs["load_url"],
-            hx_trigger="load",
-        )
+        self.attrs.setdefault("hx_trigger", "load")
+        self.attrs.setdefault("hx_get", self.attrs["load_url"])
+        self.attrs.setdefault("hx_swap", "outerHTML")
+        return div(self.attrs.get("placeholder", Loading()), **self.attrs_for(div))
```

### Comparing `ludic-0.4.0/ludic/catalog/quotes.py` & `ludic-0.4.1/ludic/catalog/quotes.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                     "margin-bottom": theme.sizes.xxs,
                     "padding": f"{theme.sizes.l} {theme.sizes.m}",
                 },
                 "blockquote p": {
                     "font-size": theme.fonts.size,
                 },
                 "footer": {
-                    "font-size": theme.fonts.size.scale(0.9),
+                    "font-size": theme.fonts.size * 0.9,
                     "color": theme.colors.dark.lighten(0.5),
                 },
                 "footer a": {
                     "text-decoration": "none",
                     "color": theme.colors.dark.darken(0.5),
                 },
                 "footer a:hover": {
```

### Comparing `ludic-0.4.0/ludic/catalog/tables.py` & `ludic-0.4.1/ludic/catalog/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         )
     """
 
     classes = ["table"]
     styles = style.use(
         lambda theme: {
             "table.table": {
-                "width": "100%",  # type: ignore
+                "inline-size": "100%",  # type: ignore
                 "border-collapse": "collapse",  # type: ignore
                 "thead": {
                     "background-color": theme.colors.light,
                 },
                 "tr th": {
                     "border": (
                         f"{theme.borders.thin} solid {theme.colors.light.darken(0.1)}"
```

### Comparing `ludic-0.4.0/ludic/styles/collect.py` & `ludic-0.4.1/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/styles/themes.py` & `ludic-0.4.1/ludic/styles/themes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, TypeVar
 
 from .types import Color, Size
-from .utils import clamp
 
 if TYPE_CHECKING:
     from ludic.types import BaseElement
 
 _T = TypeVar("_T", bound="BaseElement")
 
 
@@ -55,70 +54,104 @@
     h6: Header = field(default_factory=lambda: Header(size=Size(1, "em"), anchor=False))
 
 
 @dataclass
 class Fonts:
     """Font sizes for a theme."""
 
-    plain: str = "sans-serif"
-    serif: str = "serif"
-    mono: str = "monospace"
+    plain: str = "Helvetica Neue, Helvetica, Arial, sans-serif"
+    serif: str = "Georgia, serif"
+    mono: str = "Space Mono, Roboto Mono, monospace"
 
     size: Size = Size(1.02, "em")
 
 
 @dataclass
 class Sizes:
     """Size for a theme."""
 
-    xxxxs: str = clamp(Size(0.33), Size(0.39), Size(0.18))
-    xxxs: str = clamp(Size(0.41), Size(0.47), Size(0.25))
-    xxs: str = clamp(Size(0.51), Size(0.57), Size(0.35))
-    xs: str = clamp(Size(0.64), Size(0.69), Size(0.5))
-    s: str = clamp(Size(0.8), Size(0.84), Size(0.71))
-    m: str = clamp(Size(1), Size(1), Size(1))
-    l: str = clamp(Size(1.25), Size(1.19), Size(1.41))  # noqa
-    xl: str = clamp(Size(1.56), Size(1.39), Size(2))
-    xxl: str = clamp(Size(1.95), Size(1.61), Size(2.83))
-    xxxl: str = clamp(Size(2.44), Size(1.83), Size(4))
-    xxxxl: str = clamp(Size(3.05), Size(2.04), Size(5.65))
+    xxxxs: Size = Size(0.39)
+    xxxs: Size = Size(0.47)
+    xxs: Size = Size(0.57)
+    xs: Size = Size(0.69)
+    s: Size = Size(0.84)
+    m: Size = Size(1)
+    l: Size = Size(1.19)  # noqa
+    xl: Size = Size(1.39)
+    xxl: Size = Size(1.61)
+    xxxl: Size = Size(1.83)
+    xxxxl: Size = Size(2.04)
 
 
 @dataclass
 class Borders:
     """Border sizes for a theme."""
 
-    thin: str = clamp(Size(0.1), Size(0.18), Size(0.05))
-    normal: str = clamp(Size(0.2), Size(0.25), Size(0.1))
-    thick: str = clamp(Size(0.3), Size(0.4), Size(0.2))
+    thin: Size = Size(0.1)
+    normal: Size = Size(0.23)
+    thick: Size = Size(0.42)
 
 
 @dataclass
 class Rounding:
     """Border rounding for a theme."""
 
-    less: str = clamp(Size(0.15), Size(0.20), Size(0.08))
-    normal: str = clamp(Size(0.2), Size(0.25), Size(0.12))
-    more: str = clamp(Size(0.25), Size(0.35), Size(0.18))
+    less: Size = Size(0.20)
+    normal: Size = Size(0.25)
+    more: Size = Size(0.35)
+
+
+@dataclass
+class Sidebar:
+    """Sidebar layout config for a theme."""
+
+    # The width of the sidebar (empty means not set; defaults to the content width)
+    side_width: Size | None = None
+
+    # The narrowest the content element can be before wrapping. Should be a percentage.
+    content_min_width: str = "60%"
+
+
+@dataclass
+class Switcher:
+    """Switcher layout config for a theme."""
+
+    # The container width at which the component switches between a horizontal and
+    # vertical layout
+    threshold: Size = Size(40, "rem")
+
+    # The maximum number of elements allowed to appear in the horizontal configuration
+    limit: int = 4
+
+
+@dataclass
+class Layouts:
+    """Layout configuration for a theme."""
+
+    sidebar: Sidebar = field(default_factory=Sidebar)
+    switcher: Switcher = field(default_factory=Switcher)
 
 
 @dataclass
 class Theme(metaclass=ABCMeta):
-    """An abstract base class for theme classes."""
+    """An abstract base class for theme configuration."""
 
-    measure: Size = Size(70, "ch")
+    measure: Size = Size(110, "ch")
     line_height: float = 1.4
 
-    borders: Borders = field(default_factory=Borders)
-    rounding: Rounding = field(default_factory=Rounding)
     fonts: Fonts = field(default_factory=Fonts)
     colors: Colors = field(default_factory=Colors)
     sizes: Sizes = field(default_factory=Sizes)
+
+    borders: Borders = field(default_factory=Borders)
+    rounding: Rounding = field(default_factory=Rounding)
     headers: Headers = field(default_factory=Headers)
 
+    layouts: Layouts = field(default_factory=Layouts)
+
     def __eq__(self, other: object) -> bool:
         return isinstance(other, Theme) and self.name == other.name
 
     @property
     @abstractmethod
     def name(self) -> str:
         """Name of the theme."""
```

### Comparing `ludic-0.4.0/ludic/styles/types.py` & `ludic-0.4.1/ludic/styles/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Mapping
-from typing import Literal, Self, TypedDict
+from typing import Literal, LiteralString, Self, SupportsIndex, TypedDict
 
 from .utils import (
     darken_color,
     hex_to_rgb,
     lighten_color,
     pick_readable_color_for,
 )
@@ -71,46 +71,55 @@
                     formatted = f"{formatted}{unit}"
                 self = super().__new__(cls, formatted)
 
         self.value = value
         self.unit = unit
         return self
 
-    def scale(self, factor: float) -> Self:
+    def __mul__(self, factor: float | int | LiteralString | SupportsIndex) -> Self:
         """Scale size by a given factor.
 
         Args:
             factor (float): Scaling factor.
 
         Returns:
             str: Scaled size.
         """
-        return type(self)(self.value * factor, self.unit)
+        if isinstance(factor, float | int):
+            return type(self)(self.value * factor, self.unit)
+        else:
+            return self
 
-    def inc(self, factor: float = 1) -> Self:
+    def __add__(self, value: float | int | LiteralString | SupportsIndex) -> Self:
         """Increment size by a given factor.
 
         Args:
-            factor (float, optional): Increment factor. Defaults to 1.
+            value (float, optional): Increment value.
 
         Returns:
             str: Incremented size.
         """
-        return type(self)(self.value + float(self.value * factor), self.unit)
+        if isinstance(value, float | int):
+            return type(self)(self.value + value, self.unit)
+        else:
+            return self
 
-    def dec(self, factor: float = 1) -> Self:
+    def __sub__(self, value: float | int | LiteralString | SupportsIndex) -> Self:
         """Decrement size by a given factor.
 
         Args:
-            factor (float, optional): Decrement factor. Defaults to 1.
+            value (float, optional): Decrement value.
 
         Returns:
             str: Decremented size.
         """
-        return type(self)(self.value - float(self.value * factor), self.unit)
+        if isinstance(value, float | int):
+            return type(self)(self.value - value, self.unit)
+        else:
+            return self
 
 
 CSSProperties = TypedDict(
     "CSSProperties",
     {
         # A
         "align-content": Literal[
@@ -308,19 +317,19 @@
             "none",
             "unset",
         ],
         "empty-cells": Literal["show", "hide"],
         # F
         "filter": str,
         "flex": str,
-        "flex-basis": str,
+        "flex-basis": float | str,
         "flex-direction": Literal["row", "row-reverse", "column", "column-reverse"],
         "flex-flow": str,
-        "flex-grow": str,
-        "flex-shrink": str,
+        "flex-grow": float | str,
+        "flex-shrink": float | str,
         "flex-wrap": Literal["nowrap", "wrap", "wrap-reverse"],
         "float": Literal["left", "right", "none"],
         "font": str,
         "font-family": str,
         "font-feature-settings": str,
         "font-kerning": Literal["auto", "normal", "none"],
         "font-language-override": str,
```

### Comparing `ludic-0.4.0/ludic/styles/utils.py` & `ludic-0.4.1/ludic/styles/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/web/app.py` & `ludic-0.4.1/ludic/web/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,35 +92,43 @@
 
     def register_route(
         self,
         path: str,
         method: Literal[
             "GET", "HEAD", "POST", "PUT", "DELETE", "PATCH", "OPTIONS"
         ] = "GET",
+        name: str | None = None,
         include_in_schema: bool = True,
     ) -> Callable[[TCallable], TCallable]:
         """Register an endpoint to the application."""
 
         def register(handler: TCallable) -> TCallable:
             self.add_route(
-                path, handler, methods=[method], include_in_schema=include_in_schema
+                path,
+                handler,
+                methods=[method],
+                name=name,
+                include_in_schema=include_in_schema,
             )
             return handler
 
         return register
 
     def endpoint(
         self,
         path: str,
+        name: str | None = None,
         include_in_schema: bool = True,
     ) -> Callable[[type[TEndpoint]], type[TEndpoint]]:
         """Register a Ludic class endpoint to the application."""
 
         def register(endpoint: type[TEndpoint]) -> type[TEndpoint]:
-            self.add_route(path, endpoint, include_in_schema=include_in_schema)
+            self.add_route(
+                path, endpoint, name=name, include_in_schema=include_in_schema
+            )
             return endpoint
 
         return register
 
     def add_route(
         self,
         path: str,
```

### Comparing `ludic-0.4.0/ludic/web/datastructures.py` & `ludic-0.4.1/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/web/endpoints.py` & `ludic-0.4.1/ludic/web/endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         Returns:
             The URL.
         """
         request = self.context.get("request")
 
         if request is None or not isinstance(request, Request):
             raise RuntimeError(
-                f"{type(self).__name__} is not bound to an app, you need to set the"
-                f"{type(self).__name__}.app property in order to use Endpoint.url_for."
+                f"{type(self).__name__} is not bound to a request, you can only use "
+                f"the {type(self).__name__}.url_for method in the context of a request."
             )
 
         if inspect.isclass(endpoint) and issubclass(endpoint, Endpoint):
             endpoint_generic_args = get_element_generic_args(endpoint)
             self_generic_args = get_element_generic_args(self)
 
             if (
```

### Comparing `ludic-0.4.0/ludic/web/exceptions.py` & `ludic-0.4.1/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/web/parsers.py` & `ludic-0.4.1/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/web/requests.py` & `ludic-0.4.1/ludic/web/requests.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,17 +44,23 @@
             endpoint_name = endpoint
         elif (route := getattr(endpoint, "route", None)) and isinstance(route, Route):
             endpoint_name = route.name
         else:
             raise NoMatchFound(str(endpoint), path_params)
 
         if partial_mount := self.scope.get("partial_mount"):
-            endpoint_name = join_mounts(partial_mount, endpoint_name)
-
-        return router.url_path_for(endpoint_name, **path_params)
+            try:
+                return router.url_path_for(
+                    join_mounts(partial_mount, endpoint_name),
+                    **path_params,
+                )
+            except NoMatchFound:
+                return router.url_path_for(endpoint_name, **path_params)
+        else:
+            return router.url_path_for(endpoint_name, **path_params)
 
     def url_for(self, endpoint: str | Callable[..., Any], /, **path_params: Any) -> URL:
         """Get URL for an endpoint.
 
         Args:
             endpoint: The endpoint to get the URL for, can be name or a registered
                 endpoint class.
```

### Comparing `ludic-0.4.0/ludic/web/responses.py` & `ludic-0.4.1/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/ludic/web/routing.py` & `ludic-0.4.1/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/tests/test_components.py` & `ludic-0.4.1/tests/test_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.catalog.typography import Link, Paragraph
 from ludic.html import b
 
 
 def test_link() -> None:
     link = Link("A link!", to="https://example.com")
-    assert link.to_html() == '<a href="https://example.com">A link!</a>'
+    assert link.to_html() == '<a href="https://example.com" target="_blank">A link!</a>'
+    link = Link("A link!", to="/home")
+    assert link.to_html() == '<a href="/home">A link!</a>'
 
 
 def test_paragraph() -> None:
     paragraph = Paragraph(
         "Hello, how ",
         b("are you"),
         "? Click ",
@@ -25,44 +27,46 @@
         "<Paragraph>"
           'Hello, how <b>are you</b>? Click <Link to="https://example.com">here</Link>.'
         "</Paragraph>"
     )  # fmt: skip
     assert paragraph.to_html() == (
         '<p>'
             'Hello, how <b>are you</b>? '
-            'Click <a href="https://example.com">here</a>.'
+            'Click <a href="https://example.com" target="_blank">here</a>.'
         '</p>'
     )  # fmt: skip
 
 
 def test_navigation() -> None:
     navigation = Navigation(
         NavItem("Home", to="/"),
         NavItem("About", to="/about"),
         id="nav",
     )
     assert navigation.to_html() == (
-        '<nav id="nav">'
-            "<ul>"
-                '<li id="home"><a href="/">Home</a></li>'
-                '<li id="about"><a href="/about">About</a></li>'
+        '<nav id="nav" class="navigation">'
+            '<ul class="stack small">'
+                '<li class="nav-item"><a href="/" class="small btn link">Home</a></li>'
+                '<li class="nav-item">'
+                    '<a href="/about" class="small btn link">About</a>'
+                '</li>'
             "</ul>"
         "</nav>"
     )  # fmt: skip
 
 
 def test_pairs() -> None:
     pairs = Pairs(
         Key("Name"),
         Value("John"),
         Key("Age"),
         Value(42),
     )
     assert pairs.to_html() == (
-        '<dl class="stack stack-small">'
+        '<dl class="stack small">'
             '<dt>Name</dt>'
             '<dd>John</dd>'
             '<dt>Age</dt>'
             '<dd>42</dd>'
         "</dl>"
     )  # fmt: skip
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
 from ludic.catalog.forms import Form, InputField, TextAreaField from
 ludic.catalog.items import Key, Pairs, Value from ludic.catalog.navigation
 import Navigation, NavItem from ludic.catalog.tables import Table, TableHead,
 TableRow from ludic.catalog.typography import Link, Paragraph from ludic.html
 import b def test_link() -> None: link = Link("A link!", to="https://
-example.com") assert link.to_html() == '_A_ _l_i_n_k_!' def test_paragraph() -> None:
+example.com") assert link.to_html() == '_A_ _l_i_n_k_!' link = Link("A link!", to="/
+home") assert link.to_html() == '_A_ _l_i_n_k_!' def test_paragraph() -> None:
 paragraph = Paragraph( "Hello, how ", b("are you"), "? Click ", Link("here",
 to="https://example.com"), ".", ) assert isinstance(paragraph.children[3],
 Link) assert paragraph.children[3].attrs["to"] == "https://example.com" assert
 paragraph.to_string(pretty=False) == ( "" 'Hello, how aarree yyoouu? Click
 here.' "" ) # fmt: skip assert paragraph.to_html() == ( '
 ' 'Hello, how aarree yyoouu? ' 'Click _h_e_r_e.' '
 ' ) # fmt: skip def test_navigation() -> None: navigation = Navigation( NavItem
 ("Home", to="/"), NavItem("About", to="/about"), id="nav", ) assert
-navigation.to_html() == ( '' "
-    * " '
+navigation.to_html() == ( '' '
+    * ' '
     * _H_o_m_e
     * ' '
-    * _A_b_o_u_t
+    * ' '_A_b_o_u_t' '
     * ' "
 " "" ) # fmt: skip def test_pairs() -> None: pairs = Pairs( Key("Name"), Value
 ("John"), Key("Age"), Value(42), ) assert pairs.to_html() == ( '
 ' '
 " ) # fmt: skip def test_tables() -> None: table = Table( TableHead("Name",
 "Age"), TableRow("John", 42), TableRow("Jane", 43), ) assert table.header ==
 ("Name", "Age") assert table.getlist("Name") == ["John", "Jane"] assert
```

### Comparing `ludic-0.4.0/tests/test_elements.py` & `ludic-0.4.1/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/tests/test_examples.py` & `ludic-0.4.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/tests/test_exceptions.py` & `ludic-0.4.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/tests/test_formatting.py` & `ludic-0.4.1/tests/test_formatting.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,23 @@
     paragraph = Paragraph(
         f"Hello, how {strong("are you")}? Click {Link("here", to="https://example.com")}.",
     )
     assert isinstance(paragraph.children[3], Link)
     assert paragraph.children[3].attrs["to"] == "https://example.com"
     assert paragraph.to_string(pretty=False) == (
         "<Paragraph>"
-          'Hello, how <strong>are you</strong>? Click <Link to="https://example.com">here</Link>.'
+          'Hello, how <strong>are you</strong>? '
+          'Click <Link to="https://example.com">here</Link>.'
         "</Paragraph>"
     )  # fmt: skip
     assert paragraph.to_html() == (
-        '<p>Hello, how <strong>are you</strong>? Click <a href="https://example.com">here</a>.</p>'
+        "<p>"
+        "Hello, how <strong>are you</strong>? Click "
+        '<a href="https://example.com" target="_blank">here</a>.'
+        "</p>"
     )
 
 
 def test_escaping_works() -> None:
     link = '<a href="https://example.com">test</a>'
     dom = p(f"Hello, how <b>are you</b>? Click {link}.")
     assert dom.to_html() == (
```

#### html2text {}

```diff
@@ -21,17 +21,17 @@
 with context: text = f"test {b("baz")} {i("foo")}" assert div(text) == div
 ("test ", b("baz"), " ", i("foo")) assert div(f"test {div(f"foo {b("nested")},
 {i("nested2")}")}") == div( "test ", div("foo ", b("nested"), ", ", i
 ("nested2")), ) assert context.get() == {} def test_component_with_f_string() -
 > None: paragraph = Paragraph( f"Hello, how {strong("are you")}? Click {Link
 ("here", to="https://example.com")}.", ) assert isinstance(paragraph.children
 [3], Link) assert paragraph.children[3].attrs["to"] == "https://example.com"
-assert paragraph.to_string(pretty=False) == ( "" 'Hello, how aarree yyoouu? Click
-here.' "" ) # fmt: skip assert paragraph.to_html() == ( '
-Hello, how aarree yyoouu? Click _h_e_r_e.
-' ) def test_escaping_works() -> None: link = '_t_e_s_t' dom = p(f"Hello, how aarree
+assert paragraph.to_string(pretty=False) == ( "" 'Hello, how aarree yyoouu? ' 'Click
+here.' "" ) # fmt: skip assert paragraph.to_html() == ( "
+" "Hello, how aarree yyoouu? Click " '_h_e_r_e.' "
+" ) def test_escaping_works() -> None: link = '_t_e_s_t' dom = p(f"Hello, how aarree
 yyoouu? Click {link}.") assert dom.to_html() == ( "
 Hello, how <b>are you</b>? " 'Click <a href="https://example.com">test</a>.
 ' ) def test_quotes_not_escaped() -> None: dom = p("It's alive <3.") assert
 dom.to_html() == "
 It's alive <3.
 "
```

### Comparing `ludic-0.4.0/tests/test_types.py` & `ludic-0.4.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/tests/styles/__init__.py` & `ludic-0.4.1/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/tests/styles/test_styles.py` & `ludic-0.4.1/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/tests/styles/test_themes.py` & `ludic-0.4.1/tests/styles/test_themes.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     assert theme.colors.primary.darken(0.5).rgb == (97, 115, 126)
 
 
 def test_theme_font_sizes() -> None:
     theme = FooTheme(fonts=Fonts(size=Size(10, "px")))
 
     assert theme.fonts.size == "10px"
-    assert theme.fonts.plain == "sans-serif"
+    assert theme.fonts.plain == "Helvetica Neue, Helvetica, Arial, sans-serif"
 
 
 def test_themes_switching() -> None:
     foo, bar = FooTheme(), BarTheme()
 
     set_default_theme(foo)
     assert get_default_theme() == foo
```

#### html2text {}

```diff
@@ -11,27 +11,28 @@
 == (127, 127, 127) assert theme.colors.white.darken(1).rgb == (1, 1, 1) assert
 theme.colors.black.lighten(0.5).rgb == (127, 127, 127) assert
 theme.colors.black.lighten(1).rgb == (255, 255, 255) assert
 theme.colors.light.darken(0.5).rgb == (119, 119, 119) assert
 theme.colors.dark.lighten(0.5).rgb == (153, 153, 153) assert
 theme.colors.primary.darken(0.5).rgb == (97, 115, 126) def
 test_theme_font_sizes() -> None: theme = FooTheme(fonts=Fonts(size=Size(10,
-"px"))) assert theme.fonts.size == "10px" assert theme.fonts.plain == "sans-
-serif" def test_themes_switching() -> None: foo, bar = FooTheme(), BarTheme()
-set_default_theme(foo) assert get_default_theme() == foo set_default_theme(bar)
-assert get_default_theme() == bar def test_element_theme_switching() -> None:
-foo = FooTheme() bar = BarTheme() set_default_theme(bar) class C1(Component
-[str, GlobalAttrs]): styles = style.use( lambda theme: { "#c1 a": {"color":
-theme.colors.warning}, } ) @override def render(self) -> div: return div( b
-("Hello, ", style={"color": self.theme.colors.secondary}), a(*self.children,
-href="https://example.com"), id="c1", ) class C2(Component[str, GlobalAttrs]):
-styles = style.use( lambda theme: { "#c2 a": {"color": theme.colors.danger}, }
-) @override def render(self) -> div: return div( foo.use(C1(*self.children)),
-id="c2", style={"background-color": self.theme.colors.primary}, ) assert C2
-("World").to_html() == ( f'
+"px"))) assert theme.fonts.size == "10px" assert theme.fonts.plain ==
+"Helvetica Neue, Helvetica, Arial, sans-serif" def test_themes_switching() -
+> None: foo, bar = FooTheme(), BarTheme() set_default_theme(foo) assert
+get_default_theme() == foo set_default_theme(bar) assert get_default_theme() ==
+bar def test_element_theme_switching() -> None: foo = FooTheme() bar = BarTheme
+() set_default_theme(bar) class C1(Component[str, GlobalAttrs]): styles =
+style.use( lambda theme: { "#c1 a": {"color": theme.colors.warning}, } )
+@override def render(self) -> div: return div( b("Hello, ", style={"color":
+self.theme.colors.secondary}), a(*self.children, href="https://example.com"),
+id="c1", ) class C2(Component[str, GlobalAttrs]): styles = style.use( lambda
+theme: { "#c2 a": {"color": theme.colors.danger}, } ) @override def render
+(self) -> div: return div( foo.use(C1(*self.children)), id="c2", style=
+{"background-color": self.theme.colors.primary}, ) assert C2("World").to_html()
+== ( f'
 ' '
 ' f'HHeelllloo,, ' '_W_o_r_l_d' "
 " "
 " ) # fmt: skip assert style.from_components(C1, C2).to_html() == ( '
 " ) # fmt: skip set_default_theme(foo) assert style.from_components(C1,
 C2).to_html() == ( '
 " ) # fmt: skip
```

### Comparing `ludic-0.4.0/.gitignore` & `ludic-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/LICENCE` & `ludic-0.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/README.md` & `ludic-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.0/pyproject.toml` & `ludic-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 ]
 
 [project.optional-dependencies]
 full = [
     "python-multipart>=0.0.9",
     "starlette",
     "typeguard>=4.1.5",
+    "pygments",
+]
+dev = [
+    "mypy",
+    "types-pygments",
 ]
 test = [
     "pytest",
     "pytest-cov",
     "httpx",
 ]
```

### Comparing `ludic-0.4.0/PKG-INFO` & `ludic-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.0
+Version: 0.4.1
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.12
 Requires-Dist: typing-extensions>=4.9.0
+Provides-Extra: dev
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: types-pygments; extra == 'dev'
 Provides-Extra: full
+Requires-Dist: pygments; extra == 'full'
 Requires-Dist: python-multipart>=0.0.9; extra == 'full'
 Requires-Dist: starlette; extra == 'full'
 Requires-Dist: typeguard>=4.1.5; extra == 'full'
 Provides-Extra: test
 Requires-Dist: httpx; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
```

