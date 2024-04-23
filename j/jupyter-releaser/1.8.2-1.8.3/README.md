# Comparing `tmp/jupyter_releaser-1.8.2.tar.gz` & `tmp/jupyter_releaser-1.8.3.tar.gz`

## Comparing `jupyter_releaser-1.8.2.tar` & `jupyter_releaser-1.8.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.readthedocs.yml
--rw-r--r--   0        0        0   140606 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/RELEASE.md
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/actions/check-release/action.yml
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/actions/finalize-release/action.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/actions/install-releaser/action.yml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/actions/populate-release/action.yml
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/actions/prep-release/action.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/actions/publish-changelog/action.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/scripts/bump_tag.sh
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/scripts/install-releaser.sh
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/generate-changelog.yml
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/prep-self-release.yml
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/publish-changelog.yml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/publish-self-release.yml
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/make.bat
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/conf.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/index.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/_static/custom.css
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/_static/images/logo/favicon.svg
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/_static/images/logo/logo.svg
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/background/index.rst
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/background/theory.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/get_started/generate_changelog.md
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/get_started/index.rst
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/get_started/making_release_from_releaser.md
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/get_started/making_release_from_repo.md
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/how_to_guides/convert_repo_from_releaser.md
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/how_to_guides/convert_repo_from_repo.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/how_to_guides/index.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/how_to_guides/maintain_fork.md
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/how_to_guides/write_config.md
--rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/draft_github_release.png
--rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/final_github_release.png
--rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/fork_fetch.png
--rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/generate_changelog.png
--rw-r--r--   0        0        0    39051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/prep_release.png
--rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/prep_release_next_step.png
--rw-r--r--   0        0        0    35251 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/prep_release_repo.png
--rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/publish_release.png
--rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/publish_release_next_step.png
--rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/images/publish_release_repo.png
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/reference/api_docs.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/reference/configuration.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/reference/faq.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/reference/index.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/docs/source/reference/releaser_cli.rst
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/example-workflows/full-release.yml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/example-workflows/prep-release.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/example-workflows/publish-changelog.yml
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/example-workflows/publish-release.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/__main__.py
--rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/changelog.py
--rw-r--r--   0        0        0    21115 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/cli.py
--rw-r--r--   0        0        0    21876 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/lib.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/mock_github.py
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/npm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/py.typed
--rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/python.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/schema.json
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/tee.py
--rw-r--r--   0        0        0    24794 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/actions/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/actions/common.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/actions/finalize_release.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/actions/generate_changelog.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/actions/populate_release.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/actions/prep_release.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/jupyter_releaser/actions/publish_changelog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/tests/__init__.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/tests/conftest.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/tests/test_changelog.py
--rw-r--r--   0        0        0    28051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/tests/test_cli.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/tests/test_functions.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/tests/test_mock_github.py
--rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/tests/util.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/.gitignore
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/LICENSE
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/README.md
--rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.readthedocs.yml
+-rw-r--r--   0        0        0   141564 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/RELEASE.md
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/actions/check-release/action.yml
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/actions/finalize-release/action.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/actions/install-releaser/action.yml
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/actions/populate-release/action.yml
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/actions/prep-release/action.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/actions/publish-changelog/action.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/scripts/bump_tag.sh
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/scripts/install-releaser.sh
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/generate-changelog.yml
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/prep-self-release.yml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/publish-changelog.yml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/publish-self-release.yml
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/make.bat
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/conf.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/index.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/_static/custom.css
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/_static/images/logo/favicon.svg
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/_static/images/logo/logo.svg
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/background/index.rst
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/background/theory.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/get_started/generate_changelog.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/get_started/index.rst
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/get_started/making_release_from_releaser.md
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/get_started/making_release_from_repo.md
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/how_to_guides/convert_repo_from_releaser.md
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/how_to_guides/convert_repo_from_repo.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/how_to_guides/index.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/how_to_guides/maintain_fork.md
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/how_to_guides/write_config.md
+-rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/draft_github_release.png
+-rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/final_github_release.png
+-rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/fork_fetch.png
+-rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/generate_changelog.png
+-rw-r--r--   0        0        0    39051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/prep_release.png
+-rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/prep_release_next_step.png
+-rw-r--r--   0        0        0    35251 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/prep_release_repo.png
+-rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/publish_release.png
+-rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/publish_release_next_step.png
+-rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/images/publish_release_repo.png
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/reference/api_docs.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/reference/configuration.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/reference/faq.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/reference/index.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/docs/source/reference/releaser_cli.rst
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/example-workflows/full-release.yml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/example-workflows/prep-release.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/example-workflows/publish-changelog.yml
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/example-workflows/publish-release.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/__main__.py
+-rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/changelog.py
+-rw-r--r--   0        0        0    21115 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/cli.py
+-rw-r--r--   0        0        0    21876 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/lib.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/mock_github.py
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/npm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/py.typed
+-rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/python.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/schema.json
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/tee.py
+-rw-r--r--   0        0        0    24794 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/actions/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/actions/common.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/actions/finalize_release.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/actions/generate_changelog.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/actions/populate_release.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/actions/prep_release.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/jupyter_releaser/actions/publish_changelog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/tests/__init__.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/tests/conftest.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/tests/test_changelog.py
+-rw-r--r--   0        0        0    28051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/tests/test_cli.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/tests/test_functions.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/tests/test_mock_github.py
+-rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/tests/util.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/.gitignore
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/LICENSE
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/README.md
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.3/PKG-INFO
```

### Comparing `jupyter_releaser-1.8.2/.pre-commit-config.yaml` & `jupyter_releaser-1.8.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/CHANGELOG.md` & `jupyter_releaser-1.8.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.8.3
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...f709700203f8b3f1398fd16189ee26cc48c53ea0))
+
+### Bugs fixed
+
+- Fix `maxsplit` usage [#572](https://github.com/jupyter-server/jupyter_releaser/pull/572) ([@krassowski](https://github.com/krassowski))
+
+### Documentation improvements
+
+- Improve documentation [#569](https://github.com/jupyter-server/jupyter_releaser/pull/569) ([@fcollonval](https://github.com/fcollonval))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2024-04-22&to=2024-04-23&type=c))
+
+[@fcollonval](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Afcollonval+updated%3A2024-04-22..2024-04-23&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Akrassowski+updated%3A2024-04-22..2024-04-23&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.8.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...24ecdc098199ebbb59667fe009551ed425de08df))
 
 ### Bugs fixed
 
 - Prepend tag with Python package name if multiple packages are defined [#570](https://github.com/jupyter-server/jupyter_releaser/pull/570) ([@krassowski](https://github.com/krassowski))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2024-04-18&to=2024-04-22&type=c))
 
 [@krassowski](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Akrassowski+updated%3A2024-04-18..2024-04-22&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.8.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...ba6e1a5170e41cc76e14d9ab77bb16b0d8fe6cda))
 
 ### Bugs fixed
 
 - Normalise package name before comparison [#568](https://github.com/jupyter-server/jupyter_releaser/pull/568) ([@krassowski](https://github.com/krassowski))
```

### Comparing `jupyter_releaser-1.8.2/CONTRIBUTING.md` & `jupyter_releaser-1.8.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/actions/check-release/action.yml` & `jupyter_releaser-1.8.3/.github/actions/check-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/actions/finalize-release/action.yml` & `jupyter_releaser-1.8.3/.github/actions/finalize-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/actions/populate-release/action.yml` & `jupyter_releaser-1.8.3/.github/actions/populate-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/actions/prep-release/action.yml` & `jupyter_releaser-1.8.3/.github/actions/prep-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/actions/publish-changelog/action.yml` & `jupyter_releaser-1.8.3/.github/actions/publish-changelog/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/check-release.yml` & `jupyter_releaser-1.8.3/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/generate-changelog.yml` & `jupyter_releaser-1.8.3/.github/workflows/generate-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/prep-release.yml` & `jupyter_releaser-1.8.3/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/prep-self-release.yml` & `jupyter_releaser-1.8.3/.github/workflows/prep-self-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/publish-changelog.yml` & `jupyter_releaser-1.8.3/.github/workflows/publish-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/publish-release.yml` & `jupyter_releaser-1.8.3/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/publish-self-release.yml` & `jupyter_releaser-1.8.3/.github/workflows/publish-self-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.github/workflows/test.yml` & `jupyter_releaser-1.8.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/Makefile` & `jupyter_releaser-1.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/make.bat` & `jupyter_releaser-1.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/conf.py` & `jupyter_releaser-1.8.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/_static/images/logo/favicon.svg` & `jupyter_releaser-1.8.3/docs/source/_static/images/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/_static/images/logo/logo.svg` & `jupyter_releaser-1.8.3/docs/source/_static/images/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/background/theory.md` & `jupyter_releaser-1.8.3/docs/source/background/theory.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/get_started/generate_changelog.md` & `jupyter_releaser-1.8.3/docs/source/get_started/generate_changelog.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/get_started/making_release_from_releaser.md` & `jupyter_releaser-1.8.3/docs/source/get_started/making_release_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/get_started/making_release_from_repo.md` & `jupyter_releaser-1.8.3/docs/source/get_started/making_release_from_repo.md`

 * *Files 17% similar despite different names*

```diff
@@ -16,21 +16,16 @@
 
 - Click on the "Run workflow" dropdown button on the right
 
 - Fill in the appropriate parameters
 
   ![Prep Release Workflow Dialog](../images/prep_release_repo.png)
 
-- The "New Version Spec" will usually be the full version (e.g. 0.7.1). Repos using `tbump` can also use:
-
-  - "next" or "patch" option, which will bump the micro version (or the build version in the case of a prerelease).
-    Note: The "next" and "patch" options are not available when using dev versions, you must use explicit versions
-    instead.
-  - "minor" option, which will bump to the next minor version directly.
-  - "release" option, which will start making prereleases (a0, a1...)
+- The "New Version Spec" will usually be the full version (e.g. 0.7.1).
+  Repos using `hatch` can also use [segments](https://hatch.pypa.io/latest/version/#supported-segments) such as _patch_, _minor_, _alpha_,... .
 
 - Use the "since" field to select PRs prior to the latest tag to include in the release
 
 - Check "Use PRs with activity since the last stable git tag" if you would like to include PRs since the last non-prerelease version tagged on the target repository and branch.
 
 - The additional "Post Version Spec" field should be used if your repo uses a dev version (e.g. 0.7.0.dev0)
```

### Comparing `jupyter_releaser-1.8.2/docs/source/how_to_guides/convert_repo_from_releaser.md` & `jupyter_releaser-1.8.3/docs/source/how_to_guides/convert_repo_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/how_to_guides/convert_repo_from_repo.md` & `jupyter_releaser-1.8.3/docs/source/how_to_guides/convert_repo_from_repo.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 ## Prerequisites
 
 See checklist below for details:
 
 - Markdown changelog
 - Bump version configuration (if using Python), for example [hatch](https://hatch.pypa.io/latest/)
 - [Access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) with access to target GitHub repo to run GitHub Actions.
-- Set up:
-  - \[_modern way_\] [Add a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/) to your PyPI project
-  - \[_legacy way_\] Access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github)
+- [Add a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/) to your PyPI project
 - If needed, access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens).
 
 ## Checklist for Adoption
 
 - [ ] Set up a [GitHub App](https://docs.github.com/en/apps/creating-github-apps/about-creating-github-apps/about-creating-github-apps#github-apps-that-act-on-their-own-behalf) on your organization (or personal account for a personal project).
 
   - Disable the web hook
@@ -36,45 +34,51 @@
   - Remove global tag protection.
   - Add a branch Ruleset for all branches
     - Allow the GitHub App to bypass protections
     - Set up Pull Request and Required Checks
   - Add a tags Ruleset for all tags
     - Allow the GitHub App to bypass protections
 
-- [ ] Set up PyPI:
-
-<details><summary>Using PyPI trusted publisher (modern way)</summary>
-
-- Set up your PyPI project by [adding a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/)
-  - if you use the example workflows, the _workflow name_ is `publish-release.yml` (or `full-release.yml`) and the
-    _environment_ should be left blank.
-- Ensure the publish release job as `permissions`: `id-token : write` (see the [documentation](https://docs.pypi.org/trusted-publishers/using-a-publisher/))
+- [ ] Copy `prep-release.yml` and `publish-release.yml` (or only `full-release.yml`) from the
+  [example-workflows](https://github.com/jupyter-server/jupyter_releaser/tree/main/example-workflows) folder in this repository.
 
-</details>
-
-<details><summary>Using PyPI token (legacy way)</summary>
-
-- Add access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github) stored as `PYPI_TOKEN`.
-  _Note_ For security reasons, it is recommended that you scope the access
-  to a single repository. Additionally, this token should belong to a
-  machine account and not a user account.
+- [ ] Set up PyPI:
 
-</details>
+  - Set up your PyPI project by [adding a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/)
+    - if you use the example workflows, the _workflow name_ is `publish-release.yml` (or `full-release.yml`) and the
+      _environment_ should be `release` (the name of the GitHub environment).
+  - Ensure the publish release job as `permissions`: `id-token : write` (see the [documentation](https://docs.pypi.org/trusted-publishers/using-a-publisher/))
 
 - [ ] If needed, add access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens), saved as `NPM_TOKEN`. Again this should
   be created using a machine account that only has publish access.
+
 - [ ] Ensure that only trusted users with 2FA have admin access to the repository, since they will be able to trigger releases.
+
 - [ ] Switch to Markdown Changelog
+
   - We recommend [MyST](https://myst-parser.readthedocs.io/en/latest/?badge=latest), especially if some of your docs are in reStructuredText.
   - Can use `pandoc -s changelog.rst -o changelog.md` and some hand edits as needed.
   - Note that [directives](https://myst-parser.readthedocs.io/en/latest/using/syntax.html#syntax-directives) can still be used
-- [ ] Add HTML start and end comment markers to Changelog file - see example in [CHANGELOG.md](https://github.com/jupyter-server/jupyter_releaser/blob/main/CHANGELOG.md) (view in raw mode)
+
+- [ ] Add HTML start and end comment markers to Changelog file
+
+  - see example in [CHANGELOG.md](https://github.com/jupyter-server/jupyter_releaser/blob/main/CHANGELOG.md) (view in raw mode)
+
+```md
+# Changelog
+
+<!-- <START NEW CHANGELOG ENTRY> -->
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+```
+
 - [ ] We recommend using [hatch](https://hatch.pypa.io/latest/) for your
   build system and for version handling.
-  - If previously providing `version_info` like `version_info = (1, 7, 0, '.dev', '0')`, use a pattern like the one below in your version file:
+  - If previously providing `version_info` like `version_info = (1, 7, 0, '.dev', '0')`,
+    use a pattern like the one below in your version file:
 
 ```python
 import re
 from typing import List
 
 # Version string must appear intact for hatch versioning
 __version__ = "6.16.0"
@@ -85,44 +89,61 @@
 assert match is not None
 parts: List[object] = [int(match[part]) for part in ["major", "minor", "patch"]]
 if match["rest"]:
     parts.append(match["rest"])
 version_info = tuple(parts)
 ```
 
-- If you need to keep node and python versions in sync, use [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version). See [nbformat](https://github.com/jupyter/nbformat/blob/main/pyproject.toml) for example.
+- If you need to keep node and python versions in sync, use [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version).
+
+  - See [nbformat](https://github.com/jupyter/nbformat/blob/main/pyproject.toml) for example.
 
 - [ ] Add a GitHub Actions CI step to run the `check_release` action. For example:
 
+  - This should be run on `push` and `pull` request events. You can copy
+    the `check-release.yml` from this repo as an example.
+
 ```yaml
 - name: Check Release
   uses: jupyter-server/jupyter_releaser/.github/actions/check-release@v2
   with:
     token: ${{ secrets.GITHUB_TOKEN }}
 ```
 
-- This should be run on `push` and `pull` request events. You can copy
-  the `check-release.yml` from this repo as an example.
-
 - [ ] If you would like the release assets to be uploaded as artifacts, add the following step after the `check_release` action:
 
 ```yaml
 - name: Upload Distributions
-  uses: actions/upload-artifact@v2
+  uses: actions/upload-artifact@v4
   with:
     name: dist-${{ github.run_number }}
     path: .jupyter_releaser_checkout/dist
 ```
 
-- [ ] Add a workflow that uses the [`enforce-label`](https://github.com/jupyterlab/maintainer-tools#enforce-labels) action from `jupyterlab/maintainer-tools` to ensure that all PRs have on of the triage labels used to
-  categorize the changelog.
+- [ ] Add a workflow that uses the [`enforce-label`](https://github.com/jupyterlab/maintainer-tools#enforce-labels) action
+  from `jupyterlab/maintainer-tools` to ensure that all PRs have on of the triage labels used to categorize the changelog.
 
-- [ ] Update or add `RELEASE.md` that describes the onboarding and release process, e.g. [jupyter_server](https://github.com/jupyter-server/jupyter_server/blob/main/RELEASE.md).
+```yaml
+name: Enforce PR label
 
-- [ ] Copy `prep-release.yml` and `publish-release.yml` from the `example-workflows` folder in this repository.
+on:
+  pull_request:
+    types: [labeled, unlabeled, opened, edited, synchronize]
+
+jobs:
+  enforce-label:
+    runs-on: ubuntu-latest
+    permissions:
+      pull-requests: write
+    steps:
+      - name: enforce-triage-label
+        uses: jupyterlab/maintainer-tools/.github/actions/enforce-label@v1
+```
+
+- [ ] Update or add `RELEASE.md` that describes the onboarding and release process, e.g. [jupyter_server](https://github.com/jupyter-server/jupyter_server/blob/main/RELEASE.md).
 
 - [ ] Optionally add configuration to the repository if non-standard options or hooks are needed.
 
 - [ ] If desired, add `check_release` job, changelog, and `hatch` support to other active release branches
 
 ## Initial Release Workflow
```

### Comparing `jupyter_releaser-1.8.2/docs/source/how_to_guides/write_config.md` & `jupyter_releaser-1.8.3/docs/source/how_to_guides/write_config.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/draft_github_release.png` & `jupyter_releaser-1.8.3/docs/source/images/draft_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/final_github_release.png` & `jupyter_releaser-1.8.3/docs/source/images/final_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/fork_fetch.png` & `jupyter_releaser-1.8.3/docs/source/images/fork_fetch.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/generate_changelog.png` & `jupyter_releaser-1.8.3/docs/source/images/generate_changelog.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/prep_release.png` & `jupyter_releaser-1.8.3/docs/source/images/prep_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/prep_release_next_step.png` & `jupyter_releaser-1.8.3/docs/source/images/prep_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/prep_release_repo.png` & `jupyter_releaser-1.8.3/docs/source/images/prep_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/publish_release.png` & `jupyter_releaser-1.8.3/docs/source/images/publish_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/publish_release_next_step.png` & `jupyter_releaser-1.8.3/docs/source/images/publish_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/images/publish_release_repo.png` & `jupyter_releaser-1.8.3/docs/source/images/publish_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/reference/api_docs.rst` & `jupyter_releaser-1.8.3/docs/source/reference/api_docs.rst`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/docs/source/reference/faq.md` & `jupyter_releaser-1.8.3/docs/source/reference/faq.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/example-workflows/full-release.yml` & `jupyter_releaser-1.8.3/example-workflows/full-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/example-workflows/prep-release.yml` & `jupyter_releaser-1.8.3/example-workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/example-workflows/publish-changelog.yml` & `jupyter_releaser-1.8.3/example-workflows/publish-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/example-workflows/publish-release.yml` & `jupyter_releaser-1.8.3/example-workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/changelog.py` & `jupyter_releaser-1.8.3/jupyter_releaser/changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/cli.py` & `jupyter_releaser-1.8.3/jupyter_releaser/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 @add_options(tag_format_options)
 @use_checkout_dir()
 def bump_version(version_spec, version_cmd, changelog_path, python_packages, tag_format):
     """Prep git and env variables and bump version"""
     prev_dir = os.getcwd()
     for package in python_packages:
         package_path, package_name = (
-            package.split(":", maxsplit=2) if ":" in package else [package, None]
+            package.split(":", maxsplit=1) if ":" in package else [package, None]
         )
         os.chdir(package_path)
         lib.bump_version(
             version_spec,
             version_cmd,
             changelog_path,
             tag_format,
```

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/lib.py` & `jupyter_releaser-1.8.3/jupyter_releaser/lib.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/mock_github.py` & `jupyter_releaser-1.8.3/jupyter_releaser/mock_github.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/npm.py` & `jupyter_releaser-1.8.3/jupyter_releaser/npm.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/python.py` & `jupyter_releaser-1.8.3/jupyter_releaser/python.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/schema.json` & `jupyter_releaser-1.8.3/jupyter_releaser/schema.json`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/tee.py` & `jupyter_releaser-1.8.3/jupyter_releaser/tee.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/util.py` & `jupyter_releaser-1.8.3/jupyter_releaser/util.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/actions/common.py` & `jupyter_releaser-1.8.3/jupyter_releaser/actions/common.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/actions/generate_changelog.py` & `jupyter_releaser-1.8.3/jupyter_releaser/actions/generate_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/actions/populate_release.py` & `jupyter_releaser-1.8.3/jupyter_releaser/actions/populate_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/actions/prep_release.py` & `jupyter_releaser-1.8.3/jupyter_releaser/actions/prep_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/jupyter_releaser/actions/publish_changelog.py` & `jupyter_releaser-1.8.3/jupyter_releaser/actions/publish_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/tests/conftest.py` & `jupyter_releaser-1.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/tests/test_changelog.py` & `jupyter_releaser-1.8.3/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/tests/test_cli.py` & `jupyter_releaser-1.8.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/tests/test_functions.py` & `jupyter_releaser-1.8.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/tests/test_mock_github.py` & `jupyter_releaser-1.8.3/tests/test_mock_github.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/tests/util.py` & `jupyter_releaser-1.8.3/tests/util.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/.gitignore` & `jupyter_releaser-1.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/LICENSE` & `jupyter_releaser-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/README.md` & `jupyter_releaser-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/pyproject.toml` & `jupyter_releaser-1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.2/PKG-INFO` & `jupyter_releaser-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter_releaser
-Version: 1.8.2
+Version: 1.8.3
 Summary: Jupyter Releaser for Python and/or npm packages.
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: Copyright (c) 2021 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

