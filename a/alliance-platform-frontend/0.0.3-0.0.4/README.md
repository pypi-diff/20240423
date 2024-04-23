# Comparing `tmp/alliance_platform_frontend-0.0.3.tar.gz` & `tmp/alliance_platform_frontend-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alliance_platform_frontend-0.0.3.tar", last modified: Thu Apr 11 03:08:09 2024, max compression
+gzip compressed data, was "alliance_platform_frontend-0.0.4.tar", last modified: Tue Apr 23 21:40:21 2024, max compression
```

## Comparing `alliance_platform_frontend-0.0.3.tar` & `alliance_platform_frontend-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2946 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/README.md
--rw-r--r--   0        0        0       22 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/__init__.py
--rw-r--r--   0        0        0      784 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/button.py
--rw-r--r--   0        0        0     1839 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/date_picker.py
--rw-r--r--   0        0        0     2524 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/icon.py
--rw-r--r--   0        0        0     1421 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/inline_alert.py
--rw-r--r--   0        0        0     1464 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/menubar.py
--rw-r--r--   0        0        0     2075 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/misc.py
--rw-r--r--   0        0        0     1622 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/pagination.py
--rw-r--r--   0        0        0     2270 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/table.py
--rw-r--r--   0        0        0     1127 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/time_input.py
--rw-r--r--   0        0        0     1243 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/utils.py
--rw-r--r--   0        0        0      358 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/apps.py
--rw-r--r--   0        0        0      633 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/__init__.py
--rw-r--r--   0        0        0     2402 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/asset_registry.py
--rw-r--r--   0        0        0    15999 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/base.py
--rw-r--r--   0        0        0    17116 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/context.py
--rw-r--r--   0        0        0     2507 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/middleware.py
--rw-r--r--   0        0        0    13537 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/ssr.py
--rw-r--r--   0        0        0     7051 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vanilla_extract.py
--rw-r--r--   0        0        0    33786 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vite.py
--rw-r--r--   0        0        0      175 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vitePreload.ts
--rw-r--r--   0        0        0    11144 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/dom_possible_standard_names.py
--rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/forms/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/forms/renderers.py
--rw-r--r--   0        0        0     5370 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/management/commands/extract_frontend_assets.py
--rw-r--r--   0        0        0    10434 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/prop_handlers.py
--rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/py.typed
--rw-r--r--   0        0        0     7344 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/settings.py
--rw-r--r--   0        0        0     2684 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templates/bundler_dev_check.html
--rw-r--r--   0        0        0        0 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/__init__.py
--rw-r--r--   0        0        0     5451 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/alliance_ui.py
--rw-r--r--   0        0        0    12922 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/bundler.py
--rw-r--r--   0        0        0     9664 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/form.py
--rw-r--r--   0        0        0    56265 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/react.py
--rw-r--r--   0        0        0     4316 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/vanilla_extract.py
--rw-r--r--   0        0        0     3283 2024-04-11 03:07:45.789805 alliance_platform_frontend-0.0.3/alliance_platform/frontend/util.py
--rw-r--r--   0        0        0     2120 2024-04-11 03:08:09.277969 alliance_platform_frontend-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2503 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/build_test/manifest.json
--rw-r--r--   0        0        0       39 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/development-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0       30 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/production-css-mappings/login_css_ts.json
--rw-r--r--   0        0        0      648 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/fixtures/server_build_test/manifest.json
--rw-r--r--   0        0        0     7955 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_alliance_ui_templatetags.py
--rw-r--r--   0        0        0    11119 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_bundler.py
--rw-r--r--   0        0        0    33736 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_bundler_templatetags.py
--rw-r--r--   0        0        0     5837 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_context.py
--rw-r--r--   0        0        0      721 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-11 03:07:45.793805 alliance_platform_frontend-0.0.3/tests/test_utils/bundler.py
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2946 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/button.py
+-rw-r--r--   0        0        0     1839 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/date_picker.py
+-rw-r--r--   0        0        0     2524 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/icon.py
+-rw-r--r--   0        0        0     1421 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/inline_alert.py
+-rw-r--r--   0        0        0     1464 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/menubar.py
+-rw-r--r--   0        0        0     2075 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/misc.py
+-rw-r--r--   0        0        0     1622 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/pagination.py
+-rw-r--r--   0        0        0     2270 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/table.py
+-rw-r--r--   0        0        0     1127 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/time_input.py
+-rw-r--r--   0        0        0     1243 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/utils.py
+-rw-r--r--   0        0        0      358 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/apps.py
+-rw-r--r--   0        0        0      633 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/__init__.py
+-rw-r--r--   0        0        0     2402 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/asset_registry.py
+-rw-r--r--   0        0        0    15999 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/base.py
+-rw-r--r--   0        0        0    17116 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/context.py
+-rw-r--r--   0        0        0     2507 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/middleware.py
+-rw-r--r--   0        0        0    13537 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/ssr.py
+-rw-r--r--   0        0        0     7051 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vanilla_extract.py
+-rw-r--r--   0        0        0    33895 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vite.py
+-rw-r--r--   0        0        0      175 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vitePreload.ts
+-rw-r--r--   0        0        0    11144 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/dom_possible_standard_names.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/forms/__init__.py
+-rw-r--r--   0        0        0     1620 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/forms/renderers.py
+-rw-r--r--   0        0        0     5340 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/management/commands/extract_frontend_assets.py
+-rw-r--r--   0        0        0    10434 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/prop_handlers.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/py.typed
+-rw-r--r--   0        0        0     7344 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/settings.py
+-rw-r--r--   0        0        0     2684 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templates/bundler_dev_check.html
+-rw-r--r--   0        0        0        0 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/__init__.py
+-rw-r--r--   0        0        0     5451 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/alliance_ui.py
+-rw-r--r--   0        0        0    12922 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/bundler.py
+-rw-r--r--   0        0        0     9664 2024-04-23 21:39:51.135763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/form.py
+-rw-r--r--   0        0        0    56265 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/react.py
+-rw-r--r--   0        0        0     4316 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/vanilla_extract.py
+-rw-r--r--   0        0        0     3283 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/alliance_platform/frontend/util.py
+-rw-r--r--   0        0        0     2120 2024-04-23 21:40:21.584088 alliance_platform_frontend-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2503 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/build_test/manifest.json
+-rw-r--r--   0        0        0       39 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/development-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0       30 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/production-css-mappings/login_css_ts.json
+-rw-r--r--   0        0        0      648 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/fixtures/server_build_test/manifest.json
+-rw-r--r--   0        0        0     7955 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_alliance_ui_templatetags.py
+-rw-r--r--   0        0        0    11182 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_bundler.py
+-rw-r--r--   0        0        0    33736 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_bundler_templatetags.py
+-rw-r--r--   0        0        0     5837 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_context.py
+-rw-r--r--   0        0        0      721 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     2370 2024-04-23 21:39:51.139763 alliance_platform_frontend-0.0.4/tests/test_utils/bundler.py
+-rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 alliance_platform_frontend-0.0.4/PKG-INFO
```

### Comparing `alliance_platform_frontend-0.0.3/README.md` & `alliance_platform_frontend-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/button.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/button.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/date_picker.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/date_picker.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/icon.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/icon.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/inline_alert.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/inline_alert.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/menubar.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/menubar.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/misc.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/misc.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/pagination.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/pagination.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/table.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/table.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/time_input.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/time_input.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/alliance_ui/utils.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/alliance_ui/utils.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/__init__.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/asset_registry.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/asset_registry.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/base.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/base.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/context.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/middleware.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/middleware.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/ssr.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/ssr.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vanilla_extract.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/bundler/vite.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/bundler/vite.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,14 +267,30 @@
         root_dir: The root path everything sits under; all other paths are resolved relative to this
         path_resolvers: A list of :class:`~alliance_platform.frontend.bundler.base.PathResolver` instances used to resolve paths
         server_build_dir: The directory SSR files are outputted to (see ``yarn build:ssr``)
         build_dir: The directory client side files are outputted to (see ``yarn build:client``)
         server_host: The hostname used for the dev server (e.g. ``127.0.0.1``)
         server_port: The port used for the dev server (e.g. ``5173``)
         server_protocol: The protocol used for the dev server (``http`` or ``https``)
+        server_resolve_package_url: The URL, handled by the dev server, to use to resolve package requests in dev mode. This is
+            only used for packages in /node_modules/ so that we can use the optimized versions of packages that Vite generates.
+            Without this, you encounter errors like "Outdated Optimized Deps". The dev server should handle requests to this
+            URL and redirect to the final package file. Example implementation for fastify, where ``server_resolve_package_url="redirect-package-url"``.
+
+            .. code-block:: javascript
+
+                server.get('/redirect-package-url/*', async (req, res) => {
+                    const packagePath = (req.params as Record<string, string>)['*'];
+                    const [, resolvedId] = await vite.moduleGraph.resolveUrl(packagePath);
+                    // `resolveId` is an absolute path with query string. Resolve it relative to the project root
+                    const relativePath = normalizePath(path.relative(projectDir, resolvedId));
+                    // Convert the filesystem path to a web-accessible path
+                    const url = path.join(vite.config.base, relativePath);
+                    res.redirect(302, url);
+                });
         mode: The mode the bundler is running in; one of ``development``, ``production`` or ``preview``
         wait_for_server: Function that can be passed that will be called before requesting assets for server. This function
             should handle waiting until the dev server is ready before returning (e.g. by polling the server status)
         production_ssr_url: URL for SSR (only used in production mode)
 
     """
 
@@ -301,30 +317,29 @@
         root_dir: Path,
         path_resolvers: list[PathResolver],
         server_build_dir: Path,
         build_dir: Path,
         server_host: str,
         server_port: str,
         server_protocol: str,
+        server_resolve_package_url: str,
         mode: str,
         production_ssr_url: str | None = None,
         wait_for_server: Callable[[], None] | None = None,
     ):
         self.wait_for_server = wait_for_server
         valid_modes = ["development", "production", "preview"]
         if mode not in valid_modes:
             raise ValueError(f"'mode' must be one of {', '.join(valid_modes)}, received: '{mode}'")
         super().__init__(root_dir, path_resolvers)
         self.mode = mode
         self.server_build_dir = server_build_dir
         self.build_dir = build_dir
         self.node_modules_dir = ap_frontend_settings.NODE_MODULES_DIR
-        if self.mode == "development":
-            self.vite_metadata_path = self.node_modules_dir / ".vite/deps/_metadata.json"
-        else:
+        if self.mode != "development":
             self.server_build_manifest = ViteManifest(self.root_dir, server_build_dir / "manifest.json")
             self.build_manifest = ViteManifest(self.root_dir, build_dir / "manifest.json")
         self.dev_server_url_base = ""
         self.dev_server_url = ""
         self.production_ssr_url = production_ssr_url
         if mode == "development":
             static_url = settings.STATIC_URL
@@ -336,14 +351,19 @@
             if static_url.startswith("http"):
                 raise ValueError(f"static_url cannot be a full URL in {mode}")
             static_url = static_url.lstrip("/")
             # this is the base url for the dev server - use ``dev_server_url`` if referencing to assets
             self.dev_server_url_base = f"{server_protocol}://{server_host}:{server_port}"
             # this is what should be used anywhere assets need to be referred to
             self.dev_server_url = urljoin(self.dev_server_url_base, static_url)
+            self.dev_server_resolve_package_url = urljoin(
+                self.dev_server_url_base, server_resolve_package_url
+            )
+            if not self.dev_server_resolve_package_url.endswith("/"):
+                self.dev_server_resolve_package_url += "/"
         elif mode == "preview":
             self.preview_url = f"{server_protocol}://{server_host}:{server_port}"
 
     def resolve_url(self, path: Path | str):
         """Resolve a URL to use to serve the specified ``path``
 
         In development this will be served from the dev server and in production from ``STATIC_URL``
@@ -358,48 +378,27 @@
         if path.is_absolute():
             path = path.relative_to(self.root_dir)
         return urljoin(self.dev_server_url, str(path))
 
     _vite_dev_metadata: dict | None = None
     _vite_dev_last_modified: float | None = None
 
-    def get_vite_dev_metadata(self) -> dict | None:
-        if (
-            self.vite_metadata_path.exists()
-            and (last_modified := self.vite_metadata_path.stat().st_mtime) != self._vite_dev_last_modified
-        ):
-            self._vite_dev_last_modified = last_modified
-            _vite_dev_metadata = json.loads(self.vite_metadata_path.read_text())
-            if not isinstance(_vite_dev_metadata, dict) or "optimized" not in _vite_dev_metadata:
-                warnings.warn("Invalid vite metadata file")
-            else:
-                self._vite_dev_metadata = _vite_dev_metadata
-        return self._vite_dev_metadata
-
     def get_url(self, path: Path | str):
         """Get the URL to load asset as ``path``
 
         In development this uses the dev server, in production is served from static files.
         """
         if self.mode == "development":
             # In dev, check the vite metadata to see if the file is in the optimized list - if so
             # load from the specified file. This resolved the need to explicitly include a bunch
             # of dependencies in vite.config.ts under optimizeDeps.include
             if str(path).startswith(str(self.node_modules_dir)):
-                filename = str(path).replace(str(self.node_modules_dir) + "/", "")
-                metadata = self.get_vite_dev_metadata()
-                if metadata and (entry := metadata["optimized"].get(filename)):
-                    return self.resolve_url(
-                        # Appending the hash seems to be what would happen if we used a default vite
-                        # setup where it transforms the .html... but this sometimes results in a 504
-                        # error and also seems to make no difference that I could determine. I also
-                        # don't really understand how it's used so could be missing the point. Leaving
-                        # it here for now in case it's needed in future.
-                        f"node_modules/.vite/deps/{entry['file']}"  # "?v={metadata['browserHash']}"
-                    )
+                return urljoin(
+                    self.dev_server_resolve_package_url, str(Path(path).relative_to(self.node_modules_dir))
+                )
             return self.resolve_url(path)
         # production & preview both need to use the file from the manifest
         return self.resolve_url(self.build_manifest.get_asset(path).file)
 
     def does_asset_exist(self, filename: Path):
         """In production node_modules might not exist - instead check the manifest file"""
         if self.mode == "development":
```

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/dom_possible_standard_names.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/dom_possible_standard_names.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/forms/renderers.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/management/commands/extract_frontend_assets.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/management/commands/extract_frontend_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import io
 import json
 from pathlib import Path
 import re
 import sys
 from typing import Any
 from typing import Collection
-from typing import cast
 
 from django.core.management import BaseCommand
 from django.core.management.base import OutputWrapper
 from django.template import TemplateSyntaxError
 from django.template import engines
 from django.template.loader import get_template
 from django.template.utils import get_app_template_dirs
@@ -62,15 +61,15 @@
     errors: list[str] = []
     warnings: list[str] = []
     with BundlerAssetContext() as asset_context:
         prev = asset_context.get_asset_paths()
         for file in get_all_templates_files():
             # TODO: ability to opt out specific templates?
             try:
-                get_template(cast(str, file))
+                get_template(str(file))
                 template_assets = [p for p in asset_context.get_asset_paths() if p not in prev]
                 prev = asset_context.get_asset_paths()
                 if template_assets:
                     breakdown_templates[str(file)] = [str(p) for p in sorted(template_assets)]
             except TemplateSyntaxError:
                 warnings.append(
                     f"Failed to parse {file.relative_to(get_bundler().root_dir)} - any tags in that file will be ignored"
```

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/prop_handlers.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/prop_handlers.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/settings.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/settings.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templates/bundler_dev_check.html` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templates/bundler_dev_check.html`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/alliance_ui.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/alliance_ui.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/bundler.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/bundler.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/form.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/form.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/react.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/react.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/templatetags/vanilla_extract.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/templatetags/vanilla_extract.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/alliance_platform/frontend/util.py` & `alliance_platform_frontend-0.0.4/alliance_platform/frontend/util.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/pyproject.toml` & `alliance_platform_frontend-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 include = [
     "alliance_platform/frontend/py.typed",
 ]
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 text = "BSD-2-Clause"
 
 [project.urls]
 issues = "https://github.com/AllianceSoftware/alliance-platform-py/issues"
 homepage = "https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend"
```

### Comparing `alliance_platform_frontend-0.0.3/tests/fixtures/build_test/manifest.json` & `alliance_platform_frontend-0.0.4/tests/fixtures/build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/tests/fixtures/server_build_test/manifest.json` & `alliance_platform_frontend-0.0.4/tests/fixtures/server_build_test/manifest.json`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/tests/test_alliance_ui_templatetags.py` & `alliance_platform_frontend-0.0.4/tests/test_alliance_ui_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/tests/test_bundler.py` & `alliance_platform_frontend-0.0.4/tests/test_bundler.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             path_resolvers=[],
             build_dir=current_dir / "fixtures/build_test",
             server_build_dir=current_dir / "fixtures/server_build_test",
             mode="production",
             server_host="localhost",
             server_port="5273",
             server_protocol="http",
+            server_resolve_package_url="redirect-package-url",
         )
         bundler_kwargs.update(kwargs)
         return TestViteBundler(**bundler_kwargs)  # type: ignore [arg-type]
 
     def test_dev_url(self):
         with self.assertRaisesMessage(ValueError, "static_url cannot be a full URL in dev"):
             with override_settings(STATIC_URL="http://mycdn.com/static/"):
```

### Comparing `alliance_platform_frontend-0.0.3/tests/test_bundler_templatetags.py` & `alliance_platform_frontend-0.0.4/tests/test_bundler_templatetags.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/tests/test_context.py` & `alliance_platform_frontend-0.0.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/tests/test_utils/__init__.py` & `alliance_platform_frontend-0.0.4/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alliance_platform_frontend-0.0.3/tests/test_utils/bundler.py` & `alliance_platform_frontend-0.0.4/tests/test_utils/bundler.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     root_dir=settings.PROJECT_DIR,
     path_resolvers=[],
     build_dir=fixtures_dir / "build_test",
     server_build_dir=fixtures_dir / "server_build_test",
     server_host="localhost",
     server_port="5273",
     server_protocol="http",
+    server_resolve_package_url="redirect-package-url",
 )
 
 
 def run_prettier(code):
     p = subprocess.run(
         [
             str(ap_frontend_settings.NODE_MODULES_DIR / ".bin/prettier"),
```

### Comparing `alliance_platform_frontend-0.0.3/PKG-INFO` & `alliance_platform_frontend-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: alliance-platform-frontend
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django integration for Frontend Bundlers & React
-Keywords: django alliance alliancesoftware
+Keywords: django,alliance,alliancesoftware
 Home-page: https://github.com/AllianceSoftware/alliance-platform-py/packages/ap-frontend
 Author-Email: Alliance Software <support@alliancesoftware.com.au>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

