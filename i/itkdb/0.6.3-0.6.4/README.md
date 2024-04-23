# Comparing `tmp/itkdb-0.6.3.tar.gz` & `tmp/itkdb-0.6.4.tar.gz`

## Comparing `itkdb-0.6.3.tar` & `itkdb-0.6.4.tar`

### file list

```diff
@@ -1,183 +1,184 @@
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 itkdb-0.6.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.6.3/.linkcheckerrc
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 itkdb-0.6.3/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.6.3/add_attachment.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.6.3/add_comment.py
--rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.6.3/generatePlots.py
--rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.6.3/getContentSummary.py
--rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.6.3/getInventory.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 itkdb-0.6.3/mkdocs.yml
--rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.6.3/registerComponent.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 itkdb-0.6.3/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.6.3/ci/pre-commit-update.sh
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/config.md
--rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/examples.md
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/history.md
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/index.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/install.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/macros.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/.overrides/main.html
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/assets/css/custom.css
--rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/meta/authors.md
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/meta/faq.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/reference/gen_ref_nav.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/reference/cli/itkdb.md
--rw-r--r--   0        0        0    21379 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts.css
--rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2
--rw-r--r--   0        0        0    16700 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2
--rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2
--rw-r--r--   0        0        0    17508 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2
--rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2
--rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2
--rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2
--rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2
--rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2
--rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2
--rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2
--rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2
--rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2
--rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2
--rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2
--rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2
--rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2
--rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2
--rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2
--rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2
--rw-r--r--   0        0        0    25916 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2
--rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2
--rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/_version.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/_version.pyi
--rw-r--r--   0        0        0    14226 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/client.py
--rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/commandline.py
--rw-r--r--   0        0        0    15267 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/core.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/eos.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/py.typed
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/responses.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/typing.py
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/utils.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/caching/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/caching/adapter.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/caching/controller.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/caching/utils.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/data/1x1.jpg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/data/1x1.sh
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/data/CERN_chain.pem
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/data/README.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/data/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/data/tiny.root
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/models/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/models/component.py
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/models/file.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/models/institution.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/settings/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 itkdb-0.6.3/src/itkdb/settings/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/__init__.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/conftest.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_cli.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_client.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_image.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_response.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_scripts.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_session.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_user.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/test_utils.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_attachments.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_binaryData.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_cache.py
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_components.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_institution.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_models.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_projects.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_session.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_shipments.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_stats.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_summary.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_testproperties.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_tests.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_user.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/test_warning.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_attachments.test_add_attachment.json
--rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_empty_file.json
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_image.json
--rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_json.json
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_plainText.json
--rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_issue4.json
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_add_comment.json
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json
--rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_get.json
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_get_component_bulk.json
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_get_component_info_code.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_get_component_info_serial.json
--rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
--rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
--rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_componentsv1.json
--rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_componentsv2.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_institution.test_get.json
--rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_institution.test_pagination.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_projects.test_list_projects.json
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_session.test_fake_route.json
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_session.test_invalid_project.json
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_session.test_missing_required.json
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_session.test_no_bearer.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_session.test_unauthorized.json
--rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_stats.test_get.json
--rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_summary.test_get_summary.json
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_tests.test_list_test_types.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_user.test_user_anonymous_login.json
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_user.test_user_bad_login.json
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_user.test_user_good_login.json
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.6.3/tests/integration/cassettes/test_warnings.test_get_component.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.6.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.6.3/COPYING
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.6.3/LICENSE
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.6.3/README.md
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 itkdb-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 itkdb-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 itkdb-0.6.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.6.4/.linkcheckerrc
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 itkdb-0.6.4/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.6.4/add_attachment.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.6.4/add_comment.py
+-rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.6.4/generatePlots.py
+-rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.6.4/getContentSummary.py
+-rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.6.4/getInventory.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 itkdb-0.6.4/mkdocs.yml
+-rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.6.4/registerComponent.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 itkdb-0.6.4/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.6.4/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/config.md
+-rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/examples.md
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/history.md
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/index.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/install.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/macros.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/.overrides/main.html
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/meta/authors.md
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/meta/faq.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/reference/gen_ref_nav.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/reference/cli/itkdb.md
+-rw-r--r--   0        0        0    21379 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts.css
+-rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2
+-rw-r--r--   0        0        0    16700 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2
+-rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2
+-rw-r--r--   0        0        0    17508 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2
+-rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2
+-rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2
+-rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2
+-rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2
+-rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2
+-rw-r--r--   0        0        0    24072 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2
+-rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2
+-rw-r--r--   0        0        0    22168 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2
+-rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2
+-rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2
+-rw-r--r--   0        0        0    25916 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2
+-rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2
+-rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/_version.pyi
+-rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/client.py
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/commandline.py
+-rw-r--r--   0        0        0    15267 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/core.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/eos.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/py.typed
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/responses.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/typing.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/utils.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/caching/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/caching/adapter.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/caching/controller.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/caching/utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/data/1x1.jpg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/data/1x1.sh
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/data/CERN_chain.pem
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/data/README.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/data/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/data/tiny.root
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/models/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/models/component.py
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/models/file.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/models/institution.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/settings/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 itkdb-0.6.4/src/itkdb/settings/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/conftest.py
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_cli.py
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_client.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_image.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_response.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_scripts.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_session.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_user.py
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/test_utils.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_attachments.py
+-rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_binaryData.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_cache.py
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_components.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_institution.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_models.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_projects.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_session.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_shipments.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_summary.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_testproperties.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_tests.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_user.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/test_warning.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_attachments.test_add_attachment.json
+-rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_empty_file.json
+-rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_image.json
+-rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_json.json
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_plainText.json
+-rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_issue4.json
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_add_comment.json
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json
+-rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_get.json
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_get_component_bulk.json
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_get_component_info_code.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_get_component_info_serial.json
+-rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
+-rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
+-rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_componentsv1.json
+-rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_componentsv2.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_institution.test_get.json
+-rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_institution.test_pagination.json
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_projects.test_list_projects.json
+-rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_session.test_fake_route.json
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_session.test_invalid_project.json
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_session.test_missing_required.json
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_session.test_no_bearer.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_session.test_unauthorized.json
+-rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_stats.test_get.json
+-rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_summary.test_get_summary.json
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_tests.test_duplicate_test_run.json
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_tests.test_list_test_types.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_user.test_user_anonymous_login.json
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_user.test_user_bad_login.json
+-rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_user.test_user_good_login.json
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.6.4/tests/integration/cassettes/test_warnings.test_get_component.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.6.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.6.4/COPYING
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.6.4/LICENSE
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.6.4/README.md
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 itkdb-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     9298 2020-02-02 00:00:00.000000 itkdb-0.6.4/PKG-INFO
```

### Comparing `itkdb-0.6.3/.gitlab-ci.yml` & `itkdb-0.6.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/.pre-commit-config.yaml` & `itkdb-0.6.4/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.8.0]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.7
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.9.0"
     hooks:
```

### Comparing `itkdb-0.6.3/generatePlots.py` & `itkdb-0.6.4/generatePlots.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/getContentSummary.py` & `itkdb-0.6.4/getContentSummary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/getInventory.py` & `itkdb-0.6.4/getInventory.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/mkdocs.yml` & `itkdb-0.6.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/registerComponent.py` & `itkdb-0.6.4/registerComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tbump.toml` & `itkdb-0.6.4/tbump.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e36 2e33 220a 0a23 2045  t = "0.6.3"..# E
+00000010: 7420 3d20 2230 2e36 2e34 220a 0a23 2045  t = "0.6.4"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 362e  mp version: 0.6.
-00000150: 3320 e286 9220 7b6e 6577 5f76 6572 7369  3 ... {new_versi
+00000150: 3420 e286 9220 7b6e 6577 5f76 6572 7369  4 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `itkdb-0.6.3/ci/pre-commit-update.sh` & `itkdb-0.6.4/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/config.md` & `itkdb-0.6.4/docs/config.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/examples.md` & `itkdb-0.6.4/docs/examples.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/history.md` & `itkdb-0.6.4/docs/history.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
 **_Changed:_**
 
 **_Added:_**
 
 **_Fixed:_**
 
+## [0.6.4](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.6.4) - 2024-04-18 ## {: #itkdb-v0.6.4 }
+
+**_Added:_**
+
+- [itkdb.Client.post][] now has a keyword argument `allow_duplicate` which defaults to `True`. If set to `False`, will check if a duplicate object exists before POST'ing it to the production database. Currently, this logic is implemented for `uploadTestRunResults`. Refer to documentation of [itkdb.Client.post][] to see what other endpoints are supported.
+
 ## [0.6.3](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.6.3) - 2024-04-17 ## {: #itkdb-v0.6.3 }
 
 **_Changed:_**
 
 - Reverted changes for 0.6.2 which were broken.
 
 ## [0.6.2](https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/-/tags/v0.6.2) - 2024-04-17 ## {: #itkdb-v0.6.2 }
```

### Comparing `itkdb-0.6.3/docs/index.md` & `itkdb-0.6.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/install.md` & `itkdb-0.6.4/docs/install.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/assets/css/custom.css` & `itkdb-0.6.4/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/assets/images/logo.svg` & `itkdb-0.6.4/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/meta/faq.md` & `itkdb-0.6.4/docs/meta/faq.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/reference/gen_ref_nav.py` & `itkdb-0.6.4/docs/reference/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts.css` & `itkdb-0.6.4/docs/stylesheets/fonts.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc-CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc0CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc1CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc2CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc3CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc5CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TjASc6CsQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic-CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic0CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic1CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic2CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic3CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic5CsTKlA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOjCnqEu92Fr1Mu51TzBic6CsQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xEIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xFIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xGIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xHIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xIIzI.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xLIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOkCnqEu92Fr1Mu51xMIzIFKw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fABc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBBc4.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fBxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCBc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCRc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fChc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmSU5fCxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfABc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBBc4.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfBxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCBc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCRc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfChc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOlCnqEu92Fr1MmWUlfCxc4EsA.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4WxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu4mxK.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu5mxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu72xKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7GxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7WxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/KFOmCnqEu92Fr1Mu7mxKOzY.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSV0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSZ0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSd0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSh0mQ.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSt0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xTDF4xlVMF-BfR8bXMIhJHg45mwgGEFl0_3vrtSM1J-gEPT5Ese6hmHSx0mf0h.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtElOUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEleUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEluUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEm-Ul.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEmOUlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2` & `itkdb-0.6.4/docs/stylesheets/fonts/L0xdDF4xlVMF-BfR8bXMIjhOsXG-q2oeuFoqFrlnAIe2Imhk1T8rbociImtEn-UlYIw.woff2`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/client.py` & `itkdb-0.6.4/src/itkdb/core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,393 +1,426 @@
 from __future__ import annotations
 
 import logging
-from functools import partial
-from urllib.parse import urlparse
-
-from requests.exceptions import HTTPError
-
-from itkdb import eos, exceptions, models, utils
-from itkdb.core import Session
-from itkdb.data import path as itkdb_data
-from itkdb.responses import PagedResponse
+import pickle  # nosec
+import time
+from pathlib import Path
+from typing import Any, Callable, ClassVar, cast
+
+import cachecontrol.caches.file_cache
+import requests
+from cachecontrol.heuristics import ExpiresAfter
+from jose import jwt
+from requests.status_codes import codes
+
+from itkdb import exceptions
+from itkdb._version import __version__
+from itkdb.caching import CacheControlAdapter, CacheController
+from itkdb.settings import settings
+from itkdb.typing import UserLike
 
 log = logging.getLogger(__name__)
 
 
-class Client(Session):
+class UserBearer(UserLike):
     """
-    The top-level user-facing client for interacting with the ITk Production Database API.
+    Class for managing bearer tokens.
 
-    !!! note "Changed in version 0.4.0"
-        - added `use_eos` argument
+    Args:
+        bearer (str): Bearer token
+        prefix_url (str): The prefix for all non-absolute URIs
 
-    !!! note "Changed in version 0.4.6"
-        - added `pagination_history` argument
+    !!! note "Added in version 0.6.0"
     """
 
-    limit = -1
-
-    def __init__(self, use_eos=False, pagination_history=False, **session_kwargs):
-        self._use_eos = use_eos
-        self._pagination_history = pagination_history
-        super().__init__(**session_kwargs)
-
-    def request(self, method, url, *args, **kwargs):
-        self.limit = kwargs.pop("limit", -1)
-
-        response = super(Session, self).request(method, url, *args, **kwargs)
-        return self._response_handler(response)
-
-    def get(self, url, **kwargs):
-        is_cern_url = ".cern.ch" in urlparse(url).netloc
-        # is_binary_data = "uu-app-binarystore/getBinaryData" in url
-        if is_cern_url:
-            log.info(
-                "Identified a cern.ch request, will attach CERN SSL chain to request by overriding `verify`."
-            )
-            kwargs["verify"] = itkdb_data / "CERN_chain.pem"
-
-        # getBinaryData does not handle chunked requests
-        # if is_cern_url or is_binary_data:
-        if is_cern_url:
-            log.info(
-                "Identified a request that potentially downloads larger amounts of data, will execute chunked requests (stream=True)."
-            )
-            kwargs["stream"] = True
-            headers = kwargs.get("headers", {})
-            headers["transfer-encoding"] = "chunked"
-            kwargs["headers"] = headers
-        return super().get(url, **kwargs)
+    def __init__(
+        self,
+        bearer: str = settings.ITKDB_AUDREYTWO_API_KEY,
+    ):
+        # session handling (for injection in tests)
+        self._session = requests.Session()
+        self._session.headers.update({"User-Agent": f"itkdb/{__version__}"})
+        # store last call to authenticate
+        self._response: requests.Response | None = None
+        self._status_code: int | None = None
+        # initialization configuration
+        self._bearer: str = bearer
 
-    def _handle_warnings(self, data):
-        warnings = data.pop("uuAppErrorMap", {})
-        try:
-            for key, message in warnings.items():
-                log.warning("%s: %s", key, message)
-        except AttributeError:
-            # it's a string like:
-            #   'uuAppErrorMap': '#<UuApp::Oidc::Session:0x00561d53890118>'
-            log.warning(warnings)
+    def authenticate(self) -> bool:
+        return True
 
-    def upload_to_eos(self, response, eos_file_details=None, **_) -> None:
+    @property
+    def bearer(self) -> str:
         """
-        requests response hook function to upload a file to eos.
+        The bearer token.
         """
-        log.info("I was able to get a token to upload to EOS. Let me upload.")
-        try:
-            response.raise_for_status()
-        except HTTPError:
-            log.warning("Something went wrong with uploading to EOS.")
-            return response
+        return self._bearer
 
-        # do nothing if betamax is being used (no need to run the cURL for EOS)
-        if response.connection.__class__.__name__ == "BetamaxAdapter":
-            return None
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__:s}(bearer={self.bearer})"
 
-        token_request = response.json()
 
-        log.info(token_request)
+class User(UserLike):
+    """
+    Class for managing user tokens and authentication flow.
 
-        response.eos_response = eos.put(
-            token_request["token"], token_request["url"], eos_file_details
-        )
-        return None
+    Args:
+        access_code1 (str): ITkPD Access Code 1
+        access_code2 (str): ITkPD Access Code 2
+        audience (str): ITkPD OIDC Audience
+        prefix_url (str): The prefix for all non-absolute URIs
+        jwt_options (dict): Additional JWT options to pass through
+        save_auth (pathlib.Path | str | None): If set, save authentication information to the file path specified
+        auth_expiry_threshold (int): Number of seconds until token expiration to do a reauthentication
 
-    def delete_from_eos(self, response, **_) -> None:
-        """
-        requests response hook function to delete a file from eos.
-        """
-        try:
-            response.raise_for_status()
-        except HTTPError:
-            log.warning("Something went wrong with deleting the attachment.")
-            return response
-
-        data = response.json()
-
-        # do nothing if it's not an EOS-type attachment
-        # or if betamax is being used (no need to run the cURL for EOS)
-        if (
-            data["attachment"]["type"] != "eos"
-            or response.connection.__class__.__name__ == "BetamaxAdapter"
-        ):
-            return None
-
-        if "token" not in data:
-            log.warning(
-                "It seems there is no token, so we are not deleting this from EOS."
+    !!! note "Changed in version 0.4.0"
+        - renamed `accessCode1` / `accessCode2` to `access_code1` / `access_code2`
+
+    !!! note "Added in version 0.4.7"
+        - `auth_expiry_threshold` to force reauthentication sooner
+
+    """
+
+    def __init__(
+        self,
+        access_code1: str = settings.ITKDB_ACCESS_CODE1,
+        access_code2: str = settings.ITKDB_ACCESS_CODE2,
+        audience: str = settings.ITKDB_ACCESS_AUDIENCE,
+        prefix_url: str = settings.ITKDB_AUTH_URL,
+        jwt_options: dict[str, Any] | None = None,
+        save_auth: Path | str | None = None,
+        auth_expiry_threshold: int = 15,
+    ):
+        # session handling (for injection in tests)
+        self._session = requests.Session()
+        self._session.headers.update({"User-Agent": f"itkdb/{__version__}"})
+        # store last call to authenticate
+        self._response: requests.Response | None = None
+        self._status_code: int | None = None
+        # store jwks for validation/verification
+        self._jwks: dict[str, Any] | None = None
+        # store information after authorization occurs
+        self._access_token: str | None = None
+        self._raw_id_token: str | None = None
+        self._id_token: dict[str, Any] | None = None
+        # initialization configuration
+        self._access_code1: str = access_code1
+        self._access_code2: str = access_code2
+        self._audience: str = audience
+        self._prefix_url: str = prefix_url
+        # update jwt_options if provided
+        self._jwt_options: dict[str, Any] = {
+            "leeway": int(settings.ITKDB_LEEWAY)
+        }  # **jwt_options, python3 only
+        self._jwt_options.update(jwt_options or {})
+        # serialization/persistence
+        self._save_auth: Path | None = Path(save_auth) if save_auth else None
+        self.auth_expiry_threshold: int = auth_expiry_threshold
+        self._load()
+
+    def _load(self) -> bool:
+        if self._save_auth and self._save_auth.is_file():
+            try:
+                with self._save_auth.open("rb") as _pickle_file:
+                    saved_user = pickle.load(_pickle_file)  # nosec
+                if saved_user.is_expired():
+                    log.warning(
+                        "Saved user session is expired in %s. Creating a new one.",
+                        self._save_auth,
+                    )
+                    return False
+                if saved_user.is_authenticated():
+                    self.__dict__.update(saved_user.__dict__)
+                    return True
+            except pickle.UnpicklingError:
+                log.warning(
+                    "Unable to load user session from %s. Creating a new one.",
+                    self._save_auth,
+                )
+        return False
+
+    def _dump(self) -> bool:
+        if self.is_authenticated() and not self.is_expired() and self._save_auth:
+            with self._save_auth.open("wb") as fpointer:
+                try:
+                    pickle.dump(self, fpointer, pickle.HIGHEST_PROTOCOL)
+                    return True
+                except (pickle.PicklingError, AttributeError, TypeError):
+                    log.warning("Unable to save user session to %s.", self._save_auth)
+            return False
+        return False
+
+    def _load_jwks(self, force: bool = False) -> None:
+        if self._jwks is None or force:
+            self._jwks = self._session.get(
+                "https://uuidentity.plus4u.net/uu-oidc-maing02/bb977a99f4cc4c37a2afce3fd599d0a7/oidc/listKeys"
+            ).json()
+
+    def _parse_id_token(self) -> None:
+        if self._raw_id_token:
+            self._load_jwks()
+            assert self._jwks
+            self._id_token = jwt.decode(
+                self._raw_id_token,
+                self._jwks,
+                algorithms="RS256",
+                audience=self._audience,
+                options=self._jwt_options,
             )
-            return None
 
-        log.info(
-            "It looks like you're deleting an attachment from ITk PD that is stored on EOS, I will try to delete it from EOS for you."
+    def authenticate(self) -> bool:
+        """
+        Authenticate the current user if not already authenticated.
+
+        If the current user session is expired, this will attempt to reauthenticate.
+        """
+        # if not expired, do nothing
+        if self.is_authenticated():
+            if not self.is_expired():
+                return True
+            log.warning("User session is expired. Creating a new one.")
+
+        # session-less request
+        response = self._session.post(
+            requests.compat.urljoin(self._prefix_url, "grantToken"),
+            json={
+                "grant_type": "password",
+                "accessCode1": self._access_code1,
+                "accessCode2": self._access_code2,
+                "scope": settings.ITKDB_ACCESS_SCOPE,
+            },
         )
+        self._response = response
+        self._status_code = response.status_code
+        self._access_token = response.json().get("access_token")
+        self._raw_id_token = response.json().get("id_token")
+        self._id_token = None
 
-        response.eos_response = eos.delete(data["token"], data["attachment"]["url"])
-        return None
+        # handle parsing the id token
+        self._parse_id_token()
 
-    def _request_handler(self, request):
-        if request.url == self._normalize_url("/itkdbPoisonPillTest"):
-            request.url = self._normalize_url("/poison")
-        elif request.url == self._normalize_url("/createComponentAttachment"):
-            if not self.use_eos:
-                return
-
-            if not eos.HAS_PYCURL:
-                msg = "You are trying to upload to EOS, but you did not install itkdb[eos] or pycurl is not installed correctly."
-                raise RuntimeError(msg)
+        if not self.is_authenticated():
+            raise exceptions.ResponseException(self._response)
 
-            fname, fpointer, ftype, fheaders = utils.get_file_components(request.files)
+        self._dump()
+        return True
 
-            if not utils.is_eos_uploadable(fname, fpointer):
-                return
+    @property
+    def access_code1(self) -> str:
+        """
+        The first access code.
+        """
+        return self._access_code1
 
-            log.info(
-                "It looks like you're attaching an image, root, or large file, I will try to put it on EOS for you."
-            )
+    @property
+    def access_code2(self) -> str:
+        """
+        The second access code.
+        """
+        return self._access_code2
 
-            # update headers
-            fheaders = fheaders or {}
-            request.headers.update(fheaders)
-
-            ftype = ftype or utils.get_mimetype(fname, fpointer)
-
-            details = {
-                "type": "component",
-                "id": request.data["component"],
-                "title": request.data["title"],
-                "description": request.data["description"],
-                "filesize": utils.get_filesize(fname, fpointer),
-            }
-
-            leftover = {
-                k: v
-                for k, v in request.data.items()
-                if k not in ["component", "title", "description"]
-            }
-
-            if leftover:
-                log.warning("Ignoring user-specified data=%s", leftover)
-
-            request.json = details
-            request.data = None
-            request.files = None
-            request.hooks["response"] = [
-                partial(
-                    self.upload_to_eos,
-                    eos_file_details=(fname, fpointer, ftype, fheaders),
-                )
-            ]
-            request.url = self._normalize_url("requestUploadEosFile")
-        elif request.url == self._normalize_url("/createTestRunAttachment"):
-            if not self.use_eos:
-                return
-
-            if not eos.HAS_PYCURL:
-                msg = "You are trying to upload to EOS, but you did not install itkdb[eos] or pycurl is not installed correctly."
-                raise RuntimeError(msg)
+    @property
+    def access_token(self) -> str | None:
+        """
+        The opaque access token for the user.
+        """
+        return self._access_token
+
+    @property
+    def id_token(self) -> dict[str, str | list[str] | int]:
+        """
+        The parsed JWT identity token for the user.
+        """
+        return self._id_token if self._id_token else {}
 
-            fname, fpointer, ftype, fheaders = utils.get_file_components(request.files)
+    @property
+    def name(self) -> str:
+        """
+        The name for the user.
+        """
+        return cast(str, self.id_token.get("name", ""))
 
-            if not utils.is_eos_uploadable(fname, fpointer):
-                return
+    @property
+    def expires_at(self) -> int:
+        """
+        The Epoch Unix Timestamp that the user session expires at.
+        """
+        return cast(int, self.id_token.get("exp", 0))
 
-            log.info(
-                "It looks like you're attaching an image, root, or large file, I will try to put it on EOS for you."
-            )
+    @property
+    def expires_in(self) -> int:
+        """
+        The time until expiration in seconds.
+        """
+        expires_in: float = self.expires_at - time.time()
+        return 0 if expires_in < 0 else int(expires_in)
 
-            # update headers
-            fheaders = fheaders or {}
-            request.headers.update(fheaders)
-
-            ftype = ftype or utils.get_mimetype(fname, fpointer)
-
-            details = {
-                "type": "testRun",
-                "id": request.data["testRun"],
-                "title": request.data["title"],
-                "description": request.data["description"],
-                "filesize": utils.get_filesize(fname, fpointer),
-            }
-
-            leftover = {
-                k: v
-                for k, v in request.data.items()
-                if k not in ["component", "title", "description"]
-            }
-
-            if leftover:
-                log.warning("Ignoring user-specified data=%s", leftover)
-
-            request.json = details
-            request.data = None
-            request.files = None
-            request.hooks["response"] = [
-                partial(
-                    self.upload_to_eos,
-                    eos_file_details=(fname, fpointer, ftype, fheaders),
-                )
-            ]
-            request.url = self._normalize_url("requestUploadEosFile")
-        elif request.url == self._normalize_url("/createShipmentAttachment"):
-            if not self.use_eos:
-                return
-
-            if not eos.HAS_PYCURL:
-                msg = "You are trying to upload to EOS, but you did not install itkdb[eos] or pycurl is not installed correctly."
-                raise RuntimeError(msg)
+    @property
+    def identity(self) -> str:
+        """
+        The identity for the user in the ITk Production Database.
+        """
+        return cast(str, self.id_token.get("uuidentity", ""))
 
-            fname, fpointer, ftype, fheaders = utils.get_file_components(request.files)
+    @property
+    def bearer(self) -> str:
+        """
+        The bearer token for the user.
+        """
+        return self._raw_id_token if self._raw_id_token else ""
 
-            if not utils.is_eos_uploadable(fname, fpointer):
-                return
+    def is_authenticated(self) -> bool:
+        """
+        Whether current user is authenticated.
+        """
+        return bool(
+            self._status_code == codes["ok"]
+            and self._access_token
+            and self._raw_id_token
+        )
 
-            log.info(
-                "It looks like you're attaching an image, root, or large file, I will try to put it on EOS for you."
-            )
+    def is_expired(self) -> bool:
+        """
+        Whether current user session is expired given the expiration threshold.
+        """
+        return not self.expires_in > self.auth_expiry_threshold
 
-            # update headers
-            request.headers.update(fheaders)
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__:s}(name={self.name:s}, expires_in={self.expires_in:d}s)"
 
-            details = {
-                "type": "shipment",
-                "id": request.data["shipment"],
-                "title": request.data["title"],
-                "description": request.data["description"],
-                "filesize": utils.get_filesize(fname, fpointer),
-            }
-
-            leftover = {
-                k: v
-                for k, v in request.data.items()
-                if k not in ["component", "title", "description"]
-            }
-
-            if leftover:
-                log.warning("Ignoring user-specified data=%s", leftover)
-
-            request.json = details
-            request.data = None
-            request.files = None
-            request.hooks["response"] = [
-                partial(
-                    self.upload_to_eos,
-                    eos_file_details=(fname, fpointer, ftype, fheaders),
-                )
-            ]
-            request.url = self._normalize_url("requestUploadEosFile")
-        elif request.url in [
-            self._normalize_url("/deleteComponentAttachment"),
-            self._normalize_url("/deleteTestRunAttachment"),
-            self._normalize_url("/deleteShipmentAttachment"),
-        ]:
-            if not self.use_eos or not eos.HAS_PYCURL:
-                msg = "You are trying to delete an attachment that might be on EOS, but you did not install itkdb[eos] or pycurl is not installed correctly."
-                raise RuntimeError(msg)
-
-            request.hooks["response"] = [self.delete_from_eos]
-
-    def _response_handler(self, response):
-        # sometimes we don't get content-type, so make sure it's a string at least
-        content_type = response.headers.get("content-type", "")
-        if content_type is None and not response.url.startswith(
-            "https://eosatlas.cern.ch"
-        ):
-            return response
-
-        if (
-            content_type.startswith("application/json")
-            and not response.url.endswith("uu-app-binarystore/getBinaryData")
-            and not response.url.startswith("https://eosatlas.cern.ch")
-        ):
-            if response.headers.get("content-length") == "0":
-                return {}
 
-            try:
-                data = response.json()
-                self._handle_warnings(data)
-            except ValueError as err:
-                raise exceptions.BadJSON(response) from err
-
-            limit = self.limit
-            self.limit = -1  # reset the limit again
-            if "pageItemList" in data:
-                return PagedResponse(
-                    super(),
-                    response,
-                    history=self._pagination_history,
-                    limit=limit,
-                    key="pageItemList",
-                )
+class Session(requests.Session):
+    """
+    Lightweight wrapper around `requests.Session` with basic error-handling, auto-(re)authentication, and URI prefixing.
 
-            if "itemList" in data:
-                page_info = data.get("pageInfo", None)
-                if page_info and (
-                    page_info["pageIndex"] * page_info["pageSize"] < page_info["total"]
-                ):
-                    return PagedResponse(
-                        super(),
-                        response,
-                        history=self._pagination_history,
-                        limit=limit,
-                        key="itemList",
-                    )
-                return data["itemList"]
+    For more information, see python requests.
 
-            if "testRunList" in data:
-                return data["testRunList"]
+    Attributes:
+        STATUS_EXCEPTIONS (dict): Mapping from status code to [itkdb.exceptions][]
+        SUCCESS_STATUSES (dict): List of status codes that are OK
+        auth (callable): Call [itkdb.core.Session.authorize][]
+        prefix_url (str): The prefix for all non-absolute URIs
+        user (itkdb.core.User): The user object for authentication
+
+    Args:
+        user (itkdb.core.User): A user object. Create one if not specified.
+        prefix_url (str): The prefix url to use for all requests.
+        save_auth (pathlib.Path | str | None): A file path to where to save authentication information.
+        cache (str): A CacheControl.caches object for cache (default: cachecontrol.caches.file_cache.FileCache). Set to False to disable cache.
+        expires_after (dict): The arguments are the same as the datetime.timedelta object. This will override or add the Expires header and override or set the Cache-Control header to public.
+        auth_expiry_threshold (int): Number of seconds until token expiration to do a reauthentication (see itkdb.core.User)
 
-            if "dtoSample" in data:
-                return data["dtoSample"]
+    !!! note "Added in version 0.4.7"
+        - `auth_expiry_threshold` to force reauthentication sooner
 
-            return data
-
-        # we've got a file or attachment we're downloading of some kind, so
-        # dump to tempfile and seek from there to determine behavior
-        binary_file = models.BinaryFile.from_response(response)
-        is_cern_url = ".cern.ch" in urlparse(response.url).netloc
-
-        if (
-            is_cern_url
-            and binary_file.mimetype == "application/octet-stream"
-            and binary_file.content_type != "application/octet-stream"
-        ):
-            log.warning(
-                "Changing the mimetype for the response from EOS from 'application/octet-stream' to '%s'.",
-                binary_file.content_type,
-            )
-            binary_file._mimetype = (  # pylint: disable=protected-access
-                binary_file.content_type
-            )
-            response.headers["content-type"] = binary_file.mimetype
+    """
 
-        mimetype = binary_file.mimetype or ""
-        if mimetype.startswith("image/"):
-            binary_file.__class__ = models.ImageFile
-        elif mimetype.startswith(("text/", "text")) or mimetype == "application/json":
-            binary_file.__class__ = models.TextFile
-        elif mimetype == "application/zip":
-            binary_file = models.ZipFile(binary_file)
-        elif binary_file.mimetype is None:
-            log.warning(
-                "No mimetype available. This is likely an empty file. Defaulting to BinaryFile."
+    STATUS_EXCEPTIONS: ClassVar[dict[int, type[exceptions.ITkDBException]]] = {
+        codes["bad_gateway"]: exceptions.ServerError,
+        codes["bad_request"]: exceptions.BadRequest,
+        codes["conflict"]: exceptions.Conflict,
+        codes["found"]: exceptions.Redirect,
+        codes["forbidden"]: exceptions.Forbidden,
+        codes["gateway_timeout"]: exceptions.ServerError,
+        codes["internal_server_error"]: exceptions.ServerError,
+        codes["media_type"]: exceptions.SpecialError,
+        codes["not_found"]: exceptions.NotFound,
+        codes["request_entity_too_large"]: exceptions.TooLarge,
+        codes["service_unavailable"]: exceptions.ServerError,
+        codes["unauthorized"]: exceptions.Forbidden,
+        codes["unavailable_for_legal_reasons"]: exceptions.UnavailableForLegalReasons,
+    }
+    SUCCESS_STATUSES: ClassVar[set[int]] = {codes["created"], codes["ok"]}
+
+    def __init__(
+        self,
+        user: User | None = None,
+        prefix_url: str = settings.ITKDB_API_URL,
+        save_auth: Path | str | None = None,
+        cache: bool | object = True,
+        expires_after: dict[str, int] | None = None,
+        auth_expiry_threshold: int = 15,
+    ):
+        super().__init__()
+        self.headers.update({"User-Agent": f"itkdb/{__version__}"})
+        self.user: UserLike = (
+            user
+            if user
+            else User(save_auth=save_auth, auth_expiry_threshold=auth_expiry_threshold)
+        )
+        self.auth: Callable[[requests.PreparedRequest], requests.PreparedRequest] = (
+            self.authorize
+        )
+        self.prefix_url: str = prefix_url
+        # store last call
+        self._response: requests.Response | None = None
+
+        cache_options = {}
+        if cache:
+            cache = (
+                cachecontrol.caches.file_cache.FileCache(".webcache")
+                if cache is True
+                else cache
             )
-        else:
-            log.warning(
-                "No model available for Content-Type: '%s'. Defaulting to BinaryFile.",
-                mimetype,
+            cache_options.update({"cache": cache})
+
+        # handle expirations for cache
+        if expires_after and isinstance(expires_after, dict):
+            cache_options.update({"heuristic": ExpiresAfter(**expires_after)})
+
+        if cache_options:
+            # add caching
+            super().mount(
+                self.prefix_url,
+                CacheControlAdapter(controller_class=CacheController, **cache_options),
             )
 
-        return binary_file
+    def authorize(self, req: requests.PreparedRequest) -> requests.PreparedRequest:
+        """
+        Add authentication information to the request by updating the headers.
+        """
+        if req.url.startswith(self.prefix_url):  # type: ignore[union-attr]
+            self.user.authenticate()
+            req.headers.update({"Authorization": f"Bearer {self.user.bearer:s}"})
+        return req
+
+    def _normalize_url(self, url: str | bytes) -> str:
+        url_str = url.decode("utf-8") if isinstance(url, bytes) else url
+        return requests.compat.urljoin(self.prefix_url, url_str)
+
+    def _check_response(self, response: requests.Response) -> None:
+        if response.status_code in self.STATUS_EXCEPTIONS:
+            raise self.STATUS_EXCEPTIONS[response.status_code](response)
+
+        try:
+            response.raise_for_status()
+        except BaseException as err:
+            raise exceptions.UnhandledResponse(response) from err
 
-    def prepare_request(self, request):
+    def prepare_request(self, request: requests.Request) -> requests.PreparedRequest:
         request.url = self._normalize_url(request.url)
-        self._request_handler(request)
         return super().prepare_request(request)
 
-    @property
-    def use_eos(self):
-        """
-        Flag indicating whether to use eos for uploading attachments.
-        """
-        return self._use_eos
+    def send(
+        self, request: requests.PreparedRequest, **kwargs: Any
+    ) -> requests.Response:
+        response = super().send(request, **kwargs)
+        self._response = response
+        log.debug(
+            "Response: %s (%s bytes)",
+            response.status_code,
+            response.headers.get("content-length"),
+        )
+        self._check_response(response)
+        return response
+
+    def request(
+        self, method: str | bytes, url: str | bytes, *args: Any, **kwargs: Any
+    ) -> requests.Response:
+        url = self._normalize_url(url)
+        return super().request(method, url, *args, **kwargs)
+
+    def __call__(self, *args: Any, **kwargs: Any) -> requests.Response:
+        if len(args) == 1:
+            return self.send(self.prepare_request(*args), **kwargs)
+
+        return self.request(*args, **kwargs)
```

### Comparing `itkdb-0.6.3/src/itkdb/commandline.py` & `itkdb-0.6.4/src/itkdb/commandline.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/eos.py` & `itkdb-0.6.4/src/itkdb/eos.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/exceptions.py` & `itkdb-0.6.4/src/itkdb/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,7 +145,15 @@
 
 class UnavailableForLegalReasons(ResponseException):
     """Indicate that the requested URL is unavailable due to legal reasons."""
 
 
 class UnhandledResponse(ResponseException):
     """Indicate a response status code we have not dealt with yet."""
+
+
+class DuplicateObjectsInDB(ITkDBException):
+    """Indicate duplicate checker found a duplicate item when not allowing for duplicates."""
+
+
+class DuplicateTestRuns(DuplicateObjectsInDB):
+    """Indicate that duplicate test runs were found."""
```

### Comparing `itkdb-0.6.3/src/itkdb/responses.py` & `itkdb-0.6.4/src/itkdb/responses.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/typing.py` & `itkdb-0.6.4/src/itkdb/typing.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/utils.py` & `itkdb-0.6.4/src/itkdb/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/caching/adapter.py` & `itkdb-0.6.4/src/itkdb/caching/adapter.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/caching/controller.py` & `itkdb-0.6.4/src/itkdb/caching/controller.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/caching/utils.py` & `itkdb-0.6.4/src/itkdb/caching/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/data/1x1.sh` & `itkdb-0.6.4/src/itkdb/data/1x1.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/data/CERN_chain.pem` & `itkdb-0.6.4/src/itkdb/data/CERN_chain.pem`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/data/README.md` & `itkdb-0.6.4/src/itkdb/data/README.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/models/component.py` & `itkdb-0.6.4/src/itkdb/models/component.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/models/file.py` & `itkdb-0.6.4/src/itkdb/models/file.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/models/institution.py` & `itkdb-0.6.4/src/itkdb/models/institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/src/itkdb/settings/base.py` & `itkdb-0.6.4/src/itkdb/settings/base.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/conftest.py` & `itkdb-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/test_cli.py` & `itkdb-0.6.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/test_client.py` & `itkdb-0.6.4/tests/test_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import math
 
 import betamax
+import pytest
 import requests
 
 import itkdb
 
 
 def test_client(auth_user):
     assert itkdb.Client(user=auth_user)
@@ -155,7 +156,37 @@
 
     assert prepped.url == auth_client._normalize_url("/requestUploadEosFile")
     assert prepped.headers.get("content-type") == "application/json"
     assert req.data is None
     assert req.files is None
     assert req.json is not None
     assert len(prepped.hooks["response"]) != 0
+
+
+def test_duplicate_test_run_exception_no_json(auth_client):
+    auth_client._get_duplicate_test_runs = lambda _: ["duplicate_test_run_id"]
+
+    with pytest.raises(ValueError, match="didn't provide any data"):
+        auth_client.post("uploadTestRunResults", allow_duplicate=False)
+
+    with pytest.raises(ValueError, match="didn't provide any data"):
+        auth_client.post(
+            "uploadTestRunResults", data={"key": "value"}, allow_duplicate=False
+        )
+
+
+def test_duplicate_test_run_exception_has_duplicates(auth_client):
+    auth_client._get_duplicate_test_runs = lambda _: ["duplicate_test_run_id"]
+
+    with pytest.raises(itkdb.exceptions.DuplicateTestRuns):
+        auth_client.post(
+            "uploadTestRunResults", json={"key": "value"}, allow_duplicate=False
+        )
+
+
+def test_duplicate_test_run_exception_unsupported_endpoint(auth_client):
+    auth_client._get_duplicate_test_runs = lambda _: ["duplicate_test_run_id"]
+
+    with pytest.raises(ValueError, match="No logic exists to check"):
+        auth_client.post(
+            "fakeRouteNotHandled", json={"key": "value"}, allow_duplicate=False
+        )
```

### Comparing `itkdb-0.6.3/tests/test_image.py` & `itkdb-0.6.4/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/test_response.py` & `itkdb-0.6.4/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/test_scripts.py` & `itkdb-0.6.4/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/test_session.py` & `itkdb-0.6.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/test_user.py` & `itkdb-0.6.4/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/test_utils.py` & `itkdb-0.6.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_attachments.py` & `itkdb-0.6.4/tests/integration/test_attachments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_binaryData.py` & `itkdb-0.6.4/tests/integration/test_binaryData.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_cache.py` & `itkdb-0.6.4/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_components.py` & `itkdb-0.6.4/tests/integration/test_components.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_institution.py` & `itkdb-0.6.4/tests/integration/test_institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_session.py` & `itkdb-0.6.4/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_shipments.py` & `itkdb-0.6.4/tests/integration/test_shipments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_summary.py` & `itkdb-0.6.4/tests/integration/test_summary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_testproperties.py` & `itkdb-0.6.4/tests/integration/test_testproperties.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_user.py` & `itkdb-0.6.4/tests/integration/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/test_warning.py` & `itkdb-0.6.4/tests/integration/test_warning.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_attachments.test_add_attachment.json` & `itkdb-0.6.4/tests/integration/cassettes/test_attachments.test_add_attachment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_attachments.test_list_all_attachments.json` & `itkdb-0.6.4/tests/integration/cassettes/test_attachments.test_list_all_attachments.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_empty_file.json` & `itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_empty_file.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_image.json` & `itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_image.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json` & `itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_json.json` & `itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_json.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_plainText.json` & `itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_plainText.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_get_zipfile.json` & `itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_get_zipfile.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_binaryData.test_issue4.json` & `itkdb-0.6.4/tests/integration/cassettes/test_binaryData.test_issue4.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_add_comment.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_add_comment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_delete_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_get.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_get_component_bulk.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_get_component_bulk.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_get_component_info_code.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_get_component_info_code.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_get_component_info_serial.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_get_component_info_serial.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_componentsv1.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_componentsv1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_components.test_list_componentsv2.json` & `itkdb-0.6.4/tests/integration/cassettes/test_components.test_list_componentsv2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_institution.test_get.json` & `itkdb-0.6.4/tests/integration/cassettes/test_institution.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_institution.test_pagination.json` & `itkdb-0.6.4/tests/integration/cassettes/test_institution.test_pagination.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_projects.test_list_projects.json` & `itkdb-0.6.4/tests/integration/cassettes/test_projects.test_list_projects.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json` & `itkdb-0.6.4/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json` & `itkdb-0.6.4/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json` & `itkdb-0.6.4/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_session.test_fake_route.json` & `itkdb-0.6.4/tests/integration/cassettes/test_session.test_fake_route.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_session.test_invalid_project.json` & `itkdb-0.6.4/tests/integration/cassettes/test_session.test_invalid_project.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_session.test_missing_required.json` & `itkdb-0.6.4/tests/integration/cassettes/test_session.test_missing_required.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_session.test_no_bearer.json` & `itkdb-0.6.4/tests/integration/cassettes/test_session.test_no_bearer.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json` & `itkdb-0.6.4/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_stats.test_get.json` & `itkdb-0.6.4/tests/integration/cassettes/test_stats.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_summary.test_get_summary.json` & `itkdb-0.6.4/tests/integration/cassettes/test_summary.test_get_summary.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_testproperties.test_delete_test_property.json` & `itkdb-0.6.4/tests/integration/cassettes/test_testproperties.test_delete_test_property.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json` & `itkdb-0.6.4/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_tests.test_list_test_types.json` & `itkdb-0.6.4/tests/integration/cassettes/test_tests.test_list_test_types.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_user.test_user_anonymous_login.json` & `itkdb-0.6.4/tests/integration/cassettes/test_user.test_user_anonymous_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_user.test_user_bad_login.json` & `itkdb-0.6.4/tests/integration/cassettes/test_user.test_user_bad_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_user.test_user_good_login.json` & `itkdb-0.6.4/tests/integration/cassettes/test_user.test_user_good_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/tests/integration/cassettes/test_warnings.test_get_component.json` & `itkdb-0.6.4/tests/integration/cassettes/test_warnings.test_get_component.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/.gitignore` & `itkdb-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/COPYING` & `itkdb-0.6.4/COPYING`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/LICENSE` & `itkdb-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/README.md` & `itkdb-0.6.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ITk DB v0.6.3
+# ITk DB v0.6.4
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

### Comparing `itkdb-0.6.3/pyproject.toml` & `itkdb-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkdb-0.6.3/PKG-INFO` & `itkdb-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkdb
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python wrapper to interface with ITk DB.
 Project-URL: Documentation, https://itkdb.docs.cern.ch/0.6/
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Author-email: Giordon Stark <kratsg@gmail.com>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>
@@ -42,15 +42,15 @@
 Requires-Dist: urllib3>=1.26.11
 Provides-Extra: contrib
 Requires-Dist: html2text; extra == 'contrib'
 Provides-Extra: eos
 Requires-Dist: pycurl; extra == 'eos'
 Description-Content-Type: text/markdown
 
-# ITk DB v0.6.3
+# ITk DB v0.6.4
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

