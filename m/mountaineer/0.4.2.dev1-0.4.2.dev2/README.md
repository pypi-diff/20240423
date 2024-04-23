# Comparing `tmp/mountaineer-0.4.2.dev1.tar.gz` & `tmp/mountaineer-0.4.2.dev2.tar.gz`

## Comparing `mountaineer-0.4.2.dev1.tar` & `mountaineer-0.4.2.dev2.tar`

### file list

```diff
@@ -1,259 +1,259 @@
--rw-r--r--   0     1001      127      269 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src_go/Cargo.toml
--rw-r--r--   0     1001      127     1995 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src_go/build.rs
--rw-r--r--   0     1001      127     5657 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src_go/go/js_build.go
--rw-r--r--   0     1001      127      168 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src_go/go.mod
--rw-r--r--   0     1001      127      376 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src_go/go.sum
--rw-r--r--   0     1001      127     5750 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src_go/src/lib.rs
--rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev1/Cargo.toml
--rw-r--r--   0     1001      127      133 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.git-blame-ignore-revs
--rw-r--r--   0     1001      127      138 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.gitattributes
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/README_SCRIPTS.md
--rw-r--r--   0     1001      127    14036 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/poetry.lock
--rw-r--r--   0     1001      127      767 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/scripts/__init__.py
--rw-r--r--   0     1001      127     3032 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/scripts/__tests__/test_update_version.py
--rw-r--r--   0     1001      127     2181 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/scripts/check_dependencies.py
--rw-r--r--   0     1001      127     3382 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/scripts/update_version.py
--rw-r--r--   0     1001      127     1321 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127    19767 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/workflows/test.yml
--rw-r--r--   0     1001      127      504 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.github/workflows/validate.yml
--rw-r--r--   0     1001      127     3404 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/.gitignore
--rw-r--r--   0     1001      127     1750 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/Dockerfile
--rw-r--r--   0     1001      127     1079 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/LICENSE
--rw-r--r--   0     1001      127     4976 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/Makefile
--rw-r--r--   0     1001      127    14891 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/README.md
--rw-r--r--   0     1001      127      105 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/benchmarking/README.md
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/benchmarking/benchmarking/__init__.py
--rw-r--r--   0     1001      127      425 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/benchmarking/benchmarking/simple_render.py
--rw-r--r--   0     1001      127   127093 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/benchmarking/poetry.lock
--rw-r--r--   0     1001      127      291 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/benchmarking/pyproject.toml
--rw-r--r--   0     1001      127      850 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/README.md
--rw-r--r--   0     1001      127        1 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/__init__.py
--rw-r--r--   0     1001      127      775 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/app.py
--rw-r--r--   0     1001      127      489 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/cli.py
--rw-r--r--   0     1001      127      111 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/config.py
--rw-r--r--   0     1001      127        1 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/__init__.py
--rw-r--r--   0     1001      127     1433 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/complex.py
--rw-r--r--   0     1001      127      581 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/detail.py
--rw-r--r--   0     1001      127     1658 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/home.py
--rw-r--r--   0     1001      127      559 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/stream.py
--rw-r--r--   0     1001      127       77 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/main.py
--rw-r--r--   0     1001      127      208 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/__init__.py
--rw-r--r--   0     1001      127     2261 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx
--rw-r--r--   0     1001      127      453 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/detail/page.tsx
--rw-r--r--   0     1001      127     2822 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx
--rw-r--r--   0     1001      127       59 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/main.css
--rw-r--r--   0     1001      127      708 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx
--rw-r--r--   0     1001      127   125408 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/package-lock.json
--rw-r--r--   0     1001      127      453 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/postcss.config.js
--rw-r--r--   0     1001      127      161 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/tailwind.config.js
--rw-r--r--   0     1001      127   107805 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/poetry.lock
--rw-r--r--   0     1001      127      724 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/ci_webapp/pyproject.toml
--rw-r--r--   0     1001      127     1593 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/README.md
--rw-r--r--   0     1001      127        1 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
--rw-r--r--   0     1001      127     1055 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
--rw-r--r--   0     1001      127     7904 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
--rw-r--r--   0     1001      127      292 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
--rw-r--r--   0     1001      127      816 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
--rw-r--r--   0     1001      127     4277 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/builder.py
--rw-r--r--   0     1001      127     4656 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/cli.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
--rw-r--r--   0     1001      127     1383 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py
--rw-r--r--   0     1001      127     4591 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
--rw-r--r--   0     1001      127     1832 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py
--rw-r--r--   0     1001      127     1336 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/external.py
--rw-r--r--   0     1001      127     1925 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/generation.py
--rw-r--r--   0     1001      127      327 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/io.py
--rw-r--r--   0     1001      127       30 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
--rw-r--r--   0     1001      127      212 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
--rw-r--r--   0     1001      127      190 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
--rw-r--r--   0     1001      127      137 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
--rw-r--r--   0     1001      127      109 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
--rw-r--r--   0     1001      127      170 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.env
--rw-r--r--   0     1001      127     3373 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
--rw-r--r--   0     1001      127      645 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
--rw-r--r--   0     1001      127       17 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
--rw-r--r--   0     1001      127      767 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
--rw-r--r--   0     1001      127      947 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
--rw-r--r--   0     1001      127      282 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
--rw-r--r--   0     1001      127      227 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
--rw-r--r--   0     1001      127     1702 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
--rw-r--r--   0     1001      127     1124 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
--rw-r--r--   0     1001      127       84 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
--rw-r--r--   0     1001      127      157 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
--rw-r--r--   0     1001      127     1219 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
--rw-r--r--   0     1001      127      995 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
--rw-r--r--   0     1001      127       95 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
--rw-r--r--   0     1001      127      524 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
--rw-r--r--   0     1001      127      117 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
--rw-r--r--   0     1001      127      195 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
--rw-r--r--   0     1001      127      332 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
--rw-r--r--   0     1001      127     1493 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
--rw-r--r--   0     1001      127    61104 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/poetry.lock
--rw-r--r--   0     1001      127     1214 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/create_mountaineer_app/pyproject.toml
--rw-r--r--   0     1001      127       30 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/.zed/settings.json
--rw-r--r--   0     1001      127      107 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/README.md
--rw-r--r--   0     1001      127       15 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/CNAME
--rw-r--r--   0     1001      127      310 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/actions.md
--rw-r--r--   0     1001      127      454 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/api_exception.md
--rw-r--r--   0     1001      127       99 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/app-controller.md
--rw-r--r--   0     1001      127      281 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/build_plugins/base.md
--rw-r--r--   0     1001      127       57 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/build_plugins/javascript.md
--rw-r--r--   0     1001      127       62 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/build_plugins/postcss.md
--rw-r--r--   0     1001      127      411 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/cli.md
--rw-r--r--   0     1001      127      376 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/config.md
--rw-r--r--   0     1001      127       61 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/controller.md
--rw-r--r--   0     1001      127       67 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/core_dependencies.md
--rw-r--r--   0     1001      127       66 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/database/config.md
--rw-r--r--   0     1001      127       71 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/database/dependencies.md
--rw-r--r--   0     1001      127       80 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/logging.md
--rw-r--r--   0     1001      127      479 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/render.md
--rw-r--r--   0     1001      127      365 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/ssr.md
--rw-r--r--   0     1001      127      299 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/api/watch_server.md
--rw-r--r--   0     1001      127     9375 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/client_actions.md
--rw-r--r--   0     1001      127      753 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/cma.md
--rw-r--r--   0     1001      127     3021 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/database.md
--rw-r--r--   0     1001      127     4677 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/deploy.md
--rw-r--r--   0     1001      127     7698 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/error_handling.md
--rw-r--r--   0     1001      127     1081 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/index.md
--rw-r--r--   0     1001      127     1541 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/internal/core_library.md
--rw-r--r--   0     1001      127     2156 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/links.md
--rw-r--r--   0     1001      127   365251 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/media/final_todo_list.png
--rw-r--r--   0     1001      127   148261 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/media/ide_typehints.png
--rw-r--r--   0     1001      127   545494 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/media/network_debug.png
--rw-r--r--   0     1001      127   346903 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/media/server_side_rendering.png
--rw-r--r--   0     1001      127     2263 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/metadata.md
--rw-r--r--   0     1001      127     2347 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/postcss.md
--rw-r--r--   0     1001      127    12265 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/quickstart.md
--rw-r--r--   0     1001      127     4875 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/static_analysis.md
--rw-r--r--   0     1001      127     2490 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/structure.md
--rw-r--r--   0     1001      127     1219 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127     4080 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/docs/views.md
--rw-r--r--   0     1001      127     1823 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/mkdocs.yml
--rw-r--r--   0     1001      127      109 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/overrides/partials/footer.html
--rw-r--r--   0     1001      127   156250 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/poetry.lock
--rw-r--r--   0     1001      127      479 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/docs_website/pyproject.toml
--rw-r--r--   0     1001      127   675789 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/media/header.png
--rw-r--r--   0     1001      127      954 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/actions/__init__.py
--rw-r--r--   0     1001      127     7884 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/actions/test_fields.py
--rw-r--r--   0     1001      127     9707 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/actions/test_passthrough.py
--rw-r--r--   0     1001      127     9074 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/actions/test_sideeffect.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/__init__.py
--rw-r--r--   0     1001      127    14334 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_build_actions.py
--rw-r--r--   0     1001      127     4816 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_build_links.py
--rw-r--r--   0     1001      127    10097 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py
--rw-r--r--   0     1001      127     5001 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_builder.py
--rw-r--r--   0     1001      127     4153 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_typescript.py
--rw-r--r--   0     1001      127      319 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/common.py
--rw-r--r--   0     1001      127      497 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/conftest.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/database/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/database/dependencies/__init__.py
--rw-r--r--   0     1001      127      208 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/database/dependencies/conftest.py
--rw-r--r--   0     1001      127      801 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/database/dependencies/test_core.py
--rw-r--r--   0     1001      127      627 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/database/test_config.py
--rw-r--r--   0     1001      127      616 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/database/test_sqlmodel.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/dependencies/__init__.py
--rw-r--r--   0     1001      127     2567 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/dependencies/test_base.py
--rw-r--r--   0     1001      127      211 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/fixtures/__init__.py
--rw-r--r--   0     1001      127   571338 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
--rw-r--r--   0     1001      127  1638568 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
--rw-r--r--   0     1001      127   575422 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/js_compiler/__init__.py
--rw-r--r--   0     1001      127     9973 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/js_compiler/test_javascript.py
--rw-r--r--   0     1001      127      808 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/js_compiler/test_postcss.py
--rw-r--r--   0     1001      127     2823 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py
--rw-r--r--   0     1001      127     1236 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_annotation_helpers.py
--rw-r--r--   0     1001      127     8602 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_app.py
--rw-r--r--   0     1001      127      734 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_cache.py
--rw-r--r--   0     1001      127     5281 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_cli.py
--rw-r--r--   0     1001      127      494 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_config.py
--rw-r--r--   0     1001      127     6571 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_controller.py
--rw-r--r--   0     1001      127     3239 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_cropper.py
--rw-r--r--   0     1001      127     1227 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_exceptions.py
--rw-r--r--   0     1001      127     1924 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_logging.py
--rw-r--r--   0     1001      127     8419 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_paths.py
--rw-r--r--   0     1001      127     2565 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_ssr.py
--rw-r--r--   0     1001      127     3177 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/__tests__/test_watch.py
--rw-r--r--   0     1001      127      397 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/actions/__init__.py
--rw-r--r--   0     1001      127    12321 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/actions/fields.py
--rw-r--r--   0     1001      127     6835 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/actions/passthrough.py
--rw-r--r--   0     1001      127    11635 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/actions/sideeffect.py
--rw-r--r--   0     1001      127     4352 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/annotation_helpers.py
--rw-r--r--   0     1001      127    18916 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/app.py
--rw-r--r--   0     1001      127     3216 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/cache.py
--rw-r--r--   0     1001      127    18059 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/cli.py
--rw-r--r--   0     1001      127    11390 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/client_builder/build_actions.py
--rw-r--r--   0     1001      127     4002 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/client_builder/build_links.py
--rw-r--r--   0     1001      127    10172 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/client_builder/build_schemas.py
--rw-r--r--   0     1001      127    28719 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/client_builder/builder.py
--rw-r--r--   0     1001      127    11199 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/client_builder/openapi.py
--rw-r--r--   0     1001      127     5070 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/client_builder/typescript.py
--rw-r--r--   0     1001      127     2424 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/config.py
--rw-r--r--   0     1001      127       40 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/constants.py
--rw-r--r--   0     1001      127    14854 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/controller.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/controllers/__init__.py
--rw-r--r--   0     1001      127     1216 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/controllers/exception_controller.py
--rw-r--r--   0     1001      127    10359 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/cropper.py
--rw-r--r--   0     1001      127      327 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/database/__init__.py
--rw-r--r--   0     1001      127     1866 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/database/cli.py
--rw-r--r--   0     1001      127     1822 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/database/config.py
--rw-r--r--   0     1001      127      133 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/database/dependencies/__init__.py
--rw-r--r--   0     1001      127     3188 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/database/dependencies/core.py
--rw-r--r--   0     1001      127     7969 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/database/sqlmodel.py
--rw-r--r--   0     1001      127     8737 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/database/validator.py
--rw-r--r--   0     1001      127      251 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/dependencies/__init__.py
--rw-r--r--   0     1001      127     5122 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/dependencies/base.py
--rw-r--r--   0     1001      127      116 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/dependencies/core/__init__.py
--rw-r--r--   0     1001      127     1069 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/dependencies/core/core.py
--rw-r--r--   0     1001      127     3317 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/exceptions.py
--rw-r--r--   0     1001      127     1188 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/io.py
--rw-r--r--   0     1001      127        1 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/js_compiler/__init__.py
--rw-r--r--   0     1001      127     1731 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/js_compiler/base.py
--rw-r--r--   0     1001      127      199 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/js_compiler/exceptions.py
--rw-r--r--   0     1001      127    15443 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/js_compiler/javascript.py
--rw-r--r--   0     1001      127     4163 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/js_compiler/postcss.py
--rw-r--r--   0     1001      127     5614 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/js_compiler/source_maps.py
--rw-r--r--   0     1001      127     2039 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/logging.py
--rw-r--r--   0     1001      127    12599 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/paths.py
--rw-r--r--   0     1001      127        0 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/py.typed
--rw-r--r--   0     1001      127     5816 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/render.py
--rw-r--r--   0     1001      127     3228 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/ssr.py
--rw-r--r--   0     1001      127      210 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/static/__init__.py
--rw-r--r--   0     1001      127     6299 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/static/api.ts
--rw-r--r--   0     1001      127     3976 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/static/live_reload.ts
--rw-r--r--   0     1001      127      323 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/static/ssr_polyfills.js
--rw-r--r--   0     1001      127     7261 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/test_utilities.py
--rw-r--r--   0     1001      127      213 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/__init__.py
--rw-r--r--   0     1001      127      432 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/core/exception/page.tsx
--rw-r--r--   0     1001      127      178 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/core/layout.tsx
--rw-r--r--   0     1001      127       59 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/core/main.css
--rw-r--r--   0     1001      127     1478 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/package-lock.json
--rw-r--r--   0     1001      127      257 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/package.json
--rw-r--r--   0     1001      127       83 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/postcss.config.js
--rw-r--r--   0     1001      127      162 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/views/tailwind.config.js
--rw-r--r--   0     1001      127     8378 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/watch.py
--rw-r--r--   0     1001      127     3087 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/watch_server.py
--rw-r--r--   0     1001      127      866 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/mountaineer/webservice.py
--rw-r--r--   0     1001      127   125089 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/poetry.lock
--rw-r--r--   0     1001      127   453080 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt
--rw-r--r--   0     1001      127   575422 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/benches/fixtures/home_controller_ssr_with_react.js
--rw-r--r--   0     1001      127      322 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/benches/fixtures/ssr_polyfill_archive.js
--rw-r--r--   0     1001      127      899 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/benches/lexers_benchmark.rs
--rw-r--r--   0     1001      127     1089 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/benches/source_map_benchmark.rs
--rw-r--r--   0     1001      127     1595 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/benches/ssr_benchmark.rs
--rw-r--r--   0     1001      127      499 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/errors.rs
--rw-r--r--   0     1001      127     4648 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/lexers.rs
--rw-r--r--   0     1001      127     8366 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/lib.rs
--rw-r--r--   0     1001      127      680 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/logging.rs
--rw-r--r--   0     1001      127    17549 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/source_map.rs
--rw-r--r--   0     1001      127    15113 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/ssr.rs
--rw-r--r--   0     1001      127     3998 2024-04-23 14:54:19.000000 mountaineer-0.4.2.dev1/src/timeout.rs
--rw-r--r--   0     1001      127    32093 2024-04-23 14:54:34.000000 mountaineer-0.4.2.dev1/Cargo.lock
--rw-r--r--   0     1001      127     1599 2024-04-23 14:54:32.000000 mountaineer-0.4.2.dev1/pyproject.toml
--rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev1/PKG-INFO
+-rw-r--r--   0     1001      127      269 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/Cargo.toml
+-rw-r--r--   0     1001      127     1995 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/build.rs
+-rw-r--r--   0     1001      127     5657 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/go/js_build.go
+-rw-r--r--   0     1001      127      168 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/go.mod
+-rw-r--r--   0     1001      127      376 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/go.sum
+-rw-r--r--   0     1001      127     5750 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src_go/src/lib.rs
+-rw-r--r--   0        0        0     1055 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev2/Cargo.toml
+-rw-r--r--   0     1001      127      133 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.git-blame-ignore-revs
+-rw-r--r--   0     1001      127      138 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.gitattributes
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/README_SCRIPTS.md
+-rw-r--r--   0     1001      127    14036 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/poetry.lock
+-rw-r--r--   0     1001      127      767 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/__init__.py
+-rw-r--r--   0     1001      127     3032 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/__tests__/test_update_version.py
+-rw-r--r--   0     1001      127     2181 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/check_dependencies.py
+-rw-r--r--   0     1001      127     3382 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/scripts/update_version.py
+-rw-r--r--   0     1001      127     1321 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127    19767 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      504 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.github/workflows/validate.yml
+-rw-r--r--   0     1001      127     3404 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/.gitignore
+-rw-r--r--   0     1001      127     1750 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/Dockerfile
+-rw-r--r--   0     1001      127     1079 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/LICENSE
+-rw-r--r--   0     1001      127     4976 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/Makefile
+-rw-r--r--   0     1001      127    14891 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/README.md
+-rw-r--r--   0     1001      127      105 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/README.md
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/benchmarking/__init__.py
+-rw-r--r--   0     1001      127      425 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/benchmarking/simple_render.py
+-rw-r--r--   0     1001      127   127093 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/poetry.lock
+-rw-r--r--   0     1001      127      291 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/benchmarking/pyproject.toml
+-rw-r--r--   0     1001      127      850 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/README.md
+-rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/__init__.py
+-rw-r--r--   0     1001      127      775 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/app.py
+-rw-r--r--   0     1001      127      489 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/cli.py
+-rw-r--r--   0     1001      127      111 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/config.py
+-rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/__init__.py
+-rw-r--r--   0     1001      127     1433 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/complex.py
+-rw-r--r--   0     1001      127      581 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/detail.py
+-rw-r--r--   0     1001      127     1658 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/home.py
+-rw-r--r--   0     1001      127      559 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/stream.py
+-rw-r--r--   0     1001      127       77 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/main.py
+-rw-r--r--   0     1001      127      208 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/__init__.py
+-rw-r--r--   0     1001      127     2261 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/complex/page.tsx
+-rw-r--r--   0     1001      127      453 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127     2822 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       59 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/main.css
+-rw-r--r--   0     1001      127      708 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/stream/page.tsx
+-rw-r--r--   0     1001      127   125408 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/package-lock.json
+-rw-r--r--   0     1001      127      453 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/postcss.config.js
+-rw-r--r--   0     1001      127      161 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/tailwind.config.js
+-rw-r--r--   0     1001      127   107805 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/poetry.lock
+-rw-r--r--   0     1001      127      724 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/ci_webapp/pyproject.toml
+-rw-r--r--   0     1001      127     1593 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/README.md
+-rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/__init__.py
+-rw-r--r--   0     1001      127     1055 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/common.py
+-rw-r--r--   0     1001      127     7904 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py
+-rw-r--r--   0     1001      127      292 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      816 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py
+-rw-r--r--   0     1001      127     4277 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/builder.py
+-rw-r--r--   0     1001      127     4656 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/cli.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/__init__.py
+-rw-r--r--   0     1001      127     1383 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/base.py
+-rw-r--r--   0     1001      127     4591 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/poetry.py
+-rw-r--r--   0     1001      127     1832 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/venv.py
+-rw-r--r--   0     1001      127     1336 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/external.py
+-rw-r--r--   0     1001      127     1925 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/generation.py
+-rw-r--r--   0     1001      127      327 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/io.py
+-rw-r--r--   0     1001      127       30 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/.zed/settings.json
+-rw-r--r--   0     1001      127      212 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/__init__.py
+-rw-r--r--   0     1001      127      190 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vim/.vimrc
+-rw-r--r--   0     1001      127      137 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/vscode/.vscode/settings.json
+-rw-r--r--   0     1001      127      109 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/editor_configs/zed/pyrightconfig.json
+-rw-r--r--   0     1001      127      170 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.env
+-rw-r--r--   0     1001      127     3373 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore
+-rw-r--r--   0     1001      127      645 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/README.md
+-rw-r--r--   0     1001      127       17 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/__init__.py
+-rw-r--r--   0     1001      127      767 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py
+-rw-r--r--   0     1001      127      947 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py
+-rw-r--r--   0     1001      127      282 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/config.py
+-rw-r--r--   0     1001      127      227 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/__init__.py
+-rw-r--r--   0     1001      127     1702 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py
+-rw-r--r--   0     1001      127     1124 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py
+-rw-r--r--   0     1001      127       84 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/main.py
+-rw-r--r--   0     1001      127      157 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/models/detail.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/__init__.py
+-rw-r--r--   0     1001      127     1219 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx
+-rw-r--r--   0     1001      127      995 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx
+-rw-r--r--   0     1001      127       95 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/main.css
+-rw-r--r--   0     1001      127      524 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json
+-rw-r--r--   0     1001      127      117 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/postcss.config.js
+-rw-r--r--   0     1001      127      195 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/tailwind.config.js
+-rw-r--r--   0     1001      127      332 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/docker-compose.yml
+-rw-r--r--   0     1001      127     1493 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml
+-rw-r--r--   0     1001      127    61104 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/poetry.lock
+-rw-r--r--   0     1001      127     1214 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/create_mountaineer_app/pyproject.toml
+-rw-r--r--   0     1001      127       30 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/.zed/settings.json
+-rw-r--r--   0     1001      127      107 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/README.md
+-rw-r--r--   0     1001      127       15 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/CNAME
+-rw-r--r--   0     1001      127      310 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/actions.md
+-rw-r--r--   0     1001      127      454 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/api_exception.md
+-rw-r--r--   0     1001      127       99 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/app-controller.md
+-rw-r--r--   0     1001      127      281 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/build_plugins/base.md
+-rw-r--r--   0     1001      127       57 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/build_plugins/javascript.md
+-rw-r--r--   0     1001      127       62 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/build_plugins/postcss.md
+-rw-r--r--   0     1001      127      411 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/cli.md
+-rw-r--r--   0     1001      127      376 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/config.md
+-rw-r--r--   0     1001      127       61 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/controller.md
+-rw-r--r--   0     1001      127       67 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/core_dependencies.md
+-rw-r--r--   0     1001      127       66 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/database/config.md
+-rw-r--r--   0     1001      127       71 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/database/dependencies.md
+-rw-r--r--   0     1001      127       80 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/logging.md
+-rw-r--r--   0     1001      127      479 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/render.md
+-rw-r--r--   0     1001      127      365 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/ssr.md
+-rw-r--r--   0     1001      127      299 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/api/watch_server.md
+-rw-r--r--   0     1001      127     9375 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/client_actions.md
+-rw-r--r--   0     1001      127      753 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/cma.md
+-rw-r--r--   0     1001      127     3021 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/database.md
+-rw-r--r--   0     1001      127     4677 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/deploy.md
+-rw-r--r--   0     1001      127     7698 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/error_handling.md
+-rw-r--r--   0     1001      127     1081 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/index.md
+-rw-r--r--   0     1001      127     1541 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/internal/core_library.md
+-rw-r--r--   0     1001      127     2156 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/links.md
+-rw-r--r--   0     1001      127   365251 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/final_todo_list.png
+-rw-r--r--   0     1001      127   148261 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/ide_typehints.png
+-rw-r--r--   0     1001      127   545494 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/network_debug.png
+-rw-r--r--   0     1001      127   346903 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/media/server_side_rendering.png
+-rw-r--r--   0     1001      127     2263 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/metadata.md
+-rw-r--r--   0     1001      127     2347 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/postcss.md
+-rw-r--r--   0     1001      127    12265 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/quickstart.md
+-rw-r--r--   0     1001      127     4875 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/static_analysis.md
+-rw-r--r--   0     1001      127     2490 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/structure.md
+-rw-r--r--   0     1001      127     1219 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127     4080 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/docs/views.md
+-rw-r--r--   0     1001      127     1823 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/mkdocs.yml
+-rw-r--r--   0     1001      127      109 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/overrides/partials/footer.html
+-rw-r--r--   0     1001      127   156250 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/poetry.lock
+-rw-r--r--   0     1001      127      479 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/docs_website/pyproject.toml
+-rw-r--r--   0     1001      127   675789 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/media/header.png
+-rw-r--r--   0     1001      127      954 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/__init__.py
+-rw-r--r--   0     1001      127     7884 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_fields.py
+-rw-r--r--   0     1001      127     9707 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_passthrough.py
+-rw-r--r--   0     1001      127     9074 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_sideeffect.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/__init__.py
+-rw-r--r--   0     1001      127    14334 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_actions.py
+-rw-r--r--   0     1001      127     4816 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_links.py
+-rw-r--r--   0     1001      127    10097 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_schemas.py
+-rw-r--r--   0     1001      127     5001 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_builder.py
+-rw-r--r--   0     1001      127     4153 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_typescript.py
+-rw-r--r--   0     1001      127      319 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/common.py
+-rw-r--r--   0     1001      127      497 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/conftest.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127      208 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/conftest.py
+-rw-r--r--   0     1001      127      801 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/test_core.py
+-rw-r--r--   0     1001      127      627 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_config.py
+-rw-r--r--   0     1001      127      616 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_sqlmodel.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/dependencies/__init__.py
+-rw-r--r--   0     1001      127     2567 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/dependencies/test_base.py
+-rw-r--r--   0     1001      127      211 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/__init__.py
+-rw-r--r--   0     1001      127   571338 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127  1638568 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_source_map.js.map
+-rw-r--r--   0     1001      127   575422 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     9973 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_javascript.py
+-rw-r--r--   0     1001      127      808 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_postcss.py
+-rw-r--r--   0     1001      127     2823 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_source_maps.py
+-rw-r--r--   0     1001      127     1236 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_annotation_helpers.py
+-rw-r--r--   0     1001      127     8602 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_app.py
+-rw-r--r--   0     1001      127      734 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cache.py
+-rw-r--r--   0     1001      127     5281 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cli.py
+-rw-r--r--   0     1001      127      494 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_config.py
+-rw-r--r--   0     1001      127     6571 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_controller.py
+-rw-r--r--   0     1001      127     3239 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cropper.py
+-rw-r--r--   0     1001      127     1227 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_exceptions.py
+-rw-r--r--   0     1001      127     1924 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_logging.py
+-rw-r--r--   0     1001      127     8419 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_paths.py
+-rw-r--r--   0     1001      127     2565 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_ssr.py
+-rw-r--r--   0     1001      127     3177 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/__tests__/test_watch.py
+-rw-r--r--   0     1001      127      397 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/__init__.py
+-rw-r--r--   0     1001      127    12321 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/fields.py
+-rw-r--r--   0     1001      127     6835 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/passthrough.py
+-rw-r--r--   0     1001      127    11635 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/actions/sideeffect.py
+-rw-r--r--   0     1001      127     4352 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/annotation_helpers.py
+-rw-r--r--   0     1001      127    18916 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/app.py
+-rw-r--r--   0     1001      127     3216 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/cache.py
+-rw-r--r--   0     1001      127    18059 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/cli.py
+-rw-r--r--   0     1001      127    11390 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/build_actions.py
+-rw-r--r--   0     1001      127     4002 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/build_links.py
+-rw-r--r--   0     1001      127    10172 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/build_schemas.py
+-rw-r--r--   0     1001      127    29025 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/builder.py
+-rw-r--r--   0     1001      127    11199 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/openapi.py
+-rw-r--r--   0     1001      127     5070 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/client_builder/typescript.py
+-rw-r--r--   0     1001      127     2424 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/config.py
+-rw-r--r--   0     1001      127       40 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/constants.py
+-rw-r--r--   0     1001      127    14854 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/controller.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/controllers/__init__.py
+-rw-r--r--   0     1001      127     1216 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/controllers/exception_controller.py
+-rw-r--r--   0     1001      127    10359 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/cropper.py
+-rw-r--r--   0     1001      127      327 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/__init__.py
+-rw-r--r--   0     1001      127     1866 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/cli.py
+-rw-r--r--   0     1001      127     1822 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/config.py
+-rw-r--r--   0     1001      127      133 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/dependencies/__init__.py
+-rw-r--r--   0     1001      127     3188 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/dependencies/core.py
+-rw-r--r--   0     1001      127     7969 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/sqlmodel.py
+-rw-r--r--   0     1001      127     8737 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/database/validator.py
+-rw-r--r--   0     1001      127      251 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/base.py
+-rw-r--r--   0     1001      127      116 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/core/__init__.py
+-rw-r--r--   0     1001      127     1069 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/dependencies/core/core.py
+-rw-r--r--   0     1001      127     3317 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/exceptions.py
+-rw-r--r--   0     1001      127     1188 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/io.py
+-rw-r--r--   0     1001      127        1 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/__init__.py
+-rw-r--r--   0     1001      127     1731 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/base.py
+-rw-r--r--   0     1001      127      199 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/exceptions.py
+-rw-r--r--   0     1001      127    15443 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/javascript.py
+-rw-r--r--   0     1001      127     4163 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/postcss.py
+-rw-r--r--   0     1001      127     5614 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/js_compiler/source_maps.py
+-rw-r--r--   0     1001      127     2039 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/logging.py
+-rw-r--r--   0     1001      127    12826 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/paths.py
+-rw-r--r--   0     1001      127        0 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/py.typed
+-rw-r--r--   0     1001      127     5816 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/render.py
+-rw-r--r--   0     1001      127     3228 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/ssr.py
+-rw-r--r--   0     1001      127      210 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/__init__.py
+-rw-r--r--   0     1001      127     6299 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/api.ts
+-rw-r--r--   0     1001      127     3976 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/live_reload.ts
+-rw-r--r--   0     1001      127      323 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/static/ssr_polyfills.js
+-rw-r--r--   0     1001      127     7261 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/test_utilities.py
+-rw-r--r--   0     1001      127      213 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/__init__.py
+-rw-r--r--   0     1001      127      432 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/core/exception/page.tsx
+-rw-r--r--   0     1001      127      178 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/core/layout.tsx
+-rw-r--r--   0     1001      127       59 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/core/main.css
+-rw-r--r--   0     1001      127     1478 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/package-lock.json
+-rw-r--r--   0     1001      127      257 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/package.json
+-rw-r--r--   0     1001      127       83 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/postcss.config.js
+-rw-r--r--   0     1001      127      162 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/views/tailwind.config.js
+-rw-r--r--   0     1001      127     8378 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/watch.py
+-rw-r--r--   0     1001      127     3087 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/watch_server.py
+-rw-r--r--   0     1001      127      866 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/mountaineer/webservice.py
+-rw-r--r--   0     1001      127   125089 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/poetry.lock
+-rw-r--r--   0     1001      127   453080 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/fixtures/complex_sourcemap_mapping.txt
+-rw-r--r--   0     1001      127   575422 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/fixtures/home_controller_ssr_with_react.js
+-rw-r--r--   0     1001      127      322 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/fixtures/ssr_polyfill_archive.js
+-rw-r--r--   0     1001      127      899 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/lexers_benchmark.rs
+-rw-r--r--   0     1001      127     1089 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/source_map_benchmark.rs
+-rw-r--r--   0     1001      127     1595 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/benches/ssr_benchmark.rs
+-rw-r--r--   0     1001      127      499 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/errors.rs
+-rw-r--r--   0     1001      127     4648 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/lexers.rs
+-rw-r--r--   0     1001      127     8366 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/lib.rs
+-rw-r--r--   0     1001      127      680 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/logging.rs
+-rw-r--r--   0     1001      127    17549 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/source_map.rs
+-rw-r--r--   0     1001      127    15113 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/ssr.rs
+-rw-r--r--   0     1001      127     3998 2024-04-23 16:35:39.000000 mountaineer-0.4.2.dev2/src/timeout.rs
+-rw-r--r--   0     1001      127    32093 2024-04-23 16:35:54.000000 mountaineer-0.4.2.dev2/Cargo.lock
+-rw-r--r--   0     1001      127     1599 2024-04-23 16:35:52.000000 mountaineer-0.4.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 mountaineer-0.4.2.dev2/PKG-INFO
```

### Comparing `mountaineer-0.4.2.dev1/src_go/build.rs` & `mountaineer-0.4.2.dev2/src_go/build.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src_go/go/js_build.go` & `mountaineer-0.4.2.dev2/src_go/go/js_build.go`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src_go/src/lib.rs` & `mountaineer-0.4.2.dev2/src_go/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/Cargo.toml` & `mountaineer-0.4.2.dev2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [[bench]]
 path = "src/benches/lexers_benchmark.rs"
 name = "lexers_benchmark"
 harness = false
 
 [package]
 name = "mountaineer"
-version = "0.4.2-dev1"
+version = "0.4.2-dev2"
 edition = "2021"
 
 [dependencies]
 v8 = "0.89.0"
 deno_core_icudata = "0.73.0"
 lazy_static = "1.4.0"
 serde_json = "1.0"
```

### Comparing `mountaineer-0.4.2.dev1/.github/poetry.lock` & `mountaineer-0.4.2.dev2/.github/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/.github/pyproject.toml` & `mountaineer-0.4.2.dev2/.github/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/.github/scripts/__tests__/test_update_version.py` & `mountaineer-0.4.2.dev2/.github/scripts/__tests__/test_update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/.github/scripts/check_dependencies.py` & `mountaineer-0.4.2.dev2/.github/scripts/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/.github/scripts/update_version.py` & `mountaineer-0.4.2.dev2/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/.github/workflows/publish_docs.yml` & `mountaineer-0.4.2.dev2/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/.github/workflows/test.yml` & `mountaineer-0.4.2.dev2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/.gitignore` & `mountaineer-0.4.2.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/Dockerfile` & `mountaineer-0.4.2.dev2/Dockerfile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/LICENSE` & `mountaineer-0.4.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/Makefile` & `mountaineer-0.4.2.dev2/Makefile`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/README.md` & `mountaineer-0.4.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/benchmarking/poetry.lock` & `mountaineer-0.4.2.dev2/benchmarking/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/README.md` & `mountaineer-0.4.2.dev2/ci_webapp/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/app.py` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/complex.py` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/complex.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/detail.py` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/home.py` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/controllers/stream.py` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/controllers/stream.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/complex/page.tsx` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/complex/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/home/page.tsx` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/app/stream/page.tsx` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/app/stream/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/ci_webapp/views/package-lock.json` & `mountaineer-0.4.2.dev2/ci_webapp/ci_webapp/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/poetry.lock` & `mountaineer-0.4.2.dev2/ci_webapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/ci_webapp/pyproject.toml` & `mountaineer-0.4.2.dev2/ci_webapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/README.md` & `mountaineer-0.4.2.dev2/create_mountaineer_app/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/common.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/common.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/__tests__/test_generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/builder.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/cli.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/base.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/poetry.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/poetry.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/environments/venv.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/environments/venv.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/external.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/external.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/generation.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/generation.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/README.md` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/README.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/detail.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/controllers/home.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/detail/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/app/home/page.tsx`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/[project_name]/views/package.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml` & `mountaineer-0.4.2.dev2/create_mountaineer_app/create_mountaineer_app/templates/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/poetry.lock` & `mountaineer-0.4.2.dev2/create_mountaineer_app/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/create_mountaineer_app/pyproject.toml` & `mountaineer-0.4.2.dev2/create_mountaineer_app/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/client_actions.md` & `mountaineer-0.4.2.dev2/docs_website/docs/client_actions.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/cma.md` & `mountaineer-0.4.2.dev2/docs_website/docs/cma.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/database.md` & `mountaineer-0.4.2.dev2/docs_website/docs/database.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/deploy.md` & `mountaineer-0.4.2.dev2/docs_website/docs/deploy.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/error_handling.md` & `mountaineer-0.4.2.dev2/docs_website/docs/error_handling.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/index.md` & `mountaineer-0.4.2.dev2/docs_website/docs/index.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/internal/core_library.md` & `mountaineer-0.4.2.dev2/docs_website/docs/internal/core_library.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/links.md` & `mountaineer-0.4.2.dev2/docs_website/docs/links.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/media/final_todo_list.png` & `mountaineer-0.4.2.dev2/docs_website/docs/media/final_todo_list.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/media/ide_typehints.png` & `mountaineer-0.4.2.dev2/docs_website/docs/media/ide_typehints.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/media/network_debug.png` & `mountaineer-0.4.2.dev2/docs_website/docs/media/network_debug.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/media/server_side_rendering.png` & `mountaineer-0.4.2.dev2/docs_website/docs/media/server_side_rendering.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/metadata.md` & `mountaineer-0.4.2.dev2/docs_website/docs/metadata.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/postcss.md` & `mountaineer-0.4.2.dev2/docs_website/docs/postcss.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/quickstart.md` & `mountaineer-0.4.2.dev2/docs_website/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/static_analysis.md` & `mountaineer-0.4.2.dev2/docs_website/docs/static_analysis.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/structure.md` & `mountaineer-0.4.2.dev2/docs_website/docs/structure.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/stylesheets/extra.css` & `mountaineer-0.4.2.dev2/docs_website/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/docs/views.md` & `mountaineer-0.4.2.dev2/docs_website/docs/views.md`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/mkdocs.yml` & `mountaineer-0.4.2.dev2/docs_website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/docs_website/poetry.lock` & `mountaineer-0.4.2.dev2/docs_website/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/media/header.png` & `mountaineer-0.4.2.dev2/media/header.png`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__init__.py` & `mountaineer-0.4.2.dev2/mountaineer/__init__.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/actions/test_fields.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/actions/test_passthrough.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/actions/test_sideeffect.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/actions/test_sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_build_actions.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_build_links.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_build_schemas.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_builder.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/client_builder/test_typescript.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/client_builder/test_typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/database/dependencies/test_core.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/database/dependencies/test_core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/database/test_config.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/database/test_sqlmodel.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/database/test_sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/dependencies/test_base.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/dependencies/test_base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/complex_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/fixtures/home_controller_source_map.js.map` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_source_map.js.map`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/js_compiler/test_javascript.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/js_compiler/test_postcss.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/js_compiler/test_source_maps.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/js_compiler/test_source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_annotation_helpers.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_app.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_cache.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_cli.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_controller.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_cropper.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_exceptions.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_logging.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_paths.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_paths.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_ssr.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/__tests__/test_watch.py` & `mountaineer-0.4.2.dev2/mountaineer/__tests__/test_watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/actions/fields.py` & `mountaineer-0.4.2.dev2/mountaineer/actions/fields.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/actions/passthrough.py` & `mountaineer-0.4.2.dev2/mountaineer/actions/passthrough.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/actions/sideeffect.py` & `mountaineer-0.4.2.dev2/mountaineer/actions/sideeffect.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/annotation_helpers.py` & `mountaineer-0.4.2.dev2/mountaineer/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/app.py` & `mountaineer-0.4.2.dev2/mountaineer/app.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/cache.py` & `mountaineer-0.4.2.dev2/mountaineer/cache.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/cli.py` & `mountaineer-0.4.2.dev2/mountaineer/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/client_builder/build_actions.py` & `mountaineer-0.4.2.dev2/mountaineer/client_builder/build_actions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/client_builder/build_links.py` & `mountaineer-0.4.2.dev2/mountaineer/client_builder/build_links.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/client_builder/build_schemas.py` & `mountaineer-0.4.2.dev2/mountaineer/client_builder/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/client_builder/builder.py` & `mountaineer-0.4.2.dev2/mountaineer/client_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from collections import defaultdict
 from dataclasses import asdict, dataclass
 from json import dumps as json_dumps
 from pathlib import Path
-from shutil import move as shutil_move, rmtree
+from shutil import move as shutil_move, rmtree as shutil_rmtree
 from tempfile import TemporaryDirectory
 from time import monotonic_ns
 from typing import Any
 
 from click import secho
 from fastapi import APIRouter
 from inflection import camelize
@@ -502,20 +502,25 @@
             )
             shutil_move(self.view_root.get_managed_ssr_dir(tmp_build=True), tmp_ssr_dir)
 
             static_dir = self.view_root.get_managed_static_dir()
             ssr_dir = self.view_root.get_managed_ssr_dir()
             for clear_dir in [static_dir, ssr_dir]:
                 if clear_dir.exists():
-                    rmtree(clear_dir)
-                clear_dir.mkdir(parents=True)
+                    shutil_rmtree(clear_dir)
 
-            # Final move
-            shutil_move(tmp_static_dir, self.view_root.get_managed_static_dir())
-            shutil_move(tmp_ssr_dir, self.view_root.get_managed_ssr_dir())
+            # Final move - shutil requires the destination directory to not exist, otherwise
+            # it will place the folder within the given folder. Since we just want a regular
+            # rename, we make sure to not create the destination directory
+            shutil_move(
+                tmp_static_dir, self.view_root.get_managed_static_dir(create_dir=False)
+            )
+            shutil_move(
+                tmp_ssr_dir, self.view_root.get_managed_ssr_dir(create_dir=False)
+            )
 
     def cache_is_outdated(self):
         """
         Determines if our last build is outdated and we need to rebuild the client. Running
         this function will also update the cache to the current state.
 
         """
```

### Comparing `mountaineer-0.4.2.dev1/mountaineer/client_builder/openapi.py` & `mountaineer-0.4.2.dev2/mountaineer/client_builder/openapi.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/client_builder/typescript.py` & `mountaineer-0.4.2.dev2/mountaineer/client_builder/typescript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/config.py` & `mountaineer-0.4.2.dev2/mountaineer/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/controller.py` & `mountaineer-0.4.2.dev2/mountaineer/controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/controllers/exception_controller.py` & `mountaineer-0.4.2.dev2/mountaineer/controllers/exception_controller.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/cropper.py` & `mountaineer-0.4.2.dev2/mountaineer/cropper.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/database/cli.py` & `mountaineer-0.4.2.dev2/mountaineer/database/cli.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/database/config.py` & `mountaineer-0.4.2.dev2/mountaineer/database/config.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/database/dependencies/core.py` & `mountaineer-0.4.2.dev2/mountaineer/database/dependencies/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/database/sqlmodel.py` & `mountaineer-0.4.2.dev2/mountaineer/database/sqlmodel.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/database/validator.py` & `mountaineer-0.4.2.dev2/mountaineer/database/validator.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/dependencies/base.py` & `mountaineer-0.4.2.dev2/mountaineer/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/dependencies/core/core.py` & `mountaineer-0.4.2.dev2/mountaineer/dependencies/core/core.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/exceptions.py` & `mountaineer-0.4.2.dev2/mountaineer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/io.py` & `mountaineer-0.4.2.dev2/mountaineer/io.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/js_compiler/base.py` & `mountaineer-0.4.2.dev2/mountaineer/js_compiler/base.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/js_compiler/javascript.py` & `mountaineer-0.4.2.dev2/mountaineer/js_compiler/javascript.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/js_compiler/postcss.py` & `mountaineer-0.4.2.dev2/mountaineer/js_compiler/postcss.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/js_compiler/source_maps.py` & `mountaineer-0.4.2.dev2/mountaineer/js_compiler/source_maps.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/logging.py` & `mountaineer-0.4.2.dev2/mountaineer/logging.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/paths.py` & `mountaineer-0.4.2.dev2/mountaineer/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,51 +83,56 @@
         """
         if self.package_root_link is None:
             raise ValueError(
                 f"Cannot get package root link from current view path: {self}"
             )
         return self.package_root_link
 
-    def get_managed_code_dir(self):
-        return self.get_managed_dir_common("_server")
+    def get_managed_code_dir(self, create_dir: bool = True):
+        return self.get_managed_dir_common("_server", create_dir=create_dir)
 
-    def get_managed_static_dir(self, tmp_build: bool = False):
+    def get_managed_static_dir(self, tmp_build: bool = False, create_dir: bool = True):
         # Only root paths can have static directories
         if not self.is_root_link:
             raise ValueError(
                 "Cannot get static directory from a non-root linked view path"
             )
-        path = self.get_managed_dir_common("_static")
+        path = self.get_managed_dir_common("_static", create_dir=create_dir)
         if tmp_build:
             path = path / "tmp"
             path.mkdir(exist_ok=True)
         return path
 
-    def get_managed_ssr_dir(self, tmp_build: bool = False):
+    def get_managed_ssr_dir(self, tmp_build: bool = False, create_dir: bool = True):
         # Only root paths can have SSR directories
         if not self.is_root_link:
             raise ValueError(
                 "Cannot get SSR directory from a non-root linked view path"
             )
-        path = self.get_managed_dir_common("_ssr")
+        path = self.get_managed_dir_common("_ssr", create_dir=create_dir)
         if tmp_build:
             path = path / "tmp"
             path.mkdir(exist_ok=True)
         return path
 
-    def get_managed_dir_common(self, managed_dir: str):
+    def get_managed_dir_common(
+        self,
+        managed_dir: str,
+        create_dir: bool = True,
+    ):
         # If the path is to a file, we want to get the parent directory
         # so that we can create the managed code directory
         # We also create the managed code directory if it doesn't exist so all subsequent
         # calls can immediately start writing to it
         path = self
         if path.is_file():
             path = path.parent
         managed_code_dir = path / managed_dir
-        managed_code_dir.mkdir(exist_ok=True)
+        if create_dir:
+            managed_code_dir.mkdir(exist_ok=True)
         return managed_code_dir
 
     def get_controller_view_path(self, controller: "ControllerBase"):
         """
         Assume all paths are specified in terms of their relative root
         """
         # Ensure we are being take relative to the root view
```

### Comparing `mountaineer-0.4.2.dev1/mountaineer/render.py` & `mountaineer-0.4.2.dev2/mountaineer/render.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/ssr.py` & `mountaineer-0.4.2.dev2/mountaineer/ssr.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/static/api.ts` & `mountaineer-0.4.2.dev2/mountaineer/static/api.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/static/live_reload.ts` & `mountaineer-0.4.2.dev2/mountaineer/static/live_reload.ts`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/test_utilities.py` & `mountaineer-0.4.2.dev2/mountaineer/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/views/package-lock.json` & `mountaineer-0.4.2.dev2/mountaineer/views/package-lock.json`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/watch.py` & `mountaineer-0.4.2.dev2/mountaineer/watch.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/watch_server.py` & `mountaineer-0.4.2.dev2/mountaineer/watch_server.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/mountaineer/webservice.py` & `mountaineer-0.4.2.dev2/mountaineer/webservice.py`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/poetry.lock` & `mountaineer-0.4.2.dev2/poetry.lock`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/benches/fixtures/complex_sourcemap_mapping.txt` & `mountaineer-0.4.2.dev2/src/benches/fixtures/complex_sourcemap_mapping.txt`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/benches/fixtures/home_controller_ssr_with_react.js` & `mountaineer-0.4.2.dev2/src/benches/fixtures/home_controller_ssr_with_react.js`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/benches/lexers_benchmark.rs` & `mountaineer-0.4.2.dev2/src/benches/lexers_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/benches/source_map_benchmark.rs` & `mountaineer-0.4.2.dev2/src/benches/source_map_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/benches/ssr_benchmark.rs` & `mountaineer-0.4.2.dev2/src/benches/ssr_benchmark.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/lexers.rs` & `mountaineer-0.4.2.dev2/src/lexers.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/lib.rs` & `mountaineer-0.4.2.dev2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/logging.rs` & `mountaineer-0.4.2.dev2/src/logging.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/source_map.rs` & `mountaineer-0.4.2.dev2/src/source_map.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/ssr.rs` & `mountaineer-0.4.2.dev2/src/ssr.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/src/timeout.rs` & `mountaineer-0.4.2.dev2/src/timeout.rs`

 * *Files identical despite different names*

### Comparing `mountaineer-0.4.2.dev1/Cargo.lock` & `mountaineer-0.4.2.dev2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mountaineer"
-version = "0.4.2-dev1"
+version = "0.4.2-dev2"
 dependencies = [
  "criterion",
  "deno_core_icudata",
  "env_logger",
  "lazy_static",
  "libc",
  "log",
```

### Comparing `mountaineer-0.4.2.dev1/pyproject.toml` & `mountaineer-0.4.2.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mountaineer"
 dependencies = [ "pydantic", "fastapi", "inflection", "click", "uvicorn[standard]", "packaging", "watchdog", "pydantic-settings", "sqlmodel", "asyncpg", "sqlalchemy[asyncio]",]
 exclude = [ "fixtures", "ci_webapp", "create_mountaineer_app", "media", "docs_website", "benchmarking",]
 
 [tool.poetry]
 name = "mountaineer"
-version = "0.4.2.dev1"
+version = "0.4.2.dev2"
 description = ""
 authors = [ "Pierce Freeman <pierce@freeman.vc>",]
 readme = "README.md"
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
```

### Comparing `mountaineer-0.4.2.dev1/PKG-INFO` & `mountaineer-0.4.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mountaineer
-Version: 0.4.2.dev1
+Version: 0.4.2.dev2
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: inflection
 Requires-Dist: click
 Requires-Dist: uvicorn[standard]
 Requires-Dist: packaging
 Requires-Dist: watchdog
```

