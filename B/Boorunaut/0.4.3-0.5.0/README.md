# Comparing `tmp/Boorunaut-0.4.3.tar.gz` & `tmp/Boorunaut-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Boorunaut-0.4.3.tar", last modified: Fri Aug 21 02:00:31 2020, max compression
+gzip compressed data, was "Boorunaut-0.5.0.tar", last modified: Tue Apr 23 00:11:52 2024, max compression
```

## Comparing `Boorunaut-0.4.3.tar` & `Boorunaut-0.5.0.tar`

### file list

```diff
@@ -1,163 +1,169 @@
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.522037 Boorunaut-0.4.3/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.864788 Boorunaut-0.4.3/Boorunaut.egg-info/
--rw-rw-rw-   0        0        0     2350 2020-08-21 02:00:30.000000 Boorunaut-0.4.3/Boorunaut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4805 2020-08-21 02:00:30.000000 Boorunaut-0.4.3/Boorunaut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-21 02:00:30.000000 Boorunaut-0.4.3/Boorunaut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2020-08-21 02:00:30.000000 Boorunaut-0.4.3/Boorunaut.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      258 2020-08-21 02:00:30.000000 Boorunaut-0.4.3/Boorunaut.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2020-08-21 02:00:30.000000 Boorunaut-0.4.3/Boorunaut.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/LICENSE
--rw-rw-rw-   0        0        0      191 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2350 2020-08-21 02:00:31.511066 Boorunaut-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1278 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.903072 Boorunaut-0.4.3/booru/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.958481 Boorunaut-0.4.3/booru/account/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/__init__.py
--rw-rw-rw-   0        0        0      553 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/admin.py
--rw-rw-rw-   0        0        0      100 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/apps.py
--rw-rw-rw-   0        0        0      594 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/decorators.py
--rw-rw-rw-   0        0        0     5126 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/forms.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.974439 Boorunaut-0.4.3/booru/account/migrations/
--rw-rw-rw-   0        0        0     4434 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1304 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/migrations/0002_auto_20181113_2121.py
--rw-rw-rw-   0        0        0      639 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/migrations/0003_auto_20181113_2139.py
--rw-rw-rw-   0        0        0      541 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/migrations/0004_auto_20181130_1530.py
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/migrations/__init__.py
--rw-rw-rw-   0        0        0     4265 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/models.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.787112 Boorunaut-0.4.3/booru/account/static/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.788110 Boorunaut-0.4.3/booru/account/static/booru/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.788110 Boorunaut-0.4.3/booru/account/static/booru/account/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.975436 Boorunaut-0.4.3/booru/account/static/booru/account/js/
--rw-rw-rw-   0        0        0      350 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/static/booru/account/js/profile.js
--rw-rw-rw-   0        0        0       63 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/tests.py
--rw-rw-rw-   0        0        0      368 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/urls.py
--rw-rw-rw-   0        0        0     8634 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/account/views.py
--rw-rw-rw-   0        0        0      455 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/admin.py
--rw-rw-rw-   0        0        0       90 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/apps.py
--rw-rw-rw-   0        0        0      687 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/context_processors.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.018322 Boorunaut-0.4.3/booru/core/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/__init__.py
--rw-rw-rw-   0        0        0      152 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/admin.py
--rw-rw-rw-   0        0        0       94 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/apps.py
--rw-rw-rw-   0        0        0      827 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/forms.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.101099 Boorunaut-0.4.3/booru/core/migrations/
--rw-rw-rw-   0        0        0      938 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      549 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0002_bannedhash.py
--rw-rw-rw-   0        0        0     1264 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0003_auto_20181120_1549.py
--rw-rw-rw-   0        0        0      406 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0004_auto_20181120_1657.py
--rw-rw-rw-   0        0        0      523 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0005_auto_20181120_1943.py
--rw-rw-rw-   0        0        0     1202 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0006_postflag.py
--rw-rw-rw-   0        0        0      453 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0007_postflag_status.py
--rw-rw-rw-   0        0        0      401 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0008_auto_20181209_2237.py
--rw-rw-rw-   0        0        0      445 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/0009_auto_20181210_2031.py
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     1377 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/models.py
--rw-rw-rw-   0        0        0       63 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/tests.py
--rw-rw-rw-   0        0        0      683 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/urls.py
--rw-rw-rw-   0        0        0     6170 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/core/views.py
--rw-rw-rw-   0        0        0    12693 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/forms.py
--rw-rw-rw-   0        0        0     1700 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/managers.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.148518 Boorunaut-0.4.3/booru/migrations/
--rw-rw-rw-   0        0        0    16807 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1276 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0002_auto_20181113_2136.py
--rw-rw-rw-   0        0        0      712 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0003_auto_20181118_1918.py
--rw-rw-rw-   0        0        0      644 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0004_auto_20181118_2126.py
--rw-rw-rw-   0        0        0      447 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0005_auto_20181206_1852.py
--rw-rw-rw-   0        0        0      407 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0006_comment_is_hidden.py
--rw-rw-rw-   0        0        0      710 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0007_auto_20181211_2031.py
--rw-rw-rw-   0        0        0      577 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/0008_auto_20181213_1831.py
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/migrations/__init__.py
--rw-rw-rw-   0        0        0    14225 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/models.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.161484 Boorunaut-0.4.3/booru/setup/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.177441 Boorunaut-0.4.3/booru/setup/project_template/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/project_template/__init__.py
--rw-rw-rw-   0        0        0      565 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/project_template/manage.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.203370 Boorunaut-0.4.3/booru/setup/project_template/project_name/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/project_template/project_name/__init__.py
--rw-rw-rw-   0        0        0     1643 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/project_template/project_name/roles.py
--rw-rw-rw-   0        0        0     4786 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/project_template/project_name/settings.py
--rw-rw-rw-   0        0        0     1654 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/project_template/project_name/urls.py
--rw-rw-rw-   0        0        0      444 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/project_template/project_name/wsgi.py
--rw-rw-rw-   0        0        0     1909 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/setup/start_project.py
--rw-rw-rw-   0        0        0      876 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/sitemaps.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.812048 Boorunaut-0.4.3/booru/static/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.815039 Boorunaut-0.4.3/booru/static/booru/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.813043 Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.217334 Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/css/
--rw-rw-rw-   0        0        0     1902 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/css/bootstrap-toggle.css
--rw-rw-rw-   0        0        0     1721 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.219329 Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/js/
--rw-rw-rw-   0        0        0     5718 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.js
--rw-rw-rw-   0        0        0     4241 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.246257 Boorunaut-0.4.3/booru/static/booru/css/
--rw-rw-rw-   0        0        0      369 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/css/base.css
--rw-rw-rw-   0        0        0   205821 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/css/custom_cosmo.css
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/css/index.css
--rw-rw-rw-   0        0        0      361 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/css/post_detail.css
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.261217 Boorunaut-0.4.3/booru/static/booru/jQuery-Tags-Input-1.3.6/
--rw-rw-rw-   0        0        0      829 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css
--rw-rw-rw-   0        0        0     6632 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.287148 Boorunaut-0.4.3/booru/static/booru/js/
--rw-rw-rw-   0        0        0     3590 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/js/post_detail.js
--rw-rw-rw-   0        0        0      711 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/static/booru/js/tag_search_autocomplete.js
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:30.816036 Boorunaut-0.4.3/booru/templates/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.427290 Boorunaut-0.4.3/booru/templates/booru/
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.453221 Boorunaut-0.4.3/booru/templates/booru/account/
--rw-rw-rw-   0        0        0     1811 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/account/login.html
--rw-rw-rw-   0        0        0     9186 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/account/profile.html
--rw-rw-rw-   0        0        0     3346 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/account/register.html
--rw-rw-rw-   0        0        0     3974 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/account/settings.html
--rw-rw-rw-   0        0        0     3893 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/base.html
--rw-rw-rw-   0        0        0     4466 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/base_admin.html
--rw-rw-rw-   0        0        0     2273 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/base_index.html
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.466187 Boorunaut-0.4.3/booru/templates/booru/core/
--rw-rw-rw-   0        0        0      500 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/core/privacy_policy.html
--rw-rw-rw-   0        0        0      506 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/core/terms_of_service.html
--rw-rw-rw-   0        0        0      615 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/gallery_create.html
--rw-rw-rw-   0        0        0     3339 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/gallery_detail.html
--rw-rw-rw-   0        0        0      650 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/gallery_edit.html
--rw-rw-rw-   0        0        0     3669 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/gallery_history.html
--rw-rw-rw-   0        0        0     3166 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/gallery_list.html
--rw-rw-rw-   0        0        0      864 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/implication_create.html
--rw-rw-rw-   0        0        0     3517 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/implication_detail.html
--rw-rw-rw-   0        0        0     4424 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/implication_list.html
--rw-rw-rw-   0        0        0     2516 2020-08-21 01:59:37.000000 Boorunaut-0.4.3/booru/templates/booru/index.html
--rw-rw-rw-   0        0        0     5021 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/navbar.html
--rw-rw-rw-   0        0        0    22335 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/post_detail.html
--rw-rw-rw-   0        0        0      797 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/post_flag.html
--rw-rw-rw-   0        0        0     4460 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/post_history.html
--rw-rw-rw-   0        0        0     5133 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/posts.html
--rw-rw-rw-   0        0        0     1984 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/staff_hash_ban.html
--rw-rw-rw-   0        0        0     1575 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/staff_mass_rename.html
--rw-rw-rw-   0        0        0     2521 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/staff_mod_queue.html
--rw-rw-rw-   0        0        0     1686 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/staff_page.html
--rw-rw-rw-   0        0        0     1323 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/staff_site_configuration.html
--rw-rw-rw-   0        0        0      789 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/staff_user_tools.html
--rw-rw-rw-   0        0        0      537 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/tag_confirm_delete.html
--rw-rw-rw-   0        0        0     5769 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/tag_detail.html
--rw-rw-rw-   0        0        0      504 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/tag_edit.html
--rw-rw-rw-   0        0        0     4099 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/tag_history.html
--rw-rw-rw-   0        0        0     3568 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/tag_list.html
--rw-rw-rw-   0        0        0     1390 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/tag_revision_diff.html
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.468181 Boorunaut-0.4.3/booru/templates/booru/templatetags/
--rw-rw-rw-   0        0        0      259 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templates/booru/templatetags/version_comparator.html
--rw-rw-rw-   0        0        0     5904 2020-08-21 01:47:51.000000 Boorunaut-0.4.3/booru/templates/booru/upload.html
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.482143 Boorunaut-0.4.3/booru/templatetags/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2013 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templatetags/number_converter.py
--rw-rw-rw-   0        0        0     1032 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/templatetags/version_comparator.py
-drwxrwxrwx   0        0        0        0 2020-08-21 02:00:31.510069 Boorunaut-0.4.3/booru/tests/
--rw-rw-rw-   0        0        0        0 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/tests/__init__.py
--rw-rw-rw-   0        0        0     2902 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/tests/tests_booru_clients.py
--rw-rw-rw-   0        0        0     3465 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/tests/tests_booru_forms.py
--rw-rw-rw-   0        0        0     4728 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/tests/tests_booru_staff_page_clients.py
--rw-rw-rw-   0        0        0     9340 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/tests/tests_booru_tags_operators.py
--rw-rw-rw-   0        0        0     1513 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/tests/tests_booru_utilities.py
--rw-rw-rw-   0        0        0     4173 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/urls.py
--rw-rw-rw-   0        0        0    11965 2020-08-17 20:05:56.000000 Boorunaut-0.4.3/booru/utils.py
--rw-rw-rw-   0        0        0    23391 2020-08-17 19:56:36.000000 Boorunaut-0.4.3/booru/views.py
--rw-rw-rw-   0        0        0      270 2020-08-21 00:31:00.000000 Boorunaut-0.4.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2020-08-21 02:00:31.522037 Boorunaut-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1528 2020-08-21 01:59:34.000000 Boorunaut-0.4.3/setup.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.830899 Boorunaut-0.5.0/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/Boorunaut.egg-info/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4551 2024-04-23 00:11:52.000000 Boorunaut-0.5.0/Boorunaut.egg-info/PKG-INFO
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     5192 2024-04-23 00:11:52.000000 Boorunaut-0.5.0/Boorunaut.egg-info/SOURCES.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        1 2024-04-23 00:11:52.000000 Boorunaut-0.5.0/Boorunaut.egg-info/dependency_links.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       62 2024-04-23 00:11:52.000000 Boorunaut-0.5.0/Boorunaut.egg-info/entry_points.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      352 2024-04-23 00:11:52.000000 Boorunaut-0.5.0/Boorunaut.egg-info/requires.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       17 2024-04-23 00:11:52.000000 Boorunaut-0.5.0/Boorunaut.egg-info/top_level.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1066 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/LICENSE
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      183 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/MANIFEST.in
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4551 2024-04-23 00:11:52.830899 Boorunaut-0.5.0/PKG-INFO
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3736 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/README.md
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/__init__.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/account/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      539 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/admin.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       95 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/apps.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      576 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/decorators.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4993 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/forms.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/account/migrations/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4361 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/migrations/0001_initial.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1271 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/migrations/0002_auto_20181113_2121.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      619 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/migrations/0003_auto_20181113_2139.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      524 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/migrations/0004_auto_20181130_1530.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      431 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/migrations/0005_alter_account_first_name.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      874 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/migrations/0006_alter_account_id_alter_privilege_id_alter_timeout_id.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/migrations/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4149 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/models.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/booru/account/static/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/booru/account/static/booru/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/booru/account/static/booru/account/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/account/static/booru/account/js/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      337 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/static/booru/account/js/profile.js
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       60 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/tests.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      356 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/urls.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     8475 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/account/views.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      441 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/admin.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       85 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/apps.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      668 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/context_processors.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/core/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      147 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/admin.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       89 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/apps.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      802 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/forms.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/core/migrations/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      915 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0001_initial.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      527 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0002_bannedhash.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1227 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0003_auto_20181120_1549.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      388 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0004_auto_20181120_1657.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      503 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0005_auto_20181120_1943.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1171 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0006_postflag.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      435 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0007_postflag_status.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      383 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0008_auto_20181209_2237.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      427 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0009_auto_20181210_2031.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      656 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/0010_alter_bannedhash_id_alter_postflag_id.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/migrations/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1337 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/models.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       60 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/tests.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      669 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/urls.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     6014 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/core/views.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)    12380 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/forms.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1647 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/managers.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/migrations/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)    16526 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0001_initial.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1247 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0002_auto_20181113_2136.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      684 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0003_auto_20181118_1918.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      621 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0004_auto_20181118_2126.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      430 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0005_auto_20181206_1852.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      389 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0006_comment_is_hidden.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      685 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0007_auto_20181211_2031.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      558 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0008_auto_20181213_1831.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3234 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0009_alter_historicalgallery_options_and_more.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3237 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/0010_alter_category_id_alter_comment_id_and_more.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/migrations/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)    13826 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/models.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/setup/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/__init__.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/setup/project_template/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/project_template/__init__.py
+-rwxrwxr-x   0 thiago    (1000) thiago    (1000)      550 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/project_template/manage.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/setup/project_template/project_name/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/project_template/project_name/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1586 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/project_template/project_name/roles.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4685 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/project_template/project_name/settings.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1612 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/project_template/project_name/urls.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      428 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/project_template/project_name/wsgi.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1841 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/setup/start_project.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      838 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/sitemaps.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/booru/static/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/booru/static/booru/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/css/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1819 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/css/bootstrap-toggle.css
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1692 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/js/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     5538 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.js
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4231 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/static/booru/css/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      350 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/css/base.css
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)   196688 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/css/custom_cosmo.css
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/css/index.css
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      336 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/css/post_detail.css
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/static/booru/jQuery-Tags-Input-1.3.6/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      829 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     6632 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.822899 Boorunaut-0.5.0/booru/static/booru/js/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3478 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/js/post_detail.js
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      689 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/static/booru/js/tag_search_autocomplete.js
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.818899 Boorunaut-0.5.0/booru/templates/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.826899 Boorunaut-0.5.0/booru/templates/booru/
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.826899 Boorunaut-0.5.0/booru/templates/booru/account/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1753 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/account/login.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     8965 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/account/profile.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3255 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/account/register.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3887 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/account/settings.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3799 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/base.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4373 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/base_admin.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     2226 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/base_index.html
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.830899 Boorunaut-0.5.0/booru/templates/booru/core/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      468 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/core/privacy_policy.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      474 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/core/terms_of_service.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      586 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/gallery_create.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3262 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/gallery_detail.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      622 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/gallery_edit.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3578 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/gallery_history.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3084 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/gallery_list.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      832 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/implication_create.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3432 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/implication_detail.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4327 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/implication_list.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     2450 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/index.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4917 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/navbar.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)    21898 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/post_detail.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      765 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/post_flag.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4350 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/post_history.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     5019 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/posts.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1918 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/staff_hash_ban.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1524 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/staff_mass_rename.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     2442 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/staff_mod_queue.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1627 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/staff_page.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1281 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/staff_site_configuration.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      756 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/staff_user_tools.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      507 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/tag_confirm_delete.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     5636 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/tag_detail.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      478 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/tag_edit.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4008 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/tag_history.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3480 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/tag_list.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1338 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/tag_revision_diff.html
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.830899 Boorunaut-0.5.0/booru/templates/booru/templatetags/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      251 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/templatetags/version_comparator.html
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     5749 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templates/booru/upload.html
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.830899 Boorunaut-0.5.0/booru/templatetags/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templatetags/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      839 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templatetags/number_converter.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      607 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/templatetags/version_comparator.py
+drwxrwxr-x   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:11:52.830899 Boorunaut-0.5.0/booru/tests/
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)        0 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/tests/__init__.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     2813 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/tests/tests_booru_clients.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     3374 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/tests/tests_booru_forms.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4605 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/tests/tests_booru_staff_page_clients.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     9123 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/tests/tests_booru_tags_operators.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      894 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/tests/tests_booru_templatetags.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1472 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/tests/tests_booru_utilities.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     4110 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/urls.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)    11648 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/utils.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)    22780 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/booru/views.py
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)      351 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/requirements.txt
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)       38 2024-04-23 00:11:52.830899 Boorunaut-0.5.0/setup.cfg
+-rw-rw-r--   0 thiago    (1000) thiago    (1000)     1495 2024-04-23 00:02:54.000000 Boorunaut-0.5.0/setup.py
```

### Comparing `Boorunaut-0.4.3/Boorunaut.egg-info/SOURCES.txt` & `Boorunaut-0.5.0/Boorunaut.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 booru/account/tests.py
 booru/account/urls.py
 booru/account/views.py
 booru/account/migrations/0001_initial.py
 booru/account/migrations/0002_auto_20181113_2121.py
 booru/account/migrations/0003_auto_20181113_2139.py
 booru/account/migrations/0004_auto_20181130_1530.py
+booru/account/migrations/0005_alter_account_first_name.py
+booru/account/migrations/0006_alter_account_id_alter_privilege_id_alter_timeout_id.py
 booru/account/migrations/__init__.py
 booru/account/static/booru/account/js/profile.js
 booru/core/__init__.py
 booru/core/admin.py
 booru/core/apps.py
 booru/core/forms.py
 booru/core/models.py
@@ -48,23 +50,26 @@
 booru/core/migrations/0003_auto_20181120_1549.py
 booru/core/migrations/0004_auto_20181120_1657.py
 booru/core/migrations/0005_auto_20181120_1943.py
 booru/core/migrations/0006_postflag.py
 booru/core/migrations/0007_postflag_status.py
 booru/core/migrations/0008_auto_20181209_2237.py
 booru/core/migrations/0009_auto_20181210_2031.py
+booru/core/migrations/0010_alter_bannedhash_id_alter_postflag_id.py
 booru/core/migrations/__init__.py
 booru/migrations/0001_initial.py
 booru/migrations/0002_auto_20181113_2136.py
 booru/migrations/0003_auto_20181118_1918.py
 booru/migrations/0004_auto_20181118_2126.py
 booru/migrations/0005_auto_20181206_1852.py
 booru/migrations/0006_comment_is_hidden.py
 booru/migrations/0007_auto_20181211_2031.py
 booru/migrations/0008_auto_20181213_1831.py
+booru/migrations/0009_alter_historicalgallery_options_and_more.py
+booru/migrations/0010_alter_category_id_alter_comment_id_and_more.py
 booru/migrations/__init__.py
 booru/setup/__init__.py
 booru/setup/start_project.py
 booru/setup/project_template/__init__.py
 booru/setup/project_template/manage.py
 booru/setup/project_template/project_name/__init__.py
 booru/setup/project_template/project_name/roles.py
@@ -124,8 +129,9 @@
 booru/templatetags/number_converter.py
 booru/templatetags/version_comparator.py
 booru/tests/__init__.py
 booru/tests/tests_booru_clients.py
 booru/tests/tests_booru_forms.py
 booru/tests/tests_booru_staff_page_clients.py
 booru/tests/tests_booru_tags_operators.py
+booru/tests/tests_booru_templatetags.py
 booru/tests/tests_booru_utilities.py
```

### Comparing `Boorunaut-0.4.3/LICENSE` & `Boorunaut-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2017 Boorunaut
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2017 Boorunaut
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `Boorunaut-0.4.3/booru/account/decorators.py` & `Boorunaut-0.5.0/booru/account/decorators.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from django.shortcuts import redirect
-
-def user_is_not_blocked(function):
-    def wrap(request, *args, **kwargs):
-        if hasattr(request, 'request'):
-            user_request = request.request.user # work as self.request.user
-        else:
-            user_request = request.user
-
-        if user_request.is_authenticated and not user_request.has_priv("can_login"):
-            return redirect('account:logout')
-        else:
-            return function(request, *args, **kwargs)
-
-    wrap.__doc__ = function.__doc__
-    wrap.__name__ = function.__name__
-
-    return wrap
+from django.shortcuts import redirect
+
+def user_is_not_blocked(function):
+    def wrap(request, *args, **kwargs):
+        if hasattr(request, 'request'):
+            user_request = request.request.user # work as self.request.user
+        else:
+            user_request = request.user
+
+        if user_request.is_authenticated and not user_request.has_priv("can_login"):
+            return redirect('account:logout')
+        else:
+            return function(request, *args, **kwargs)
+
+    wrap.__doc__ = function.__doc__
+    wrap.__name__ = function.__name__
+
+    return wrap
```

### Comparing `Boorunaut-0.4.3/booru/account/forms.py` & `Boorunaut-0.5.0/booru/account/forms.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from django import forms
-from django.contrib.auth.forms import (AuthenticationForm, UserCreationForm,
-                                       UsernameField)
-from django.contrib.auth.models import Group
-from django.db.models import Q
-from django.template.defaultfilters import slugify
-
-import booru.utils
-from booru.account.models import Account
-
-
-class UniqueUserEmailField(forms.EmailField):
-    """
-    An EmailField which only is valid if no Account has that email.
-    """
-
-    def validate(self, value):
-        super().validate(value)
-        try:
-            Account.objects.get(email=value)
-            raise forms.ValidationError("A user with that email already exists.")
-        except Account.MultipleObjectsReturned:
-            raise forms.ValidationError("A user with that email already exists.")
-        except Account.DoesNotExist:
-            pass
-
-class UsernameExistsField(UsernameField):
-    """
-    An UsernameField that raises an error when the name is
-    not registered on the database.
-    """
-
-    def validate(self, value):
-        super().validate(value)
-        try:
-            Account.objects.get(username=value)
-        except Account.DoesNotExist:
-            raise forms.ValidationError("There's no user registered with that username.")
-
-class UsernameNotBlockedField(UsernameExistsField):
-    """
-    An UsernameExistsField that raises an error when the account
-    is banned from the website.
-    """
-
-    def validate(self, value):
-        super().validate(value)
-        account = Account.objects.get(slug=slugify(value))
-        priv_timeout = account.get_priv_timeout("can_login")
-        if priv_timeout.exists(): # is banned
-            raise forms.ValidationError("This user is currently banned until {}.".format(priv_timeout.first().expiration))
-
-
-class UniqueUsernameField(UsernameField):
-    """
-    An UsernameField that raises an error when the
-    name is already in use.
-    """
-
-    def validate(self, value):
-        super().validate(value)
-        try:
-            Account.objects.get(slug=slugify(value))
-            raise forms.ValidationError("There's already an user registered with that username.")
-        except Account.MultipleObjectsReturned:
-            raise forms.ValidationError("There's already an user registered with that username.")
-        except Account.DoesNotExist:
-            pass
-
-class UserRegisterForm(UserCreationForm):
-    """
-    Extends the built in UserCreationForm to include the Account email
-    and the form-control class in each widget.
-    """
-
-    email = UniqueUserEmailField(required=True, label='Email address')
-    username = UniqueUsernameField(
-        max_length=254,
-        widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control'}),
-    )
-
-    class Meta:
-        model = Account
-        fields = ("username", "email")
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.fields['password1'].widget = forms.PasswordInput(attrs={'class': 'form-control'})
-        self.fields['password2'].widget = forms.PasswordInput(attrs={'class': 'form-control'})
-        self.fields['email'].widget = forms.EmailInput(attrs={'class': 'form-control'})
-
-class UserAuthenticationForm(AuthenticationForm):
-    """
-    Extends the built in AuthenticationForm to add
-    the form-control class in each widget.
-    """
-
-    username = UsernameNotBlockedField(
-        max_length=254,
-        widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control'}),
-    )
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.fields['password'].widget = forms.PasswordInput(attrs={'class': 'form-control'})
-
-class UserSettingsForm(forms.ModelForm):
-    """
-    Form for modifying the user settings.
-    """
-
-    class Meta:
-        model = Account
-        fields = ["safe_only", "show_comments", "tag_blacklist"]
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.fields['safe_only'].widget = forms.CheckboxInput(attrs={'class': 'form-control', 'data-toggle': 'toggle'})
-        self.fields['show_comments'].widget = forms.CheckboxInput(attrs={'class': 'form-control', 'data-toggle': 'toggle'})
-        # TODO: implement the tag blacklist
-        #self.fields['tag_blacklist'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows': '4', 'placeholder': 'Ex.: wall rating:explicit user:girugamesh'})
-        self.fields['tag_blacklist'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows': '4', 'placeholder': "This feature wasn't implemented yet.", "disabled": ""})
-
-class StaffUserGroupForm(forms.Form):
-    group = forms.ChoiceField()
-    
-    class Meta:
-        fields = "__all__"
-
-    def __init__(self, *args, **kwargs):
-        super(StaffUserGroupForm, self).__init__(*args, **kwargs)
-        self.fields['group'].widget = forms.Select(attrs={'class': 'form-control'})
-        self.fields['group'].choices = booru.utils.get_all_roles()
+from django import forms
+from django.contrib.auth.forms import (AuthenticationForm, UserCreationForm,
+                                       UsernameField)
+from django.contrib.auth.models import Group
+from django.db.models import Q
+from django.template.defaultfilters import slugify
+
+import booru.utils
+from booru.account.models import Account
+
+
+class UniqueUserEmailField(forms.EmailField):
+    """
+    An EmailField which only is valid if no Account has that email.
+    """
+
+    def validate(self, value):
+        super().validate(value)
+        try:
+            Account.objects.get(email=value)
+            raise forms.ValidationError("A user with that email already exists.")
+        except Account.MultipleObjectsReturned:
+            raise forms.ValidationError("A user with that email already exists.")
+        except Account.DoesNotExist:
+            pass
+
+class UsernameExistsField(UsernameField):
+    """
+    An UsernameField that raises an error when the name is
+    not registered on the database.
+    """
+
+    def validate(self, value):
+        super().validate(value)
+        try:
+            Account.objects.get(username=value)
+        except Account.DoesNotExist:
+            raise forms.ValidationError("There's no user registered with that username.")
+
+class UsernameNotBlockedField(UsernameExistsField):
+    """
+    An UsernameExistsField that raises an error when the account
+    is banned from the website.
+    """
+
+    def validate(self, value):
+        super().validate(value)
+        account = Account.objects.get(slug=slugify(value))
+        priv_timeout = account.get_priv_timeout("can_login")
+        if priv_timeout.exists(): # is banned
+            raise forms.ValidationError("This user is currently banned until {}.".format(priv_timeout.first().expiration))
+
+
+class UniqueUsernameField(UsernameField):
+    """
+    An UsernameField that raises an error when the
+    name is already in use.
+    """
+
+    def validate(self, value):
+        super().validate(value)
+        try:
+            Account.objects.get(slug=slugify(value))
+            raise forms.ValidationError("There's already an user registered with that username.")
+        except Account.MultipleObjectsReturned:
+            raise forms.ValidationError("There's already an user registered with that username.")
+        except Account.DoesNotExist:
+            pass
+
+class UserRegisterForm(UserCreationForm):
+    """
+    Extends the built in UserCreationForm to include the Account email
+    and the form-control class in each widget.
+    """
+
+    email = UniqueUserEmailField(required=True, label='Email address')
+    username = UniqueUsernameField(
+        max_length=254,
+        widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control'}),
+    )
+
+    class Meta:
+        model = Account
+        fields = ("username", "email")
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.fields['password1'].widget = forms.PasswordInput(attrs={'class': 'form-control'})
+        self.fields['password2'].widget = forms.PasswordInput(attrs={'class': 'form-control'})
+        self.fields['email'].widget = forms.EmailInput(attrs={'class': 'form-control'})
+
+class UserAuthenticationForm(AuthenticationForm):
+    """
+    Extends the built in AuthenticationForm to add
+    the form-control class in each widget.
+    """
+
+    username = UsernameNotBlockedField(
+        max_length=254,
+        widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control'}),
+    )
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.fields['password'].widget = forms.PasswordInput(attrs={'class': 'form-control'})
+
+class UserSettingsForm(forms.ModelForm):
+    """
+    Form for modifying the user settings.
+    """
+
+    class Meta:
+        model = Account
+        fields = ["safe_only", "show_comments", "tag_blacklist"]
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.fields['safe_only'].widget = forms.CheckboxInput(attrs={'class': 'form-control', 'data-toggle': 'toggle'})
+        self.fields['show_comments'].widget = forms.CheckboxInput(attrs={'class': 'form-control', 'data-toggle': 'toggle'})
+        # TODO: implement the tag blacklist
+        #self.fields['tag_blacklist'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows': '4', 'placeholder': 'Ex.: wall rating:explicit user:girugamesh'})
+        self.fields['tag_blacklist'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows': '4', 'placeholder': "This feature wasn't implemented yet.", "disabled": ""})
+
+class StaffUserGroupForm(forms.Form):
+    group = forms.ChoiceField()
+    
+    class Meta:
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super(StaffUserGroupForm, self).__init__(*args, **kwargs)
+        self.fields['group'].widget = forms.Select(attrs={'class': 'form-control'})
+        self.fields['group'].choices = booru.utils.get_all_roles()
```

### Comparing `Boorunaut-0.4.3/booru/account/migrations/0001_initial.py` & `Boorunaut-0.5.0/booru/account/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# Generated by Django 2.1.2 on 2018-11-13 21:21
-
-import booru.managers
-from django.conf import settings
-import django.contrib.auth.validators
-from django.db import migrations, models
-import django.db.models.deletion
-import django.utils.timezone
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='Account',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('password', models.CharField(max_length=128, verbose_name='password')),
-                ('last_login', models.DateTimeField(blank=True, null=True, verbose_name='last login')),
-                ('is_superuser', models.BooleanField(default=False, help_text='Designates that this user has all permissions without explicitly assigning them.', verbose_name='superuser status')),
-                ('username', models.CharField(error_messages={'unique': 'A user with that username already exists.'}, help_text='Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.', max_length=150, unique=True, validators=[django.contrib.auth.validators.UnicodeUsernameValidator()], verbose_name='username')),
-                ('first_name', models.CharField(blank=True, max_length=30, verbose_name='first name')),
-                ('last_name', models.CharField(blank=True, max_length=150, verbose_name='last name')),
-                ('email', models.EmailField(blank=True, max_length=254, verbose_name='email address')),
-                ('is_staff', models.BooleanField(default=False, help_text='Designates whether the user can log into this admin site.', verbose_name='staff status')),
-                ('is_active', models.BooleanField(default=True, help_text='Designates whether this user should be treated as active. Unselect this instead of deleting accounts.', verbose_name='active')),
-                ('date_joined', models.DateTimeField(default=django.utils.timezone.now, verbose_name='date joined')),
-                ('slug', models.SlugField(blank=True, default='', max_length=250)),
-                ('email_activated', models.BooleanField(default=False)),
-                ('comments_locked', models.BooleanField(default=False)),
-                ('about', models.CharField(blank=True, max_length=2500)),
-                ('safe_only', models.BooleanField(default=True)),
-                ('show_comments', models.BooleanField(default=True)),
-                ('tag_blacklist', models.CharField(blank=True, max_length=2500)),
-                ('is_deleted', models.BooleanField(default=False)),
-            ],
-            options={
-                'permissions': (('modify_profile', 'Can change values from all profiles.'),),
-            },
-            managers=[
-                ('objects', booru.managers.UserManager()),
-            ],
-        ),
-        migrations.CreateModel(
-            name='Privilege',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=255, verbose_name='name')),
-                ('codename', models.CharField(max_length=100, verbose_name='codename')),
-            ],
-            options={
-                'verbose_name': 'privilege',
-                'verbose_name_plural': 'privileges',
-                'ordering': ['codename'],
-            },
-        ),
-        migrations.CreateModel(
-            name='Timeout',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('reason', models.CharField(max_length=2500)),
-                ('expiration', models.DateTimeField()),
-                ('author', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='timeout_creator', to=settings.AUTH_USER_MODEL)),
-                ('revoked', models.ManyToManyField(blank=True, help_text='Privileges revoked from this user.', related_name='revoked_privs', related_query_name='user', to='account.Privilege', verbose_name='privileges')),
-                ('target_user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='user_timedout', to=settings.AUTH_USER_MODEL)),
-            ],
-        ),
-    ]
+# Generated by Django 2.1.2 on 2018-11-13 21:21
+
+import booru.managers
+from django.conf import settings
+import django.contrib.auth.validators
+from django.db import migrations, models
+import django.db.models.deletion
+import django.utils.timezone
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='Account',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('password', models.CharField(max_length=128, verbose_name='password')),
+                ('last_login', models.DateTimeField(blank=True, null=True, verbose_name='last login')),
+                ('is_superuser', models.BooleanField(default=False, help_text='Designates that this user has all permissions without explicitly assigning them.', verbose_name='superuser status')),
+                ('username', models.CharField(error_messages={'unique': 'A user with that username already exists.'}, help_text='Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.', max_length=150, unique=True, validators=[django.contrib.auth.validators.UnicodeUsernameValidator()], verbose_name='username')),
+                ('first_name', models.CharField(blank=True, max_length=30, verbose_name='first name')),
+                ('last_name', models.CharField(blank=True, max_length=150, verbose_name='last name')),
+                ('email', models.EmailField(blank=True, max_length=254, verbose_name='email address')),
+                ('is_staff', models.BooleanField(default=False, help_text='Designates whether the user can log into this admin site.', verbose_name='staff status')),
+                ('is_active', models.BooleanField(default=True, help_text='Designates whether this user should be treated as active. Unselect this instead of deleting accounts.', verbose_name='active')),
+                ('date_joined', models.DateTimeField(default=django.utils.timezone.now, verbose_name='date joined')),
+                ('slug', models.SlugField(blank=True, default='', max_length=250)),
+                ('email_activated', models.BooleanField(default=False)),
+                ('comments_locked', models.BooleanField(default=False)),
+                ('about', models.CharField(blank=True, max_length=2500)),
+                ('safe_only', models.BooleanField(default=True)),
+                ('show_comments', models.BooleanField(default=True)),
+                ('tag_blacklist', models.CharField(blank=True, max_length=2500)),
+                ('is_deleted', models.BooleanField(default=False)),
+            ],
+            options={
+                'permissions': (('modify_profile', 'Can change values from all profiles.'),),
+            },
+            managers=[
+                ('objects', booru.managers.UserManager()),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Privilege',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=255, verbose_name='name')),
+                ('codename', models.CharField(max_length=100, verbose_name='codename')),
+            ],
+            options={
+                'verbose_name': 'privilege',
+                'verbose_name_plural': 'privileges',
+                'ordering': ['codename'],
+            },
+        ),
+        migrations.CreateModel(
+            name='Timeout',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('reason', models.CharField(max_length=2500)),
+                ('expiration', models.DateTimeField()),
+                ('author', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='timeout_creator', to=settings.AUTH_USER_MODEL)),
+                ('revoked', models.ManyToManyField(blank=True, help_text='Privileges revoked from this user.', related_name='revoked_privs', related_query_name='user', to='account.Privilege', verbose_name='privileges')),
+                ('target_user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='user_timedout', to=settings.AUTH_USER_MODEL)),
+            ],
+        ),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/account/migrations/0002_auto_20181113_2121.py` & `Boorunaut-0.5.0/booru/account/migrations/0002_auto_20181113_2121.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Generated by Django 2.1.2 on 2018-11-13 21:21
-
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('booru', '0001_initial'),
-        ('auth', '0009_alter_user_last_name_max_length'),
-        ('account', '0001_initial'),
-    ]
-
-    operations = [
-        migrations.AddField(
-            model_name='account',
-            name='avatar',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='booru.Post'),
-        ),
-        migrations.AddField(
-            model_name='account',
-            name='groups',
-            field=models.ManyToManyField(blank=True, help_text='The groups this user belongs to. A user will get all permissions granted to each of their groups.', related_name='user_set', related_query_name='user', to='auth.Group', verbose_name='groups'),
-        ),
-        migrations.AddField(
-            model_name='account',
-            name='user_permissions',
-            field=models.ManyToManyField(blank=True, help_text='Specific permissions for this user.', related_name='user_set', related_query_name='user', to='auth.Permission', verbose_name='user permissions'),
-        ),
-    ]
+# Generated by Django 2.1.2 on 2018-11-13 21:21
+
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('booru', '0001_initial'),
+        ('auth', '0009_alter_user_last_name_max_length'),
+        ('account', '0001_initial'),
+    ]
+
+    operations = [
+        migrations.AddField(
+            model_name='account',
+            name='avatar',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to='booru.Post'),
+        ),
+        migrations.AddField(
+            model_name='account',
+            name='groups',
+            field=models.ManyToManyField(blank=True, help_text='The groups this user belongs to. A user will get all permissions granted to each of their groups.', related_name='user_set', related_query_name='user', to='auth.Group', verbose_name='groups'),
+        ),
+        migrations.AddField(
+            model_name='account',
+            name='user_permissions',
+            field=models.ManyToManyField(blank=True, help_text='Specific permissions for this user.', related_name='user_set', related_query_name='user', to='auth.Permission', verbose_name='user permissions'),
+        ),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/account/migrations/0003_auto_20181113_2139.py` & `Boorunaut-0.5.0/booru/account/migrations/0003_auto_20181113_2139.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Generated by Django 2.1.2 on 2018-11-13 21:39
-
-from django.db import migrations
-
-
-def create_configs(apps, schema_editor):
-    db_alias = schema_editor.connection.alias
-    Privilege = apps.get_model("account", "Privilege")
-    Privilege.objects.using(db_alias).create(codename="can_comment", name="User can make a comment")
-    Privilege.objects.using(db_alias).create(codename="can_login", name="User can login into the site")
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('account', '0002_auto_20181113_2121'),
-    ]
-
-    operations = [
-        migrations.RunPython(create_configs),
-    ]
+# Generated by Django 2.1.2 on 2018-11-13 21:39
+
+from django.db import migrations
+
+
+def create_configs(apps, schema_editor):
+    db_alias = schema_editor.connection.alias
+    Privilege = apps.get_model("account", "Privilege")
+    Privilege.objects.using(db_alias).create(codename="can_comment", name="User can make a comment")
+    Privilege.objects.using(db_alias).create(codename="can_login", name="User can login into the site")
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('account', '0002_auto_20181113_2121'),
+    ]
+
+    operations = [
+        migrations.RunPython(create_configs),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/account/migrations/0004_auto_20181130_1530.py` & `Boorunaut-0.5.0/booru/account/migrations/0004_auto_20181130_1530.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Generated by Django 2.1.2 on 2018-11-30 15:30
-
-from django.db import migrations
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('account', '0003_auto_20181113_2139'),
-    ]
-
-    operations = [
-        migrations.AlterModelOptions(
-            name='account',
-            options={'permissions': (('modify_profile', 'Can change values from all profiles.'), ('change_user_group', 'Can set the group of a user.'), ('ban_user', 'Can ban users.'), ('ban_mod', 'Can ban moderators.'))},
-        ),
-    ]
+# Generated by Django 2.1.2 on 2018-11-30 15:30
+
+from django.db import migrations
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('account', '0003_auto_20181113_2139'),
+    ]
+
+    operations = [
+        migrations.AlterModelOptions(
+            name='account',
+            options={'permissions': (('modify_profile', 'Can change values from all profiles.'), ('change_user_group', 'Can set the group of a user.'), ('ban_user', 'Can ban users.'), ('ban_mod', 'Can ban moderators.'))},
+        ),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/account/models.py` & `Boorunaut-0.5.0/booru/account/models.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from django.apps import apps
-from django.contrib.auth.models import AbstractUser, Group
-from django.contrib.contenttypes.fields import (GenericForeignKey,
-                                                GenericRelation)
-from django.db import models
-from django.template.defaultfilters import slugify
-from django.urls import reverse
-from django.utils import timezone
-from django.utils.translation import gettext as _
-from rolepermissions.roles import assign_role
-
-from booru.managers import UserManager
-
-
-class Privilege(models.Model):
-    name = models.CharField(_('name'), max_length=255)
-    codename = models.CharField(_('codename'), max_length=100)
-
-    class Meta:
-        verbose_name = _('privilege')
-        verbose_name_plural = _('privileges')
-        ordering = ['codename']
-
-    def __str__(self):
-        return "{} | {}".format(self.codename, self.name)
-
-class Timeout(models.Model):
-    reason      = models.CharField(max_length=2500)
-    expiration  = models.DateTimeField()
-    revoked     = models.ManyToManyField(
-        Privilege,
-        verbose_name=_('privileges'),
-        blank=True,
-        help_text=_('Privileges revoked from this user.'),
-        related_name="revoked_privs",
-        related_query_name="user",
-    )
-    target_user = models.ForeignKey('account.Account', related_name="user_timedout", on_delete=models.CASCADE)
-    author      = models.ForeignKey('account.Account', related_name="timeout_creator", on_delete=models.CASCADE)
-
-
-class Account(AbstractUser):
-    avatar          = models.ForeignKey('booru.Post', null=True, blank=True, on_delete=models.SET_NULL)
-    slug            = models.SlugField(max_length=250, default="", blank=True)
-    email_activated = models.BooleanField(default=False)
-    comments_locked = models.BooleanField(default=False)
-    about           = models.CharField(max_length=2500, blank=True)
-    comments        = GenericRelation('booru.Comment')
-    # Account settings
-    safe_only       = models.BooleanField(default=True)
-    show_comments   = models.BooleanField(default=True)
-    tag_blacklist   = models.CharField(max_length=2500, blank=True)
-
-    is_deleted = models.BooleanField(default=False)
-
-    objects = UserManager()
-
-    def save(self, *args, **kwargs):
-        give_role = False
-        if self.__is_a_new_user():
-            give_role = True
-            self.slug = slugify(self.username)
-        super(Account, self).save(*args, **kwargs)
-
-        if give_role:
-            if self.is_staff:
-                assign_role(self, 'administrator')
-            else:
-                assign_role(self, 'user')
-
-    def __is_a_new_user(self):
-        return not self.id
-
-    def get_absolute_url(self):
-        if self.is_deleted == False:
-            return reverse('booru:profile', kwargs={'account_slug': self.slug})
-        else:
-            return "#"
-
-    def get_name(self):
-        if self.is_deleted == False:
-            return self.username
-        else:
-            return "Anonymous User"
-
-    def get_posts(self):
-        Post = apps.get_model('booru', 'Post')
-        return Post.objects.all().filter(uploader=self)
-
-    def get_favorites_count(self):
-        return self.account_favorites.count()
-
-    def get_comments_count(self):
-        Comment = apps.get_model('booru', 'Comment')
-        return Comment.objects.filter(author=self, content_type__model="post").count()
-
-    def get_priv_timeout(self, codename):
-        timeouts = Timeout.objects.filter(target_user=self, revoked__in=Privilege.objects.filter(codename=codename))
-        timeouts.filter(expiration__lt=timezone.now()).delete() # deleting timeouts if already expired
-        return timeouts
-
-    def has_priv(self, codename):
-        return not self.get_priv_timeout(codename=codename).exists()
-
-    def anonymize(self):
-        self.email = ""
-        self.is_deleted = True
-        self.save()
-
-    class Meta:
-        permissions = (
-            ("modify_profile", "Can change values from all profiles."),
-            ("change_user_group", "Can set the group of a user."),
-            ("ban_user", "Can ban users."),
-            ("ban_mod", "Can ban moderators."),
-        )
+from django.apps import apps
+from django.contrib.auth.models import AbstractUser, Group
+from django.contrib.contenttypes.fields import (GenericForeignKey,
+                                                GenericRelation)
+from django.db import models
+from django.template.defaultfilters import slugify
+from django.urls import reverse
+from django.utils import timezone
+from django.utils.translation import gettext as _
+from rolepermissions.roles import assign_role
+
+from booru.managers import UserManager
+
+
+class Privilege(models.Model):
+    name = models.CharField(_('name'), max_length=255)
+    codename = models.CharField(_('codename'), max_length=100)
+
+    class Meta:
+        verbose_name = _('privilege')
+        verbose_name_plural = _('privileges')
+        ordering = ['codename']
+
+    def __str__(self):
+        return "{} | {}".format(self.codename, self.name)
+
+class Timeout(models.Model):
+    reason      = models.CharField(max_length=2500)
+    expiration  = models.DateTimeField()
+    revoked     = models.ManyToManyField(
+        Privilege,
+        verbose_name=_('privileges'),
+        blank=True,
+        help_text=_('Privileges revoked from this user.'),
+        related_name="revoked_privs",
+        related_query_name="user",
+    )
+    target_user = models.ForeignKey('account.Account', related_name="user_timedout", on_delete=models.CASCADE)
+    author      = models.ForeignKey('account.Account', related_name="timeout_creator", on_delete=models.CASCADE)
+
+
+class Account(AbstractUser):
+    avatar          = models.ForeignKey('booru.Post', null=True, blank=True, on_delete=models.SET_NULL)
+    slug            = models.SlugField(max_length=250, default="", blank=True)
+    email_activated = models.BooleanField(default=False)
+    comments_locked = models.BooleanField(default=False)
+    about           = models.CharField(max_length=2500, blank=True)
+    comments        = GenericRelation('booru.Comment')
+    # Account settings
+    safe_only       = models.BooleanField(default=True)
+    show_comments   = models.BooleanField(default=True)
+    tag_blacklist   = models.CharField(max_length=2500, blank=True)
+
+    is_deleted = models.BooleanField(default=False)
+
+    objects = UserManager()
+
+    def save(self, *args, **kwargs):
+        give_role = False
+        if self.__is_a_new_user():
+            give_role = True
+            self.slug = slugify(self.username)
+        super(Account, self).save(*args, **kwargs)
+
+        if give_role:
+            if self.is_staff:
+                assign_role(self, 'administrator')
+            else:
+                assign_role(self, 'user')
+
+    def __is_a_new_user(self):
+        return not self.id
+
+    def get_absolute_url(self):
+        if self.is_deleted == False:
+            return reverse('booru:profile', kwargs={'account_slug': self.slug})
+        else:
+            return "#"
+
+    def get_name(self):
+        if self.is_deleted == False:
+            return self.username
+        else:
+            return "Anonymous User"
+
+    def get_posts(self):
+        Post = apps.get_model('booru', 'Post')
+        return Post.objects.all().filter(uploader=self)
+
+    def get_favorites_count(self):
+        return self.account_favorites.count()
+
+    def get_comments_count(self):
+        Comment = apps.get_model('booru', 'Comment')
+        return Comment.objects.filter(author=self, content_type__model="post").count()
+
+    def get_priv_timeout(self, codename):
+        timeouts = Timeout.objects.filter(target_user=self, revoked__in=Privilege.objects.filter(codename=codename))
+        timeouts.filter(expiration__lt=timezone.now()).delete() # deleting timeouts if already expired
+        return timeouts
+
+    def has_priv(self, codename):
+        return not self.get_priv_timeout(codename=codename).exists()
+
+    def anonymize(self):
+        self.email = ""
+        self.is_deleted = True
+        self.save()
+
+    class Meta:
+        permissions = (
+            ("modify_profile", "Can change values from all profiles."),
+            ("change_user_group", "Can set the group of a user."),
+            ("ban_user", "Can ban users."),
+            ("ban_mod", "Can ban moderators."),
+        )
```

### Comparing `Boorunaut-0.4.3/booru/account/views.py` & `Boorunaut-0.5.0/booru/account/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,224 +1,225 @@
-from django.contrib.auth import REDIRECT_FIELD_NAME, authenticate
-from django.contrib.auth import login as auth_login
-from django.contrib.auth import logout as auth_logout
-from django.core.paginator import Paginator
-from django.http import HttpResponseRedirect
-from django.shortcuts import get_object_or_404, redirect, render
-from django.utils.decorators import method_decorator
-from django.utils.http import is_safe_url
-from django.views.decorators.cache import never_cache
-from django.views.decorators.csrf import csrf_protect
-from django.views.decorators.debug import sensitive_post_parameters
-from django.views.generic import FormView, RedirectView, TemplateView
-from rolepermissions.checkers import has_permission, has_role
-from rolepermissions.roles import assign_role, clear_roles
-
-from booru.account.decorators import user_is_not_blocked
-from booru.models import Comment, Post
-
-from .forms import (StaffUserGroupForm, UserAuthenticationForm,
-                    UserRegisterForm, UserSettingsForm)
-from .models import Account
-
-
-class LoginView(FormView):
-    """
-    Provides the ability to login as a user with a username and password
-    """
-    success_url = '/post/list'
-    form_class = UserAuthenticationForm
-    redirect_field_name = REDIRECT_FIELD_NAME
-    template_name = "booru/account/login.html"
-
-    @method_decorator(sensitive_post_parameters('password'))
-    @method_decorator(csrf_protect)
-    @method_decorator(never_cache)
-    def dispatch(self, request, *args, **kwargs):
-        if request.user.is_authenticated:
-            return HttpResponseRedirect('/post/list')
-        
-        # Sets a test cookie to make sure the user has cookies enabled
-        request.session.set_test_cookie()
-
-        return super(LoginView, self).dispatch(request, *args, **kwargs)
-
-    def form_valid(self, form):
-        auth_login(self.request, form.get_user())
-
-        # If the test cookie worked, go ahead and
-        # delete it since its no longer needed
-        if self.request.session.test_cookie_worked():
-            self.request.session.delete_test_cookie()
-
-        return super(LoginView, self).form_valid(form)
-
-    def get_success_url(self):
-        redirect_to = self.request.GET.get(self.redirect_field_name)
-        if not is_safe_url(url=redirect_to, allowed_hosts=self.request.get_host()):
-            redirect_to = self.success_url
-        return redirect_to
-
-class LogoutView(RedirectView):
-    """
-    Provides users the ability to logout
-    """
-    url = '/account/login/'
-
-    def get(self, request, *args, **kwargs):
-        auth_logout(request)
-        return super(LogoutView, self).get(request, *args, **kwargs)
-
-class RegisterView(FormView):
-    """
-    Provides the ability to a visitor to register as new user
-    with an username, an email and a password
-    """
-    success_url = '/post/list'
-    form_class = UserRegisterForm
-    redirect_field_name = REDIRECT_FIELD_NAME
-    template_name = "booru/account/register.html"
-
-    @method_decorator(sensitive_post_parameters('password1'))
-    @method_decorator(sensitive_post_parameters('password2'))
-    @method_decorator(csrf_protect)
-    @method_decorator(never_cache)
-    def dispatch(self, request, *args, **kwargs):
-        if request.user.is_authenticated:
-            return HttpResponseRedirect('/post/list')
-
-        # Sets a test cookie to make sure the user has cookies enabled
-        request.session.set_test_cookie()
-
-        return super(RegisterView, self).dispatch(request, *args, **kwargs)
-
-    def form_valid(self, form):
-        form.save()
-
-        username = form.cleaned_data.get('username')
-        raw_password = form.cleaned_data.get('password1')
-
-        user = authenticate(username=username, password=raw_password)
-        auth_login(self.request, user)
-
-        # If the test cookie worked, go ahead and
-        # delete it since its no longer needed
-        if self.request.session.test_cookie_worked():
-            self.request.session.delete_test_cookie()
-
-        return super(RegisterView, self).form_valid(form)
-
-    def get_success_url(self):
-        redirect_to = self.request.GET.get(self.redirect_field_name)
-        if not is_safe_url(url=redirect_to, allowed_hosts=self.request.get_host()):
-            redirect_to = self.success_url
-        return redirect_to
-
-@user_is_not_blocked
-def profile(request, account_slug):
-    account = get_object_or_404(Account.objects.active(), slug=account_slug)
-
-    can_modify_profile = (request.user == account or has_permission(request.user, "modify_profile"))
-
-    user_group_form = StaffUserGroupForm(request.POST or None, request.FILES or None)
-
-    if request.method == "POST":
-        newCommentTextarea = request.POST.get("newCommentTextarea")
-        aboutUserTextarea = request.POST.get("aboutUserTextarea")
-        
-        if not request.user.is_authenticated:
-            return redirect('account:login')
-        elif newCommentTextarea and has_comment_priv: # Comment creating
-            comment_content = newCommentTextarea
-            Comment.objects.create(content=comment_content, author=request.user, content_object=account)
-            return redirect('booru:profile', account_slug=account.slug)
-        elif aboutUserTextarea and can_modify_profile: # About myself editing
-            account.about = aboutUserTextarea
-            account.save()
-            return redirect('booru:profile', account_slug=account.slug)
-
-    if request.user.is_authenticated:
-        if user_group_form.is_valid() and has_permission(request.user, "change_user_group"):
-            group = user_group_form.cleaned_data['group']
-            clear_roles(account)
-            assign_role(account, group)
-
-            if group in ['administrator','moderator','janitor']:
-                account.is_staff = True
-                account.save()
-        
-        has_comment_priv = request.user.has_priv("can_comment")
-        can_change_group = has_permission(request.user, "change_user_group")
-    else:
-        has_comment_priv = False
-        can_change_group = False
-
-    # TODO: I don't remember if I can safely pass account as
-    # an parameter to the render.
-    favorites = Post.objects.filter(favorites__account=account)[:5]
-    
-    context = {
-        'account' : account,
-        'recent_favorites' : favorites,
-        'recent_uploads' : account.get_posts().not_deleted().order_by('-id'),
-        'deleted_posts' : account.get_posts().deleted(),
-        'can_modify_profile': request.user.is_authenticated and can_modify_profile,
-        'can_comment': has_comment_priv,
-        'user_group_form': user_group_form,
-        'can_change_group': can_change_group
-    }
-
-    return render(request, 'booru/account/profile.html', context)
-
-class SettingsView(FormView):
-    """
-    Provides the ability to a visitor to register as new user
-    with an username, an email and a password.
-    """
-    success_url = '.'
-    form_class = UserSettingsForm
-    redirect_field_name = REDIRECT_FIELD_NAME
-    template_name = "booru/account/settings.html"
-
-    def get_initial(self):
-        """
-        Returns the initial data to use for forms on this view.
-        """
-        initial = super().get_initial()
-        account = self.request.user
-
-        initial['safe_only'] = account.safe_only
-        initial['show_comments'] = account.show_comments
-        # TODO: implement the tag blacklist
-        #initial['tag_blacklist'] = account.tag_blacklist
-
-        return initial
-
-    def form_valid(self, form):
-        account = self.request.user
-
-        account.safe_only = form.cleaned_data.get('safe_only')
-        account.show_comments = form.cleaned_data.get('show_comments')
-        account.tag_blacklist = form.cleaned_data.get('tag_blacklist')
-        account.save()
-
-        return super().form_valid(form)
-    
-    @user_is_not_blocked
-    @method_decorator(csrf_protect)
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated:
-            return redirect('account:login')
-
-        return super().dispatch(request, *args, **kwargs)
-
-class DeleteAccountView(RedirectView):
-    """
-    Provides users the ability to logout
-    """
-    url = '/account/logout'
-
-    def get(self, request, *args, **kwargs):
-        if kwargs['account_slug'] == self.request.user.slug:
-            self.request.user.anonymize()
-        
-        return super(DeleteAccountView, self).get(request, *args, **kwargs)
+from django.contrib.auth import REDIRECT_FIELD_NAME, authenticate
+from django.contrib.auth import login as auth_login
+from django.contrib.auth import logout as auth_logout
+from django.core.paginator import Paginator
+from django.http import HttpResponseRedirect
+from django.shortcuts import get_object_or_404, redirect, render
+from django.utils.decorators import method_decorator
+from django.utils.http import url_has_allowed_host_and_scheme
+from django.views.decorators.cache import never_cache
+from django.views.decorators.csrf import csrf_protect
+from django.views.decorators.debug import sensitive_post_parameters
+from django.views.generic import FormView, RedirectView, TemplateView
+from rolepermissions.checkers import has_permission, has_role
+from rolepermissions.roles import assign_role, clear_roles
+
+from booru.account.decorators import user_is_not_blocked
+from booru.models import Comment, Post
+
+from .forms import (StaffUserGroupForm, UserAuthenticationForm,
+                    UserRegisterForm, UserSettingsForm)
+from .models import Account
+
+
+class LoginView(FormView):
+    """
+    Provides the ability to login as a user with a username and password
+    """
+    success_url = '/post/list'
+    form_class = UserAuthenticationForm
+    redirect_field_name = REDIRECT_FIELD_NAME
+    template_name = "booru/account/login.html"
+
+    @method_decorator(sensitive_post_parameters('password'))
+    @method_decorator(csrf_protect)
+    @method_decorator(never_cache)
+    def dispatch(self, request, *args, **kwargs):
+        if request.user.is_authenticated:
+            return HttpResponseRedirect('/post/list')
+        
+        # Sets a test cookie to make sure the user has cookies enabled
+        request.session.set_test_cookie()
+
+        return super(LoginView, self).dispatch(request, *args, **kwargs)
+
+    def form_valid(self, form):
+        auth_login(self.request, form.get_user())
+
+        # If the test cookie worked, go ahead and
+        # delete it since its no longer needed
+        if self.request.session.test_cookie_worked():
+            self.request.session.delete_test_cookie()
+
+        return super(LoginView, self).form_valid(form)
+
+    def get_success_url(self):
+        redirect_to = self.request.GET.get(self.redirect_field_name)
+        if not url_has_allowed_host_and_scheme(url=redirect_to, allowed_hosts=self.request.get_host()):
+            redirect_to = self.success_url
+        return redirect_to
+
+class LogoutView(RedirectView):
+    """
+    Provides users the ability to logout
+    """
+    url = '/account/login/'
+
+    def get(self, request, *args, **kwargs):
+        auth_logout(request)
+        return super(LogoutView, self).get(request, *args, **kwargs)
+
+class RegisterView(FormView):
+    """
+    Provides the ability to a visitor to register as new user
+    with an username, an email and a password
+    """
+    success_url = '/post/list'
+    form_class = UserRegisterForm
+    redirect_field_name = REDIRECT_FIELD_NAME
+    template_name = "booru/account/register.html"
+
+    @method_decorator(sensitive_post_parameters('password1'))
+    @method_decorator(sensitive_post_parameters('password2'))
+    @method_decorator(csrf_protect)
+    @method_decorator(never_cache)
+    def dispatch(self, request, *args, **kwargs):
+        if request.user.is_authenticated:
+            return HttpResponseRedirect('/post/list')
+
+        # Sets a test cookie to make sure the user has cookies enabled
+        request.session.set_test_cookie()
+
+        return super(RegisterView, self).dispatch(request, *args, **kwargs)
+
+    def form_valid(self, form):
+        form.save()
+
+        username = form.cleaned_data.get('username')
+        raw_password = form.cleaned_data.get('password1')
+
+        user = authenticate(username=username, password=raw_password)
+        auth_login(self.request, user)
+
+        # If the test cookie worked, go ahead and
+        # delete it since its no longer needed
+        if self.request.session.test_cookie_worked():
+            self.request.session.delete_test_cookie()
+
+        return super(RegisterView, self).form_valid(form)
+
+    def get_success_url(self):
+        redirect_to = self.request.GET.get(self.redirect_field_name)
+        if not url_has_allowed_host_and_scheme(url=redirect_to, allowed_hosts=self.request.get_host()):
+            redirect_to = self.success_url
+        return redirect_to
+
+@user_is_not_blocked
+def profile(request, account_slug):
+    account = get_object_or_404(Account.objects.active(), slug=account_slug)
+
+    can_modify_profile = (request.user == account or has_permission(request.user, "modify_profile"))
+
+    user_group_form = StaffUserGroupForm(request.POST or None, request.FILES or None)
+
+    if request.user.is_authenticated:
+        if user_group_form.is_valid() and has_permission(request.user, "change_user_group"):
+            group = user_group_form.cleaned_data['group']
+            clear_roles(account)
+            assign_role(account, group)
+
+            if group in ['administrator','moderator','janitor']:
+                account.is_staff = True
+                account.save()
+        
+        has_comment_priv = request.user.has_priv("can_comment")
+        can_change_group = has_permission(request.user, "change_user_group")
+    else:
+        has_comment_priv = False
+        can_change_group = False
+
+    
+    if request.method == "POST":
+        newCommentTextarea = request.POST.get("newCommentTextarea")
+        aboutUserTextarea = request.POST.get("aboutUserTextarea")
+        
+        if not request.user.is_authenticated:
+            return redirect('account:login')
+        elif newCommentTextarea and has_comment_priv: # Comment creating
+            comment_content = newCommentTextarea
+            Comment.objects.create(content=comment_content, author=request.user, content_object=account)
+            return redirect('booru:profile', account_slug=account.slug)
+        elif aboutUserTextarea and can_modify_profile: # About myself editing
+            account.about = aboutUserTextarea
+            account.save()
+            return redirect('booru:profile', account_slug=account.slug)
+
+    # TODO: I don't remember if I can safely pass account as
+    # an parameter to the render.
+    favorites = Post.objects.filter(favorites__account=account)[:5]
+    
+    context = {
+        'account' : account,
+        'recent_favorites' : favorites,
+        'recent_uploads' : account.get_posts().not_deleted().order_by('-id'),
+        'deleted_posts' : account.get_posts().deleted(),
+        'can_modify_profile': request.user.is_authenticated and can_modify_profile,
+        'can_comment': has_comment_priv,
+        'user_group_form': user_group_form,
+        'can_change_group': can_change_group
+    }
+
+    return render(request, 'booru/account/profile.html', context)
+
+class SettingsView(FormView):
+    """
+    Provides the ability to a visitor to register as new user
+    with an username, an email and a password.
+    """
+    success_url = '.'
+    form_class = UserSettingsForm
+    redirect_field_name = REDIRECT_FIELD_NAME
+    template_name = "booru/account/settings.html"
+
+    def get_initial(self):
+        """
+        Returns the initial data to use for forms on this view.
+        """
+        initial = super().get_initial()
+        account = self.request.user
+
+        initial['safe_only'] = account.safe_only
+        initial['show_comments'] = account.show_comments
+        # TODO: implement the tag blacklist
+        #initial['tag_blacklist'] = account.tag_blacklist
+
+        return initial
+
+    def form_valid(self, form):
+        account = self.request.user
+
+        account.safe_only = form.cleaned_data.get('safe_only')
+        account.show_comments = form.cleaned_data.get('show_comments')
+        account.tag_blacklist = form.cleaned_data.get('tag_blacklist')
+        account.save()
+
+        return super().form_valid(form)
+    
+    @user_is_not_blocked
+    @method_decorator(csrf_protect)
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated:
+            return redirect('account:login')
+
+        return super().dispatch(request, *args, **kwargs)
+
+class DeleteAccountView(RedirectView):
+    """
+    Provides users the ability to logout
+    """
+    url = '/account/logout'
+
+    def get(self, request, *args, **kwargs):
+        if kwargs['account_slug'] == self.request.user.slug:
+            self.request.user.anonymize()
+        
+        return super(DeleteAccountView, self).get(request, *args, **kwargs)
```

### Comparing `Boorunaut-0.4.3/booru/context_processors.py` & `Boorunaut-0.5.0/booru/context_processors.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from booru.models import Configuration
-from django.conf import settings
-
-
-def site_title(request):
-    return {"SITE_TITLE": Configuration.objects.get(code_name="site_title").value}
-
-def site_description(request):
-    return {"SITE_DESCRIPTION": Configuration.objects.get(code_name="site_description").value}
-
-def announcement(request):
-    return {"SITE_ANNOUNCEMENT": Configuration.objects.get(code_name="announcement").value}
-
-def custom_code(request):
-    return {"INCLUDE_HEADER_CODE": settings.BOORUNAUT_INCLUDE_HEADER_CODE,
-            "ADS_CODE": settings.BOORUNAUT_ADS_CODE}
-
-def preferences(request):
-    return {"EMBED_MODE": settings.BOORUNAUT_EMBED_MODE}
+from booru.models import Configuration
+from django.conf import settings
+
+
+def site_title(request):
+    return {"SITE_TITLE": Configuration.objects.get(code_name="site_title").value}
+
+def site_description(request):
+    return {"SITE_DESCRIPTION": Configuration.objects.get(code_name="site_description").value}
+
+def announcement(request):
+    return {"SITE_ANNOUNCEMENT": Configuration.objects.get(code_name="announcement").value}
+
+def custom_code(request):
+    return {"INCLUDE_HEADER_CODE": settings.BOORUNAUT_INCLUDE_HEADER_CODE,
+            "ADS_CODE": settings.BOORUNAUT_ADS_CODE}
+
+def preferences(request):
+    return {"EMBED_MODE": settings.BOORUNAUT_EMBED_MODE}
```

### Comparing `Boorunaut-0.4.3/booru/core/forms.py` & `Boorunaut-0.5.0/booru/core/forms.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from django import forms
-from booru.core.models import BannedHash, PostFlag
-
-
-class BannedHashCreateForm(forms.ModelForm):
-    '''Form for creating a BannedHash.'''
-
-    class Meta:
-        model = BannedHash
-        fields = ["content"]
-
-    def __init__(self, *args, **kwargs):
-        super(BannedHashCreateForm, self).__init__(*args, **kwargs)
-        self.fields['content'].widget = forms.TextInput(attrs={'class': 'form-control'})
-
-class PostFlagCreateForm(forms.ModelForm):
-    '''Form for creating a flag for post.'''
-
-    class Meta:
-        model = PostFlag
-        fields = ['reason']
-
-    def __init__(self, *args, **kwargs):
-        super(PostFlagCreateForm, self).__init__(*args, **kwargs)
-        self.fields['reason'].widget = forms.Textarea(attrs={'class': 'form-control', 'cols':15})
+from django import forms
+from booru.core.models import BannedHash, PostFlag
+
+
+class BannedHashCreateForm(forms.ModelForm):
+    '''Form for creating a BannedHash.'''
+
+    class Meta:
+        model = BannedHash
+        fields = ["content"]
+
+    def __init__(self, *args, **kwargs):
+        super(BannedHashCreateForm, self).__init__(*args, **kwargs)
+        self.fields['content'].widget = forms.TextInput(attrs={'class': 'form-control'})
+
+class PostFlagCreateForm(forms.ModelForm):
+    '''Form for creating a flag for post.'''
+
+    class Meta:
+        model = PostFlag
+        fields = ['reason']
+
+    def __init__(self, *args, **kwargs):
+        super(PostFlagCreateForm, self).__init__(*args, **kwargs)
+        self.fields['reason'].widget = forms.Textarea(attrs={'class': 'form-control', 'cols':15})
```

### Comparing `Boorunaut-0.4.3/booru/core/migrations/0001_initial.py` & `Boorunaut-0.5.0/booru/core/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Generated by Django 2.1.2 on 2018-11-10 20:26
-
-from django.db import migrations, models
-
-
-def create_configs(apps, schema_editor):
-    db_alias = schema_editor.connection.alias
-    Configuration = apps.get_model("booru", "Configuration")
-    Configuration.objects.using(db_alias).create(code_name="site_title", value="Boorunaut")
-    Configuration.objects.using(db_alias).create(code_name="site_description", value="")
-    Configuration.objects.using(db_alias).create(code_name="google_analytics_id", value="")
-    Configuration.objects.using(db_alias).create(code_name="terms_of_service", value="")
-    Configuration.objects.using(db_alias).create(code_name="privacy_policy", value="")
-    Configuration.objects.using(db_alias).create(code_name="welcome_page", value="1")
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.RunPython(create_configs),
-    ]
+# Generated by Django 2.1.2 on 2018-11-10 20:26
+
+from django.db import migrations, models
+
+
+def create_configs(apps, schema_editor):
+    db_alias = schema_editor.connection.alias
+    Configuration = apps.get_model("booru", "Configuration")
+    Configuration.objects.using(db_alias).create(code_name="site_title", value="Boorunaut")
+    Configuration.objects.using(db_alias).create(code_name="site_description", value="")
+    Configuration.objects.using(db_alias).create(code_name="google_analytics_id", value="")
+    Configuration.objects.using(db_alias).create(code_name="terms_of_service", value="")
+    Configuration.objects.using(db_alias).create(code_name="privacy_policy", value="")
+    Configuration.objects.using(db_alias).create(code_name="welcome_page", value="1")
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.RunPython(create_configs),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/core/migrations/0003_auto_20181120_1549.py` & `Boorunaut-0.5.0/booru/core/migrations/0003_auto_20181120_1549.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# Generated by Django 2.1.2 on 2018-11-20 15:49
-
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-import django.utils.timezone
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('core', '0002_bannedhash'),
-    ]
-
-    operations = [
-        migrations.AlterModelOptions(
-            name='bannedhash',
-            options={'permissions': (('ban_hashes', 'Can ban hashes of media'),), 'verbose_name_plural': 'Banned hashes (MD5)'},
-        ),
-        migrations.AddField(
-            model_name='bannedhash',
-            name='creator',
-            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL),
-        ),
-        migrations.AddField(
-            model_name='bannedhash',
-            name='timestamp',
-            field=models.DateTimeField(auto_now_add=True, default=django.utils.timezone.now),
-            preserve_default=False,
-        ),
-        migrations.AddField(
-            model_name='bannedhash',
-            name='update_timestamp',
-            field=models.DateTimeField(auto_now=True),
-        ),
-    ]
+# Generated by Django 2.1.2 on 2018-11-20 15:49
+
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+import django.utils.timezone
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('core', '0002_bannedhash'),
+    ]
+
+    operations = [
+        migrations.AlterModelOptions(
+            name='bannedhash',
+            options={'permissions': (('ban_hashes', 'Can ban hashes of media'),), 'verbose_name_plural': 'Banned hashes (MD5)'},
+        ),
+        migrations.AddField(
+            model_name='bannedhash',
+            name='creator',
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL),
+        ),
+        migrations.AddField(
+            model_name='bannedhash',
+            name='timestamp',
+            field=models.DateTimeField(auto_now_add=True, default=django.utils.timezone.now),
+            preserve_default=False,
+        ),
+        migrations.AddField(
+            model_name='bannedhash',
+            name='update_timestamp',
+            field=models.DateTimeField(auto_now=True),
+        ),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/core/migrations/0006_postflag.py` & `Boorunaut-0.5.0/booru/core/migrations/0006_postflag.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Generated by Django 2.1.2 on 2018-12-09 18:14
-
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('booru', '0005_auto_20181206_1852'),
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('core', '0005_auto_20181120_1943'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='PostFlag',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('reason', models.CharField(max_length=32)),
-                ('timestamp', models.DateTimeField(auto_now_add=True)),
-                ('update_timestamp', models.DateTimeField(auto_now=True)),
-                ('creator', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL)),
-                ('post', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='booru.Post')),
-            ],
-            options={
-                'verbose_name_plural': 'Post flags',
-            },
-        ),
-    ]
+# Generated by Django 2.1.2 on 2018-12-09 18:14
+
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('booru', '0005_auto_20181206_1852'),
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('core', '0005_auto_20181120_1943'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='PostFlag',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('reason', models.CharField(max_length=32)),
+                ('timestamp', models.DateTimeField(auto_now_add=True)),
+                ('update_timestamp', models.DateTimeField(auto_now=True)),
+                ('creator', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL)),
+                ('post', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='booru.Post')),
+            ],
+            options={
+                'verbose_name_plural': 'Post flags',
+            },
+        ),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/core/urls.py` & `Boorunaut-0.5.0/booru/core/urls.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from django.urls import path
-
-from . import views
-
-app_name = "core"
-
-urlpatterns = [
-    path('terms_of_service/', views.TermsOfServiceView.as_view(), name="terms_of_service"),
-    path('privacy_policy/', views.PrivacyPolicyView.as_view(), name="privacy_policy"),
-    path('staff_page/hash_ban/', views.BannedHashCreateView.as_view(), name="hash_ban"),
-    path('staff_page/hash_ban/<int:pk>/delete', views.BannedHashDeleteView.as_view(), name="hash_ban_delete"),
-    path('staff_page/mod_queue/', views.ModQueueView.as_view(), name="mod_queue"),
-    path('staff_page/mod_queue/<int:pk>/resolve', views.StaffPostFlagResolveView.as_view(), name="mod_queue_resolve"),
-]
+from django.urls import path
+
+from . import views
+
+app_name = "core"
+
+urlpatterns = [
+    path('terms_of_service/', views.TermsOfServiceView.as_view(), name="terms_of_service"),
+    path('privacy_policy/', views.PrivacyPolicyView.as_view(), name="privacy_policy"),
+    path('staff_page/hash_ban/', views.BannedHashCreateView.as_view(), name="hash_ban"),
+    path('staff_page/hash_ban/<int:pk>/delete', views.BannedHashDeleteView.as_view(), name="hash_ban_delete"),
+    path('staff_page/mod_queue/', views.ModQueueView.as_view(), name="mod_queue"),
+    path('staff_page/mod_queue/<int:pk>/resolve', views.StaffPostFlagResolveView.as_view(), name="mod_queue_resolve"),
+]
```

### Comparing `Boorunaut-0.4.3/booru/core/views.py` & `Boorunaut-0.5.0/booru/core/views.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-from django.shortcuts import get_object_or_404, redirect
-from django.utils.decorators import method_decorator
-from django.views.decorators.csrf import csrf_protect
-from django.views.generic import CreateView, RedirectView, TemplateView
-from rolepermissions.checkers import has_permission
-
-from booru.account.decorators import user_is_not_blocked
-from booru.core.forms import BannedHashCreateForm, PostFlagCreateForm
-from booru.core.models import BannedHash, PostFlag
-from booru.models import Comment, Configuration, Implication, Post
-
-
-class TermsOfServiceView(TemplateView):
-    template_name = "booru/core/terms_of_service.html"
-
-    def get_context_data(self, **kwargs):
-        context = super(TermsOfServiceView, self).get_context_data(**kwargs)
-        context['terms_of_service'] = Configuration.objects.filter(code_name="terms_of_service").first().value
-        return context
-
-class PrivacyPolicyView(TemplateView):
-    template_name = "booru/core/privacy_policy.html"
-
-    def get_context_data(self, **kwargs):
-        context = super(PrivacyPolicyView, self).get_context_data(**kwargs)
-        context['privacy_policy'] = Configuration.objects.filter(code_name="privacy_policy").first().value
-        return context
-
-
-class BannedHashCreateView(CreateView):
-    """
-    Provides a form for staff members to configure their booru.
-    """
-    success_url = '.'
-    form_class = BannedHashCreateForm
-    template_name = "booru/staff_hash_ban.html"
-
-    def form_valid(self, form):
-        form.instance.creator = self.request.user
-        form.save()
-        return super().form_valid(form)
-
-    @method_decorator(csrf_protect)
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated or not has_permission(request.user,'booru.ban_hashes'):
-            return redirect('account:login')
-        return super().dispatch(request, *args, **kwargs)
-
-    def get_context_data(self, **kwargs):
-        context = super(BannedHashCreateView, self).get_context_data(**kwargs)
-        context['banned_hashes'] = BannedHash.objects.all()
-        return context
-
-class BannedHashDeleteView(RedirectView):
-
-    permanent = False
-    query_string = False
-    pattern_name = 'core:hash_ban'
-
-    @method_decorator(csrf_protect)
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated or not has_permission(request.user,'booru.ban_hashes'):
-            return redirect('account:login')
-        return super().dispatch(request, *args, **kwargs)
-
-    def get_redirect_url(self, *args, **kwargs):
-        banned_hash = get_object_or_404(BannedHash.objects.all(), id=kwargs['pk'])
-        banned_hash.delete()
-        kwargs.pop('pk', None)
-        return super().get_redirect_url(*args, **kwargs)
-
-class ModQueueView(TemplateView):
-    template_name = "booru/staff_mod_queue.html"
-
-    def get_context_data(self, **kwargs):
-        context = super(ModQueueView, self).get_context_data(**kwargs)
-        context['pending_posts'] = Post.objects.not_deleted().filter(status=Post.PENDING)
-        context['pending_implications'] = Implication.objects.filter(status=Implication.PENDING)
-        context['post_flags'] = PostFlag.objects.filter(status=PostFlag.PENDING)
-        return context
-
-class PostFlagCreateView(CreateView):
-    """
-    Provides a form for users to flag posts for deletion.
-    """
-    success_url = '.'
-    form_class = PostFlagCreateForm
-    template_name = "booru/post_flag.html"
-
-    def form_valid(self, form):
-        form.instance.creator = self.request.user
-        form.instance.post = Post.objects.get(id=self.kwargs['post_id'])
-        form.save()
-        return super().form_valid(form)
-
-    @method_decorator(csrf_protect)
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated:
-            return redirect('account:login')
-        return super().dispatch(request, *args, **kwargs)
-    
-    def get_context_data(self, **kwargs):
-        context = super(PostFlagCreateView, self).get_context_data(**kwargs)
-        context['post'] = Post.objects.get(id=self.kwargs['post_id'])
-        return context
-
-class StaffPostFlagResolveView(RedirectView):
-
-    permanent = False
-    query_string = False
-    pattern_name = 'core:mod_queue'
-
-    def get(self, request, *args, **kwargs):
-        flag = get_object_or_404(PostFlag, id=kwargs['pk'])
-        flag.status = PostFlag.RESOLVED
-        flag.save()
-        return super(StaffPostFlagResolveView, self).get(request, *args, **kwargs)
-
-    @method_decorator(csrf_protect)
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated or not has_permission(request.user,'booru.change_status'):
-            return redirect('account:login')
-        return super().dispatch(request, *args, **kwargs)
-
-    def get_redirect_url(self, *args, **kwargs):
-        kwargs.pop('pk', None)
-        return super().get_redirect_url(*args, **kwargs)
-
-class StaffCommentToggleHiddenView(RedirectView):
-
-    permanent = False
-    query_string = False
-    pattern_name = 'booru:post_detail'
-
-    def get(self, request, *args, **kwargs):
-        comment = get_object_or_404(Comment, id=kwargs['pk'])
-        comment.is_hidden = not comment.is_hidden
-        comment.save()
-        return super(StaffCommentToggleHiddenView, self).get(request, *args, **kwargs)
-
-    @method_decorator(csrf_protect)
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated or not has_permission(request.user,'booru.manage_comments'):
-            return redirect('account:login')
-        return super().dispatch(request, *args, **kwargs)
-
-    def get_redirect_url(self, *args, **kwargs):
-        comment = get_object_or_404(Comment, id=kwargs['pk'])
-        kwargs['post_id'] = comment.object_id
-        kwargs.pop('pk')
-        return super().get_redirect_url(*args, **kwargs)
+from django.shortcuts import get_object_or_404, redirect
+from django.utils.decorators import method_decorator
+from django.views.decorators.csrf import csrf_protect
+from django.views.generic import CreateView, RedirectView, TemplateView
+from rolepermissions.checkers import has_permission
+
+from booru.account.decorators import user_is_not_blocked
+from booru.core.forms import BannedHashCreateForm, PostFlagCreateForm
+from booru.core.models import BannedHash, PostFlag
+from booru.models import Comment, Configuration, Implication, Post
+
+
+class TermsOfServiceView(TemplateView):
+    template_name = "booru/core/terms_of_service.html"
+
+    def get_context_data(self, **kwargs):
+        context = super(TermsOfServiceView, self).get_context_data(**kwargs)
+        context['terms_of_service'] = Configuration.objects.filter(code_name="terms_of_service").first().value
+        return context
+
+class PrivacyPolicyView(TemplateView):
+    template_name = "booru/core/privacy_policy.html"
+
+    def get_context_data(self, **kwargs):
+        context = super(PrivacyPolicyView, self).get_context_data(**kwargs)
+        context['privacy_policy'] = Configuration.objects.filter(code_name="privacy_policy").first().value
+        return context
+
+
+class BannedHashCreateView(CreateView):
+    """
+    Provides a form for staff members to configure their booru.
+    """
+    success_url = '.'
+    form_class = BannedHashCreateForm
+    template_name = "booru/staff_hash_ban.html"
+
+    def form_valid(self, form):
+        form.instance.creator = self.request.user
+        form.save()
+        return super().form_valid(form)
+
+    @method_decorator(csrf_protect)
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated or not has_permission(request.user,'booru.ban_hashes'):
+            return redirect('account:login')
+        return super().dispatch(request, *args, **kwargs)
+
+    def get_context_data(self, **kwargs):
+        context = super(BannedHashCreateView, self).get_context_data(**kwargs)
+        context['banned_hashes'] = BannedHash.objects.all()
+        return context
+
+class BannedHashDeleteView(RedirectView):
+
+    permanent = False
+    query_string = False
+    pattern_name = 'core:hash_ban'
+
+    @method_decorator(csrf_protect)
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated or not has_permission(request.user,'booru.ban_hashes'):
+            return redirect('account:login')
+        return super().dispatch(request, *args, **kwargs)
+
+    def get_redirect_url(self, *args, **kwargs):
+        banned_hash = get_object_or_404(BannedHash.objects.all(), id=kwargs['pk'])
+        banned_hash.delete()
+        kwargs.pop('pk', None)
+        return super().get_redirect_url(*args, **kwargs)
+
+class ModQueueView(TemplateView):
+    template_name = "booru/staff_mod_queue.html"
+
+    def get_context_data(self, **kwargs):
+        context = super(ModQueueView, self).get_context_data(**kwargs)
+        context['pending_posts'] = Post.objects.not_deleted().filter(status=Post.PENDING)
+        context['pending_implications'] = Implication.objects.filter(status=Implication.PENDING)
+        context['post_flags'] = PostFlag.objects.filter(status=PostFlag.PENDING)
+        return context
+
+class PostFlagCreateView(CreateView):
+    """
+    Provides a form for users to flag posts for deletion.
+    """
+    success_url = '.'
+    form_class = PostFlagCreateForm
+    template_name = "booru/post_flag.html"
+
+    def form_valid(self, form):
+        form.instance.creator = self.request.user
+        form.instance.post = Post.objects.get(id=self.kwargs['post_id'])
+        form.save()
+        return super().form_valid(form)
+
+    @method_decorator(csrf_protect)
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated:
+            return redirect('account:login')
+        return super().dispatch(request, *args, **kwargs)
+    
+    def get_context_data(self, **kwargs):
+        context = super(PostFlagCreateView, self).get_context_data(**kwargs)
+        context['post'] = Post.objects.get(id=self.kwargs['post_id'])
+        return context
+
+class StaffPostFlagResolveView(RedirectView):
+
+    permanent = False
+    query_string = False
+    pattern_name = 'core:mod_queue'
+
+    def get(self, request, *args, **kwargs):
+        flag = get_object_or_404(PostFlag, id=kwargs['pk'])
+        flag.status = PostFlag.RESOLVED
+        flag.save()
+        return super(StaffPostFlagResolveView, self).get(request, *args, **kwargs)
+
+    @method_decorator(csrf_protect)
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated or not has_permission(request.user,'booru.change_status'):
+            return redirect('account:login')
+        return super().dispatch(request, *args, **kwargs)
+
+    def get_redirect_url(self, *args, **kwargs):
+        kwargs.pop('pk', None)
+        return super().get_redirect_url(*args, **kwargs)
+
+class StaffCommentToggleHiddenView(RedirectView):
+
+    permanent = False
+    query_string = False
+    pattern_name = 'booru:post_detail'
+
+    def get(self, request, *args, **kwargs):
+        comment = get_object_or_404(Comment, id=kwargs['pk'])
+        comment.is_hidden = not comment.is_hidden
+        comment.save()
+        return super(StaffCommentToggleHiddenView, self).get(request, *args, **kwargs)
+
+    @method_decorator(csrf_protect)
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated or not has_permission(request.user,'booru.manage_comments'):
+            return redirect('account:login')
+        return super().dispatch(request, *args, **kwargs)
+
+    def get_redirect_url(self, *args, **kwargs):
+        comment = get_object_or_404(Comment, id=kwargs['pk'])
+        kwargs['post_id'] = comment.object_id
+        kwargs.pop('pk')
+        return super().get_redirect_url(*args, **kwargs)
```

### Comparing `Boorunaut-0.4.3/booru/forms.py` & `Boorunaut-0.5.0/booru/forms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,284 +1,283 @@
-from django import forms
-from django.conf import settings
-from django.contrib.admin.widgets import AdminTextareaWidget
-from django.core.exceptions import ValidationError
-from django.core.validators import URLValidator
-from django.utils import six
-from taggit.forms import TagField, TagWidget
-from taggit.utils import edit_string_for_tags
-
-from booru import utils
-from booru.account.forms import UsernameExistsField
-from booru.account.models import Timeout
-from booru.core.models import BannedHash
-from booru.models import Category, Gallery, Implication, Post, PostTag
-
-
-def validate_sources(source):
-    sources = source.splitlines()
-
-    val = URLValidator()
-    for index, source in enumerate(sources):
-        if '://' not in source:
-            source = 'http://' + source
-            sources[index] = source
-        try:
-            val(source)
-        except ValidationError as e:
-            return None
-    sources = "\n".join(sources)
-    return sources
-
-class CreatePostForm(forms.ModelForm):
-    '''Form for creating an post.'''
-
-    media = forms.FileField(required=False)
-    media_url = forms.URLField(required=False)
-    sample = forms.ImageField(required=False)
-    preview = forms.ImageField(required=False)
-    tags = TagField(required=True, help_text="Required: Choose one or more tags.")
-    source = forms.CharField(required=False)
-    rating = forms.IntegerField()
-
-    class Meta:
-        model = Post
-        fields = ["media", "media_url", "sample", "preview", "tags", "rating", "source", "description"]
-
-    def __init__(self, *args, **kwargs):
-        super(CreatePostForm, self).__init__(*args, **kwargs)
-        self.fields['media'].widget = forms.FileInput(attrs={'class': 'custom-file-input'})
-        self.fields['media_url'].widget = forms.URLInput(attrs={'class': 'form-control'})
-        self.fields['media_url'].required = False
-        self.fields['source'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['rating'].widget = forms.Select(attrs={'class': 'form-control'},
-                                                    choices=Post.RATING_CHOICES)
-        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['tags'].widget = forms.TextInput(attrs={'class': 'form-control'})
-
-    def clean( self ):
-        cleaned_data = self.cleaned_data
-        media_file = cleaned_data.get('media')
-        media_url = cleaned_data.get('media_url')
-        detected_media = None
-
-        if media_file is None and not media_url:
-            raise forms.ValidationError("Please select an image or video.")
-        elif media_file is not None and media_url:
-            raise forms.ValidationError("Please only upload one image or video.")
-        elif media_file is not None:
-            detected_media = media_file
-        elif media_url:
-            detected_media = utils.get_remote_image_as_InMemoryUploadedFile(media_url)
-        if not utils.get_pil_image_if_valid(detected_media):
-            if not utils.check_video_is_valid(detected_media):
-                raise forms.ValidationError("Please upload a valid image or video.")
-
-        if detected_media.size >= settings.BOORUNAUT_MAX_SIZE_FILE:
-            max_size_mb = settings.BOORUNAUT_MAX_SIZE_FILE / 1024 / 1024
-            raise forms.ValidationError("Please upload a file with less than {} MB.".format(max_size_mb))
-
-        md5_checksum = utils.get_file_md5(detected_media)
-
-        if BannedHash.objects.filter(content=md5_checksum).exists():
-            raise forms.ValidationError("This file is not allowed to be uploaded. Contact the staff.")
-        
-        self.cleaned_data['media'] = detected_media
-        return cleaned_data
-
-    def clean_source(self):
-        source = self.cleaned_data['source']
-        if source:
-            source = validate_sources(self.cleaned_data['source'])
-            if not source:
-                raise forms.ValidationError("Please use valid URLs.")
-        return source
-
-class EditPostForm(forms.ModelForm):
-    '''Form for editing an post.'''
-    rating = forms.IntegerField()
-    parent = forms.IntegerField(required=False)
-    source = forms.CharField(required=False)
-    tags = TagField(required=False)
-
-    class Meta:
-        model = Post
-        fields = ["rating", "parent", "source", "tags", "description"]
-    
-    def clean_source(self):
-        source = self.cleaned_data['source']
-        if source:
-            source = validate_sources(self.cleaned_data['source'])
-            if not source:
-                raise forms.ValidationError("Please use valid URLs.")
-        return source
-
-    def __init__(self, *args, **kwargs):
-        super(EditPostForm, self).__init__(*args, **kwargs)
-        self.fields['rating'].widget = forms.Select(attrs={'class': 'form-control'},
-                                                    choices=Post.RATING_CHOICES)
-        self.fields['parent'].widget = forms.NumberInput(attrs={'class': 'form-control'})
-        self.fields['source'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows':4, 'cols':15})
-        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows':4, 'cols':15})
-
-class TagListSearchForm(forms.Form):
-    '''Form for creating an post.'''
-
-    tags = forms.CharField(required=False)
-    category = forms.ModelChoiceField(queryset=Category.objects.all(),
-                                    widget=forms.Select(attrs={'class': 'form-control form-control-sm'}),
-                                    required=False, empty_label=None)
-
-    class Meta:
-        fields = "__all__"
-
-    def __init__(self, *args, **kwargs):
-        super(TagListSearchForm, self).__init__(*args, **kwargs)
-        self.fields['tags'].widget = forms.TextInput(attrs={'class': 'form-control form-control-sm'})
-
-class TagEditForm(forms.ModelForm):
-    '''Form for creating an post.'''
-
-    category = forms.ModelChoiceField(queryset=Category.objects.all(),
-                                      widget=forms.Select(attrs={'class': 'form-control'}),
-                                      required=False, empty_label=None)
-    associated_user_name = forms.CharField(required=False)
-    aliases = TagField(required=False, help_text="Separate the aliases with spaces. They are used to find tags easier on the search bar.")
-
-    def __init__(self, *args, **kwargs):
-        super(TagEditForm, self).__init__(*args, **kwargs)
-        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['associated_link'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['associated_user_name'].widget = forms.Textarea(attrs={'class': 'form-control'})
-
-    class Meta:
-        model = PostTag
-        fields = ["category", "description", "associated_link", "associated_user_name", "aliases"]
-
-class ImplicationCreateForm(forms.Form):
-    from_tag = forms.CharField(required=True)
-    to_tag = forms.CharField(required=True)
-
-    class Meta:
-        fields = "__all__"
-
-    def __init__(self, *args, **kwargs):
-        super(ImplicationCreateForm, self).__init__(*args, **kwargs)
-        self.fields['from_tag'].widget = forms.TextInput(attrs={'class': 'form-control tag-search'})
-        self.fields['to_tag'].widget = forms.TextInput(attrs={'class': 'form-control tag-search'})
-    
-    def clean_from_tag(self):
-        from_tag = self.cleaned_data['from_tag']
-        return from_tag.lower()
-    
-    def clean_to_tag(self):
-        to_tag = self.cleaned_data['to_tag']
-        return to_tag.lower()
-
-class ImplicationFilterForm(forms.Form):
-    name = forms.CharField(required=False)
-    status = forms.ChoiceField(required=False, choices=(('', '-----'),) + Implication.STATUS_CHOICES)
-
-    class Meta:
-        fields = "__all__"
-
-    def __init__(self, *args, **kwargs):
-        super(ImplicationFilterForm, self).__init__(*args, **kwargs)
-
-class MassRenameForm(forms.Form):
-    filter_by = forms.CharField(required=False)
-    when = forms.CharField(required=True)
-    replace_with = forms.CharField(required=True)
-
-    class Meta:
-        fields = "__all__"
-
-    def __init__(self, *args, **kwargs):
-        super(MassRenameForm, self).__init__(*args, **kwargs)
-        self.fields['filter_by'].widget = forms.TextInput(attrs={'class': 'form-control'})
-        self.fields['when'].widget = forms.TextInput(attrs={'class': 'form-control'})
-        self.fields['replace_with'].widget = forms.TextInput(attrs={'class': 'form-control'})
-
-class BanUserForm(forms.ModelForm):
-    username = UsernameExistsField(
-        max_length=254,
-        widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control'}),
-    )
-
-    expiration = forms.DateTimeField(required=True, input_formats=['%m/%d/%Y'])
-    reason = forms.CharField(required=True)
-
-    class Meta:
-        model = Timeout
-        fields = ["username", "expiration", "reason"]
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.fields['username'].widget = forms.TextInput(attrs={'class': 'form-control', 'autofocus': True})
-        self.fields['expiration'].widget = forms.TextInput(attrs={'class': 'form-control', 'placeholder' : 'month/day/year'})
-        self.fields['reason'].widget = forms.TextInput(attrs={'class': 'form-control'})
-
-class GalleryCreateForm(forms.ModelForm):
-    '''Form for creating an gallery.'''
-
-    name = forms.CharField(required=True)
-    description = forms.CharField(required=False)
-    posts_ids = forms.CharField(required=False)
-
-    class Meta:
-        model = Gallery
-        fields = ["name", "description"]
-
-    def __init__(self, *args, **kwargs):
-        super(GalleryCreateForm, self).__init__(*args, **kwargs)
-        self.fields['name'].widget = forms.TextInput(attrs={'class': 'form-control'})
-        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['posts_ids'].widget = forms.Textarea(attrs={'class': 'form-control'})
-
-class GalleryEditForm(forms.ModelForm):
-    '''Form for creating an gallery.'''
-
-    name = forms.CharField(required=True)
-    description = forms.CharField(required=True)
-    posts_ids = forms.CharField(required=True)
-
-    class Meta:
-        model = Gallery
-        fields = ["name", "description"]
-
-    def __init__(self, *args, **kwargs):
-        super(GalleryEditForm, self).__init__(*args, **kwargs)
-        self.fields['name'].widget = forms.TextInput(attrs={'class': 'form-control'})
-        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['posts_ids'].widget = forms.Textarea(attrs={'class': 'form-control'})
-
-class GalleryListSearchForm(forms.Form):
-    '''Form searching galleries in the Gallery List.'''
-
-    name = forms.CharField(required=False)    
-
-    class Meta:
-        fields = "__all__"
-
-    def __init__(self, *args, **kwargs):
-        super(GalleryListSearchForm, self).__init__(*args, **kwargs)
-        self.fields['name'].widget = forms.TextInput(attrs={'class': 'form-control form-control-sm'})
-
-class SiteConfigurationForm(forms.Form):
-    site_title = forms.CharField(required=True, help_text="The name of the website to be shown.")
-    site_description = forms.CharField(required=False, help_text="The description of the website for search engines.")
-    welcome_page = forms.BooleanField(required=False)
-    terms_of_service = forms.CharField(required=False)
-    privacy_policy = forms.CharField(required=False)
-    announcement = forms.CharField(required=False, help_text="The contents here will be shown on the top of the website for all users. Markdown is enabled.")
-
-    class Meta:
-        fields = "__all__"
-
-    def __init__(self, *args, **kwargs):
-        super(SiteConfigurationForm, self).__init__(*args, **kwargs)
-        self.fields['site_title'].widget = forms.TextInput(attrs={'class': 'form-control'})
-        self.fields['site_description'].widget = forms.TextInput(attrs={'class': 'form-control'})
-        self.fields['welcome_page'].widget = forms.CheckboxInput(attrs={'class': 'form-control', 'data-toggle': 'toggle'})
-        self.fields['terms_of_service'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['privacy_policy'].widget = forms.Textarea(attrs={'class': 'form-control'})
-        self.fields['announcement'].widget = forms.Textarea(attrs={'class': 'form-control'})
+from django import forms
+from django.conf import settings
+from django.contrib.admin.widgets import AdminTextareaWidget
+from django.core.exceptions import ValidationError
+from django.core.validators import URLValidator
+from taggit.forms import TagField, TagWidget
+from taggit.utils import edit_string_for_tags
+
+from booru import utils
+from booru.account.forms import UsernameExistsField
+from booru.account.models import Timeout
+from booru.core.models import BannedHash
+from booru.models import Category, Gallery, Implication, Post, PostTag
+
+
+def validate_sources(source):
+    sources = source.splitlines()
+
+    val = URLValidator()
+    for index, source in enumerate(sources):
+        if '://' not in source:
+            source = 'http://' + source
+            sources[index] = source
+        try:
+            val(source)
+        except ValidationError as e:
+            return None
+    sources = "\n".join(sources)
+    return sources
+
+class CreatePostForm(forms.ModelForm):
+    '''Form for creating an post.'''
+
+    media = forms.FileField(required=False)
+    media_url = forms.URLField(required=False)
+    sample = forms.ImageField(required=False)
+    preview = forms.ImageField(required=False)
+    tags = TagField(required=True, help_text="Required: Choose one or more tags.")
+    source = forms.CharField(required=False)
+    rating = forms.IntegerField()
+
+    class Meta:
+        model = Post
+        fields = ["media", "media_url", "sample", "preview", "tags", "rating", "source", "description"]
+
+    def __init__(self, *args, **kwargs):
+        super(CreatePostForm, self).__init__(*args, **kwargs)
+        self.fields['media'].widget = forms.FileInput(attrs={'class': 'custom-file-input'})
+        self.fields['media_url'].widget = forms.URLInput(attrs={'class': 'form-control'})
+        self.fields['media_url'].required = False
+        self.fields['source'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['rating'].widget = forms.Select(attrs={'class': 'form-control'},
+                                                    choices=Post.RATING_CHOICES)
+        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['tags'].widget = forms.TextInput(attrs={'class': 'form-control'})
+
+    def clean( self ):
+        cleaned_data = self.cleaned_data
+        media_file = cleaned_data.get('media')
+        media_url = cleaned_data.get('media_url')
+        detected_media = None
+
+        if media_file is None and not media_url:
+            raise forms.ValidationError("Please select an image or video.")
+        elif media_file is not None and media_url:
+            raise forms.ValidationError("Please only upload one image or video.")
+        elif media_file is not None:
+            detected_media = media_file
+        elif media_url:
+            detected_media = utils.get_remote_image_as_InMemoryUploadedFile(media_url)
+        if not utils.get_pil_image_if_valid(detected_media):
+            if not utils.check_video_is_valid(detected_media):
+                raise forms.ValidationError("Please upload a valid image or video.")
+
+        if detected_media.size >= settings.BOORUNAUT_MAX_SIZE_FILE:
+            max_size_mb = settings.BOORUNAUT_MAX_SIZE_FILE / 1024 / 1024
+            raise forms.ValidationError("Please upload a file with less than {} MB.".format(max_size_mb))
+
+        md5_checksum = utils.get_file_md5(detected_media)
+
+        if BannedHash.objects.filter(content=md5_checksum).exists():
+            raise forms.ValidationError("This file is not allowed to be uploaded. Contact the staff.")
+        
+        self.cleaned_data['media'] = detected_media
+        return cleaned_data
+
+    def clean_source(self):
+        source = self.cleaned_data['source']
+        if source:
+            source = validate_sources(self.cleaned_data['source'])
+            if not source:
+                raise forms.ValidationError("Please use valid URLs.")
+        return source
+
+class EditPostForm(forms.ModelForm):
+    '''Form for editing an post.'''
+    rating = forms.IntegerField()
+    parent = forms.IntegerField(required=False)
+    source = forms.CharField(required=False)
+    tags = TagField(required=False)
+
+    class Meta:
+        model = Post
+        fields = ["rating", "parent", "source", "tags", "description"]
+    
+    def clean_source(self):
+        source = self.cleaned_data['source']
+        if source:
+            source = validate_sources(self.cleaned_data['source'])
+            if not source:
+                raise forms.ValidationError("Please use valid URLs.")
+        return source
+
+    def __init__(self, *args, **kwargs):
+        super(EditPostForm, self).__init__(*args, **kwargs)
+        self.fields['rating'].widget = forms.Select(attrs={'class': 'form-control'},
+                                                    choices=Post.RATING_CHOICES)
+        self.fields['parent'].widget = forms.NumberInput(attrs={'class': 'form-control'})
+        self.fields['source'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows':4, 'cols':15})
+        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control', 'rows':4, 'cols':15})
+
+class TagListSearchForm(forms.Form):
+    '''Form for creating an post.'''
+
+    tags = forms.CharField(required=False)
+    category = forms.ModelChoiceField(queryset=Category.objects.all(),
+                                    widget=forms.Select(attrs={'class': 'form-control form-control-sm'}),
+                                    required=False, empty_label=None)
+
+    class Meta:
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super(TagListSearchForm, self).__init__(*args, **kwargs)
+        self.fields['tags'].widget = forms.TextInput(attrs={'class': 'form-control form-control-sm'})
+
+class TagEditForm(forms.ModelForm):
+    '''Form for creating an post.'''
+
+    category = forms.ModelChoiceField(queryset=Category.objects.all(),
+                                      widget=forms.Select(attrs={'class': 'form-control'}),
+                                      required=False, empty_label=None)
+    associated_user_name = forms.CharField(required=False)
+    aliases = TagField(required=False, help_text="Separate the aliases with spaces. They are used to find tags easier on the search bar.")
+
+    def __init__(self, *args, **kwargs):
+        super(TagEditForm, self).__init__(*args, **kwargs)
+        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['associated_link'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['associated_user_name'].widget = forms.Textarea(attrs={'class': 'form-control'})
+
+    class Meta:
+        model = PostTag
+        fields = ["category", "description", "associated_link", "associated_user_name", "aliases"]
+
+class ImplicationCreateForm(forms.Form):
+    from_tag = forms.CharField(required=True)
+    to_tag = forms.CharField(required=True)
+
+    class Meta:
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super(ImplicationCreateForm, self).__init__(*args, **kwargs)
+        self.fields['from_tag'].widget = forms.TextInput(attrs={'class': 'form-control tag-search'})
+        self.fields['to_tag'].widget = forms.TextInput(attrs={'class': 'form-control tag-search'})
+    
+    def clean_from_tag(self):
+        from_tag = self.cleaned_data['from_tag']
+        return from_tag.lower()
+    
+    def clean_to_tag(self):
+        to_tag = self.cleaned_data['to_tag']
+        return to_tag.lower()
+
+class ImplicationFilterForm(forms.Form):
+    name = forms.CharField(required=False)
+    status = forms.ChoiceField(required=False, choices=(('', '-----'),) + Implication.STATUS_CHOICES)
+
+    class Meta:
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super(ImplicationFilterForm, self).__init__(*args, **kwargs)
+
+class MassRenameForm(forms.Form):
+    filter_by = forms.CharField(required=False)
+    when = forms.CharField(required=True)
+    replace_with = forms.CharField(required=True)
+
+    class Meta:
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super(MassRenameForm, self).__init__(*args, **kwargs)
+        self.fields['filter_by'].widget = forms.TextInput(attrs={'class': 'form-control'})
+        self.fields['when'].widget = forms.TextInput(attrs={'class': 'form-control'})
+        self.fields['replace_with'].widget = forms.TextInput(attrs={'class': 'form-control'})
+
+class BanUserForm(forms.ModelForm):
+    username = UsernameExistsField(
+        max_length=254,
+        widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control'}),
+    )
+
+    expiration = forms.DateTimeField(required=True, input_formats=['%m/%d/%Y'])
+    reason = forms.CharField(required=True)
+
+    class Meta:
+        model = Timeout
+        fields = ["username", "expiration", "reason"]
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.fields['username'].widget = forms.TextInput(attrs={'class': 'form-control', 'autofocus': True})
+        self.fields['expiration'].widget = forms.TextInput(attrs={'class': 'form-control', 'placeholder' : 'month/day/year'})
+        self.fields['reason'].widget = forms.TextInput(attrs={'class': 'form-control'})
+
+class GalleryCreateForm(forms.ModelForm):
+    '''Form for creating an gallery.'''
+
+    name = forms.CharField(required=True)
+    description = forms.CharField(required=False)
+    posts_ids = forms.CharField(required=False)
+
+    class Meta:
+        model = Gallery
+        fields = ["name", "description"]
+
+    def __init__(self, *args, **kwargs):
+        super(GalleryCreateForm, self).__init__(*args, **kwargs)
+        self.fields['name'].widget = forms.TextInput(attrs={'class': 'form-control'})
+        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['posts_ids'].widget = forms.Textarea(attrs={'class': 'form-control'})
+
+class GalleryEditForm(forms.ModelForm):
+    '''Form for creating an gallery.'''
+
+    name = forms.CharField(required=True)
+    description = forms.CharField(required=True)
+    posts_ids = forms.CharField(required=True)
+
+    class Meta:
+        model = Gallery
+        fields = ["name", "description"]
+
+    def __init__(self, *args, **kwargs):
+        super(GalleryEditForm, self).__init__(*args, **kwargs)
+        self.fields['name'].widget = forms.TextInput(attrs={'class': 'form-control'})
+        self.fields['description'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['posts_ids'].widget = forms.Textarea(attrs={'class': 'form-control'})
+
+class GalleryListSearchForm(forms.Form):
+    '''Form searching galleries in the Gallery List.'''
+
+    name = forms.CharField(required=False)    
+
+    class Meta:
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super(GalleryListSearchForm, self).__init__(*args, **kwargs)
+        self.fields['name'].widget = forms.TextInput(attrs={'class': 'form-control form-control-sm'})
+
+class SiteConfigurationForm(forms.Form):
+    site_title = forms.CharField(required=True, help_text="The name of the website to be shown.")
+    site_description = forms.CharField(required=False, help_text="The description of the website for search engines.")
+    welcome_page = forms.BooleanField(required=False)
+    terms_of_service = forms.CharField(required=False)
+    privacy_policy = forms.CharField(required=False)
+    announcement = forms.CharField(required=False, help_text="The contents here will be shown on the top of the website for all users. Markdown is enabled.")
+
+    class Meta:
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super(SiteConfigurationForm, self).__init__(*args, **kwargs)
+        self.fields['site_title'].widget = forms.TextInput(attrs={'class': 'form-control'})
+        self.fields['site_description'].widget = forms.TextInput(attrs={'class': 'form-control'})
+        self.fields['welcome_page'].widget = forms.CheckboxInput(attrs={'class': 'form-control', 'data-toggle': 'toggle'})
+        self.fields['terms_of_service'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['privacy_policy'].widget = forms.Textarea(attrs={'class': 'form-control'})
+        self.fields['announcement'].widget = forms.Textarea(attrs={'class': 'form-control'})
```

### Comparing `Boorunaut-0.4.3/booru/managers.py` & `Boorunaut-0.5.0/booru/managers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# -*- coding: utf-8 -*-
-from django.contrib.auth.models import AbstractUser
-from django.contrib.auth.models import UserManager as AbstractUserManager
-from django.db import models
-from django.db.models import Q
-
-
-class PostQueryset(models.query.QuerySet):
-    def pending(self):
-        return self.filter(status=0)
-
-    def approved(self):
-        return self.filter(status=1)
-
-    def deleted(self):
-        return self.filter(status=2)
-
-    def not_deleted(self):
-        return self.filter(~Q(status=2))
-
-class PostManager(models.Manager):
-    '''Custom manager for Posts.'''
-    def get_queryset(self):
-        return PostQueryset(self.model, using=self._db)
-
-    def pending(self):
-        '''Returns a QuerySet with only Posts that are pending.'''
-        return self.get_queryset().pending()
-
-    def approved(self):
-        '''Returns a QuerySet with only Posts that are approved.'''
-        return self.get_queryset().approved()
-
-    def deleted(self):
-        '''Returns a QuerySet with only Posts that are deleted.'''
-        return self.get_queryset().deleted()
-
-    def not_deleted(self):
-        '''Returns a QuerySet with only Posts that aren't deleted (pending or approved).'''
-        return self.get_queryset().not_deleted()
-
-class UserQueryset(models.query.QuerySet):
-    def active(self):
-        return self.exclude(is_deleted=True)
-
-class UserManager(AbstractUserManager):
-    '''Custom manager for User.'''
-    def get_queryset(self):
-        return UserQueryset(self.model, using=self._db)
-
-    def active(self):
-        '''Returns a QuerySet with only Users that are active.'''
-        return self.get_queryset().active()
+# -*- coding: utf-8 -*-
+from django.contrib.auth.models import AbstractUser
+from django.contrib.auth.models import UserManager as AbstractUserManager
+from django.db import models
+from django.db.models import Q
+
+
+class PostQueryset(models.query.QuerySet):
+    def pending(self):
+        return self.filter(status=0)
+
+    def approved(self):
+        return self.filter(status=1)
+
+    def deleted(self):
+        return self.filter(status=2)
+
+    def not_deleted(self):
+        return self.filter(~Q(status=2))
+
+class PostManager(models.Manager):
+    '''Custom manager for Posts.'''
+    def get_queryset(self):
+        return PostQueryset(self.model, using=self._db)
+
+    def pending(self):
+        '''Returns a QuerySet with only Posts that are pending.'''
+        return self.get_queryset().pending()
+
+    def approved(self):
+        '''Returns a QuerySet with only Posts that are approved.'''
+        return self.get_queryset().approved()
+
+    def deleted(self):
+        '''Returns a QuerySet with only Posts that are deleted.'''
+        return self.get_queryset().deleted()
+
+    def not_deleted(self):
+        '''Returns a QuerySet with only Posts that aren't deleted (pending or approved).'''
+        return self.get_queryset().not_deleted()
+
+class UserQueryset(models.query.QuerySet):
+    def active(self):
+        return self.exclude(is_deleted=True)
+
+class UserManager(AbstractUserManager):
+    '''Custom manager for User.'''
+    def get_queryset(self):
+        return UserQueryset(self.model, using=self._db)
+
+    def active(self):
+        '''Returns a QuerySet with only Users that are active.'''
+        return self.get_queryset().active()
```

### Comparing `Boorunaut-0.4.3/booru/migrations/0001_initial.py` & `Boorunaut-0.5.0/booru/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-# Generated by Django 2.1.2 on 2018-11-13 21:21
-
-import booru.models
-from django.conf import settings
-from django.db import migrations, models
-import django.db.models.deletion
-import simple_history.models
-import taggit.managers
-import uuid
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('contenttypes', '0002_remove_content_type_name'),
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('taggit', '0002_auto_20150616_2121'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='Category',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('label', models.CharField(blank=True, max_length=100)),
-                ('title_singular', models.CharField(blank=True, max_length=100)),
-                ('title_plural', models.CharField(blank=True, max_length=100)),
-                ('color', models.CharField(blank=True, max_length=6)),
-            ],
-            options={
-                'verbose_name_plural': 'Categories',
-            },
-        ),
-        migrations.CreateModel(
-            name='Comment',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('content', models.CharField(blank=True, max_length=1000)),
-                ('timestamp', models.DateTimeField(auto_now_add=True)),
-                ('update_timestamp', models.DateTimeField(auto_now=True)),
-                ('object_id', models.PositiveIntegerField()),
-                ('author', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
-                ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='contenttypes.ContentType')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='CommentVote',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('point', models.IntegerField(default=1)),
-                ('account', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
-                ('comment', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='booru.Comment')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='Configuration',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('code_name', models.CharField(max_length=100)),
-                ('value', models.CharField(blank=True, max_length=1000)),
-            ],
-            options={
-                'permissions': (('change_configurations', 'Can change the configurations of the booru'),),
-            },
-        ),
-        migrations.CreateModel(
-            name='Favorite',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('account', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='account_favorites', to=settings.AUTH_USER_MODEL)),
-            ],
-        ),
-        migrations.CreateModel(
-            name='Gallery',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(blank=True, max_length=100)),
-                ('description', models.CharField(blank=True, max_length=1000)),
-                ('posts_mirror', models.CharField(blank=True, max_length=1000)),
-                ('is_active', models.BooleanField(default=True)),
-            ],
-            options={
-                'verbose_name_plural': 'Galleries',
-            },
-        ),
-        migrations.CreateModel(
-            name='HistoricalGallery',
-            fields=[
-                ('id', models.IntegerField(auto_created=True, blank=True, db_index=True, verbose_name='ID')),
-                ('name', models.CharField(blank=True, max_length=100)),
-                ('description', models.CharField(blank=True, max_length=1000)),
-                ('posts_mirror', models.CharField(blank=True, max_length=1000)),
-                ('is_active', models.BooleanField(default=True)),
-                ('history_id', models.AutoField(primary_key=True, serialize=False)),
-                ('history_change_reason', models.CharField(max_length=100, null=True)),
-                ('history_date', models.DateTimeField()),
-                ('history_type', models.CharField(choices=[('+', 'Created'), ('~', 'Changed'), ('-', 'Deleted')], max_length=1)),
-                ('history_user', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to=settings.AUTH_USER_MODEL)),
-            ],
-            options={
-                'verbose_name': 'historical gallery',
-                'ordering': ('-history_date', '-history_id'),
-                'get_latest_by': 'history_date',
-            },
-            bases=(simple_history.models.HistoricalChanges, models.Model),
-        ),
-        migrations.CreateModel(
-            name='HistoricalPost',
-            fields=[
-                ('id', models.IntegerField(auto_created=True, blank=True, db_index=True, verbose_name='ID')),
-                ('parent', models.IntegerField(blank=True, null=True)),
-                ('preview', models.TextField(blank=True, max_length=100)),
-                ('sample', models.TextField(blank=True, max_length=100)),
-                ('image', models.TextField(blank=True, max_length=100)),
-                ('timestamp', models.DateTimeField(blank=True, editable=False)),
-                ('update_timestamp', models.DateTimeField(blank=True, editable=False)),
-                ('source', models.TextField(blank=True)),
-                ('score', models.IntegerField(default=0)),
-                ('identifier', models.UUIDField(default=uuid.uuid4, editable=False)),
-                ('locked', models.BooleanField(default=False)),
-                ('tags_mirror', models.CharField(blank=True, max_length=1000)),
-                ('description', models.TextField(blank=True, max_length=1000)),
-                ('rating', models.IntegerField(choices=[(0, 'None'), (1, 'Safe'), (2, 'Questionable'), (3, 'Explicit')], default=0)),
-                ('status', models.IntegerField(choices=[(0, 'Pending'), (1, 'Approved'), (2, 'Hidden'), (3, 'Deleted')], default=0)),
-                ('history_id', models.AutoField(primary_key=True, serialize=False)),
-                ('history_change_reason', models.CharField(max_length=100, null=True)),
-                ('history_date', models.DateTimeField()),
-                ('history_type', models.CharField(choices=[('+', 'Created'), ('~', 'Changed'), ('-', 'Deleted')], max_length=1)),
-                ('history_user', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to=settings.AUTH_USER_MODEL)),
-                ('uploader', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to=settings.AUTH_USER_MODEL)),
-            ],
-            options={
-                'verbose_name': 'historical post',
-                'ordering': ('-history_date', '-history_id'),
-                'get_latest_by': 'history_date',
-            },
-            bases=(simple_history.models.HistoricalChanges, models.Model),
-        ),
-        migrations.CreateModel(
-            name='HistoricalPostTag',
-            fields=[
-                ('id', models.IntegerField(auto_created=True, blank=True, db_index=True, verbose_name='ID')),
-                ('name', models.CharField(db_index=True, max_length=100, verbose_name='Name')),
-                ('slug', models.SlugField(max_length=100, verbose_name='Slug')),
-                ('description', models.CharField(blank=True, max_length=100)),
-                ('associated_link', models.CharField(blank=True, max_length=100)),
-                ('timestamp', models.DateTimeField(blank=True, editable=False)),
-                ('history_id', models.AutoField(primary_key=True, serialize=False)),
-                ('history_change_reason', models.CharField(max_length=100, null=True)),
-                ('history_date', models.DateTimeField()),
-                ('history_type', models.CharField(choices=[('+', 'Created'), ('~', 'Changed'), ('-', 'Deleted')], max_length=1)),
-                ('associated_user', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to=settings.AUTH_USER_MODEL)),
-                ('author', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to=settings.AUTH_USER_MODEL)),
-                ('category', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to='booru.Category')),
-                ('history_user', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to=settings.AUTH_USER_MODEL)),
-            ],
-            options={
-                'verbose_name': 'historical Tag',
-                'ordering': ('-history_date', '-history_id'),
-                'get_latest_by': 'history_date',
-            },
-            bases=(simple_history.models.HistoricalChanges, models.Model),
-        ),
-        migrations.CreateModel(
-            name='Implication',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('timestamp', models.DateTimeField(auto_now_add=True)),
-                ('status', models.IntegerField(choices=[(0, 'Pending'), (1, 'Approved'), (2, 'Unapproved')], default=0)),
-                ('approver', models.ForeignKey(blank=True, default=None, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='approved_implications', to=settings.AUTH_USER_MODEL)),
-                ('author', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='authored_implications', to=settings.AUTH_USER_MODEL)),
-            ],
-        ),
-        migrations.CreateModel(
-            name='Post',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('parent', models.IntegerField(blank=True, null=True)),
-                ('preview', models.ImageField(blank=True, upload_to=booru.models.get_file_path_preview)),
-                ('sample', models.ImageField(blank=True, upload_to=booru.models.get_file_path_sample)),
-                ('image', models.ImageField(blank=True, upload_to=booru.models.get_file_path_media)),
-                ('timestamp', models.DateTimeField(auto_now_add=True)),
-                ('update_timestamp', models.DateTimeField(auto_now=True)),
-                ('source', models.TextField(blank=True)),
-                ('score', models.IntegerField(default=0)),
-                ('identifier', models.UUIDField(default=uuid.uuid4, editable=False)),
-                ('locked', models.BooleanField(default=False)),
-                ('tags_mirror', models.CharField(blank=True, max_length=1000)),
-                ('description', models.TextField(blank=True, max_length=1000)),
-                ('rating', models.IntegerField(choices=[(0, 'None'), (1, 'Safe'), (2, 'Questionable'), (3, 'Explicit')], default=0)),
-                ('status', models.IntegerField(choices=[(0, 'Pending'), (1, 'Approved'), (2, 'Hidden'), (3, 'Deleted')], default=0)),
-            ],
-            options={
-                'permissions': (('change_status', 'Can change the status of posts'), ('mass_rename', 'Can mass rename posts')),
-            },
-        ),
-        migrations.CreateModel(
-            name='PostTag',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=100, unique=True, verbose_name='Name')),
-                ('slug', models.SlugField(max_length=100, unique=True, verbose_name='Slug')),
-                ('description', models.CharField(blank=True, max_length=100)),
-                ('associated_link', models.CharField(blank=True, max_length=100)),
-                ('timestamp', models.DateTimeField(auto_now_add=True)),
-                ('aliases', taggit.managers.TaggableManager(help_text='A comma-separated list of tags.', through='taggit.TaggedItem', to='taggit.Tag', verbose_name='Tags')),
-                ('associated_user', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='associated_tags', to=settings.AUTH_USER_MODEL)),
-                ('author', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='authored_tags', to=settings.AUTH_USER_MODEL)),
-                ('category', models.ForeignKey(default=1, on_delete=django.db.models.deletion.SET_DEFAULT, to='booru.Category')),
-            ],
-            options={
-                'verbose_name': 'Tag',
-                'verbose_name_plural': 'Tags',
-            },
-        ),
-        migrations.CreateModel(
-            name='ScoreVote',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('point', models.IntegerField(default=1)),
-                ('account', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
-                ('post', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='booru.Post')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='TaggedPost',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('object_id', models.IntegerField(db_index=True, verbose_name='Object id')),
-                ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='booru_taggedpost_tagged_items', to='contenttypes.ContentType', verbose_name='Content type')),
-                ('tag', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='booru_taggedpost_items', to='booru.PostTag')),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-        migrations.AddField(
-            model_name='post',
-            name='tags',
-            field=taggit.managers.TaggableManager(help_text='A comma-separated list of tags.', related_name='posts', through='booru.TaggedPost', to='booru.PostTag', verbose_name='Tags'),
-        ),
-        migrations.AddField(
-            model_name='post',
-            name='uploader',
-            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL),
-        ),
-        migrations.AddField(
-            model_name='implication',
-            name='from_tag',
-            field=models.ForeignKey(blank=True, default=None, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='from_implications', to='booru.PostTag'),
-        ),
-        migrations.AddField(
-            model_name='implication',
-            name='to_tag',
-            field=models.ForeignKey(blank=True, default=None, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='to_implications', to='booru.PostTag'),
-        ),
-        migrations.AddField(
-            model_name='gallery',
-            name='posts',
-            field=models.ManyToManyField(to='booru.Post'),
-        ),
-        migrations.AddField(
-            model_name='favorite',
-            name='post',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='favorites', to='booru.Post'),
-        ),
-        migrations.AlterUniqueTogether(
-            name='scorevote',
-            unique_together={('account', 'post')},
-        ),
-        migrations.AlterUniqueTogether(
-            name='favorite',
-            unique_together={('account', 'post')},
-        ),
-        migrations.AlterUniqueTogether(
-            name='commentvote',
-            unique_together={('account', 'comment')},
-        ),
-    ]
+# Generated by Django 2.1.2 on 2018-11-13 21:21
+
+import booru.models
+from django.conf import settings
+from django.db import migrations, models
+import django.db.models.deletion
+import simple_history.models
+import taggit.managers
+import uuid
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('contenttypes', '0002_remove_content_type_name'),
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('taggit', '0002_auto_20150616_2121'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='Category',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('label', models.CharField(blank=True, max_length=100)),
+                ('title_singular', models.CharField(blank=True, max_length=100)),
+                ('title_plural', models.CharField(blank=True, max_length=100)),
+                ('color', models.CharField(blank=True, max_length=6)),
+            ],
+            options={
+                'verbose_name_plural': 'Categories',
+            },
+        ),
+        migrations.CreateModel(
+            name='Comment',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('content', models.CharField(blank=True, max_length=1000)),
+                ('timestamp', models.DateTimeField(auto_now_add=True)),
+                ('update_timestamp', models.DateTimeField(auto_now=True)),
+                ('object_id', models.PositiveIntegerField()),
+                ('author', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+                ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='contenttypes.ContentType')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='CommentVote',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('point', models.IntegerField(default=1)),
+                ('account', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+                ('comment', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='booru.Comment')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Configuration',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('code_name', models.CharField(max_length=100)),
+                ('value', models.CharField(blank=True, max_length=1000)),
+            ],
+            options={
+                'permissions': (('change_configurations', 'Can change the configurations of the booru'),),
+            },
+        ),
+        migrations.CreateModel(
+            name='Favorite',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('account', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='account_favorites', to=settings.AUTH_USER_MODEL)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Gallery',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(blank=True, max_length=100)),
+                ('description', models.CharField(blank=True, max_length=1000)),
+                ('posts_mirror', models.CharField(blank=True, max_length=1000)),
+                ('is_active', models.BooleanField(default=True)),
+            ],
+            options={
+                'verbose_name_plural': 'Galleries',
+            },
+        ),
+        migrations.CreateModel(
+            name='HistoricalGallery',
+            fields=[
+                ('id', models.IntegerField(auto_created=True, blank=True, db_index=True, verbose_name='ID')),
+                ('name', models.CharField(blank=True, max_length=100)),
+                ('description', models.CharField(blank=True, max_length=1000)),
+                ('posts_mirror', models.CharField(blank=True, max_length=1000)),
+                ('is_active', models.BooleanField(default=True)),
+                ('history_id', models.AutoField(primary_key=True, serialize=False)),
+                ('history_change_reason', models.CharField(max_length=100, null=True)),
+                ('history_date', models.DateTimeField()),
+                ('history_type', models.CharField(choices=[('+', 'Created'), ('~', 'Changed'), ('-', 'Deleted')], max_length=1)),
+                ('history_user', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to=settings.AUTH_USER_MODEL)),
+            ],
+            options={
+                'verbose_name': 'historical gallery',
+                'ordering': ('-history_date', '-history_id'),
+                'get_latest_by': 'history_date',
+            },
+            bases=(simple_history.models.HistoricalChanges, models.Model),
+        ),
+        migrations.CreateModel(
+            name='HistoricalPost',
+            fields=[
+                ('id', models.IntegerField(auto_created=True, blank=True, db_index=True, verbose_name='ID')),
+                ('parent', models.IntegerField(blank=True, null=True)),
+                ('preview', models.TextField(blank=True, max_length=100)),
+                ('sample', models.TextField(blank=True, max_length=100)),
+                ('image', models.TextField(blank=True, max_length=100)),
+                ('timestamp', models.DateTimeField(blank=True, editable=False)),
+                ('update_timestamp', models.DateTimeField(blank=True, editable=False)),
+                ('source', models.TextField(blank=True)),
+                ('score', models.IntegerField(default=0)),
+                ('identifier', models.UUIDField(default=uuid.uuid4, editable=False)),
+                ('locked', models.BooleanField(default=False)),
+                ('tags_mirror', models.CharField(blank=True, max_length=1000)),
+                ('description', models.TextField(blank=True, max_length=1000)),
+                ('rating', models.IntegerField(choices=[(0, 'None'), (1, 'Safe'), (2, 'Questionable'), (3, 'Explicit')], default=0)),
+                ('status', models.IntegerField(choices=[(0, 'Pending'), (1, 'Approved'), (2, 'Hidden'), (3, 'Deleted')], default=0)),
+                ('history_id', models.AutoField(primary_key=True, serialize=False)),
+                ('history_change_reason', models.CharField(max_length=100, null=True)),
+                ('history_date', models.DateTimeField()),
+                ('history_type', models.CharField(choices=[('+', 'Created'), ('~', 'Changed'), ('-', 'Deleted')], max_length=1)),
+                ('history_user', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to=settings.AUTH_USER_MODEL)),
+                ('uploader', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to=settings.AUTH_USER_MODEL)),
+            ],
+            options={
+                'verbose_name': 'historical post',
+                'ordering': ('-history_date', '-history_id'),
+                'get_latest_by': 'history_date',
+            },
+            bases=(simple_history.models.HistoricalChanges, models.Model),
+        ),
+        migrations.CreateModel(
+            name='HistoricalPostTag',
+            fields=[
+                ('id', models.IntegerField(auto_created=True, blank=True, db_index=True, verbose_name='ID')),
+                ('name', models.CharField(db_index=True, max_length=100, verbose_name='Name')),
+                ('slug', models.SlugField(max_length=100, verbose_name='Slug')),
+                ('description', models.CharField(blank=True, max_length=100)),
+                ('associated_link', models.CharField(blank=True, max_length=100)),
+                ('timestamp', models.DateTimeField(blank=True, editable=False)),
+                ('history_id', models.AutoField(primary_key=True, serialize=False)),
+                ('history_change_reason', models.CharField(max_length=100, null=True)),
+                ('history_date', models.DateTimeField()),
+                ('history_type', models.CharField(choices=[('+', 'Created'), ('~', 'Changed'), ('-', 'Deleted')], max_length=1)),
+                ('associated_user', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to=settings.AUTH_USER_MODEL)),
+                ('author', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to=settings.AUTH_USER_MODEL)),
+                ('category', models.ForeignKey(blank=True, db_constraint=False, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to='booru.Category')),
+                ('history_user', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to=settings.AUTH_USER_MODEL)),
+            ],
+            options={
+                'verbose_name': 'historical Tag',
+                'ordering': ('-history_date', '-history_id'),
+                'get_latest_by': 'history_date',
+            },
+            bases=(simple_history.models.HistoricalChanges, models.Model),
+        ),
+        migrations.CreateModel(
+            name='Implication',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('timestamp', models.DateTimeField(auto_now_add=True)),
+                ('status', models.IntegerField(choices=[(0, 'Pending'), (1, 'Approved'), (2, 'Unapproved')], default=0)),
+                ('approver', models.ForeignKey(blank=True, default=None, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='approved_implications', to=settings.AUTH_USER_MODEL)),
+                ('author', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='authored_implications', to=settings.AUTH_USER_MODEL)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Post',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('parent', models.IntegerField(blank=True, null=True)),
+                ('preview', models.ImageField(blank=True, upload_to=booru.models.get_file_path_preview)),
+                ('sample', models.ImageField(blank=True, upload_to=booru.models.get_file_path_sample)),
+                ('image', models.ImageField(blank=True, upload_to=booru.models.get_file_path_media)),
+                ('timestamp', models.DateTimeField(auto_now_add=True)),
+                ('update_timestamp', models.DateTimeField(auto_now=True)),
+                ('source', models.TextField(blank=True)),
+                ('score', models.IntegerField(default=0)),
+                ('identifier', models.UUIDField(default=uuid.uuid4, editable=False)),
+                ('locked', models.BooleanField(default=False)),
+                ('tags_mirror', models.CharField(blank=True, max_length=1000)),
+                ('description', models.TextField(blank=True, max_length=1000)),
+                ('rating', models.IntegerField(choices=[(0, 'None'), (1, 'Safe'), (2, 'Questionable'), (3, 'Explicit')], default=0)),
+                ('status', models.IntegerField(choices=[(0, 'Pending'), (1, 'Approved'), (2, 'Hidden'), (3, 'Deleted')], default=0)),
+            ],
+            options={
+                'permissions': (('change_status', 'Can change the status of posts'), ('mass_rename', 'Can mass rename posts')),
+            },
+        ),
+        migrations.CreateModel(
+            name='PostTag',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=100, unique=True, verbose_name='Name')),
+                ('slug', models.SlugField(max_length=100, unique=True, verbose_name='Slug')),
+                ('description', models.CharField(blank=True, max_length=100)),
+                ('associated_link', models.CharField(blank=True, max_length=100)),
+                ('timestamp', models.DateTimeField(auto_now_add=True)),
+                ('aliases', taggit.managers.TaggableManager(help_text='A comma-separated list of tags.', through='taggit.TaggedItem', to='taggit.Tag', verbose_name='Tags')),
+                ('associated_user', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='associated_tags', to=settings.AUTH_USER_MODEL)),
+                ('author', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='authored_tags', to=settings.AUTH_USER_MODEL)),
+                ('category', models.ForeignKey(default=1, on_delete=django.db.models.deletion.SET_DEFAULT, to='booru.Category')),
+            ],
+            options={
+                'verbose_name': 'Tag',
+                'verbose_name_plural': 'Tags',
+            },
+        ),
+        migrations.CreateModel(
+            name='ScoreVote',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('point', models.IntegerField(default=1)),
+                ('account', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+                ('post', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='booru.Post')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='TaggedPost',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('object_id', models.IntegerField(db_index=True, verbose_name='Object id')),
+                ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='booru_taggedpost_tagged_items', to='contenttypes.ContentType', verbose_name='Content type')),
+                ('tag', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='booru_taggedpost_items', to='booru.PostTag')),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+        migrations.AddField(
+            model_name='post',
+            name='tags',
+            field=taggit.managers.TaggableManager(help_text='A comma-separated list of tags.', related_name='posts', through='booru.TaggedPost', to='booru.PostTag', verbose_name='Tags'),
+        ),
+        migrations.AddField(
+            model_name='post',
+            name='uploader',
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL),
+        ),
+        migrations.AddField(
+            model_name='implication',
+            name='from_tag',
+            field=models.ForeignKey(blank=True, default=None, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='from_implications', to='booru.PostTag'),
+        ),
+        migrations.AddField(
+            model_name='implication',
+            name='to_tag',
+            field=models.ForeignKey(blank=True, default=None, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='to_implications', to='booru.PostTag'),
+        ),
+        migrations.AddField(
+            model_name='gallery',
+            name='posts',
+            field=models.ManyToManyField(to='booru.Post'),
+        ),
+        migrations.AddField(
+            model_name='favorite',
+            name='post',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='favorites', to='booru.Post'),
+        ),
+        migrations.AlterUniqueTogether(
+            name='scorevote',
+            unique_together={('account', 'post')},
+        ),
+        migrations.AlterUniqueTogether(
+            name='favorite',
+            unique_together={('account', 'post')},
+        ),
+        migrations.AlterUniqueTogether(
+            name='commentvote',
+            unique_together={('account', 'comment')},
+        ),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/migrations/0002_auto_20181113_2136.py` & `Boorunaut-0.5.0/booru/migrations/0002_auto_20181113_2136.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# Generated by Django 2.1.2 on 2018-11-13 21:36
-
-from django.db import migrations
-
-
-def create_types(apps, schema_editor):
-    db_alias = schema_editor.connection.alias
-    Category = apps.get_model("booru", "Category")
-    Category.objects.using(db_alias).create(label="general", title_singular="General",
-                                            title_plural="General", color="")
-    Category.objects.using(db_alias).create(label="artist", title_singular="Artist",
-                                            title_plural="Artists", color="BB6666")
-    Category.objects.using(db_alias).create(label="copyright", title_singular="Copyright",
-                                            title_plural="Copyrights", color="AA00AA")
-    Category.objects.using(db_alias).create(label="character", title_singular="Character",
-                                            title_plural="Characters", color="66BB66"),
-    Category.objects.using(db_alias).create(label="meta", title_singular="Meta",
-                                            title_plural="Meta", color="FF8800")
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('booru', '0001_initial'),
-    ]
-
-    operations = [
-        migrations.RunPython(create_types),
-    ]
+# Generated by Django 2.1.2 on 2018-11-13 21:36
+
+from django.db import migrations
+
+
+def create_types(apps, schema_editor):
+    db_alias = schema_editor.connection.alias
+    Category = apps.get_model("booru", "Category")
+    Category.objects.using(db_alias).create(label="general", title_singular="General",
+                                            title_plural="General", color="")
+    Category.objects.using(db_alias).create(label="artist", title_singular="Artist",
+                                            title_plural="Artists", color="BB6666")
+    Category.objects.using(db_alias).create(label="copyright", title_singular="Copyright",
+                                            title_plural="Copyrights", color="AA00AA")
+    Category.objects.using(db_alias).create(label="character", title_singular="Character",
+                                            title_plural="Characters", color="66BB66"),
+    Category.objects.using(db_alias).create(label="meta", title_singular="Meta",
+                                            title_plural="Meta", color="FF8800")
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('booru', '0001_initial'),
+    ]
+
+    operations = [
+        migrations.RunPython(create_types),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/migrations/0003_auto_20181118_1918.py` & `Boorunaut-0.5.0/booru/migrations/0003_auto_20181118_1918.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Generated by Django 2.1.2 on 2018-11-18 19:18
-
-import booru.models
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('booru', '0002_auto_20181113_2136'),
-    ]
-
-    operations = [
-        migrations.RenameField(
-            model_name='historicalpost',
-            old_name='image',
-            new_name='media',
-        ),
-        migrations.RemoveField(
-            model_name='post',
-            name='image',
-        ),
-        migrations.AddField(
-            model_name='post',
-            name='media',
-            field=models.FileField(blank=True, upload_to=booru.models.get_file_path_media),
-        ),
-    ]
+# Generated by Django 2.1.2 on 2018-11-18 19:18
+
+import booru.models
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('booru', '0002_auto_20181113_2136'),
+    ]
+
+    operations = [
+        migrations.RenameField(
+            model_name='historicalpost',
+            old_name='image',
+            new_name='media',
+        ),
+        migrations.RemoveField(
+            model_name='post',
+            name='image',
+        ),
+        migrations.AddField(
+            model_name='post',
+            name='media',
+            field=models.FileField(blank=True, upload_to=booru.models.get_file_path_media),
+        ),
+    ]
```

### Comparing `Boorunaut-0.4.3/booru/models.py` & `Boorunaut-0.5.0/booru/models.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,399 +1,399 @@
-import os
-import urllib.parse
-import uuid
-from urllib.parse import urlparse
-
-from django.conf import settings
-from django.contrib.contenttypes.fields import (GenericForeignKey,
-                                                GenericRelation)
-from django.contrib.contenttypes.models import ContentType
-from django.core.files.images import get_image_dimensions
-from django.db import models
-from django.db.models import Q, Sum
-from django.db.models.signals import m2m_changed
-from django.urls import reverse
-from simple_history.models import HistoricalRecords
-from taggit.managers import TaggableManager
-from taggit.models import GenericTaggedItemBase, Tag, TagBase, TaggedItem
-
-from booru import utils
-from booru.account.models import Account
-from booru.managers import PostManager
-
-
-def get_file_path(instance, filename):
-    ext = filename.split('.')[-1]
-    filename = "%s.%s" % (uuid.uuid4(), ext)
-    return filename
-
-def get_file_path_preview(instance, filename):
-    name = get_file_path(instance, filename)
-    return os.path.join('data/preview/', name)
-
-def get_file_path_sample(instance, filename):
-    name = get_file_path(instance, filename)
-    return os.path.join('data/sample/', name)
-
-def get_file_path_media(instance, filename):
-    name = get_file_path(instance, filename)
-    return os.path.join('data/media/', name)
-
-class Comment(models.Model):
-    author = models.ForeignKey(Account, on_delete=models.CASCADE)
-    content = models.CharField(max_length=1000, blank=True)
-    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
-    update_timestamp = models.DateTimeField(auto_now=True, auto_now_add=False)
-    is_hidden = models.BooleanField(default=False)
-
-    content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
-    object_id = models.PositiveIntegerField()
-    content_object = GenericForeignKey('content_type', 'object_id')
-
-    def get_vote_count(self):
-        return self.commentvote_set.count()
-    
-    def get_score(self):
-        upvotes = self.commentvote_set.filter(point=1).count()
-        downvotes = self.commentvote_set.filter(point=-1).count()
-        return upvotes - downvotes
-
-class Implication(models.Model):
-    from_tag = models.ForeignKey('booru.PostTag', blank=True, null=True, default=None, on_delete=models.CASCADE, related_name="from_implications")
-    to_tag = models.ForeignKey('booru.PostTag', blank=True, null=True, default=None, on_delete=models.CASCADE, related_name="to_implications")
-    author = models.ForeignKey(Account, null=True, on_delete=models.SET_NULL, related_name="authored_implications")
-    approver = models.ForeignKey(Account, blank=True, null=True, default=None, on_delete=models.SET_NULL, related_name="approved_implications")
-    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
-    
-    PENDING = 0
-    APPROVED = 1
-    UNAPPROVED = 2
-    STATUS_CHOICES = (
-        (PENDING, 'Pending'),
-        (APPROVED, 'Approved'),
-        (UNAPPROVED, 'Unapproved')
-    )
-    status = models.IntegerField(
-        choices=STATUS_CHOICES,
-        default=PENDING,
-    )
-
-    def __str__(self):
-        return "{} -> {}".format(self.from_tag, self.to_tag)
-
-class Category(models.Model):
-    '''Basic model for the content app. It should be inherited from the other models.'''
-    label = models.CharField(max_length=100, blank=True)
-    title_singular = models.CharField(max_length=100, blank=True)
-    title_plural = models.CharField(max_length=100, blank=True)
-    color = models.CharField(max_length=6, blank=True)
-
-    def __str__(self):
-        return self.title_singular
-
-    class Meta:
-        verbose_name_plural = 'Categories'
-
-class PostTag(TagBase):
-    category = models.ForeignKey(Category, default=1, on_delete=models.SET_DEFAULT)
-    description = models.CharField(max_length=100, blank=True)
-    associated_link = models.CharField(max_length=100, blank=True)
-    associated_user = models.ForeignKey(Account, null=True, blank=True,
-                                                 on_delete=models.SET_NULL, related_name="associated_tags")
-    author = models.ForeignKey(Account, null=True, on_delete=models.SET_NULL, related_name="authored_tags")
-    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
-    update_timestamp = models.DateTimeField(auto_now=True, auto_now_add=False)
-    aliases = TaggableManager()
-    history = HistoricalRecords()
-
-    class Meta:
-        verbose_name = ("Tag")
-        verbose_name_plural = ("Tags")
-        permissions = (
-            ("manage_tags", "Can manage tags"),
-        )
-
-    def get_absolute_url(self):
-        return reverse('booru:tag_detail', kwargs={'tag_id': self.id})
-    
-    def get_search_url(self):
-        tags = urllib.parse.quote_plus(self.name)
-        return reverse('booru:posts') + "?tags=%s" % tags
-
-    def get_count(self):
-        return TaggedPost.objects.filter(tag=self).count()
-
-class TaggedPost(GenericTaggedItemBase):
-    tag = models.ForeignKey(PostTag, related_name="%(app_label)s_%(class)s_items", on_delete=models.CASCADE)
-
-    def save(self, *args, **kwargs):
-        super(TaggedPost, self).save(*args, **kwargs)
-
-        tag_name = self.tag
-        utils.verify_and_perform_implications(tag_name)
-
-class Gallery(models.Model):
-    name = models.CharField(max_length=100, blank=True)
-    description = models.CharField(max_length=1000, blank=True)
-    posts = models.ManyToManyField('booru.Post')
-    posts_mirror = models.CharField(max_length=1000, blank=True)
-    is_active = models.BooleanField(default=True)
-
-    history = HistoricalRecords()
-
-    def __str__(self):
-        return "{}".format(self.name)
-
-    class Meta:
-        verbose_name_plural = 'Galleries'
-    
-    def get_count(self):
-        return self.posts.count()
-
-    def get_absolute_url(self):
-        return reverse('booru:gallery_detail', kwargs={'gallery_id': self.id})
-
-class Post(models.Model):
-    parent = models.IntegerField(null=True, blank=True)
-    preview = models.ImageField(upload_to=get_file_path_preview, blank=True)
-    sample = models.ImageField(upload_to=get_file_path_sample, blank=True)
-    media = models.FileField(upload_to=get_file_path_media, blank=True)
-    uploader = models.ForeignKey(Account, null=True, on_delete=models.SET_NULL)
-    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
-    update_timestamp = models.DateTimeField(auto_now=True, auto_now_add=False)
-    source = models.TextField(blank=True)
-    score = models.IntegerField(default=0)
-    identifier = models.UUIDField(default=uuid.uuid4, editable=False)
-    locked = models.BooleanField(default=False)
-    tags = TaggableManager(through=TaggedPost, related_name="posts")
-    tags_mirror = models.CharField(max_length=1000, blank=True)
-    description = models.TextField(max_length=1000, blank=True)
-    comments = GenericRelation(Comment)
-
-    objects = PostManager()
-    history = HistoricalRecords()
-
-    NONE = 0
-    SAFE = 1
-    QUESTIONABLE = 2
-    EXPLICIT = 3
-    RATING_CHOICES = (
-        (NONE, 'None'),
-        (SAFE, 'Safe'),
-        (QUESTIONABLE, 'Questionable'),
-        (EXPLICIT, 'Explicit')
-    )
-    rating = models.IntegerField(
-        choices=RATING_CHOICES,
-        default=NONE,
-    )
-
-    PENDING = 0
-    APPROVED = 1
-    HIDDEN = 2
-    DELETED = 3
-    STATUS_CHOICES = (
-        (PENDING, 'Pending'),
-        (APPROVED, 'Approved'),
-        (HIDDEN, 'Hidden'),
-        (DELETED, 'Deleted')
-    )
-    status = models.IntegerField(
-        choices=STATUS_CHOICES,
-        default=PENDING,
-    )
-
-    IMAGE = 0
-    VIDEO = 1
-    MEDIA_TYPE_CHOICES = (
-        (IMAGE, 'Image'),
-        (VIDEO, 'Video')
-    )
-    media_type = models.IntegerField(
-        choices=MEDIA_TYPE_CHOICES,
-        default=IMAGE,
-    )
-
-    def __str__(self):
-        return "#{}".format(self.id)
-
-    def save(self, *args, **kwargs):
-        if not self.id:
-            pil_image = utils.get_pil_image_if_valid(self.media)
-
-            if pil_image:
-                if settings.BOORUNAUT_EMBED_MODE == False:
-                    width, height = pil_image.size
-                    media = utils.image_resizer(pil_image, (width, height))
-                    self.media.save(".jpg", media, save=False)
-
-                    sample = None
-                    if width > 850 or height > 850:
-                        sample = utils.image_resizer(pil_image, (850, 850))
-                    
-                    if sample:
-                        self.sample.save(".jpg", sample, save=False)
-
-                preview = utils.image_resizer(pil_image, (150, 150))
-                if preview:
-                    self.preview.save(".jpg", preview, save=False)
-
-                self.media_type = self.IMAGE
-
-                if settings.BOORUNAUT_EMBED_MODE == True:
-                    self.media.delete()
-            else:
-                self.media_type = self.VIDEO
-        super(Post, self).save(*args, **kwargs)
-        if self.media_type == self.VIDEO and not self.preview:
-            preview = utils.get_video_preview(self.media)
-            self.preview.save(".jpg", preview, save=False)
-
-    def get_sample_url(self):
-        if self.sample:
-            return self.sample.url
-        else:
-            return self.media.url
-
-    def get_absolute_url(self):
-        return reverse('booru:post_detail', kwargs={'post_id': self.id})
-
-    def get_ordered_tags(self):
-        ordered_tags = {}
-        tags = self.tags.all().order_by('category', 'name')
-        
-        for tag in tags:
-            try:
-                ordered_tags[tag.category]
-            except:
-                ordered_tags[tag.category] = []
-            ordered_tags[tag.category].append(tag)
-        
-        return ordered_tags
-
-    def get_score_count(self):
-        votes = ScoreVote.objects.filter(post=self)
-        
-        if votes.exists():
-            votes = votes.aggregate(Sum('point'))['point__sum']
-        else:
-            votes = 0
-        
-        return votes
-
-    def get_favorites_count(self):
-        return self.favorites.count()
-
-    def check_and_update_mirror(self):
-        mirror = " ".join(self.tags.names())
-
-        if self.tags_mirror != mirror:
-            self.tags_mirror = mirror
-        
-        self.save_without_historical_record()
-
-    def check_and_update_implications(self):
-        missing_implications = Implication.objects.filter(from_tag__in=self.tags.all(), status=1)\
-                                                    .exclude(to_tag__in=self.tags.all()).distinct()
-        if missing_implications.exists():
-            for implication in missing_implications:
-                self.tags.add(implication.to_tag)
-        
-        self.check_and_update_mirror()
-
-    def save_without_historical_record(self, *args, **kwargs):
-        self.skip_history_when_saving = True
-        try:
-            ret = self.save(*args, **kwargs)
-        finally:
-            del self.skip_history_when_saving
-        return ret
-    
-    def get_media_width(self):
-        if self.media_type == self.IMAGE:
-            width, height = get_image_dimensions(self.media.file)
-        else:
-            width, height = utils.get_video_dimensions(self.media)
-        return width
-
-    def get_media_height(self):
-        if self.media_type == self.IMAGE:
-            width, height = get_image_dimensions(self.media.file)
-        else:
-            width, height = utils.get_video_dimensions(self.media)
-        return height
-    
-    def get_sources(self):
-        sources = self.source.splitlines()
-        return sources
-    
-    def get_embed_code(self):
-        sources = self.get_sources()
-
-        if sources:
-            url = sources[0]
-            return f'''
-            <a class="embedly-card" data-card-controls="0" href="{url}"></a>
-            <script async src="//cdn.embedly.com/widgets/platform.js" charset="UTF-8"></script>
-            '''
-        else:
-            return None
-    
-    def get_parent(self):
-        if self.parent:
-            return Post.objects.not_deleted().filter(id=self.parent).first()
-        return None
-    
-    def get_siblings(self):
-        if self.parent:
-            return Post.objects.not_deleted().filter(parent=self.parent).exclude(id=self.id)
-        return None
-    
-    def get_children(self):
-        return Post.objects.not_deleted().filter(parent=self.id) or None
-
-    def is_deleted(self):
-        return self.status == Post.DELETED
-
-    def is_hidden(self):
-        return self.status == Post.HIDDEN
-    
-    class Meta:
-        permissions = (
-            ("change_status", "Can change the status of posts"),
-            ("mass_rename", "Can mass rename posts"),
-        )
-
-class Favorite(models.Model):
-    account = models.ForeignKey(Account, on_delete=models.CASCADE, related_name="account_favorites")
-    post = models.ForeignKey(Post, on_delete=models.CASCADE, related_name="favorites")
-
-    class Meta:
-        unique_together = ('account', 'post',)
-
-class ScoreVote(models.Model):
-    account = models.ForeignKey(Account, on_delete=models.CASCADE)
-    post = models.ForeignKey(Post, on_delete=models.CASCADE)
-    point = models.IntegerField(default=1)
-
-    class Meta:
-        unique_together = ('account', 'post',)
-
-class CommentVote(models.Model):
-    account = models.ForeignKey(Account, on_delete=models.CASCADE)
-    comment = models.ForeignKey(Comment, on_delete=models.CASCADE)
-    point = models.IntegerField(default=1)
-
-    class Meta:
-        unique_together = ('account', 'comment',)
-
-class Configuration(models.Model):
-    code_name = models.CharField(max_length=100, blank=False)
-    value = models.CharField(max_length=1000, blank=True)
-
-    def __str__(self):
-        return "{}".format(self.code_name)
-
-    class Meta:
-        permissions = (
-            ("change_configurations", "Can change the configurations of the booru"),
-        )
+import os
+import urllib.parse
+import uuid
+from urllib.parse import urlparse
+
+from django.conf import settings
+from django.contrib.contenttypes.fields import (GenericForeignKey,
+                                                GenericRelation)
+from django.contrib.contenttypes.models import ContentType
+from django.core.files.images import get_image_dimensions
+from django.db import models
+from django.db.models import Q, Sum
+from django.db.models.signals import m2m_changed
+from django.urls import reverse
+from simple_history.models import HistoricalRecords
+from taggit.managers import TaggableManager
+from taggit.models import GenericTaggedItemBase, Tag, TagBase, TaggedItem
+
+from booru import utils
+from booru.account.models import Account
+from booru.managers import PostManager
+
+
+def get_file_path(instance, filename):
+    ext = filename.split('.')[-1]
+    filename = "%s.%s" % (uuid.uuid4(), ext)
+    return filename
+
+def get_file_path_preview(instance, filename):
+    name = get_file_path(instance, filename)
+    return os.path.join('data/preview/', name)
+
+def get_file_path_sample(instance, filename):
+    name = get_file_path(instance, filename)
+    return os.path.join('data/sample/', name)
+
+def get_file_path_media(instance, filename):
+    name = get_file_path(instance, filename)
+    return os.path.join('data/media/', name)
+
+class Comment(models.Model):
+    author = models.ForeignKey(Account, on_delete=models.CASCADE)
+    content = models.CharField(max_length=1000, blank=True)
+    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
+    update_timestamp = models.DateTimeField(auto_now=True, auto_now_add=False)
+    is_hidden = models.BooleanField(default=False)
+
+    content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
+    object_id = models.PositiveIntegerField()
+    content_object = GenericForeignKey('content_type', 'object_id')
+
+    def get_vote_count(self):
+        return self.commentvote_set.count()
+    
+    def get_score(self):
+        upvotes = self.commentvote_set.filter(point=1).count()
+        downvotes = self.commentvote_set.filter(point=-1).count()
+        return upvotes - downvotes
+
+class Implication(models.Model):
+    from_tag = models.ForeignKey('booru.PostTag', blank=True, null=True, default=None, on_delete=models.CASCADE, related_name="from_implications")
+    to_tag = models.ForeignKey('booru.PostTag', blank=True, null=True, default=None, on_delete=models.CASCADE, related_name="to_implications")
+    author = models.ForeignKey(Account, null=True, on_delete=models.SET_NULL, related_name="authored_implications")
+    approver = models.ForeignKey(Account, blank=True, null=True, default=None, on_delete=models.SET_NULL, related_name="approved_implications")
+    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
+    
+    PENDING = 0
+    APPROVED = 1
+    UNAPPROVED = 2
+    STATUS_CHOICES = (
+        (PENDING, 'Pending'),
+        (APPROVED, 'Approved'),
+        (UNAPPROVED, 'Unapproved')
+    )
+    status = models.IntegerField(
+        choices=STATUS_CHOICES,
+        default=PENDING,
+    )
+
+    def __str__(self):
+        return "{} -> {}".format(self.from_tag, self.to_tag)
+
+class Category(models.Model):
+    '''Basic model for the content app. It should be inherited from the other models.'''
+    label = models.CharField(max_length=100, blank=True)
+    title_singular = models.CharField(max_length=100, blank=True)
+    title_plural = models.CharField(max_length=100, blank=True)
+    color = models.CharField(max_length=6, blank=True)
+
+    def __str__(self):
+        return self.title_singular
+
+    class Meta:
+        verbose_name_plural = 'Categories'
+
+class PostTag(TagBase):
+    category = models.ForeignKey(Category, default=1, on_delete=models.SET_DEFAULT)
+    description = models.CharField(max_length=100, blank=True)
+    associated_link = models.CharField(max_length=100, blank=True)
+    associated_user = models.ForeignKey(Account, null=True, blank=True,
+                                                 on_delete=models.SET_NULL, related_name="associated_tags")
+    author = models.ForeignKey(Account, null=True, on_delete=models.SET_NULL, related_name="authored_tags")
+    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
+    update_timestamp = models.DateTimeField(auto_now=True, auto_now_add=False)
+    aliases = TaggableManager()
+    history = HistoricalRecords()
+
+    class Meta:
+        verbose_name = ("Tag")
+        verbose_name_plural = ("Tags")
+        permissions = (
+            ("manage_tags", "Can manage tags"),
+        )
+
+    def get_absolute_url(self):
+        return reverse('booru:tag_detail', kwargs={'tag_id': self.id})
+    
+    def get_search_url(self):
+        tags = urllib.parse.quote_plus(self.name)
+        return reverse('booru:posts') + "?tags=%s" % tags
+
+    def get_count(self):
+        return TaggedPost.objects.filter(tag=self).count()
+
+class TaggedPost(GenericTaggedItemBase):
+    tag = models.ForeignKey(PostTag, related_name="%(app_label)s_%(class)s_items", on_delete=models.CASCADE)
+
+    def save(self, *args, **kwargs):
+        super(TaggedPost, self).save(*args, **kwargs)
+
+        tag_name = self.tag
+        utils.verify_and_perform_implications(tag_name)
+
+class Gallery(models.Model):
+    name = models.CharField(max_length=100, blank=True)
+    description = models.CharField(max_length=1000, blank=True)
+    posts = models.ManyToManyField('booru.Post')
+    posts_mirror = models.CharField(max_length=1000, blank=True)
+    is_active = models.BooleanField(default=True)
+
+    history = HistoricalRecords()
+
+    def __str__(self):
+        return "{}".format(self.name)
+
+    class Meta:
+        verbose_name_plural = 'Galleries'
+    
+    def get_count(self):
+        return self.posts.count()
+
+    def get_absolute_url(self):
+        return reverse('booru:gallery_detail', kwargs={'gallery_id': self.id})
+
+class Post(models.Model):
+    parent = models.IntegerField(null=True, blank=True)
+    preview = models.ImageField(upload_to=get_file_path_preview, blank=True)
+    sample = models.ImageField(upload_to=get_file_path_sample, blank=True)
+    media = models.FileField(upload_to=get_file_path_media, blank=True)
+    uploader = models.ForeignKey(Account, null=True, on_delete=models.SET_NULL)
+    timestamp = models.DateTimeField(auto_now=False, auto_now_add=True)
+    update_timestamp = models.DateTimeField(auto_now=True, auto_now_add=False)
+    source = models.TextField(blank=True)
+    score = models.IntegerField(default=0)
+    identifier = models.UUIDField(default=uuid.uuid4, editable=False)
+    locked = models.BooleanField(default=False)
+    tags = TaggableManager(through=TaggedPost, related_name="posts")
+    tags_mirror = models.CharField(max_length=1000, blank=True)
+    description = models.TextField(max_length=1000, blank=True)
+    comments = GenericRelation(Comment)
+
+    objects = PostManager()
+    history = HistoricalRecords()
+
+    NONE = 0
+    SAFE = 1
+    QUESTIONABLE = 2
+    EXPLICIT = 3
+    RATING_CHOICES = (
+        (NONE, 'None'),
+        (SAFE, 'Safe'),
+        (QUESTIONABLE, 'Questionable'),
+        (EXPLICIT, 'Explicit')
+    )
+    rating = models.IntegerField(
+        choices=RATING_CHOICES,
+        default=NONE,
+    )
+
+    PENDING = 0
+    APPROVED = 1
+    HIDDEN = 2
+    DELETED = 3
+    STATUS_CHOICES = (
+        (PENDING, 'Pending'),
+        (APPROVED, 'Approved'),
+        (HIDDEN, 'Hidden'),
+        (DELETED, 'Deleted')
+    )
+    status = models.IntegerField(
+        choices=STATUS_CHOICES,
+        default=PENDING,
+    )
+
+    IMAGE = 0
+    VIDEO = 1
+    MEDIA_TYPE_CHOICES = (
+        (IMAGE, 'Image'),
+        (VIDEO, 'Video')
+    )
+    media_type = models.IntegerField(
+        choices=MEDIA_TYPE_CHOICES,
+        default=IMAGE,
+    )
+
+    def __str__(self):
+        return "#{}".format(self.id)
+
+    def save(self, *args, **kwargs):
+        if not self.id:
+            pil_image = utils.get_pil_image_if_valid(self.media)
+
+            if pil_image:
+                if settings.BOORUNAUT_EMBED_MODE == False:
+                    width, height = pil_image.size
+                    media = utils.image_resizer(pil_image, (width, height))
+                    self.media.save(".jpg", media, save=False)
+
+                    sample = None
+                    if width > 850 or height > 850:
+                        sample = utils.image_resizer(pil_image, (850, 850))
+                    
+                    if sample:
+                        self.sample.save(".jpg", sample, save=False)
+
+                preview = utils.image_resizer(pil_image, (150, 150))
+                if preview:
+                    self.preview.save(".jpg", preview, save=False)
+
+                self.media_type = self.IMAGE
+
+                if settings.BOORUNAUT_EMBED_MODE == True:
+                    self.media.delete()
+            else:
+                self.media_type = self.VIDEO
+        super(Post, self).save(*args, **kwargs)
+        if self.media_type == self.VIDEO and not self.preview:
+            preview = utils.get_video_preview(self.media)
+            self.preview.save(".jpg", preview, save=False)
+
+    def get_sample_url(self):
+        if self.sample:
+            return self.sample.url
+        else:
+            return self.media.url
+
+    def get_absolute_url(self):
+        return reverse('booru:post_detail', kwargs={'post_id': self.id})
+
+    def get_ordered_tags(self):
+        ordered_tags = {}
+        tags = self.tags.all().order_by('category', 'name')
+        
+        for tag in tags:
+            try:
+                ordered_tags[tag.category]
+            except:
+                ordered_tags[tag.category] = []
+            ordered_tags[tag.category].append(tag)
+        
+        return ordered_tags
+
+    def get_score_count(self):
+        votes = ScoreVote.objects.filter(post=self)
+        
+        if votes.exists():
+            votes = votes.aggregate(Sum('point'))['point__sum']
+        else:
+            votes = 0
+        
+        return votes
+
+    def get_favorites_count(self):
+        return self.favorites.count()
+
+    def check_and_update_mirror(self):
+        mirror = " ".join(self.tags.names())
+
+        if self.tags_mirror != mirror:
+            self.tags_mirror = mirror
+        
+        self.save_without_historical_record()
+
+    def check_and_update_implications(self):
+        missing_implications = Implication.objects.filter(from_tag__in=self.tags.all(), status=1)\
+                                                    .exclude(to_tag__in=self.tags.all()).distinct()
+        if missing_implications.exists():
+            for implication in missing_implications:
+                self.tags.add(implication.to_tag)
+        
+        self.check_and_update_mirror()
+
+    def save_without_historical_record(self, *args, **kwargs):
+        self.skip_history_when_saving = True
+        try:
+            ret = self.save(*args, **kwargs)
+        finally:
+            del self.skip_history_when_saving
+        return ret
+    
+    def get_media_width(self):
+        if self.media_type == self.IMAGE:
+            width, height = get_image_dimensions(self.media.file)
+        else:
+            width, height = utils.get_video_dimensions(self.media)
+        return width
+
+    def get_media_height(self):
+        if self.media_type == self.IMAGE:
+            width, height = get_image_dimensions(self.media.file)
+        else:
+            width, height = utils.get_video_dimensions(self.media)
+        return height
+    
+    def get_sources(self):
+        sources = self.source.splitlines()
+        return sources
+    
+    def get_embed_code(self):
+        sources = self.get_sources()
+
+        if sources:
+            url = sources[0]
+            return f'''
+            <a class="embedly-card" data-card-controls="0" href="{url}"></a>
+            <script async src="//cdn.embedly.com/widgets/platform.js" charset="UTF-8"></script>
+            '''
+        else:
+            return None
+    
+    def get_parent(self):
+        if self.parent:
+            return Post.objects.not_deleted().filter(id=self.parent).first()
+        return None
+    
+    def get_siblings(self):
+        if self.parent:
+            return Post.objects.not_deleted().filter(parent=self.parent).exclude(id=self.id)
+        return None
+    
+    def get_children(self):
+        return Post.objects.not_deleted().filter(parent=self.id) or None
+
+    def is_deleted(self):
+        return self.status == Post.DELETED
+
+    def is_hidden(self):
+        return self.status == Post.HIDDEN
+    
+    class Meta:
+        permissions = (
+            ("change_status", "Can change the status of posts"),
+            ("mass_rename", "Can mass rename posts"),
+        )
+
+class Favorite(models.Model):
+    account = models.ForeignKey(Account, on_delete=models.CASCADE, related_name="account_favorites")
+    post = models.ForeignKey(Post, on_delete=models.CASCADE, related_name="favorites")
+
+    class Meta:
+        unique_together = ('account', 'post',)
+
+class ScoreVote(models.Model):
+    account = models.ForeignKey(Account, on_delete=models.CASCADE)
+    post = models.ForeignKey(Post, on_delete=models.CASCADE)
+    point = models.IntegerField(default=1)
+
+    class Meta:
+        unique_together = ('account', 'post',)
+
+class CommentVote(models.Model):
+    account = models.ForeignKey(Account, on_delete=models.CASCADE)
+    comment = models.ForeignKey(Comment, on_delete=models.CASCADE)
+    point = models.IntegerField(default=1)
+
+    class Meta:
+        unique_together = ('account', 'comment',)
+
+class Configuration(models.Model):
+    code_name = models.CharField(max_length=100, blank=False)
+    value = models.CharField(max_length=1000, blank=True)
+
+    def __str__(self):
+        return "{}".format(self.code_name)
+
+    class Meta:
+        permissions = (
+            ("change_configurations", "Can change the configurations of the booru"),
+        )
```

### Comparing `Boorunaut-0.4.3/booru/setup/start_project.py` & `Boorunaut-0.5.0/booru/setup/start_project.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-from __future__ import unicode_literals, absolute_import, print_function
-
-import os
-import functools
-import argparse
-from importlib import import_module
-from subprocess import call
-
-
-def create_project(project_name, path, exit_err):
-    try:
-        import_module(project_name)
-    except ImportError:
-        pass
-    else:
-        exit_err(
-            "'%s' conflicts with the name of an existing "
-            "Python module and cannot be used as a project "
-            "name" % project_name)
-
-    extra_path = os.path.dirname(os.path.dirname(__file__))
-    template_path = os.path.join(extra_path, 'setup/project_template')
-
-    command = [
-        'django-admin',
-        'startproject',
-        '--template=' + template_path,
-        project_name]
-
-    if path:
-        command.append(path)
-
-    print('Creating a new Boorunaut project...')
-
-    if call(command) != 0:
-        exit_err(
-            "Tried to run \"%s\" but it "
-            "returned an error "
-            "(should be printed above)\n" % ' '.join(command))
-
-    print('Project created!')
-
-
-def execute_from_command_line():
-    parser = argparse.ArgumentParser(description='Boorunaut commands')
-    subparsers = parser.add_subparsers(help='sub-command help')
-    start_parser = subparsers.add_parser(
-        'startproject', help='creates a Boorunaut project directory structure')
-    start_parser.add_argument(
-        'project_name', help='name of the project')
-    start_parser.add_argument(
-        '--path', default=None, help='optional destination directory')
-    args = parser.parse_args()
-    create_project(
-        project_name=args.project_name,
-        path=args.path,
-        exit_err=functools.partial(parser.exit, 1))
-
-
-def main():
-    execute_from_command_line()
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+from __future__ import unicode_literals, absolute_import, print_function
+
+import os
+import functools
+import argparse
+from importlib import import_module
+from subprocess import call
+
+
+def create_project(project_name, path, exit_err):
+    try:
+        import_module(project_name)
+    except ImportError:
+        pass
+    else:
+        exit_err(
+            "'%s' conflicts with the name of an existing "
+            "Python module and cannot be used as a project "
+            "name" % project_name)
+
+    extra_path = os.path.dirname(os.path.dirname(__file__))
+    template_path = os.path.join(extra_path, 'setup/project_template')
+
+    command = [
+        'django-admin',
+        'startproject',
+        '--template=' + template_path,
+        project_name]
+
+    if path:
+        command.append(path)
+
+    print('Creating a new Boorunaut project...')
+
+    if call(command) != 0:
+        exit_err(
+            "Tried to run \"%s\" but it "
+            "returned an error "
+            "(should be printed above)\n" % ' '.join(command))
+
+    print('Project created!')
+
+
+def execute_from_command_line():
+    parser = argparse.ArgumentParser(description='Boorunaut commands')
+    subparsers = parser.add_subparsers(help='sub-command help')
+    start_parser = subparsers.add_parser(
+        'startproject', help='creates a Boorunaut project directory structure')
+    start_parser.add_argument(
+        'project_name', help='name of the project')
+    start_parser.add_argument(
+        '--path', default=None, help='optional destination directory')
+    args = parser.parse_args()
+    create_project(
+        project_name=args.project_name,
+        path=args.path,
+        exit_err=functools.partial(parser.exit, 1))
+
+
+def main():
+    execute_from_command_line()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css` & `Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-/*! ========================================================================
- * Bootstrap Toggle: bootstrap-toggle.css v2.2.0
- * http://www.bootstraptoggle.com
- * ========================================================================
- * Copyright 2014 Min Hur, The New York Times Company
- * Licensed under MIT
- * ========================================================================
- * Modified for Boorunaut
- * ======================================================================== */
-.checkbox label .toggle,.checkbox-inline .toggle{margin-left:-20px;margin-right:5px}
-.toggle{position:relative;overflow:hidden}
-.toggle input[type=checkbox]{display:none}
-.toggle-group{position:absolute;width:200%;top:0;bottom:0;left:0;transition:left .35s;-webkit-transition:left .35s;-moz-user-select:none;-webkit-user-select:none}
-.toggle.off .toggle-group{left:-100%}
-.toggle-on{position:absolute;top:0;bottom:0;left:0;right:50%;margin:0;border:0;border-radius:0}
-.toggle-off{position:absolute;top:0;bottom:0;left:50%;right:0;margin:0;border:0;border-radius:0}
-.toggle-handle{position:relative;margin:0 auto;padding-top:0;padding-bottom:0;height:100%;width:0;border-width:0 1px}
-.toggle.btn{min-width:59px;min-height:34px}
-.toggle-on.btn{padding-right:24px}
-.toggle-off.btn{padding-left:24px}
-.toggle.btn-lg{min-width:79px;min-height:45px}
-.toggle-on.btn-lg{padding-right:31px}
-.toggle-off.btn-lg{padding-left:31px}
-.toggle-handle.btn-lg{width:40px}
-.toggle.btn-sm{min-width:50px;min-height:30px}
-.toggle-on.btn-sm{padding-right:20px}
-.toggle-off.btn-sm{padding-left:20px}
-.toggle.btn-xs{min-width:35px;min-height:22px}
-.toggle-on.btn-xs{padding-right:12px}
+/*! ========================================================================
+ * Bootstrap Toggle: bootstrap-toggle.css v2.2.0
+ * http://www.bootstraptoggle.com
+ * ========================================================================
+ * Copyright 2014 Min Hur, The New York Times Company
+ * Licensed under MIT
+ * ========================================================================
+ * Modified for Boorunaut
+ * ======================================================================== */
+.checkbox label .toggle,.checkbox-inline .toggle{margin-left:-20px;margin-right:5px}
+.toggle{position:relative;overflow:hidden}
+.toggle input[type=checkbox]{display:none}
+.toggle-group{position:absolute;width:200%;top:0;bottom:0;left:0;transition:left .35s;-webkit-transition:left .35s;-moz-user-select:none;-webkit-user-select:none}
+.toggle.off .toggle-group{left:-100%}
+.toggle-on{position:absolute;top:0;bottom:0;left:0;right:50%;margin:0;border:0;border-radius:0}
+.toggle-off{position:absolute;top:0;bottom:0;left:50%;right:0;margin:0;border:0;border-radius:0}
+.toggle-handle{position:relative;margin:0 auto;padding-top:0;padding-bottom:0;height:100%;width:0;border-width:0 1px}
+.toggle.btn{min-width:59px;min-height:34px}
+.toggle-on.btn{padding-right:24px}
+.toggle-off.btn{padding-left:24px}
+.toggle.btn-lg{min-width:79px;min-height:45px}
+.toggle-on.btn-lg{padding-right:31px}
+.toggle-off.btn-lg{padding-left:31px}
+.toggle-handle.btn-lg{width:40px}
+.toggle.btn-sm{min-width:50px;min-height:30px}
+.toggle-on.btn-sm{padding-right:20px}
+.toggle-off.btn-sm{padding-left:20px}
+.toggle.btn-xs{min-width:35px;min-height:22px}
+.toggle-on.btn-xs{padding-right:12px}
 .toggle-off.btn-xs{padding-left:12px}
```

### Comparing `Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.js` & `Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,183 +1,183 @@
-/*! ========================================================================
- * Bootstrap Toggle: bootstrap-toggle.js v2.2.0
- * http://www.bootstraptoggle.com
- * ========================================================================
- * Copyright 2014 Min Hur, The New York Times Company
- * Licensed under MIT
- * ======================================================================== */
-
-
-+ function($) {
-    'use strict';
-
-    // TOGGLE PUBLIC CLASS DEFINITION
-    // ==============================
-
-    var Toggle = function(element, options) {
-        this.$element = $(element)
-        this.options = $.extend({}, this.defaults(), options)
-        this.render()
-    }
-
-    Toggle.VERSION = '2.2.0'
-
-    Toggle.DEFAULTS = {
-        on: 'On',
-        off: 'Off',
-        onstyle: 'primary',
-        offstyle: 'default',
-        size: 'normal',
-        style: '',
-        width: null,
-        height: null
-    }
-
-    Toggle.prototype.defaults = function() {
-        return {
-            on: this.$element.attr('data-on') || Toggle.DEFAULTS.on,
-            off: this.$element.attr('data-off') || Toggle.DEFAULTS.off,
-            onstyle: this.$element.attr('data-onstyle') || Toggle.DEFAULTS.onstyle,
-            offstyle: this.$element.attr('data-offstyle') || Toggle.DEFAULTS.offstyle,
-            size: this.$element.attr('data-size') || Toggle.DEFAULTS.size,
-            style: this.$element.attr('data-style') || Toggle.DEFAULTS.style,
-            width: this.$element.attr('data-width') || Toggle.DEFAULTS.width,
-            height: this.$element.attr('data-height') || Toggle.DEFAULTS.height
-        }
-    }
-
-    Toggle.prototype.render = function() {
-        this._onstyle = 'btn-' + this.options.onstyle
-        this._offstyle = 'btn-' + this.options.offstyle
-        var size = this.options.size === 'large' ? 'btn-lg' :
-            this.options.size === 'small' ? 'btn-sm' :
-            this.options.size === 'mini' ? 'btn-xs' :
-            ''
-        var $toggleOn = $('<label class="btn">').html(this.options.on)
-            .addClass(this._onstyle + ' ' + size)
-        var $toggleOff = $('<label class="btn">').html(this.options.off)
-            .addClass(this._offstyle + ' ' + size + ' active')
-        var $toggleHandle = $('<span class="toggle-handle btn btn-default">')
-            .addClass(size)
-        var $toggleGroup = $('<div class="toggle-group">')
-            .append($toggleOn, $toggleOff, $toggleHandle)
-        var $toggle = $('<div class="toggle btn" data-toggle="toggle">')
-            .addClass(this.$element.prop('checked') ? this._onstyle : this._offstyle + ' off')
-            .addClass(size).addClass(this.options.style)
-
-        this.$element.wrap($toggle)
-        $.extend(this, {
-            $toggle: this.$element.parent(),
-            $toggleOn: $toggleOn,
-            $toggleOff: $toggleOff,
-            $toggleGroup: $toggleGroup
-        })
-        this.$toggle.append($toggleGroup)
-
-        var width = this.options.width || Math.max($toggleOn.outerWidth(), $toggleOff.outerWidth()) + ($toggleHandle.outerWidth() / 2)
-        var height = this.options.height || Math.max($toggleOn.outerHeight(), $toggleOff.outerHeight())
-        $toggleOn.addClass('toggle-on')
-        $toggleOff.addClass('toggle-off')
-        this.$toggle.css({
-            width: width,
-            height: height
-        })
-        if (this.options.height) {
-            $toggleOn.css('line-height', $toggleOn.height() + 'px')
-            $toggleOff.css('line-height', $toggleOff.height() + 'px')
-        }
-        this.update(true)
-        this.trigger(true)
-    }
-
-    Toggle.prototype.toggle = function() {
-        if (this.$element.prop('checked')) this.off()
-        else this.on()
-    }
-
-    Toggle.prototype.on = function(silent) {
-        if (this.$element.prop('disabled')) return false
-        this.$toggle.removeClass(this._offstyle + ' off').addClass(this._onstyle)
-        this.$element.prop('checked', true)
-        if (!silent) this.trigger()
-    }
-
-    Toggle.prototype.off = function(silent) {
-        if (this.$element.prop('disabled')) return false
-        this.$toggle.removeClass(this._onstyle).addClass(this._offstyle + ' off')
-        this.$element.prop('checked', false)
-        if (!silent) this.trigger()
-    }
-
-    Toggle.prototype.enable = function() {
-        this.$toggle.removeAttr('disabled')
-        this.$element.prop('disabled', false)
-    }
-
-    Toggle.prototype.disable = function() {
-        this.$toggle.attr('disabled', 'disabled')
-        this.$element.prop('disabled', true)
-    }
-
-    Toggle.prototype.update = function(silent) {
-        if (this.$element.prop('disabled')) this.disable()
-        else this.enable()
-        if (this.$element.prop('checked')) this.on(silent)
-        else this.off(silent)
-    }
-
-    Toggle.prototype.trigger = function(silent) {
-        this.$element.off('change.bs.toggle')
-        if (!silent) this.$element.change()
-        this.$element.on('change.bs.toggle', $.proxy(function() {
-            this.update()
-        }, this))
-    }
-
-    Toggle.prototype.destroy = function() {
-        this.$element.off('change.bs.toggle')
-        this.$toggleGroup.remove()
-        this.$element.removeData('bs.toggle')
-        this.$element.unwrap()
-    }
-
-    // TOGGLE PLUGIN DEFINITION
-    // ========================
-
-    function Plugin(option) {
-        return this.each(function() {
-            var $this = $(this)
-            var data = $this.data('bs.toggle')
-            var options = typeof option == 'object' && option
-
-            if (!data) $this.data('bs.toggle', (data = new Toggle(this, options)))
-            if (typeof option == 'string' && data[option]) data[option]()
-        })
-    }
-
-    var old = $.fn.bootstrapToggle
-
-    $.fn.bootstrapToggle = Plugin
-    $.fn.bootstrapToggle.Constructor = Toggle
-
-    // TOGGLE NO CONFLICT
-    // ==================
-
-    $.fn.toggle.noConflict = function() {
-        $.fn.bootstrapToggle = old
-        return this
-    }
-
-    // TOGGLE DATA-API
-    // ===============
-
-    $(function() {
-        $('input[type=checkbox][data-toggle^=toggle]').bootstrapToggle()
-    })
-
-    $(document).on('click.bs.toggle', 'div[data-toggle^=toggle]', function(e) {
-        var $checkbox = $(this).find('input[type=checkbox]')
-        $checkbox.bootstrapToggle('toggle')
-        e.preventDefault()
-    })
-
+/*! ========================================================================
+ * Bootstrap Toggle: bootstrap-toggle.js v2.2.0
+ * http://www.bootstraptoggle.com
+ * ========================================================================
+ * Copyright 2014 Min Hur, The New York Times Company
+ * Licensed under MIT
+ * ======================================================================== */
+
+
++ function($) {
+    'use strict';
+
+    // TOGGLE PUBLIC CLASS DEFINITION
+    // ==============================
+
+    var Toggle = function(element, options) {
+        this.$element = $(element)
+        this.options = $.extend({}, this.defaults(), options)
+        this.render()
+    }
+
+    Toggle.VERSION = '2.2.0'
+
+    Toggle.DEFAULTS = {
+        on: 'On',
+        off: 'Off',
+        onstyle: 'primary',
+        offstyle: 'default',
+        size: 'normal',
+        style: '',
+        width: null,
+        height: null
+    }
+
+    Toggle.prototype.defaults = function() {
+        return {
+            on: this.$element.attr('data-on') || Toggle.DEFAULTS.on,
+            off: this.$element.attr('data-off') || Toggle.DEFAULTS.off,
+            onstyle: this.$element.attr('data-onstyle') || Toggle.DEFAULTS.onstyle,
+            offstyle: this.$element.attr('data-offstyle') || Toggle.DEFAULTS.offstyle,
+            size: this.$element.attr('data-size') || Toggle.DEFAULTS.size,
+            style: this.$element.attr('data-style') || Toggle.DEFAULTS.style,
+            width: this.$element.attr('data-width') || Toggle.DEFAULTS.width,
+            height: this.$element.attr('data-height') || Toggle.DEFAULTS.height
+        }
+    }
+
+    Toggle.prototype.render = function() {
+        this._onstyle = 'btn-' + this.options.onstyle
+        this._offstyle = 'btn-' + this.options.offstyle
+        var size = this.options.size === 'large' ? 'btn-lg' :
+            this.options.size === 'small' ? 'btn-sm' :
+            this.options.size === 'mini' ? 'btn-xs' :
+            ''
+        var $toggleOn = $('<label class="btn">').html(this.options.on)
+            .addClass(this._onstyle + ' ' + size)
+        var $toggleOff = $('<label class="btn">').html(this.options.off)
+            .addClass(this._offstyle + ' ' + size + ' active')
+        var $toggleHandle = $('<span class="toggle-handle btn btn-default">')
+            .addClass(size)
+        var $toggleGroup = $('<div class="toggle-group">')
+            .append($toggleOn, $toggleOff, $toggleHandle)
+        var $toggle = $('<div class="toggle btn" data-toggle="toggle">')
+            .addClass(this.$element.prop('checked') ? this._onstyle : this._offstyle + ' off')
+            .addClass(size).addClass(this.options.style)
+
+        this.$element.wrap($toggle)
+        $.extend(this, {
+            $toggle: this.$element.parent(),
+            $toggleOn: $toggleOn,
+            $toggleOff: $toggleOff,
+            $toggleGroup: $toggleGroup
+        })
+        this.$toggle.append($toggleGroup)
+
+        var width = this.options.width || Math.max($toggleOn.outerWidth(), $toggleOff.outerWidth()) + ($toggleHandle.outerWidth() / 2)
+        var height = this.options.height || Math.max($toggleOn.outerHeight(), $toggleOff.outerHeight())
+        $toggleOn.addClass('toggle-on')
+        $toggleOff.addClass('toggle-off')
+        this.$toggle.css({
+            width: width,
+            height: height
+        })
+        if (this.options.height) {
+            $toggleOn.css('line-height', $toggleOn.height() + 'px')
+            $toggleOff.css('line-height', $toggleOff.height() + 'px')
+        }
+        this.update(true)
+        this.trigger(true)
+    }
+
+    Toggle.prototype.toggle = function() {
+        if (this.$element.prop('checked')) this.off()
+        else this.on()
+    }
+
+    Toggle.prototype.on = function(silent) {
+        if (this.$element.prop('disabled')) return false
+        this.$toggle.removeClass(this._offstyle + ' off').addClass(this._onstyle)
+        this.$element.prop('checked', true)
+        if (!silent) this.trigger()
+    }
+
+    Toggle.prototype.off = function(silent) {
+        if (this.$element.prop('disabled')) return false
+        this.$toggle.removeClass(this._onstyle).addClass(this._offstyle + ' off')
+        this.$element.prop('checked', false)
+        if (!silent) this.trigger()
+    }
+
+    Toggle.prototype.enable = function() {
+        this.$toggle.removeAttr('disabled')
+        this.$element.prop('disabled', false)
+    }
+
+    Toggle.prototype.disable = function() {
+        this.$toggle.attr('disabled', 'disabled')
+        this.$element.prop('disabled', true)
+    }
+
+    Toggle.prototype.update = function(silent) {
+        if (this.$element.prop('disabled')) this.disable()
+        else this.enable()
+        if (this.$element.prop('checked')) this.on(silent)
+        else this.off(silent)
+    }
+
+    Toggle.prototype.trigger = function(silent) {
+        this.$element.off('change.bs.toggle')
+        if (!silent) this.$element.change()
+        this.$element.on('change.bs.toggle', $.proxy(function() {
+            this.update()
+        }, this))
+    }
+
+    Toggle.prototype.destroy = function() {
+        this.$element.off('change.bs.toggle')
+        this.$toggleGroup.remove()
+        this.$element.removeData('bs.toggle')
+        this.$element.unwrap()
+    }
+
+    // TOGGLE PLUGIN DEFINITION
+    // ========================
+
+    function Plugin(option) {
+        return this.each(function() {
+            var $this = $(this)
+            var data = $this.data('bs.toggle')
+            var options = typeof option == 'object' && option
+
+            if (!data) $this.data('bs.toggle', (data = new Toggle(this, options)))
+            if (typeof option == 'string' && data[option]) data[option]()
+        })
+    }
+
+    var old = $.fn.bootstrapToggle
+
+    $.fn.bootstrapToggle = Plugin
+    $.fn.bootstrapToggle.Constructor = Toggle
+
+    // TOGGLE NO CONFLICT
+    // ==================
+
+    $.fn.toggle.noConflict = function() {
+        $.fn.bootstrapToggle = old
+        return this
+    }
+
+    // TOGGLE DATA-API
+    // ===============
+
+    $(function() {
+        $('input[type=checkbox][data-toggle^=toggle]').bootstrapToggle()
+    })
+
+    $(document).on('click.bs.toggle', 'div[data-toggle^=toggle]', function(e) {
+        var $checkbox = $(this).find('input[type=checkbox]')
+        $checkbox.bootstrapToggle('toggle')
+        e.preventDefault()
+    })
+
 }(jQuery);
```

### Comparing `Boorunaut-0.4.3/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js` & `Boorunaut-0.5.0/booru/static/booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,93 +1,93 @@
-/*! ========================================================================
- * Bootstrap Toggle: bootstrap-toggle.js v2.2.0
- * http://www.bootstraptoggle.com
- * ========================================================================
- * Copyright 2014 Min Hur, The New York Times Company
- * Licensed under MIT
- * ========================================================================
- * Modified for Boorunaut
- * ======================================================================== */
-+ function(a) {
-    "use strict";
-
-    function b(b) {
-        return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.toggle"),
-                f = "object" == typeof b && b;
-            e || d.data("bs.toggle", e = new c(this, f)), "string" == typeof b && e[b] && e[b]()
-        })
-    }
-    var c = function(b, c) {
-        this.$element = a(b), this.options = a.extend({}, this.defaults(), c), this.render()
-    };
-    c.VERSION = "2.2.0", c.DEFAULTS = {
-        on: "On",
-        off: "Off",
-        onstyle: "primary",
-        offstyle: "secondary",
-        size: "normal",
-        style: "",
-        width: null,
-        height: null
-    }, c.prototype.defaults = function() {
-        return {
-            on: this.$element.attr("data-on") || c.DEFAULTS.on,
-            off: this.$element.attr("data-off") || c.DEFAULTS.off,
-            onstyle: this.$element.attr("data-onstyle") || c.DEFAULTS.onstyle,
-            offstyle: this.$element.attr("data-offstyle") || c.DEFAULTS.offstyle,
-            size: this.$element.attr("data-size") || c.DEFAULTS.size,
-            style: this.$element.attr("data-style") || c.DEFAULTS.style,
-            width: this.$element.attr("data-width") || c.DEFAULTS.width,
-            height: this.$element.attr("data-height") || c.DEFAULTS.height
-        }
-    }, c.prototype.render = function() {
-        this._onstyle = "btn-" + this.options.onstyle, this._offstyle = "btn-" + this.options.offstyle;
-        var b = "large" === this.options.size ? "btn-lg" : "small" === this.options.size ? "btn-sm" : "mini" === this.options.size ? "btn-xs" : "",
-            c = a('<label class="btn">').html(this.options.on).addClass(this._onstyle + " " + b),
-            d = a('<label class="btn">').html(this.options.off).addClass(this._offstyle + " " + b + " active"),
-            e = a('<span class="toggle-handle btn btn-light">').addClass(b),
-            f = a('<div class="toggle-group">').append(c, d, e),
-            g = a('<div class="toggle btn" data-toggle="toggle">').addClass(this.$element.prop("checked") ? this._onstyle : this._offstyle + " off").addClass(b).addClass(this.options.style);
-        this.$element.wrap(g), a.extend(this, {
-            $toggle: this.$element.parent(),
-            $toggleOn: c,
-            $toggleOff: d,
-            $toggleGroup: f
-        }), this.$toggle.append(f);
-        var h = this.options.width || Math.max(c.outerWidth(), d.outerWidth()) + e.outerWidth() / 2,
-            i = this.options.height || Math.max(c.outerHeight(), d.outerHeight());
-        c.addClass("toggle-on"), d.addClass("toggle-off"), this.$toggle.css({
-            width: h,
-            height: i
-        }), this.options.height && (c.css("line-height", c.height() + "px"), d.css("line-height", d.height() + "px")), this.update(!0), this.trigger(!0)
-    }, c.prototype.toggle = function() {
-        this.$element.prop("checked") ? this.off() : this.on()
-    }, c.prototype.on = function(a) {
-        return this.$element.prop("disabled") ? !1 : (this.$toggle.removeClass(this._offstyle + " off").addClass(this._onstyle), this.$element.prop("checked", !0), void(a || this.trigger()))
-    }, c.prototype.off = function(a) {
-        return this.$element.prop("disabled") ? !1 : (this.$toggle.removeClass(this._onstyle).addClass(this._offstyle + " off"), this.$element.prop("checked", !1), void(a || this.trigger()))
-    }, c.prototype.enable = function() {
-        this.$toggle.removeAttr("disabled"), this.$element.prop("disabled", !1)
-    }, c.prototype.disable = function() {
-        this.$toggle.attr("disabled", "disabled"), this.$element.prop("disabled", !0)
-    }, c.prototype.update = function(a) {
-        this.$element.prop("disabled") ? this.disable() : this.enable(), this.$element.prop("checked") ? this.on(a) : this.off(a)
-    }, c.prototype.trigger = function(b) {
-        this.$element.off("change.bs.toggle"), b || this.$element.change(), this.$element.on("change.bs.toggle", a.proxy(function() {
-            this.update()
-        }, this))
-    }, c.prototype.destroy = function() {
-        this.$element.off("change.bs.toggle"), this.$toggleGroup.remove(), this.$element.removeData("bs.toggle"), this.$element.unwrap()
-    };
-    var d = a.fn.bootstrapToggle;
-    a.fn.bootstrapToggle = b, a.fn.bootstrapToggle.Constructor = c, a.fn.toggle.noConflict = function() {
-        return a.fn.bootstrapToggle = d, this
-    }, a(function() {
-        a("input[type=checkbox][data-toggle^=toggle]").bootstrapToggle()
-    }), a(document).on("click.bs.toggle", "div[data-toggle^=toggle]", function(b) {
-        var c = a(this).find("input[type=checkbox]");
-        c.bootstrapToggle("toggle"), b.preventDefault()
-    })
-}(jQuery);
+/*! ========================================================================
+ * Bootstrap Toggle: bootstrap-toggle.js v2.2.0
+ * http://www.bootstraptoggle.com
+ * ========================================================================
+ * Copyright 2014 Min Hur, The New York Times Company
+ * Licensed under MIT
+ * ========================================================================
+ * Modified for Boorunaut
+ * ======================================================================== */
++ function(a) {
+    "use strict";
+
+    function b(b) {
+        return this.each(function() {
+            var d = a(this),
+                e = d.data("bs.toggle"),
+                f = "object" == typeof b && b;
+            e || d.data("bs.toggle", e = new c(this, f)), "string" == typeof b && e[b] && e[b]()
+        })
+    }
+    var c = function(b, c) {
+        this.$element = a(b), this.options = a.extend({}, this.defaults(), c), this.render()
+    };
+    c.VERSION = "2.2.0", c.DEFAULTS = {
+        on: "On",
+        off: "Off",
+        onstyle: "primary",
+        offstyle: "secondary",
+        size: "normal",
+        style: "",
+        width: null,
+        height: null
+    }, c.prototype.defaults = function() {
+        return {
+            on: this.$element.attr("data-on") || c.DEFAULTS.on,
+            off: this.$element.attr("data-off") || c.DEFAULTS.off,
+            onstyle: this.$element.attr("data-onstyle") || c.DEFAULTS.onstyle,
+            offstyle: this.$element.attr("data-offstyle") || c.DEFAULTS.offstyle,
+            size: this.$element.attr("data-size") || c.DEFAULTS.size,
+            style: this.$element.attr("data-style") || c.DEFAULTS.style,
+            width: this.$element.attr("data-width") || c.DEFAULTS.width,
+            height: this.$element.attr("data-height") || c.DEFAULTS.height
+        }
+    }, c.prototype.render = function() {
+        this._onstyle = "btn-" + this.options.onstyle, this._offstyle = "btn-" + this.options.offstyle;
+        var b = "large" === this.options.size ? "btn-lg" : "small" === this.options.size ? "btn-sm" : "mini" === this.options.size ? "btn-xs" : "",
+            c = a('<label class="btn">').html(this.options.on).addClass(this._onstyle + " " + b),
+            d = a('<label class="btn">').html(this.options.off).addClass(this._offstyle + " " + b + " active"),
+            e = a('<span class="toggle-handle btn btn-light">').addClass(b),
+            f = a('<div class="toggle-group">').append(c, d, e),
+            g = a('<div class="toggle btn" data-toggle="toggle">').addClass(this.$element.prop("checked") ? this._onstyle : this._offstyle + " off").addClass(b).addClass(this.options.style);
+        this.$element.wrap(g), a.extend(this, {
+            $toggle: this.$element.parent(),
+            $toggleOn: c,
+            $toggleOff: d,
+            $toggleGroup: f
+        }), this.$toggle.append(f);
+        var h = this.options.width || Math.max(c.outerWidth(), d.outerWidth()) + e.outerWidth() / 2,
+            i = this.options.height || Math.max(c.outerHeight(), d.outerHeight());
+        c.addClass("toggle-on"), d.addClass("toggle-off"), this.$toggle.css({
+            width: h,
+            height: i
+        }), this.options.height && (c.css("line-height", c.height() + "px"), d.css("line-height", d.height() + "px")), this.update(!0), this.trigger(!0)
+    }, c.prototype.toggle = function() {
+        this.$element.prop("checked") ? this.off() : this.on()
+    }, c.prototype.on = function(a) {
+        return this.$element.prop("disabled") ? !1 : (this.$toggle.removeClass(this._offstyle + " off").addClass(this._onstyle), this.$element.prop("checked", !0), void(a || this.trigger()))
+    }, c.prototype.off = function(a) {
+        return this.$element.prop("disabled") ? !1 : (this.$toggle.removeClass(this._onstyle).addClass(this._offstyle + " off"), this.$element.prop("checked", !1), void(a || this.trigger()))
+    }, c.prototype.enable = function() {
+        this.$toggle.removeAttr("disabled"), this.$element.prop("disabled", !1)
+    }, c.prototype.disable = function() {
+        this.$toggle.attr("disabled", "disabled"), this.$element.prop("disabled", !0)
+    }, c.prototype.update = function(a) {
+        this.$element.prop("disabled") ? this.disable() : this.enable(), this.$element.prop("checked") ? this.on(a) : this.off(a)
+    }, c.prototype.trigger = function(b) {
+        this.$element.off("change.bs.toggle"), b || this.$element.change(), this.$element.on("change.bs.toggle", a.proxy(function() {
+            this.update()
+        }, this))
+    }, c.prototype.destroy = function() {
+        this.$element.off("change.bs.toggle"), this.$toggleGroup.remove(), this.$element.removeData("bs.toggle"), this.$element.unwrap()
+    };
+    var d = a.fn.bootstrapToggle;
+    a.fn.bootstrapToggle = b, a.fn.bootstrapToggle.Constructor = c, a.fn.toggle.noConflict = function() {
+        return a.fn.bootstrapToggle = d, this
+    }, a(function() {
+        a("input[type=checkbox][data-toggle^=toggle]").bootstrapToggle()
+    }), a(document).on("click.bs.toggle", "div[data-toggle^=toggle]", function(b) {
+        var c = a(this).find("input[type=checkbox]");
+        c.bootstrapToggle("toggle"), b.preventDefault()
+    })
+}(jQuery);
 //# sourceMappingURL=bootstrap-toggle.min.js.map
```

### Comparing `Boorunaut-0.4.3/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css` & `Boorunaut-0.5.0/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css`

 * *Files identical despite different names*

### Comparing `Boorunaut-0.4.3/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js` & `Boorunaut-0.5.0/booru/static/booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js`

 * *Files identical despite different names*

### Comparing `Boorunaut-0.4.3/booru/static/booru/js/tag_search_autocomplete.js` & `Boorunaut-0.5.0/booru/static/booru/js/tag_search_autocomplete.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
-$(function() {
-    $('.tag-search').tagsInput({
-        'autocomplete_url': tag_search_url,
-        'delimiter': [' '], // Or a string with a single delimiter. Ex: ';'
-        'width': '100%',
-        'height': '45px',
-    });
-
-    $('#tags_tagsinput').addClass("col-md-9");
-
-    $('#id_tags').tagsInput({
-        'autocomplete_url': tag_search_url,
-        'delimiter': [' '], // Or a string with a single delimiter. Ex: ';'
-        'height': '100%',
-        'width': '100%'
-    });
-
-    let searchParams = new URLSearchParams(window.location.search);
-    if (searchParams.has('tags')) {
-        let tags = searchParams.get('tags');
-        $('.tag-search').importTags(tags);
-    }
+$(function() {
+    $('.tag-search').tagsInput({
+        'autocomplete_url': tag_search_url,
+        'delimiter': [' '], // Or a string with a single delimiter. Ex: ';'
+        'width': '100%',
+        'height': '45px',
+    });
+
+    $('#tags_tagsinput').addClass("col-md-9");
+
+    $('#id_tags').tagsInput({
+        'autocomplete_url': tag_search_url,
+        'delimiter': [' '], // Or a string with a single delimiter. Ex: ';'
+        'height': '100%',
+        'width': '100%'
+    });
+
+    let searchParams = new URLSearchParams(window.location.search);
+    if (searchParams.has('tags')) {
+        let tags = searchParams.get('tags');
+        $('.tag-search').importTags(tags);
+    }
 });
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/account/login.html` & `Boorunaut-0.5.0/booru/templates/booru/account/login.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-<div class="container">
-    <div class="row">
-        <div class="col">
-            <h1>Login</h1>
-
-            <form method="post" enctype="multipart/form-data">
-                {% csrf_token %}
-
-                <div class="form-group row">
-                    <label for="{{ form.username.auto_id }}" class="col-1 col-form-label">{{ form.username.label }}</label>
-                    
-                    <div class="col-4">
-                        {{form.username}}
-                        <span class="custom-file-control"></span>
-                    </div>
-
-                    {% if form.username.errors %}
-                    <div class="col-md-offset-2 col-8 text-danger small">
-                        {{form.username.errors}}
-                    </div>
-                    {% endif %}
-                </div>
-
-                <div class="form-group row">
-                    <label for="{{ form.password.auto_id }}" class="col-1 col-form-label">{{ form.password.label }}</label>
-                    
-                    <div class="col-4">
-                        {{form.password}}
-                        <span class="custom-file-control"></span>
-                    </div>
-
-                    {% if not form.username.errors and form.errors %}
-                    <div class="col-md-offset-2 col-8 text-danger small">
-                        The given password is incorrect.
-                    </div>
-                    {% endif %}
-                </div>
-
-                <button type="submit" class="btn btn-primary">Login</button>
-            </form>
-        </div>
-    </div>
-</div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+<div class="container">
+    <div class="row">
+        <div class="col">
+            <h1>Login</h1>
+
+            <form method="post" enctype="multipart/form-data">
+                {% csrf_token %}
+
+                <div class="form-group row">
+                    <label for="{{ form.username.auto_id }}" class="col-1 col-form-label">{{ form.username.label }}</label>
+                    
+                    <div class="col-4">
+                        {{form.username}}
+                        <span class="custom-file-control"></span>
+                    </div>
+
+                    {% if form.username.errors %}
+                    <div class="col-md-offset-2 col-8 text-danger small">
+                        {{form.username.errors}}
+                    </div>
+                    {% endif %}
+                </div>
+
+                <div class="form-group row">
+                    <label for="{{ form.password.auto_id }}" class="col-1 col-form-label">{{ form.password.label }}</label>
+                    
+                    <div class="col-4">
+                        {{form.password}}
+                        <span class="custom-file-control"></span>
+                    </div>
+
+                    {% if not form.username.errors and form.errors %}
+                    <div class="col-md-offset-2 col-8 text-danger small">
+                        The given password is incorrect.
+                    </div>
+                    {% endif %}
+                </div>
+
+                <button type="submit" class="btn btn-primary">Login</button>
+            </form>
+        </div>
+    </div>
+</div>
 {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/account/register.html` & `Boorunaut-0.5.0/booru/templates/booru/account/register.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-<div class="container">
-    <div class="row">
-        <div class="col">
-            <h1>Register</h1>
-            <p class="text-muted">
-                With a account, you are able to comment, upload images and mark favorites. These actions are public and are subject to web-crawlers. <br/>
-                Choose a username you are comfortable being associated with.
-            </p>
-
-            <form method="post" enctype="multipart/form-data">
-                {% csrf_token %}
-
-                <div class="form-group row">
-                    <label for="{{ form.username.auto_id }}" class="col-1 col-form-label">{{ form.username.label }}</label>
-                    
-                    <div class="col-4">
-                        {{form.username}}
-                        <span class="custom-file-control"></span>
-                    </div>
-
-                    {% if form.username.errors %}
-                    <div class="col-md-offset-2 col-8 text-danger small">
-                        {{form.username.errors}}
-                    </div>
-                    {% endif %}
-                </div>
-
-                <div class="form-group row">
-                    <label for="{{ form.email.auto_id }}" class="col-1 col-form-label">{{ form.email.label }}</label>
-                    
-                    <div class="col-4">
-                        {{form.email}}
-                        <span class="custom-file-control"></span>
-                    </div>
-
-                    {% if form.email.errors %}
-                    <div class="col-md-offset-2 col-8 text-danger small">
-                        {{form.email.errors}}
-                    </div>
-                    {% endif %}
-                </div>
-
-                <div class="form-group row">
-                    <label for="{{ form.password1.auto_id }}" class="col-1 col-form-label">{{ form.password1.label }}</label>
-                    
-                    <div class="col-4">
-                        {{form.password1}}
-                        <span class="custom-file-control"></span>
-                    </div>
-
-                    {% if form.password1.errors %}
-                    <div class="col-md-offset-2 col-8 text-danger small">
-                        {{form.password1.errors}}
-                    </div>
-                    {% endif %}
-                </div>
-
-                <div class="form-group row">
-                    <label for="{{ form.password2.auto_id }}" class="col-1 col-form-label">{{ form.password2.label }}</label>
-                    
-                    <div class="col-4">
-                        {{form.password2}}
-                        <span class="custom-file-control"></span>
-                    </div>
-
-                    {% if form.password2.errors %}
-                    <div class="col-md-offset-2 col-8 text-danger small">
-                        {{form.password2.errors}}
-                    </div>
-                    {% endif %}
-                </div>
-
-                <button type="submit" class="btn btn-primary">Register</button>
-            </form>
-        </div>
-    </div>
-</div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+<div class="container">
+    <div class="row">
+        <div class="col">
+            <h1>Register</h1>
+            <p class="text-muted">
+                With an account, you are able to comment, upload images and mark favorites. These actions are public and are subject to web-crawlers. <br/>
+                Choose a username you are comfortable being associated with.
+            </p>
+
+            <form method="post" enctype="multipart/form-data">
+                {% csrf_token %}
+
+                <div class="form-group row">
+                    <label for="{{ form.username.auto_id }}" class="col-1 col-form-label">{{ form.username.label }}</label>
+                    
+                    <div class="col-4">
+                        {{form.username}}
+                        <span class="custom-file-control"></span>
+                    </div>
+
+                    {% if form.username.errors %}
+                    <div class="col-md-offset-2 col-8 text-danger small">
+                        {{form.username.errors}}
+                    </div>
+                    {% endif %}
+                </div>
+
+                <div class="form-group row">
+                    <label for="{{ form.email.auto_id }}" class="col-1 col-form-label">{{ form.email.label }}</label>
+                    
+                    <div class="col-4">
+                        {{form.email}}
+                        <span class="custom-file-control"></span>
+                    </div>
+
+                    {% if form.email.errors %}
+                    <div class="col-md-offset-2 col-8 text-danger small">
+                        {{form.email.errors}}
+                    </div>
+                    {% endif %}
+                </div>
+
+                <div class="form-group row">
+                    <label for="{{ form.password1.auto_id }}" class="col-1 col-form-label">{{ form.password1.label }}</label>
+                    
+                    <div class="col-4">
+                        {{form.password1}}
+                        <span class="custom-file-control"></span>
+                    </div>
+
+                    {% if form.password1.errors %}
+                    <div class="col-md-offset-2 col-8 text-danger small">
+                        {{form.password1.errors}}
+                    </div>
+                    {% endif %}
+                </div>
+
+                <div class="form-group row">
+                    <label for="{{ form.password2.auto_id }}" class="col-1 col-form-label">{{ form.password2.label }}</label>
+                    
+                    <div class="col-4">
+                        {{form.password2}}
+                        <span class="custom-file-control"></span>
+                    </div>
+
+                    {% if form.password2.errors %}
+                    <div class="col-md-offset-2 col-8 text-danger small">
+                        {{form.password2.errors}}
+                    </div>
+                    {% endif %}
+                </div>
+
+                <button type="submit" class="btn btn-primary">Register</button>
+            </form>
+        </div>
+    </div>
+</div>
 {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/account/settings.html` & `Boorunaut-0.5.0/booru/templates/booru/account/settings.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-    <link href="{% static 'booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css' %}" rel="stylesheet">
-{% endblock %}
-
-{% block scripts %}
-    <script src="{% static 'booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js' %}"></script>
-{% endblock %}
-
-{% block body %}
-    {% load humanize %}
-    <div class="row">
-        <div class="col" id="account-settings">
-            <h1 class="mb-4">Account Settings</h1>
-            <form method="post" action="." enctype="multipart/form-data">
-                {% csrf_token %}
-                <div class="row">
-                    <div class="col-md-5 ml-md-4">
-                        <div class="col p-0">
-                            <div class="form-group">
-                                <div class="row">
-                                    <div class="col-8">
-                                        <h3>Safe Only Listing</h3>
-
-                                        <p>All posts is not rated as safe will be hidden from all results.</p>
-                                    </div>
-                                    <div class="col-4 pt-4">
-                                        {{form.safe_only}}
-                                    </div>
-                                </div>
-
-                                <div class="row">
-                                    <div class="col-8">
-                                        <h3>Show Comments</h3>
-    
-                                        <p>All comments on posts and profiles will be shown.</p>
-                                    </div>
-                                    <div class="col-4 pt-4">
-                                        {{form.show_comments}}
-                                    </div>
-                                </div>
-                                <div class="row mt-5">
-                                    <div class="col-8">
-                                        <h3>Danger zone</h3>
-                                        <h4>Delete account</h4>
-    
-                                        <p>Contact the administration if you need the removal of sensitive data in posts.</p>
-                                    </div>
-                                    <div class="col-4 pt-4">
-                                        <div class="dropdown">
-                                            <button class="btn btn-danger dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
-                                                Delete
-                                            </button>
-                                            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
-                                                <a class="dropdown-item" href="{% url 'booru:profile_delete' user.slug %}">Confirm</a>
-                                            </div>
-                                        </div>
-                                    </div>
-                                </div>
-                            </div>
-                        </div>
-                    </div>
-
-                    <div class="form-group col-md-6">
-                        <h3>Tag Blacklist</h3>
-    
-                        <p>Any posts that contains the tags, ratings or users listed here will be shown as censored in any search result.</p>
-    
-                        {{form.tag_blacklist}}
-                    </div>
-                </div>
-
-                <div class="row">
-                    <div class="form-group col">
-                        <button type="submit" id="sendTagBlacklist" class="btn btn-primary float-right mt-1 col-sm-12 col-md-2">Save changes</button>
-                    </div>
-                </div>
-            </form>
-        </div>
-    </div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+    <link href="{% static 'booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css' %}" rel="stylesheet">
+{% endblock %}
+
+{% block scripts %}
+    <script src="{% static 'booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js' %}"></script>
+{% endblock %}
+
+{% block body %}
+    {% load humanize %}
+    <div class="row">
+        <div class="col" id="account-settings">
+            <h1 class="mb-4">Account Settings</h1>
+            <form method="post" action="." enctype="multipart/form-data">
+                {% csrf_token %}
+                <div class="row">
+                    <div class="col-md-5 ml-md-4">
+                        <div class="col p-0">
+                            <div class="form-group">
+                                <div class="row">
+                                    <div class="col-8">
+                                        <h3>Safe Only Listing</h3>
+
+                                        <p>All posts is not rated as safe will be hidden from all results.</p>
+                                    </div>
+                                    <div class="col-4 pt-4">
+                                        {{form.safe_only}}
+                                    </div>
+                                </div>
+
+                                <div class="row">
+                                    <div class="col-8">
+                                        <h3>Show Comments</h3>
+    
+                                        <p>All comments on posts and profiles will be shown.</p>
+                                    </div>
+                                    <div class="col-4 pt-4">
+                                        {{form.show_comments}}
+                                    </div>
+                                </div>
+                                <div class="row mt-5">
+                                    <div class="col-8">
+                                        <h3>Danger zone</h3>
+                                        <h4>Delete account</h4>
+    
+                                        <p>Contact the administration if you need the removal of sensitive data in posts.</p>
+                                    </div>
+                                    <div class="col-4 pt-4">
+                                        <div class="dropdown">
+                                            <button class="btn btn-danger dropdown-toggle" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                                                Delete
+                                            </button>
+                                            <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
+                                                <a class="dropdown-item" href="{% url 'booru:profile_delete' user.slug %}">Confirm</a>
+                                            </div>
+                                        </div>
+                                    </div>
+                                </div>
+                            </div>
+                        </div>
+                    </div>
+
+                    <div class="form-group col-md-6">
+                        <h3>Tag Blacklist</h3>
+    
+                        <p>Any posts that contains the tags, ratings or users listed here will be shown as censored in any search result.</p>
+    
+                        {{form.tag_blacklist}}
+                    </div>
+                </div>
+
+                <div class="row">
+                    <div class="form-group col">
+                        <button type="submit" id="sendTagBlacklist" class="btn btn-primary float-right mt-1 col-sm-12 col-md-2">Save changes</button>
+                    </div>
+                </div>
+            </form>
+        </div>
+    </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'booru/base.html' %} {% block css %} {% load staticfiles %}
+{% extends 'booru/base.html' %} {% block css %} {% load static %}
 {% endblock %} {% block scripts %}
 {% endblock %} {% block body %} {% load humanize %}
 ************ AAccccoouunntt SSeettttiinnggss ************
 {% csrf_token %}
 ******** SSaaffee OOnnllyy LLiissttiinngg ********
 All posts is not rated as safe will be hidden from all results.
 {{form.safe_only}}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/base.html` & `Boorunaut-0.5.0/booru/templates/booru/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-<!doctype html>
-<html lang="en" prefix="og: http://ogp.me/ns#">
-    <head>
-        <meta charset="utf-8"/>
-        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
-
-        {% load staticfiles %}
-        <!-- <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootswatch/4.0.0/cosmo/bootstrap.min.css"> -->
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/custom_cosmo.css' %}"/>
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/base.css' %}"/>
-        <link rel="stylesheet" type="text/css" href="https://code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css">
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css' %}"/>
-        <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.5.0/css/all.css" integrity="sha384-B4dIYHKNBt8Bc12p+WXckhzcICo0wtJAoU8YZTY5qE0Id1GSseTk6S+L3BlXeVIU" crossorigin="anonymous">
-        {% block css %}
-        {% endblock %}
-        
-        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
-        <script src="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js' %}"></script>
-        <script src="{% static 'booru/js/tag_search_autocomplete.js' %}"></script>
-        <script>
-            var tag_search_url = "{% url 'booru:tag_search' %}";
-            var tags = "{{tags}}";
-        </script>
-        {% block scripts %}
-        {% endblock %}
-
-        <title>
-            {% block title %}{{SITE_TITLE}} | Imageboard{% endblock %}
-        </title>
-        
-        <script type="application/ld+json">
-        {
-            "@context": "http://schema.org",
-            "@type": "WebSite",
-            "name": "{{SITE_TITLE}}",
-            "url" : "http://{{request.get_host}}",
-            "potentialAction": [{
-                "@type": "SearchAction",
-                "target": "{{request.get_host}}{% url 'booru:posts' %}?tags={search_term}",
-                "query-input": "required name=search_term"
-            }]
-        }
-        </script>
-
-        {{ INCLUDE_HEADER_CODE |safe }}
-
-        {% block ld_json %}
-        <link href="{{request.get_host}}" rel="canonical" />
-        {% endblock %}
-        <meta name="description" content="{{SITE_DESCRIPTION}}">
-    </head>
-    <body>
-        {% load static %}
-        {% include 'booru/navbar.html' %}
-
-        {% if SITE_ANNOUNCEMENT %}
-        <div class="container">
-            {% load markdown_deux_tags %}
-            <div class="alert alert-info" role="alert">
-                {{SITE_ANNOUNCEMENT|markdown}}
-            </div>
-        </div>
-        {% endif %}
-
-        <div class="container">
-            {% if SHOW_ADS %}
-            {{ ADS_CODE |safe }}
-            {% endif %}
-        </div>
-
-        <div class="container-fluid mt-4">
-        {% block body %}
-        {% endblock %}
-        </div>
-
-        <footer class="page-footer font-small pt-4">
-            <div class="text-center py-3">
-                Running <a href="https://github.com/Boorunaut/Boorunaut">Boorunaut</a> - <a href="{% url 'core:terms_of_service' %}">Terms of service</a> - <a href="{% url 'core:privacy_policy' %}">Privacy policy</a>
-            </div>
-        </footer>
-
-        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
-        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
-        <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.min.js"></script>
-    </body>
+<!doctype html>
+<html lang="en" prefix="og: http://ogp.me/ns#">
+    <head>
+        <meta charset="utf-8"/>
+        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
+
+        {% load static %}
+        <!-- <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootswatch/4.0.0/cosmo/bootstrap.min.css"> -->
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/custom_cosmo.css' %}"/>
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/base.css' %}"/>
+        <link rel="stylesheet" type="text/css" href="https://code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css">
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css' %}"/>
+        <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.5.0/css/all.css" integrity="sha384-B4dIYHKNBt8Bc12p+WXckhzcICo0wtJAoU8YZTY5qE0Id1GSseTk6S+L3BlXeVIU" crossorigin="anonymous">
+        {% block css %}
+        {% endblock %}
+        
+        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
+        <script src="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js' %}"></script>
+        <script src="{% static 'booru/js/tag_search_autocomplete.js' %}"></script>
+        <script>
+            var tag_search_url = "{% url 'booru:tag_search' %}";
+            var tags = "{{tags}}";
+        </script>
+        {% block scripts %}
+        {% endblock %}
+
+        <title>
+            {% block title %}{{SITE_TITLE}} | Imageboard{% endblock %}
+        </title>
+        
+        <script type="application/ld+json">
+        {
+            "@context": "http://schema.org",
+            "@type": "WebSite",
+            "name": "{{SITE_TITLE}}",
+            "url" : "http://{{request.get_host}}",
+            "potentialAction": [{
+                "@type": "SearchAction",
+                "target": "{{request.get_host}}{% url 'booru:posts' %}?tags={search_term}",
+                "query-input": "required name=search_term"
+            }]
+        }
+        </script>
+
+        {{ INCLUDE_HEADER_CODE |safe }}
+
+        {% block ld_json %}
+        <link href="{{request.get_host}}" rel="canonical" />
+        {% endblock %}
+        <meta name="description" content="{{SITE_DESCRIPTION}}">
+    </head>
+    <body>
+        {% load static %}
+        {% include 'booru/navbar.html' %}
+
+        {% if SITE_ANNOUNCEMENT %}
+        <div class="container">
+            {% load markdownify %}
+            <div class="alert alert-info" role="alert">
+                {{SITE_ANNOUNCEMENT|markdownify}}
+            </div>
+        </div>
+        {% endif %}
+
+        <div class="container">
+            {% if SHOW_ADS %}
+            {{ ADS_CODE |safe }}
+            {% endif %}
+        </div>
+
+        <div class="container-fluid mt-4">
+        {% block body %}
+        {% endblock %}
+        </div>
+
+        <footer class="page-footer font-small pt-4">
+            <div class="text-center py-3">
+                Running <a href="https://github.com/Boorunaut/Boorunaut">Boorunaut</a> - <a href="{% url 'core:terms_of_service' %}">Terms of service</a> - <a href="{% url 'core:privacy_policy' %}">Privacy policy</a>
+            </div>
+        </footer>
+
+        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
+        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
+        <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.min.js"></script>
+    </body>
 </html>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-{% load staticfiles %}
+{% load static %}
 {% block css %} {% endblock %}
 {% block scripts %} {% endblock %}
 {{ INCLUDE_HEADER_CODE |safe }} {% block ld_json %}
 {% endblock %}
 {% load static %} {% include 'booru/navbar.html' %} {% if SITE_ANNOUNCEMENT %}
-{% load markdown_deux_tags %}
-{{SITE_ANNOUNCEMENT|markdown}}
+{% load markdownify %}
+{{SITE_ANNOUNCEMENT|markdownify}}
 {% endif %}
 {% if SHOW_ADS %} {{ ADS_CODE |safe }} {% endif %}
 {% block body %} {% endblock %}
 Running _B_o_o_r_u_n_a_u_t - _T_e_r_m_s_ _o_f_ _s_e_r_v_i_c_e - _P_r_i_v_a_c_y_ _p_o_l_i_c_y
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/base_admin.html` & `Boorunaut-0.5.0/booru/templates/booru/base_admin.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-<!doctype html>
-<html lang="en" prefix="og: http://ogp.me/ns#">
-    <head>
-        <meta charset="utf-8"/>
-        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
-
-        {% load staticfiles %}
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/custom_cosmo.css' %}"/>
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/base.css' %}"/>
-        <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.5.0/css/all.css" integrity="sha384-B4dIYHKNBt8Bc12p+WXckhzcICo0wtJAoU8YZTY5qE0Id1GSseTk6S+L3BlXeVIU" crossorigin="anonymous">
-        {% block css %}
-        {% endblock %}
-        
-        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
-
-        {{ INCLUDE_HEADER_CODE |safe }}
-
-        {% block scripts %}
-        {% endblock %}
-
-        <title>
-            {% block title %}{{SITE_TITLE}} | Imageboard{% endblock %}
-        </title>
-    </head>
-    <body class="bg-light">
-        <div class="container-fluid">
-            {% with sidebar_size=2 %}
-            <div class="row">
-                <div class="col-{{sidebar_size}} bg-dark fixed-top fixed-bottom" style="z-index: -1;">
-                </div>
-            </div>
-            <div class="row">
-                <div id="sidebar-menu" class="col-{{sidebar_size}} pl-0 pr-0 text-white">
-                    <div class="col sticky-top pl-0 pr-0">
-                        <a class="navbar-brand col text-white text-center mt-4 mb-4" href="{% url 'booru:posts' %}">{{SITE_TITLE}}</a>
-
-                        <a type="button" href="{% url 'booru:staff_page' %}" class="btn btn-dark col text-left">
-                            <i class="fas fa-chart-line"></i> Statistics
-                        </a>
-
-                        <a type="button" href="{% url 'core:mod_queue' %}" class="btn btn-dark col text-left">
-                            <i class="fas fa-tasks"></i> Mod Queue
-                        </a>
-
-                        <a type="button" href="{% url 'booru:staff_site_configuration' %}" class="btn btn-dark col text-left">
-                            <i class="fas fa-cogs"></i> Board Configuration
-                        </a>
-
-                        <a type="button" href="{% url 'booru:staff_mass_rename' %}" class="btn btn-dark col text-left">
-                            <i class="fas fa-exchange-alt"></i> Mass Rename
-                        </a>
-
-                        <a type="button" href="{% url 'booru:staff_block' %}" class="btn btn-dark col text-left">
-                            <i class="fas fa-user-slash"></i> User Tools
-                        </a>
-
-                        <a type="button" href="{% url 'core:hash_ban' %}" class="btn btn-dark col text-left">
-                            <i class="fas fa-ban"></i> Hash Ban
-                        </a>
-
-                        <a type="button" href="#" class="btn btn-dark col text-left disabled">
-                            <i class="fas fa-box"></i> Extension Manager
-                        </a>
-                    </div>
-                    <div class="col-{{sidebar_size}} fixed-bottom">
-                        <div class="row pl-0 pr-0">
-                            <a href="{{user.get_absolute_url}}" class="btn btn-dark col">
-                                {{user}}
-                            </a>
-                        </div>
-                        <div class="row pl-0 pr-0">
-                            <a href="{% url 'account:logout' %}" class="btn btn-dark col">
-                                Logout
-                            </a>
-                        </div>
-                    </div>
-                </div>
-                <div id="content" class="col pl-0 pr-0">
-                    {% block content %}
-                    {% endblock %}
-                </div>
-            </div>
-            {% endwith %}
-        </div>
-
-        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
-        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
-    </body>
+<!doctype html>
+<html lang="en" prefix="og: http://ogp.me/ns#">
+    <head>
+        <meta charset="utf-8"/>
+        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
+
+        {% load static %}
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/custom_cosmo.css' %}"/>
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/base.css' %}"/>
+        <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.5.0/css/all.css" integrity="sha384-B4dIYHKNBt8Bc12p+WXckhzcICo0wtJAoU8YZTY5qE0Id1GSseTk6S+L3BlXeVIU" crossorigin="anonymous">
+        {% block css %}
+        {% endblock %}
+        
+        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
+
+        {{ INCLUDE_HEADER_CODE |safe }}
+
+        {% block scripts %}
+        {% endblock %}
+
+        <title>
+            {% block title %}{{SITE_TITLE}} | Imageboard{% endblock %}
+        </title>
+    </head>
+    <body class="bg-light">
+        <div class="container-fluid">
+            {% with sidebar_size=2 %}
+            <div class="row">
+                <div class="col-{{sidebar_size}} bg-dark fixed-top fixed-bottom" style="z-index: -1;">
+                </div>
+            </div>
+            <div class="row">
+                <div id="sidebar-menu" class="col-{{sidebar_size}} pl-0 pr-0 text-white">
+                    <div class="col sticky-top pl-0 pr-0">
+                        <a class="navbar-brand col text-white text-center mt-4 mb-4" href="{% url 'booru:posts' %}">{{SITE_TITLE}}</a>
+
+                        <a type="button" href="{% url 'booru:staff_page' %}" class="btn btn-dark col text-left">
+                            <i class="fas fa-chart-line"></i> Statistics
+                        </a>
+
+                        <a type="button" href="{% url 'core:mod_queue' %}" class="btn btn-dark col text-left">
+                            <i class="fas fa-tasks"></i> Mod Queue
+                        </a>
+
+                        <a type="button" href="{% url 'booru:staff_site_configuration' %}" class="btn btn-dark col text-left">
+                            <i class="fas fa-cogs"></i> Board Configuration
+                        </a>
+
+                        <a type="button" href="{% url 'booru:staff_mass_rename' %}" class="btn btn-dark col text-left">
+                            <i class="fas fa-exchange-alt"></i> Mass Rename
+                        </a>
+
+                        <a type="button" href="{% url 'booru:staff_block' %}" class="btn btn-dark col text-left">
+                            <i class="fas fa-user-slash"></i> User Tools
+                        </a>
+
+                        <a type="button" href="{% url 'core:hash_ban' %}" class="btn btn-dark col text-left">
+                            <i class="fas fa-ban"></i> Hash Ban
+                        </a>
+
+                        <a type="button" href="#" class="btn btn-dark col text-left disabled">
+                            <i class="fas fa-box"></i> Extension Manager
+                        </a>
+                    </div>
+                    <div class="col-{{sidebar_size}} fixed-bottom">
+                        <div class="row pl-0 pr-0">
+                            <a href="{{user.get_absolute_url}}" class="btn btn-dark col">
+                                {{user}}
+                            </a>
+                        </div>
+                        <div class="row pl-0 pr-0">
+                            <a href="{% url 'account:logout' %}" class="btn btn-dark col">
+                                Logout
+                            </a>
+                        </div>
+                    </div>
+                </div>
+                <div id="content" class="col pl-0 pr-0">
+                    {% block content %}
+                    {% endblock %}
+                </div>
+            </div>
+            {% endwith %}
+        </div>
+
+        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
+        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
+    </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% load staticfiles %}
+{% load static %}
 {% block css %} {% endblock %}
 {{ INCLUDE_HEADER_CODE |safe }} {% block scripts %} {% endblock %}
 {% with sidebar_size=2 %}
 _{_{_S_I_T_E___T_I_T_L_E_}_}
 _S_t_a_t_i_s_t_i_c_s
 _M_o_d_ _Q_u_e_u_e
 _B_o_a_r_d_ _C_o_n_f_i_g_u_r_a_t_i_o_n
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/base_index.html` & `Boorunaut-0.5.0/booru/templates/booru/base_index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-<!doctype html>
-<html lang="en" prefix="og: http://ogp.me/ns#">
-    <head>
-        <meta charset="utf-8"/>
-        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">        
-
-        {% load staticfiles %}
-        <!-- <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootswatch/4.0.0/cosmo/bootstrap.min.css"> -->
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/custom_cosmo.css' %}"/>
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/base.css' %}"/>
-        <link rel="stylesheet" type="text/css" href="https://code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css">
-        <link rel="stylesheet" type="text/css" href="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css' %}"/>
-        {% block css %}
-        {% endblock %}
-        
-        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
-        <script defer src="https://use.fontawesome.com/releases/v5.0.8/js/all.js"></script>
-        <script src="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js' %}"></script>
-        <script src="{% static 'booru/js/tag_search_autocomplete.js' %}"></script>
-        <script>
-            var tag_search_url = "{% url 'booru:tag_search' %}";
-        </script>
-        {% block scripts %}
-        {% endblock %}
-
-        {{ INCLUDE_HEADER_CODE |safe }}
-
-        <title>
-            {% block title %}{{SITE_TITLE}} | Imageboard{% endblock %}
-        </title>
-        <meta name="description" content="{{SITE_DESCRIPTION}}">
-    </head>
-    <body>
-        <div class="container mt-4">
-        {% block body %}
-        {% endblock %}
-        </div>
-
-        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
-        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
-        <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.min.js"></script>
-    </body>
+<!doctype html>
+<html lang="en" prefix="og: http://ogp.me/ns#">
+    <head>
+        <meta charset="utf-8"/>
+        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">        
+
+        {% load static %}
+        <!-- <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootswatch/4.0.0/cosmo/bootstrap.min.css"> -->
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/custom_cosmo.css' %}"/>
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/css/base.css' %}"/>
+        <link rel="stylesheet" type="text/css" href="https://code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css">
+        <link rel="stylesheet" type="text/css" href="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.css' %}"/>
+        {% block css %}
+        {% endblock %}
+        
+        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
+        <script defer src="https://use.fontawesome.com/releases/v5.0.8/js/all.js"></script>
+        <script src="{% static 'booru/jQuery-Tags-Input-1.3.6/jquery.tagsinput.min.js' %}"></script>
+        <script src="{% static 'booru/js/tag_search_autocomplete.js' %}"></script>
+        <script>
+            var tag_search_url = "{% url 'booru:tag_search' %}";
+        </script>
+        {% block scripts %}
+        {% endblock %}
+
+        {{ INCLUDE_HEADER_CODE |safe }}
+
+        <title>
+            {% block title %}{{SITE_TITLE}} | Imageboard{% endblock %}
+        </title>
+        <meta name="description" content="{{SITE_DESCRIPTION}}">
+    </head>
+    <body>
+        <div class="container mt-4">
+        {% block body %}
+        {% endblock %}
+        </div>
+
+        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
+        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
+        <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.min.js"></script>
+    </body>
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
-{% load staticfiles %}
+{% load static %}
 {% block css %} {% endblock %}
 {% block scripts %} {% endblock %} {{ INCLUDE_HEADER_CODE |safe }}
 {% block body %} {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/gallery_create.html` & `Boorunaut-0.5.0/booru/templates/booru/gallery_create.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/index.css' %}"/>
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-{% load crispy_forms_tags %}
-<div class="container">
-    <div class="row">
-        <h1>Create new gallery</h1>
-    </div>
-
-    <form class="mb-3" method="post" enctype="multipart/x-www-form-urlencoded">
-        {% csrf_token %}
-        {{ form |crispy }}
-        <button type="submit" class="btn btn-primary">Create</button>
-    </form>
-</div>
-{% endblock %}
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/index.css' %}"/>
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+{% load crispy_forms_tags %}
+<div class="container">
+    <div class="row">
+        <h1>Create new gallery</h1>
+    </div>
+
+    <form class="mb-3" method="post" enctype="multipart/x-www-form-urlencoded">
+        {% csrf_token %}
+        {{ form |crispy }}
+        <button type="submit" class="btn btn-primary">Create</button>
+    </form>
+</div>
+{% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/implication_create.html` & `Boorunaut-0.5.0/booru/templates/booru/implication_create.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-{% load crispy_forms_tags %}
-<div class="container">
-    <div class="row">
-        <h1>Tag Implication Request</h1>
-    </div>
-    <div class="row">
-        <p class="text-muted">Every time the <span class="font-italic font-weight-bold">from</span> tag is added, the <span class="font-italic font-weight-bold">to</span> tag will also be added automatically.</p>
-    </div>
-    <form method="post" enctype="multipart/x-www-form-urlencoded">
-        {% csrf_token %}
-        {{ form |crispy }}
-        <button type="submit" class="btn btn-primary">Submit</button>
-    </form>
-    <div class="row mt-3">
-        <p>This request will be reviewed by the staff.</p>
-    </div>
-</div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+{% load crispy_forms_tags %}
+<div class="container">
+    <div class="row">
+        <h1>Tag Implication Request</h1>
+    </div>
+    <div class="row">
+        <p class="text-muted">Every time the <span class="font-italic font-weight-bold">from</span> tag is added, the <span class="font-italic font-weight-bold">to</span> tag will also be added automatically.</p>
+    </div>
+    <form method="post" enctype="multipart/x-www-form-urlencoded">
+        {% csrf_token %}
+        {{ form |crispy }}
+        <button type="submit" class="btn btn-primary">Submit</button>
+    </form>
+    <div class="row mt-3">
+        <p>This request will be reviewed by the staff.</p>
+    </div>
+</div>
 {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/implication_detail.html` & `Boorunaut-0.5.0/booru/templates/booru/implication_detail.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-{% load permission_tags %}
-<div class="container">
-    <div class="row">
-        <h1>Tag implication: {{object.from_tag}} → {{object.to_tag}}</h1>
-    </div>
-    <div class="row">
-        <div id="table" class="col mt-3">
-            <table class="table table-sm">
-                <tbody>
-                    <tr>
-                        <td><strong>From:</strong></td>
-                        <td>
-                            {% with color='#'|add:object.from_tag.category.color %}
-                            <a class="font-weight-bold" style="color: {{color}};" href="{% url 'booru:tag_detail' object.from_tag.id %}">?</a>
-                            <a style="color: {{color}};" href="{{ object.from_tag.get_search_url }}">{{object.from_tag}}</a>
-                            {% endwith %}
-                        </td>
-                    </tr>
-                    <tr>
-                        <td><strong>To:</strong></td>
-                        <td>
-                            {% with color='#'|add:object.to_tag.category.color %}
-                            <a class="font-weight-bold" style="color: {{color}};" href="{% url 'booru:tag_detail' object.to_tag.id %}">?</a>
-                            <a style="color: {{color}};" href="{{ object.to_tag.get_search_url }}">{{object.to_tag}}</a>
-                            {% endwith %}
-                        </td>
-                    </tr>
-                    <tr>
-                        <td><strong>Creator:</strong></td>
-                        <td>{{object.author}}</td>
-                    </tr>
-                    <tr>
-                        <td><strong>Date:</strong></td>
-                        <td>{{object.timestamp}}</td>
-                    </tr>
-                    <tr>
-                        <td><strong>Approver:</strong></td>
-                        <td><a href="{{object.approver.get_absolute_url}}">{{object.approver}}</a></td>
-                    </tr>
-                    <tr>
-                        <td><strong>Status:</strong></td>
-                        <td>{{object.get_status_display}}</td>
-                    </tr>
-                </tbody>
-            </table>
-            {% if user|can:'manage_tags' %}
-            <div class="row">
-                {% if object.status == 1 %}
-                <a href="{% url 'booru:implication_approve' object.id %}" class="btn btn-success btn-sm disabled mr-1">
-                    <i class="fas fa-check"></i> Approve
-                </a>
-                {% else %}
-                <a href="{% url 'booru:implication_approve' object.id %}" class="btn btn-success btn-sm mr-1">
-                    <i class="fas fa-check"></i> Approve
-                </a>
-                {% endif %}
-                {% if object.status == 2 %}
-                <a href="{% url 'booru:implication_disapprove' object.id %}" class="btn btn-danger disabled btn-sm">
-                    <i class="fas fa-times"></i> Disapprove
-                </a>
-                {% else %}
-                <a href="{% url 'booru:implication_disapprove' object.id %}" class="btn btn-danger btn-sm">
-                    <i class="fas fa-times"></i> Disapprove
-                </a>
-                {% endif %}
-            </div>
-            {% endif %}
-        </div>
-    </div>
-</div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+{% load permission_tags %}
+<div class="container">
+    <div class="row">
+        <h1>Tag implication: {{object.from_tag}} → {{object.to_tag}}</h1>
+    </div>
+    <div class="row">
+        <div id="table" class="col mt-3">
+            <table class="table table-sm">
+                <tbody>
+                    <tr>
+                        <td><strong>From:</strong></td>
+                        <td>
+                            {% with color='#'|add:object.from_tag.category.color %}
+                            <a class="font-weight-bold" style="color: {{color}};" href="{% url 'booru:tag_detail' object.from_tag.id %}">?</a>
+                            <a style="color: {{color}};" href="{{ object.from_tag.get_search_url }}">{{object.from_tag}}</a>
+                            {% endwith %}
+                        </td>
+                    </tr>
+                    <tr>
+                        <td><strong>To:</strong></td>
+                        <td>
+                            {% with color='#'|add:object.to_tag.category.color %}
+                            <a class="font-weight-bold" style="color: {{color}};" href="{% url 'booru:tag_detail' object.to_tag.id %}">?</a>
+                            <a style="color: {{color}};" href="{{ object.to_tag.get_search_url }}">{{object.to_tag}}</a>
+                            {% endwith %}
+                        </td>
+                    </tr>
+                    <tr>
+                        <td><strong>Creator:</strong></td>
+                        <td>{{object.author}}</td>
+                    </tr>
+                    <tr>
+                        <td><strong>Date:</strong></td>
+                        <td>{{object.timestamp}}</td>
+                    </tr>
+                    <tr>
+                        <td><strong>Approver:</strong></td>
+                        <td><a href="{{object.approver.get_absolute_url}}">{{object.approver}}</a></td>
+                    </tr>
+                    <tr>
+                        <td><strong>Status:</strong></td>
+                        <td>{{object.get_status_display}}</td>
+                    </tr>
+                </tbody>
+            </table>
+            {% if user|can:'manage_tags' %}
+            <div class="row">
+                {% if object.status == 1 %}
+                <a href="{% url 'booru:implication_approve' object.id %}" class="btn btn-success btn-sm disabled mr-1">
+                    <i class="fas fa-check"></i> Approve
+                </a>
+                {% else %}
+                <a href="{% url 'booru:implication_approve' object.id %}" class="btn btn-success btn-sm mr-1">
+                    <i class="fas fa-check"></i> Approve
+                </a>
+                {% endif %}
+                {% if object.status == 2 %}
+                <a href="{% url 'booru:implication_disapprove' object.id %}" class="btn btn-danger disabled btn-sm">
+                    <i class="fas fa-times"></i> Disapprove
+                </a>
+                {% else %}
+                <a href="{% url 'booru:implication_disapprove' object.id %}" class="btn btn-danger btn-sm">
+                    <i class="fas fa-times"></i> Disapprove
+                </a>
+                {% endif %}
+            </div>
+            {% endif %}
+        </div>
+    </div>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends 'booru/base.html' %} {% block css %} {% load staticfiles %} {%
-endblock %} {% block scripts %} {% endblock %} {% block body %} {% load
-permission_tags %}
+{% extends 'booru/base.html' %} {% block css %} {% load static %} {% endblock
+%} {% block scripts %} {% endblock %} {% block body %} {% load permission_tags
+%}
 ************ TTaagg iimmpplliiccaattiioonn:: {{{{oobbjjeecctt..ffrroomm__ttaagg}}}} ?â?? {{{{oobbjjeecctt..ttoo__ttaagg}}}} ************
 FFrroomm::     {% with color='#'|add:object.from_tag.category.color %} _? _{
           _{_o_b_j_e_c_t_._f_r_o_m___t_a_g_}_} {% endwith %}
 TToo::       {% with color='#'|add:object.to_tag.category.color %} _? _{
           _{_o_b_j_e_c_t_._t_o___t_a_g_}_} {% endwith %}
 CCrreeaattoorr::  {{object.author}}
 DDaattee::     {{object.timestamp}}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/implication_list.html` & `Boorunaut-0.5.0/booru/templates/booru/implication_list.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-{% load crispy_forms_tags %}
-<div class="container">
-    <div class="row">
-        <div class="col">
-            <form method="get">
-                {{ form |crispy }}
-                <button type="submit" class="btn btn-primary">Search</button>
-            </form>
-        </div>
-    </div>
-
-    <div class="row">
-        <div id="table" class="col mt-3">
-            <table class="table table-striped table-hover text-center">
-                <thead class="thead-light">
-                    <tr>
-                        <th scope="col">#</th>
-                        <th scope="col">From</th>
-                        <th scope="col">To</th>
-                        <th scope="col">Approver</th>
-                        <th scope="col">Status</th>
-                        <th scope="col"></th>
-                    </tr>
-                </thead>
-                <tbody>
-                    {% for implication in object_list %}
-                    <tr>
-                        <th scope="row">{{ forloop.counter }}</th>
-                        <td>
-                            <a class="font-weight-bold" style="color: #{{implication.from_tag.category.color}};" href="{% url 'booru:tag_detail' implication.from_tag.id %}">?</a>
-                            <a href="{{ implication.from_tag.get_search_url }}" style="color: #{{implication.from_tag.category.color}};">{{implication.from_tag}}</a> 
-                            <span class="text-muted">{{implication.from_tag.get_count}}</span>
-                        </td>
-                        <td>
-                            <a class="font-weight-bold" style="color: #{{implication.to_tag.category.color}};" href="{% url 'booru:tag_detail' implication.to_tag.id %}">?</a>
-                            <a href="{{ implication.to_tag.get_search_url }}" style="color: #{{implication.to_tag.category.color}};">{{implication.to_tag}}</a> 
-                            <span class="text-muted">{{implication.to_tag.get_count}}</span>
-                        </td>
-                        <td><a href="{{implication.approver.get_absolute_url}}">{{implication.approver}}</a></td>
-                        <td>{{implication.get_status_display}}</td>
-                        <td><a href="{% url 'booru:implication-detail' implication.id %}">Show</a></td>
-                    </tr>
-                    {% endfor %}
-                </tbody>
-            </table>
-
-            <nav aria-label="..." class="mt-4">
-                <ul class="pagination">
-                    {% if page_obj.has_previous %}
-                        <li class="page-item">
-                            <a class="page-link" href="?page={{page_obj.previous_page_number}}" tabindex="-1">Previous</a>
-                        </li>
-                    {% else %}
-                        <li class="page-item disabled">
-                            <a class="page-link" href="#" tabindex="-1">Previous</a>
-                        </li>
-                    {% endif %}
-                    {% for i in page_obj.paginator.page_range %}
-                        {% if page_obj.number == i %}
-                        <li class="page-item active">
-                            <a class="page-link" href="{% url 'booru:tags_page_list' i %}">{{i}} <span class="sr-only">(current)</span></a>
-                        </li>
-                        {% elif i > page_obj.number|add:'-3' and i < page_obj.number|add:'3' %}
-                        <li class="page-item">
-                            <a class="page-link" href="{% url 'booru:tags_page_list' i %}">{{i}}</a>
-                        </li>
-                        {% endif %}
-                    {% endfor %}
-                    {% if page_obj.has_next %}
-                        <li class="page-item">
-                            <a class="page-link" href="?page={{page_obj.next_page_number}}">Next</a>
-                        </li>
-                    {% else %}
-                        <li class="page-item disabled">
-                            <a class="page-link" href="#">Next</a>
-                        </li>
-                    {% endif %}
-                </ul>
-            </nav>
-        </div>
-    </div>
-</div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+{% load crispy_forms_tags %}
+<div class="container">
+    <div class="row">
+        <div class="col">
+            <form method="get">
+                {{ form |crispy }}
+                <button type="submit" class="btn btn-primary">Search</button>
+            </form>
+        </div>
+    </div>
+
+    <div class="row">
+        <div id="table" class="col mt-3">
+            <table class="table table-striped table-hover text-center">
+                <thead class="thead-light">
+                    <tr>
+                        <th scope="col">#</th>
+                        <th scope="col">From</th>
+                        <th scope="col">To</th>
+                        <th scope="col">Approver</th>
+                        <th scope="col">Status</th>
+                        <th scope="col"></th>
+                    </tr>
+                </thead>
+                <tbody>
+                    {% for implication in object_list %}
+                    <tr>
+                        <th scope="row">{{ forloop.counter }}</th>
+                        <td>
+                            <a class="font-weight-bold" style="color: #{{implication.from_tag.category.color}};" href="{% url 'booru:tag_detail' implication.from_tag.id %}">?</a>
+                            <a href="{{ implication.from_tag.get_search_url }}" style="color: #{{implication.from_tag.category.color}};">{{implication.from_tag}}</a> 
+                            <span class="text-muted">{{implication.from_tag.get_count}}</span>
+                        </td>
+                        <td>
+                            <a class="font-weight-bold" style="color: #{{implication.to_tag.category.color}};" href="{% url 'booru:tag_detail' implication.to_tag.id %}">?</a>
+                            <a href="{{ implication.to_tag.get_search_url }}" style="color: #{{implication.to_tag.category.color}};">{{implication.to_tag}}</a> 
+                            <span class="text-muted">{{implication.to_tag.get_count}}</span>
+                        </td>
+                        <td><a href="{{implication.approver.get_absolute_url}}">{{implication.approver}}</a></td>
+                        <td>{{implication.get_status_display}}</td>
+                        <td><a href="{% url 'booru:implication-detail' implication.id %}">Show</a></td>
+                    </tr>
+                    {% endfor %}
+                </tbody>
+            </table>
+
+            <nav aria-label="..." class="mt-4">
+                <ul class="pagination">
+                    {% if page_obj.has_previous %}
+                        <li class="page-item">
+                            <a class="page-link" href="?page={{page_obj.previous_page_number}}" tabindex="-1">Previous</a>
+                        </li>
+                    {% else %}
+                        <li class="page-item disabled">
+                            <a class="page-link" href="#" tabindex="-1">Previous</a>
+                        </li>
+                    {% endif %}
+                    {% for i in page_obj.paginator.page_range %}
+                        {% if page_obj.number == i %}
+                        <li class="page-item active">
+                            <a class="page-link" href="{% url 'booru:tags_page_list' i %}">{{i}} <span class="sr-only">(current)</span></a>
+                        </li>
+                        {% elif i > page_obj.number|add:'-3' and i < page_obj.number|add:'3' %}
+                        <li class="page-item">
+                            <a class="page-link" href="{% url 'booru:tags_page_list' i %}">{{i}}</a>
+                        </li>
+                        {% endif %}
+                    {% endfor %}
+                    {% if page_obj.has_next %}
+                        <li class="page-item">
+                            <a class="page-link" href="?page={{page_obj.next_page_number}}">Next</a>
+                        </li>
+                    {% else %}
+                        <li class="page-item disabled">
+                            <a class="page-link" href="#">Next</a>
+                        </li>
+                    {% endif %}
+                </ul>
+            </nav>
+        </div>
+    </div>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'booru/base.html' %} {% block css %} {% load staticfiles %} {%
-endblock %} {% block scripts %} {% endblock %} {% block body %} {% load
+{% extends 'booru/base.html' %} {% block css %} {% load static %} {% endblock
+%} {% block scripts %} {% endblock %} {% block body %} {% load
 crispy_forms_tags %}
 {{ form |crispy }} Search
 ##               FFrroomm                              TToo                              AApppprroovveerr                SSttaattuuss
 {{
 {{               _? _{_{_i_m_p_l_i_c_a_t_i_o_n_._f_r_o_m___t_a_g_}_} {      _? _{_{_i_m_p_l_i_c_a_t_i_o_n_._t_o___t_a_g_}_} {      _{                       {                                 _S_h_o_w
 ffoorrlloooopp..ccoouunntteerr {implication.from_tag.get_count}} {implication.to_tag.get_count}} _{_i_m_p_l_i_c_a_t_i_o_n_._a_p_p_r_o_v_e_r_}_} {implication.get_status_display}}
 }}}}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/index.html` & `Boorunaut-0.5.0/booru/templates/booru/index.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-{% extends 'booru/base_index.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/index.css' %}"/>
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-<div class="container">
-    <div class="row">
-        <div class="col">
-            <h1 class="text-center site-title"><a href="#">{{SITE_TITLE}}</a></h1>
-        </div>
-    </div>
-    <div class="row text-center">
-        <div class="col">
-            <a href="{% url 'booru:posts' %}" class="btn font-weight-bold" title="A paginated list of every post">Posts</a>
-            <a href="#" class="btn disabled" title="All comments listing">Comments</a>
-            <a href="#" class="btn disabled" title="Forum listing">Forum</a>
-            <a href="#" class="btn disabled" title="Wiki pages with database documentation">Wiki</a>
-            {% if not user.is_authenticated %}
-            <a href="{% url 'account:login' %}" class="btn">Login</a>
-            {% else %}
-            <a href="{{user.get_absolute_url}}" class="btn" title="Account options">My Account</a>
-            {% endif %}
-            <a href="#" class="btn disabled" title="Help page and tools">»</a>
-        </div>
-    </div>
-    <form action="{% url 'booru:posts' %}">
-        <div class="form-row mt-3 mb-3">
-            <div class="col">
-                <input name="tags" class="tag-search form-control form-control-sm" type="search" aria-label="Search" placeholder="lorem_ipsum dolor_sit" hidden>
-            </div>
-            <div class="col-1">
-                <button class="btn btn-primary" type="submit">Search</button>
-            </div>
-        </div>
-    </form>
-    <div class="row text-center mt-2">
-        <span class="col display-4 bg-white text-dark" title="Number of posts">
-            {{post_count}}
-        </span>
-    </div>
-    <div class="row bg-primary pt-1 mt-4 mb-5"></div>
-    <div class="">
-        <div class="row mt-2">
-            <div class="col text-center">
-                Running <a href="https://github.com/Boorunaut/Boorunaut">Boorunaut</a> Alpha 0.4.3 - <a href="{% url 'core:terms_of_service' %}">Terms of service</a>
-            </div>
-        </div>
-
-        <div class="row">
-            <div class="col text-center">
-                <small>Original concept by <a href="https://github.com/r888888888/danbooru">Danbooru</a></small>
-            </div>
-        </div>
-    </div>
-</div>
+{% extends 'booru/base_index.html' %}
+
+{% block css %}
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/index.css' %}"/>
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+<div class="container">
+    <div class="row">
+        <div class="col">
+            <h1 class="text-center site-title"><a href="#">{{SITE_TITLE}}</a></h1>
+        </div>
+    </div>
+    <div class="row text-center">
+        <div class="col">
+            <a href="{% url 'booru:posts' %}" class="btn font-weight-bold" title="A paginated list of every post">Posts</a>
+            <a href="#" class="btn disabled" title="All comments listing">Comments</a>
+            <a href="#" class="btn disabled" title="Forum listing">Forum</a>
+            <a href="#" class="btn disabled" title="Wiki pages with database documentation">Wiki</a>
+            {% if not user.is_authenticated %}
+            <a href="{% url 'account:login' %}" class="btn">Login</a>
+            {% else %}
+            <a href="{{user.get_absolute_url}}" class="btn" title="Account options">My Account</a>
+            {% endif %}
+            <a href="#" class="btn disabled" title="Help page and tools">»</a>
+        </div>
+    </div>
+    <form action="{% url 'booru:posts' %}">
+        <div class="form-row mt-3 mb-3">
+            <div class="col">
+                <input name="tags" class="tag-search form-control form-control-sm" type="search" aria-label="Search" placeholder="lorem_ipsum dolor_sit" hidden>
+            </div>
+            <div class="col-1">
+                <button class="btn btn-primary" type="submit">Search</button>
+            </div>
+        </div>
+    </form>
+    <div class="row text-center mt-2">
+        <span class="col display-4 bg-white text-dark" title="Number of posts">
+            {{post_count}}
+        </span>
+    </div>
+    <div class="row bg-primary pt-1 mt-4 mb-5"></div>
+    <div class="">
+        <div class="row mt-2">
+            <div class="col text-center">
+                Running <a href="https://github.com/Boorunaut/Boorunaut">Boorunaut</a> Alpha 0.4.3 - <a href="{% url 'core:terms_of_service' %}">Terms of service</a>
+            </div>
+        </div>
+
+        <div class="row">
+            <div class="col text-center">
+                <small>Original concept by <a href="https://github.com/r888888888/danbooru">Danbooru</a></small>
+            </div>
+        </div>
+    </div>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'booru/base_index.html' %} {% block css %} {% load staticfiles %}
+{% extends 'booru/base_index.html' %} {% block css %} {% load static %}
 {% endblock %} {% block scripts %} {% endblock %} {% block body %}
 ************ _{{_{{_SS_II_TT_EE____TT_II_TT_LL_EE_}}_}} ************
 _P_o_s_t_s _C_o_m_m_e_n_t_s _F_o_r_u_m _W_i_k_i {% if not user.is_authenticated %} _L_o_g_i_n {% else %}
 _M_y_ _A_c_c_o_u_n_t {% endif %} _Â_»
 [Unknown INPUT type]
 Search
 {{post_count}}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/navbar.html` & `Boorunaut-0.5.0/booru/templates/booru/navbar.html`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
-    <a class="navbar-brand" href="{% url 'booru:posts' %}">{{SITE_TITLE}}</a>
-    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
-        <span class="navbar-toggler-icon"></span>
-    </button>
-    
-    <div class="collapse navbar-collapse" id="navbarSupportedContent">
-        <ul class="navbar-nav">
-        <li class="nav-item active">
-            <a class="nav-link" href="{% url 'booru:upload' %}"><i class="fas fa-upload"></i> Upload</a>
-        </li>
-        </ul>
-        <form class="form-inline my-2 my-lg-0 col-md-4" action="{% url 'booru:posts' %}">
-            <input id="tags" name="tags" class="tag-search form-control col-md-9" type="search" placeholder="lorem_ipsum dolor_sit" aria-label="Search" data-role="tagsinput" hidden>
-            <div class="input-group-append">
-                <button class="btn btn-outline-light my-2 my-sm-0" type="submit">Search</button>
-            </div>
-        </form>
-        {% if user.is_staff %}
-        <ul class="navbar-nav">
-            <li class="nav-item active">
-                <a class="nav-link" href="{% url 'booru:staff_page' %}">Staff</a>
-            </li>
-        </ul>
-        {% endif %}
-        <ul class="navbar-nav ml-auto">
-            <li class="nav-item active">
-                <a class="nav-link" href="{% url 'account:settings' %}">Settings</a>
-            </li>
-            {% if not user.is_authenticated %}
-            <li class="nav-item active">
-                <a class="nav-link" href="{% url 'account:register' %}">Register</a>
-            </li>
-            <li class="nav-item active">
-                <a class="nav-link" href="{% url 'account:login' %}">Login</a>
-            </li>
-            {% else %}
-            <li class="nav-item active">
-                <a class="nav-link" href="{{user.get_absolute_url}}">Profile</a>
-            </li>
-            <li class="nav-item active">
-                <a class="nav-link" href="{% url 'account:logout' %}">Logout</a>
-            </li>
-            {% endif %}
-        </ul>
-    </div>
-</nav>
-<ul class="nav sub_navbar mb-4">
-    <li class="nav-item dropdown">
-        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
-            Images
-        </a>
-        <div class="dropdown-menu">
-            <a class="dropdown-item" href="{% url 'booru:posts' %}">List</a>
-            <a class="dropdown-item disabled" href="#">Random</a>
-        </div>
-    </li>
-    <li class="nav-item dropdown">
-        <a class="nav-link dropdown-toggle disabled" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
-            Activity
-        </a>
-        <div class="dropdown-menu">
-            <a class="dropdown-item" href="#">Rankings</a>
-            <a class="dropdown-item" href="#">Comments</a>
-        </div>
-    </li>
-    <li class="nav-item dropdown">
-        <a class="nav-link dropdown-toggle disabled" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
-            Forums
-        </a>
-        <div class="dropdown-menu">
-            <a class="dropdown-item" href="#">General Discussion</a>
-            <a class="dropdown-item" href="#">Tagging Discussion</a>
-            <a class="dropdown-item" href="#">Site and Policy</a>
-            <a class="dropdown-item" href="#">Uploader Discussion</a>
-            <a class="dropdown-item" href="#">Post Search</a>
-        </div>
-    </li>
-    <li class="nav-item dropdown">
-        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
-            Tags
-        </a>
-        <div class="dropdown-menu">
-            <a class="dropdown-item" href="{% url 'booru:tags_list' %}">List</a>
-            <a class="dropdown-item" href="{% url 'booru:implication-list' %}">Implications</a>
-        </div>
-    </li>
-    <li class="nav-item dropdown">
-        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
-            Request
-        </a>
-        <div class="dropdown-menu">
-            <a class="dropdown-item" href="{% url 'booru:implication_create' %}">New implication</a>
-        </div>
-    </li>
-    <li class="nav-item dropdown">
-        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
-            Galleries
-        </a>
-        <div class="dropdown-menu">
-            <a class="dropdown-item" href="{% url 'booru:gallery' %}">List</a>
-            <a class="dropdown-item" href="{% url 'booru:gallery_create' %}">Create</a>
-        </div>
-    </li>
+<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
+    <a class="navbar-brand" href="{% url 'booru:posts' %}">{{SITE_TITLE}}</a>
+    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
+        <span class="navbar-toggler-icon"></span>
+    </button>
+    
+    <div class="collapse navbar-collapse" id="navbarSupportedContent">
+        <ul class="navbar-nav">
+        <li class="nav-item active">
+            <a class="nav-link" href="{% url 'booru:upload' %}"><i class="fas fa-upload"></i> Upload</a>
+        </li>
+        </ul>
+        <form class="form-inline my-2 my-lg-0 col-md-4" action="{% url 'booru:posts' %}">
+            <input id="tags" name="tags" class="tag-search form-control col-md-9" type="search" placeholder="lorem_ipsum dolor_sit" aria-label="Search" data-role="tagsinput" hidden>
+            <div class="input-group-append">
+                <button class="btn btn-outline-light my-2 my-sm-0" type="submit">Search</button>
+            </div>
+        </form>
+        {% if user.is_staff %}
+        <ul class="navbar-nav">
+            <li class="nav-item active">
+                <a class="nav-link" href="{% url 'booru:staff_page' %}">Staff</a>
+            </li>
+        </ul>
+        {% endif %}
+        <ul class="navbar-nav ml-auto">
+            <li class="nav-item active">
+                <a class="nav-link" href="{% url 'account:settings' %}">Settings</a>
+            </li>
+            {% if not user.is_authenticated %}
+            <li class="nav-item active">
+                <a class="nav-link" href="{% url 'account:register' %}">Register</a>
+            </li>
+            <li class="nav-item active">
+                <a class="nav-link" href="{% url 'account:login' %}">Login</a>
+            </li>
+            {% else %}
+            <li class="nav-item active">
+                <a class="nav-link" href="{{user.get_absolute_url}}">Profile</a>
+            </li>
+            <li class="nav-item active">
+                <a class="nav-link" href="{% url 'account:logout' %}">Logout</a>
+            </li>
+            {% endif %}
+        </ul>
+    </div>
+</nav>
+<ul class="nav sub_navbar mb-4">
+    <li class="nav-item dropdown">
+        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
+            Images
+        </a>
+        <div class="dropdown-menu">
+            <a class="dropdown-item" href="{% url 'booru:posts' %}">List</a>
+            <a class="dropdown-item disabled" href="#">Random</a>
+        </div>
+    </li>
+    <li class="nav-item dropdown">
+        <a class="nav-link dropdown-toggle disabled" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
+            Activity
+        </a>
+        <div class="dropdown-menu">
+            <a class="dropdown-item" href="#">Rankings</a>
+            <a class="dropdown-item" href="#">Comments</a>
+        </div>
+    </li>
+    <li class="nav-item dropdown">
+        <a class="nav-link dropdown-toggle disabled" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
+            Forums
+        </a>
+        <div class="dropdown-menu">
+            <a class="dropdown-item" href="#">General Discussion</a>
+            <a class="dropdown-item" href="#">Tagging Discussion</a>
+            <a class="dropdown-item" href="#">Site and Policy</a>
+            <a class="dropdown-item" href="#">Uploader Discussion</a>
+            <a class="dropdown-item" href="#">Post Search</a>
+        </div>
+    </li>
+    <li class="nav-item dropdown">
+        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
+            Tags
+        </a>
+        <div class="dropdown-menu">
+            <a class="dropdown-item" href="{% url 'booru:tags_list' %}">List</a>
+            <a class="dropdown-item" href="{% url 'booru:implication-list' %}">Implications</a>
+        </div>
+    </li>
+    <li class="nav-item dropdown">
+        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
+            Request
+        </a>
+        <div class="dropdown-menu">
+            <a class="dropdown-item" href="{% url 'booru:implication_create' %}">New implication</a>
+        </div>
+    </li>
+    <li class="nav-item dropdown">
+        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
+            Galleries
+        </a>
+        <div class="dropdown-menu">
+            <a class="dropdown-item" href="{% url 'booru:gallery' %}">List</a>
+            <a class="dropdown-item" href="{% url 'booru:gallery_create' %}">Create</a>
+        </div>
+    </li>
 </ul>
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/post_detail.html` & `Boorunaut-0.5.0/booru/templates/booru/post_detail.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,432 +1,432 @@
-{% extends 'booru/base.html' %}
-
-{% load staticfiles %}
-{% block css %}
-    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/post_detail.css' %}"/>
-{% endblock %}
-
-{% block ld_json %}
-<script type="application/ld+json">
-    {% if EMBED_MODE == False %}
-    {
-      "@context": "http://schema.org",
-      "@type": "ImageObject",
-      "contentUrl": "{{post.media.url}}",
-      "datePublished": "{{post.timestamp|date:'c'}}",
-      "description": "{{post.description}}"
-    }
-    {% endif %}
-</script>
-
-<link href="{{post.get_absolute_url}}" rel="canonical" />
-{% endblock %}
-
-{% block scripts %}
-    <script src="{% static 'booru/js/post_detail.js' %}"></script>
-    <script>
-        var is_favorited = {{is_favorited|yesno:'true,false'}};
-        var current_vote = {{current_vote}};
-        var favorite_url = "{% url 'booru:post_favorite' post.id %}";
-        var vote_url = "{% url 'booru:post_score_vote' post.id %}";
-    </script>
-{% endblock %}
-
-{% block body %}
-    {% load humanize %}
-    {% load number_converter %}
-    {% load markdown_deux_tags %}
-    {% load permission_tags %}
-    {% load crispy_forms_tags %}
-    <div class="row">
-        <aside id="sidebar" class="col-md-3 col order-2 order-md-1">
-            <nav aria-label="Page navigation example">
-                <ul class="pagination justify-content-center">
-                    {% if previous_post %}
-                    <li class="page-item">
-                        <a class="page-link" href="{% url 'booru:post_detail' previous_post.id %}">
-                            <i class="fas fa-chevron-left"></i> Previous
-                        </a>
-                    </li>
-                    {% else %}
-                    <li class="page-item disabled">
-                        <a class="page-link" href="#" tabindex="-1">
-                            <i class="fas fa-chevron-left"></i> Previous
-                        </a>
-                    </li>
-                    {% endif %}
-                    {% if next_post %}
-                    <li class="page-item">
-                        <a class="page-link" href="{% url 'booru:post_detail' next_post.id %}">
-                            Next <i class="fas fa-chevron-right"></i>
-                        </a>
-                    </li>
-                    {% else %}
-                    <li class="page-item disabled">
-                        <a class="page-link" href="#">
-                            Next <i class="fas fa-chevron-right"></i>
-                        </a>
-                    </li>
-                    {% endif %}
-                </ul>
-            </nav>
-            <div class="row text-center">
-                <span class="col mb-2">
-                    <a href="{% url 'booru:post_history' post.id %}" type="button" class="btn btn-sm btn-primary">
-                        <i class="fas fa-history"></i> History
-                    </a>
-                </span>
-            </div>
-            <div id="tag-tables" class="col">
-                {% for category, tags in ordered_tags.items %}
-                <div id="tag-table-{{category.label}}" class="mb-3">
-                    <div class="row col">
-                        <span class="font-weight-bold">{{category}}</span>
-                    </div>
-                    <table class="tag-table table-sm table borderless">
-                        <tbody>
-                            {% for tag in tags %}
-                            <tr>
-                                {% if category.label == "general" %}
-                                <th class="tag-wiki-link" scope="row">
-                                    <a href="{% url 'booru:tag_detail' tag.id %}">
-                                        ?
-                                    </a>
-                                </th>
-                                <td class="tag-label">
-                                    {% url 'booru:posts' as posts_url %}
-                                    <a href="{{ tag.get_search_url }}">{{ tag }}</a>
-                                </td>
-                                {% else %}
-                                <th class="tag-wiki-link" scope="row">
-                                    <a style="color: #{{category.color}};" href="{% url 'booru:tag_detail' tag.id %}">
-                                        ?
-                                    </a>
-                                </th>
-                                <td class="tag-label">
-                                    <a style="color: #{{category.color}};" href="{{ tag.get_search_url }}">{{tag}}</a>
-                                </td>
-                                {% endif %}
-                                <td class="tag-count">{{tag.get_count|number_converter}}</td>
-                            </tr>
-                            {% endfor %}
-                        </tbody>
-                    </table>
-                </div>
-                {% endfor %}
-            </div>
-
-            <div class="col mb-3">
-                <div class="row col">
-                    <span class="font-weight-bold">Information</span>
-                </div>
-                
-                <table class="table table-sm mt-2 borderless" style="table-layout: fixed; word-break: break-all;">
-                    <tbody>
-                        <tr>
-                            <th scope="row"><i class="fas fa-hashtag"></i> ID</th>
-                            <td>{{post.id}}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row"><i class="fas fa-user"></i> Uploader</th>
-                            <td><a href="{{post.uploader.get_absolute_url}}">{{post.uploader}}</a></td>
-                        </tr>
-                        {% if post.get_parent %}
-                        <tr>
-                            <th scope="row">Parent</th>
-                            <td><a href="{{post.get_parent.get_absolute_url}}">{{post.get_parent}}</a></td>
-                        </tr>
-                        {% endif %}
-                        <tr>
-                            <th scope="row"><i class="far fa-calendar"></i> Date</th>
-                            <td>
-                                <time datetime="{{post.timestamp|date:'c'}}" title="{{post.timestamp|date}}">
-                                    {{post.timestamp|naturaltime}}
-                                </time>
-                            </td>
-                        </tr>
-                        {% if EMBED_MODE == False %}
-                        <tr>
-                            <th scope="row"><i class="far fa-image"></i> Size</th>
-                            <td>
-                                <a href="{{post.media.url}}">{{post.media.size}} KB</a>
-                                ({{post.get_media_width}}x{{post.get_media_height}})
-                            </td>
-                        </tr>
-                        {% endif %}
-                        <tr>
-                            <th scope="row"><i class="fas fa-link"></i> Source</th>
-                            <td>
-                                {% for source in post.get_sources %}
-                                {{source|urlizetrunc:22}}<br/>
-                                {% endfor %}
-                            </td>
-                        </tr>
-                        <tr>
-                            <th scope="row"><i class="far fa-eye"></i> Rating</th>
-                            <td>{{post.get_rating_display}}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row"><i class="far fa-thumbs-up"></i> Score</th>
-                            <td id="score_count">{{post.get_score_count}}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row"><i class="far fa-star"></i> Favorites</th>
-                            <td id="favorite_count">{{post.get_favorites_count}}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row"><i class="far fa-check-circle"></i> Status</th>
-                            <td>{{post.get_status_display}}</td>
-                        </tr>
-                    </tbody>
-                </table>
-                {% if user.is_authenticated %}
-                <div class="row text-center">
-                    <span class="col-2 offset-3" data-toggle="tooltip" title="Mark as favorite">
-                        <button id="btn_favorited" type="button" class="btn btn-primary">
-                            <i class="fas fa-star"></i>
-                        </button>
-                    </span>
-                    <span class="col-2" data-toggle="tooltip" title="Upvote">
-                        <button id="btn_vote_up" type="button" class="btn btn-primary">
-                            <i class="fas fa-thumbs-up"></i>
-                        </button>
-                    </span>
-                    <span class="col-2" data-toggle="tooltip" title="Downvote">
-                        <button id="btn_vote_down" type="button" class="btn btn-primary">
-                            <i class="fas fa-thumbs-down"></i>
-                        </button>
-                    </span>
-                </div>
-                {% else %}
-                <div class="row text-center">
-                    <span class="col-2 offset-3" data-toggle="tooltip" title="Login to mark posts as favorite">
-                        <button type="button" class="btn btn-primary" disabled>
-                            <i class='fas fa-star'></i>
-                        </button>
-                    </span>
-                    <span class="col-2" data-toggle="tooltip" title="Login to upvote posts">
-                        <button type="button" class="btn btn-primary" disabled>
-                            <i class="fas fa-thumbs-up"></i>
-                        </button>
-                    </span>
-                    <span class="col-2" data-toggle="tooltip" title="Login to downvote posts">
-                        <button type="button" class="btn btn-primary" disabled>
-                            <i class="fas fa-thumbs-down"></i>
-                        </button>
-                    </span>
-                </div>
-                {% endif %}
-                <div class="row mt-3 text-center">
-                    <span class="col" data-toggle="tooltip" title="Flag this post for deletion.">
-                        <a href="{% url 'booru:post_flag' post.pk %}" class="btn btn-sm btn-secondary">
-                            <i class="fas fa-flag"></i> Flag
-                        </a>
-                    </span>
-                </div>
-            </div>
-        </aside>
-        <section id="post" class="col-9 order-1 order-md-2">
-            {% if post.status == 2 %}
-            <div class="alert alert-warning text-center" role="alert">
-                This post was hid by a staff member.
-            </div>
-            {% elif post.status == 3 %}
-            <div class="alert alert-danger text-center" role="alert">
-                This post was deleted by a staff member.
-            </div>
-            {% endif %}
-            <div class="accordion mb-1" id="relationshipAccordion">
-                {% if post.get_parent %}
-                <div class="card">
-                    <div class="card-header p-0" id="parentHeading">
-                        <h5 class="mb-0">
-                            <button class="btn btn-sm collapsed col" type="button" data-toggle="collapse" data-target="#parentCollapse" aria-expanded="true" aria-controls="parentCollapse">
-                                <i class="fas fa-stream"></i> Parent
-                            </button>
-                        </h5>
-                    </div>
-                
-                    <div id="parentCollapse" class="collapse" aria-labelledby="parentHeading" data-parent="#relationshipAccordion">
-                        <div class="card-body">
-                            <a href="{{post.get_parent.get_absolute_url}}">
-                                <img src="{{post.get_parent.preview.url}}" alt="">
-                            </a>
-                        </div>
-                    </div>
-                </div>
-                {% endif %}
-                {% if post.get_siblings %}
-                <div class="card">
-                    <div class="card-header p-0" id="siblingsHeading">
-                        <h5 class="mb-0">
-                            <button class="btn btn-sm collapsed col" type="button" data-toggle="collapse" data-target="#siblingsCollapse" aria-expanded="false" aria-controls="siblingsCollapse">
-                                <i class="fas fa-stream"></i> Siblings <span class="badge badge-dark">{{post.get_siblings.count}}</span>
-                            </button>
-                        </h5>
-                    </div>
-                    <div id="siblingsCollapse" class="collapse" aria-labelledby="siblingsHeading" data-parent="#relationshipAccordion">
-                    <div class="card-body">
-                        {% for sibling in post.get_siblings %}
-                        <a href="{{sibling.get_absolute_url}}"><img src="{{sibling.preview.url}}" alt=""></a>
-                        {% endfor %}
-                    </div>
-                    </div>
-                </div>
-                {% endif %}
-                {% if post.get_children %}
-                <div class="card">
-                    <div class="card-header p-0" id="childrenHeading">
-                        <h5 class="mb-0">
-                            <button class="btn btn-sm collapsed col" type="button" data-toggle="collapse" data-target="#childrenCollapse" aria-expanded="false" aria-controls="childrenCollapse">
-                                <i class="fas fa-stream"></i> Children <span class="badge badge-dark">{{post.get_children.count}}</span>
-                            </button>
-                        </h5>
-                    </div>
-                    <div id="childrenCollapse" class="collapse" aria-labelledby="childrenHeading" data-parent="#relationshipAccordion">
-                        <div class="card-body">
-                            {% for child in post.get_children %}
-                            <a href="{{child.get_absolute_url}}"><img src="{{child.preview.url}}" alt=""></a>
-                            {% endfor %}
-                        </div>
-                    </div>
-                </div>
-                {% endif %}
-            </div>
-            <div class="row mb-3">
-                <main class="col">
-                    {% if user|can:'change_status' or not post.status == 3 %}
-                        {% if EMBED_MODE == False %}
-                            {% if post.media_type == 0 %}
-                            <img src="{{ post.get_sample_url }}" alt="{{ post.tags_mirror }}" title="{{ post.tags_mirror }}" style="max-width: 100%;">
-                            {% elif post.media_type == 1 %}
-                            <video controls>
-                                <source src="{{ post.media.url }}">
-                            </video>
-                            {% endif %}
-                        {% else %}
-                            {{post.get_embed_code |safe }}
-                        {% endif %}
-                    {% endif %}
-                </main>
-            </div>
-            <div class="row">
-                <div class="col mt-2 mb-4">
-                    {% if request.user.show_comments or not user.is_authenticated %}
-                    <button id="show_comments" class="btn btn-primary btn mr-1">Comments</button>
-                    {% endif %}
-                    <button id="show_edit_form" class="btn btn-outline-primary btn mr-3">Edit</button>
-                    {% if user|can:'change_status' %}
-                    <div class="float-right">
-                        <a id="approve_post" href="{% url 'booru:post_approve' post.id %}" class="btn btn-success btn mr-1">Approve</a>
-                        <a id="hide_post" href="{% url 'booru:post_hide' post.id %}" class="btn btn-warning btn mr-1">Hide</a>
-                        <a id="delete_post" href="{% url 'booru:post_delete' post.id %}" class="btn btn-danger btn">Delete</a>
-                    </div>
-                    {% endif %}
-                </div>
-            </div>
-            {% if post.description %}
-            <div class="row">
-                <div class="card col-10">
-                    <div class="card-body">
-                        <h5 class="card-title">Description</h5>
-                        <p class="card-text">{{post.description|markdown}}</p>
-                    </div>
-                </div>
-            </div>
-            {% endif %}
-            <div class="row mb-2">
-                <div id="edit" class="col-10" style="display: none;">
-                    <form method="post" action="." enctype="multipart/form-data">
-                        {% csrf_token %}
-                        {{ form |crispy }}
-                        <button type="submit" id="send" class="btn btn-primary submit-media">Update</button>
-                    </form>
-                </div>
-            </div>
-            {% if request.user.show_comments or not user.is_authenticated %}
-            <div id="comment-section" class="mb-3">
-                <div id="comments" class="row">
-                    {% for comment in post.comments.all %}
-                    {% if not comment.is_hidden or user|can:'manage_comments' %}
-                    <div id="comment-{{comment.id}}" class="comment col-10 border comment-border pt-3 pb-3 mb-2">
-                        <div class="row">
-                            <div class="comment col">
-                                <div class="row">
-                                    <span class="col">
-                                        {% if comment.author.is_deleted %}
-                                        <h5>{{comment.author.get_name}}</h5>
-                                        {% else %}
-                                        <h5><a href="{{comment.author.get_absolute_url}}">{{comment.author.get_name}}</a></h5>
-                                        {% endif %}
-                                    </span>
-                                </div>
-                                <div class="row">
-                                    <span class="col text-muted">
-                                        {{comment.timestamp|naturaltime}}
-                                    </span>
-                                </div>
-                                <div class="row">
-                                    <span class="col">
-                                        <small>Score: {{comment.get_score}}</small>
-                                    </span>
-                                </div>
-                                {% if comment.is_hidden %}
-                                <div class="row">
-                                    <span class="col">
-                                        <small>Comment is hidden</small>
-                                    </span>
-                                </div>
-                                {% endif %}
-                            </div>
-                            <div class="comment col-9">
-                                {{comment.content|markdown}}
-                            </div>
-                        </div>
-                        {% if user|can:'manage_comments' %}
-                        <div class="row">
-                            <div class="col offset-3">
-                                {% if comment.is_hidden %}
-                                <a href="{% url 'booru:comment-toggle-view' comment.pk %}" class="btn btn-sm btn-success">
-                                     <i class="far fa-eye"></i> Show
-                                </a>
-                                {% else %}
-                                <a href="{% url 'booru:comment-toggle-view' comment.pk %}" class="btn btn-sm btn-danger">
-                                    <i class="far fa-eye-slash"></i> Hide
-                                </a>
-                                {% endif %}
-                            </div>
-                        </div>
-                        {% endif %}
-                    </div>
-                    {% endif %}
-                    {% endfor %}
-                </div>
-                <div id="comment-create-form" class="row mt-3">
-                    <form class="col-10" method="post" action="." enctype="multipart/form-data">
-                        {% if not user.is_authenticated %}
-                        <fieldset disabled>
-                        {% endif %}
-
-                        {% csrf_token %}
-                        <div class="form-group">
-                            {% if not user.is_authenticated %}
-                            <label for="newCommentTextarea" class="text-muted">New comment (Login to comment)</label>
-                            {% else %}
-                            <label for="newCommentTextarea">New comment</label>
-                            {% endif %}
-                            <textarea class="form-control" id="newCommentTextarea" name="newCommentTextarea" rows="3" {% if not can_comment %}placeholder="This account cannot comment currently." disabled{% endif %}></textarea>
-                        </div>
-                        {% if can_comment %}
-                        <button type="submit" id="send" class="btn btn-sm btn-primary">Create comment</button>
-                        {% endif %}
-                        
-                        {% if not user.is_authenticated %}
-                        </fieldset>
-                        {% endif %}
-                    </form>
-                </div>
-            </div>
-            {% endif %}
-        </section>
-    </div>
+{% extends 'booru/base.html' %}
+
+{% load static %}
+{% block css %}
+    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/post_detail.css' %}"/>
+{% endblock %}
+
+{% block ld_json %}
+<script type="application/ld+json">
+    {% if EMBED_MODE == False %}
+    {
+      "@context": "http://schema.org",
+      "@type": "ImageObject",
+      "contentUrl": "{{post.media.url}}",
+      "datePublished": "{{post.timestamp|date:'c'}}",
+      "description": "{{post.description}}"
+    }
+    {% endif %}
+</script>
+
+<link href="{{post.get_absolute_url}}" rel="canonical" />
+{% endblock %}
+
+{% block scripts %}
+    <script src="{% static 'booru/js/post_detail.js' %}"></script>
+    <script>
+        var is_favorited = {{is_favorited|yesno:'true,false'}};
+        var current_vote = {{current_vote}};
+        var favorite_url = "{% url 'booru:post_favorite' post.id %}";
+        var vote_url = "{% url 'booru:post_score_vote' post.id %}";
+    </script>
+{% endblock %}
+
+{% block body %}
+    {% load humanize %}
+    {% load number_converter %}
+    {% load markdownify %}
+    {% load permission_tags %}
+    {% load crispy_forms_tags %}
+    <div class="row">
+        <aside id="sidebar" class="col-md-3 col order-2 order-md-1">
+            <nav aria-label="Page navigation example">
+                <ul class="pagination justify-content-center">
+                    {% if previous_post %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:post_detail' previous_post.id %}">
+                            <i class="fas fa-chevron-left"></i> Previous
+                        </a>
+                    </li>
+                    {% else %}
+                    <li class="page-item disabled">
+                        <a class="page-link" href="#" tabindex="-1">
+                            <i class="fas fa-chevron-left"></i> Previous
+                        </a>
+                    </li>
+                    {% endif %}
+                    {% if next_post %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:post_detail' next_post.id %}">
+                            Next <i class="fas fa-chevron-right"></i>
+                        </a>
+                    </li>
+                    {% else %}
+                    <li class="page-item disabled">
+                        <a class="page-link" href="#">
+                            Next <i class="fas fa-chevron-right"></i>
+                        </a>
+                    </li>
+                    {% endif %}
+                </ul>
+            </nav>
+            <div class="row text-center">
+                <span class="col mb-2">
+                    <a href="{% url 'booru:post_history' post.id %}" type="button" class="btn btn-sm btn-primary">
+                        <i class="fas fa-history"></i> History
+                    </a>
+                </span>
+            </div>
+            <div id="tag-tables" class="col">
+                {% for category, tags in ordered_tags.items %}
+                <div id="tag-table-{{category.label}}" class="mb-3">
+                    <div class="row col">
+                        <span class="font-weight-bold">{{category}}</span>
+                    </div>
+                    <table class="tag-table table-sm table borderless">
+                        <tbody>
+                            {% for tag in tags %}
+                            <tr>
+                                {% if category.label == "general" %}
+                                <th class="tag-wiki-link" scope="row">
+                                    <a href="{% url 'booru:tag_detail' tag.id %}">
+                                        ?
+                                    </a>
+                                </th>
+                                <td class="tag-label">
+                                    {% url 'booru:posts' as posts_url %}
+                                    <a href="{{ tag.get_search_url }}">{{ tag }}</a>
+                                </td>
+                                {% else %}
+                                <th class="tag-wiki-link" scope="row">
+                                    <a style="color: #{{category.color}};" href="{% url 'booru:tag_detail' tag.id %}">
+                                        ?
+                                    </a>
+                                </th>
+                                <td class="tag-label">
+                                    <a style="color: #{{category.color}};" href="{{ tag.get_search_url }}">{{tag}}</a>
+                                </td>
+                                {% endif %}
+                                <td class="tag-count">{{tag.get_count|number_converter}}</td>
+                            </tr>
+                            {% endfor %}
+                        </tbody>
+                    </table>
+                </div>
+                {% endfor %}
+            </div>
+
+            <div class="col mb-3">
+                <div class="row col">
+                    <span class="font-weight-bold">Information</span>
+                </div>
+                
+                <table class="table table-sm mt-2 borderless" style="table-layout: fixed; word-break: break-all;">
+                    <tbody>
+                        <tr>
+                            <th scope="row"><i class="fas fa-hashtag"></i> ID</th>
+                            <td>{{post.id}}</td>
+                        </tr>
+                        <tr>
+                            <th scope="row"><i class="fas fa-user"></i> Uploader</th>
+                            <td><a href="{{post.uploader.get_absolute_url}}">{{post.uploader}}</a></td>
+                        </tr>
+                        {% if post.get_parent %}
+                        <tr>
+                            <th scope="row">Parent</th>
+                            <td><a href="{{post.get_parent.get_absolute_url}}">{{post.get_parent}}</a></td>
+                        </tr>
+                        {% endif %}
+                        <tr>
+                            <th scope="row"><i class="far fa-calendar"></i> Date</th>
+                            <td>
+                                <time datetime="{{post.timestamp|date:'c'}}" title="{{post.timestamp|date}}">
+                                    {{post.timestamp|naturaltime}}
+                                </time>
+                            </td>
+                        </tr>
+                        {% if EMBED_MODE == False %}
+                        <tr>
+                            <th scope="row"><i class="far fa-image"></i> Size</th>
+                            <td>
+                                <a href="{{post.media.url}}">{{post.media.size}} KB</a>
+                                ({{post.get_media_width}}x{{post.get_media_height}})
+                            </td>
+                        </tr>
+                        {% endif %}
+                        <tr>
+                            <th scope="row"><i class="fas fa-link"></i> Source</th>
+                            <td>
+                                {% for source in post.get_sources %}
+                                {{source|urlizetrunc:22}}<br/>
+                                {% endfor %}
+                            </td>
+                        </tr>
+                        <tr>
+                            <th scope="row"><i class="far fa-eye"></i> Rating</th>
+                            <td>{{post.get_rating_display}}</td>
+                        </tr>
+                        <tr>
+                            <th scope="row"><i class="far fa-thumbs-up"></i> Score</th>
+                            <td id="score_count">{{post.get_score_count}}</td>
+                        </tr>
+                        <tr>
+                            <th scope="row"><i class="far fa-star"></i> Favorites</th>
+                            <td id="favorite_count">{{post.get_favorites_count}}</td>
+                        </tr>
+                        <tr>
+                            <th scope="row"><i class="far fa-check-circle"></i> Status</th>
+                            <td>{{post.get_status_display}}</td>
+                        </tr>
+                    </tbody>
+                </table>
+                {% if user.is_authenticated %}
+                <div class="row text-center">
+                    <span class="col-2 offset-3" data-toggle="tooltip" title="Mark as favorite">
+                        <button id="btn_favorited" type="button" class="btn btn-primary">
+                            <i class="fas fa-star"></i>
+                        </button>
+                    </span>
+                    <span class="col-2" data-toggle="tooltip" title="Upvote">
+                        <button id="btn_vote_up" type="button" class="btn btn-primary">
+                            <i class="fas fa-thumbs-up"></i>
+                        </button>
+                    </span>
+                    <span class="col-2" data-toggle="tooltip" title="Downvote">
+                        <button id="btn_vote_down" type="button" class="btn btn-primary">
+                            <i class="fas fa-thumbs-down"></i>
+                        </button>
+                    </span>
+                </div>
+                {% else %}
+                <div class="row text-center">
+                    <span class="col-2 offset-3" data-toggle="tooltip" title="Login to mark posts as favorite">
+                        <button type="button" class="btn btn-primary" disabled>
+                            <i class='fas fa-star'></i>
+                        </button>
+                    </span>
+                    <span class="col-2" data-toggle="tooltip" title="Login to upvote posts">
+                        <button type="button" class="btn btn-primary" disabled>
+                            <i class="fas fa-thumbs-up"></i>
+                        </button>
+                    </span>
+                    <span class="col-2" data-toggle="tooltip" title="Login to downvote posts">
+                        <button type="button" class="btn btn-primary" disabled>
+                            <i class="fas fa-thumbs-down"></i>
+                        </button>
+                    </span>
+                </div>
+                {% endif %}
+                <div class="row mt-3 text-center">
+                    <span class="col" data-toggle="tooltip" title="Flag this post for deletion.">
+                        <a href="{% url 'booru:post_flag' post.pk %}" class="btn btn-sm btn-secondary">
+                            <i class="fas fa-flag"></i> Flag
+                        </a>
+                    </span>
+                </div>
+            </div>
+        </aside>
+        <section id="post" class="col-9 order-1 order-md-2">
+            {% if post.status == 2 %}
+            <div class="alert alert-warning text-center" role="alert">
+                This post was hid by a staff member.
+            </div>
+            {% elif post.status == 3 %}
+            <div class="alert alert-danger text-center" role="alert">
+                This post was deleted by a staff member.
+            </div>
+            {% endif %}
+            <div class="accordion mb-1" id="relationshipAccordion">
+                {% if post.get_parent %}
+                <div class="card">
+                    <div class="card-header p-0" id="parentHeading">
+                        <h5 class="mb-0">
+                            <button class="btn btn-sm collapsed col" type="button" data-toggle="collapse" data-target="#parentCollapse" aria-expanded="true" aria-controls="parentCollapse">
+                                <i class="fas fa-stream"></i> Parent
+                            </button>
+                        </h5>
+                    </div>
+                
+                    <div id="parentCollapse" class="collapse" aria-labelledby="parentHeading" data-parent="#relationshipAccordion">
+                        <div class="card-body">
+                            <a href="{{post.get_parent.get_absolute_url}}">
+                                <img src="{{post.get_parent.preview.url}}" alt="">
+                            </a>
+                        </div>
+                    </div>
+                </div>
+                {% endif %}
+                {% if post.get_siblings %}
+                <div class="card">
+                    <div class="card-header p-0" id="siblingsHeading">
+                        <h5 class="mb-0">
+                            <button class="btn btn-sm collapsed col" type="button" data-toggle="collapse" data-target="#siblingsCollapse" aria-expanded="false" aria-controls="siblingsCollapse">
+                                <i class="fas fa-stream"></i> Siblings <span class="badge badge-dark">{{post.get_siblings.count}}</span>
+                            </button>
+                        </h5>
+                    </div>
+                    <div id="siblingsCollapse" class="collapse" aria-labelledby="siblingsHeading" data-parent="#relationshipAccordion">
+                    <div class="card-body">
+                        {% for sibling in post.get_siblings %}
+                        <a href="{{sibling.get_absolute_url}}"><img src="{{sibling.preview.url}}" alt=""></a>
+                        {% endfor %}
+                    </div>
+                    </div>
+                </div>
+                {% endif %}
+                {% if post.get_children %}
+                <div class="card">
+                    <div class="card-header p-0" id="childrenHeading">
+                        <h5 class="mb-0">
+                            <button class="btn btn-sm collapsed col" type="button" data-toggle="collapse" data-target="#childrenCollapse" aria-expanded="false" aria-controls="childrenCollapse">
+                                <i class="fas fa-stream"></i> Children <span class="badge badge-dark">{{post.get_children.count}}</span>
+                            </button>
+                        </h5>
+                    </div>
+                    <div id="childrenCollapse" class="collapse" aria-labelledby="childrenHeading" data-parent="#relationshipAccordion">
+                        <div class="card-body">
+                            {% for child in post.get_children %}
+                            <a href="{{child.get_absolute_url}}"><img src="{{child.preview.url}}" alt=""></a>
+                            {% endfor %}
+                        </div>
+                    </div>
+                </div>
+                {% endif %}
+            </div>
+            <div class="row mb-3">
+                <main class="col">
+                    {% if user|can:'change_status' or not post.status == 3 %}
+                        {% if EMBED_MODE == False %}
+                            {% if post.media_type == 0 %}
+                            <img src="{{ post.get_sample_url }}" alt="{{ post.tags_mirror }}" title="{{ post.tags_mirror }}" style="max-width: 100%;">
+                            {% elif post.media_type == 1 %}
+                            <video controls>
+                                <source src="{{ post.media.url }}">
+                            </video>
+                            {% endif %}
+                        {% else %}
+                            {{post.get_embed_code |safe }}
+                        {% endif %}
+                    {% endif %}
+                </main>
+            </div>
+            <div class="row">
+                <div class="col mt-2 mb-4">
+                    {% if request.user.show_comments or not user.is_authenticated %}
+                    <button id="show_comments" class="btn btn-primary btn mr-1">Comments</button>
+                    {% endif %}
+                    <button id="show_edit_form" class="btn btn-outline-primary btn mr-3">Edit</button>
+                    {% if user|can:'change_status' %}
+                    <div class="float-right">
+                        <a id="approve_post" href="{% url 'booru:post_approve' post.id %}" class="btn btn-success btn mr-1">Approve</a>
+                        <a id="hide_post" href="{% url 'booru:post_hide' post.id %}" class="btn btn-warning btn mr-1">Hide</a>
+                        <a id="delete_post" href="{% url 'booru:post_delete' post.id %}" class="btn btn-danger btn">Delete</a>
+                    </div>
+                    {% endif %}
+                </div>
+            </div>
+            {% if post.description %}
+            <div class="row">
+                <div class="card col-10">
+                    <div class="card-body">
+                        <h5 class="card-title">Description</h5>
+                        <p class="card-text">{{post.description|markdownify}}</p>
+                    </div>
+                </div>
+            </div>
+            {% endif %}
+            <div class="row mb-2">
+                <div id="edit" class="col-10" style="display: none;">
+                    <form method="post" action="." enctype="multipart/form-data">
+                        {% csrf_token %}
+                        {{ form |crispy }}
+                        <button type="submit" id="send" class="btn btn-primary submit-media">Update</button>
+                    </form>
+                </div>
+            </div>
+            {% if request.user.show_comments or not user.is_authenticated %}
+            <div id="comment-section" class="mb-3">
+                <div id="comments" class="row">
+                    {% for comment in post.comments.all %}
+                    {% if not comment.is_hidden or user|can:'manage_comments' %}
+                    <div id="comment-{{comment.id}}" class="comment col-10 border comment-border pt-3 pb-3 mb-2">
+                        <div class="row">
+                            <div class="comment col">
+                                <div class="row">
+                                    <span class="col">
+                                        {% if comment.author.is_deleted %}
+                                        <h5>{{comment.author.get_name}}</h5>
+                                        {% else %}
+                                        <h5><a href="{{comment.author.get_absolute_url}}">{{comment.author.get_name}}</a></h5>
+                                        {% endif %}
+                                    </span>
+                                </div>
+                                <div class="row">
+                                    <span class="col text-muted">
+                                        {{comment.timestamp|naturaltime}}
+                                    </span>
+                                </div>
+                                <div class="row">
+                                    <span class="col">
+                                        <small>Score: {{comment.get_score}}</small>
+                                    </span>
+                                </div>
+                                {% if comment.is_hidden %}
+                                <div class="row">
+                                    <span class="col">
+                                        <small>Comment is hidden</small>
+                                    </span>
+                                </div>
+                                {% endif %}
+                            </div>
+                            <div class="comment col-9">
+                                {{comment.content|markdownify}}
+                            </div>
+                        </div>
+                        {% if user|can:'manage_comments' %}
+                        <div class="row">
+                            <div class="col offset-3">
+                                {% if comment.is_hidden %}
+                                <a href="{% url 'booru:comment-toggle-view' comment.pk %}" class="btn btn-sm btn-success">
+                                     <i class="far fa-eye"></i> Show
+                                </a>
+                                {% else %}
+                                <a href="{% url 'booru:comment-toggle-view' comment.pk %}" class="btn btn-sm btn-danger">
+                                    <i class="far fa-eye-slash"></i> Hide
+                                </a>
+                                {% endif %}
+                            </div>
+                        </div>
+                        {% endif %}
+                    </div>
+                    {% endif %}
+                    {% endfor %}
+                </div>
+                <div id="comment-create-form" class="row mt-3">
+                    <form class="col-10" method="post" action="." enctype="multipart/form-data">
+                        {% if not user.is_authenticated %}
+                        <fieldset disabled>
+                        {% endif %}
+
+                        {% csrf_token %}
+                        <div class="form-group">
+                            {% if not user.is_authenticated %}
+                            <label for="newCommentTextarea" class="text-muted">New comment (Login to comment)</label>
+                            {% else %}
+                            <label for="newCommentTextarea">New comment</label>
+                            {% endif %}
+                            <textarea class="form-control" id="newCommentTextarea" name="newCommentTextarea" rows="3" {% if not can_comment %}placeholder="This account cannot comment currently." disabled{% endif %}></textarea>
+                        </div>
+                        {% if can_comment %}
+                        <button type="submit" id="send" class="btn btn-sm btn-primary">Create comment</button>
+                        {% endif %}
+                        
+                        {% if not user.is_authenticated %}
+                        </fieldset>
+                        {% endif %}
+                    </form>
+                </div>
+            </div>
+            {% endif %}
+        </section>
+    </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
-{% extends 'booru/base.html' %} {% load staticfiles %} {% block css %}
+{% extends 'booru/base.html' %} {% load static %} {% block css %}
 {% endblock %} {% block ld_json %}
 {% endblock %} {% block scripts %}
 {% endblock %} {% block body %} {% load humanize %} {% load number_converter %}
-{% load markdown_deux_tags %} {% load permission_tags %} {% load
-crispy_forms_tags %}
+{% load markdownify %} {% load permission_tags %} {% load crispy_forms_tags %}
     * {% if previous_post %}
     * _P_r_e_v_i_o_u_s
     * {% else %}
     * _P_r_e_v_i_o_u_s
     * {% endif %} {% if next_post %}
     * _N_e_x_t
     * {% else %}
@@ -56,15 +55,15 @@
 {% endif %} {% endif %}
 {% if request.user.show_comments or not user.is_authenticated %} Comments {%
 endif %} Edit {% if user|can:'change_status' %}
 _A_p_p_r_o_v_e _H_i_d_e _D_e_l_e_t_e
 {% endif %}
 {% if post.description %}
 **** DDeessccrriippttiioonn ****
-{{post.description|markdown}}
+{{post.description|markdownify}}
 {% endif %}
 {% csrf_token %} {{ form |crispy }} Update
 {% if request.user.show_comments or not user.is_authenticated %}
 {% for comment in post.comments.all %} {% if not comment.is_hidden or user|can:
 'manage_comments' %}
 {% if comment.author.is_deleted %}
 **** {{{{ccoommmmeenntt..aauutthhoorr..ggeett__nnaammee}}}} ****
@@ -72,15 +71,15 @@
 **** _{{_{{_cc_oo_mm_mm_ee_nn_tt_.._aa_uu_tt_hh_oo_rr_.._gg_ee_tt____nn_aa_mm_ee_}}_}} ****
 {% endif %}
 {{comment.timestamp|naturaltime}}
 Score: {{comment.get_score}}
 {% if comment.is_hidden %}
 Comment is hidden
 {% endif %}
-{{comment.content|markdown}}
+{{comment.content|markdownify}}
 {% if user|can:'manage_comments' %}
 {% if comment.is_hidden %}
 _S_h_o_w
 {% else %}
 _H_i_d_e
 {% endif %}
 {% endif %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/posts.html` & `Boorunaut-0.5.0/booru/templates/booru/posts.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/post_detail.css' %}"/>
-    {% endblock %}
-
-{% block scripts %}
-<script>
-$(function () {
-    $('[data-toggle="tooltip"]').tooltip()
-})
-</script>
-{% endblock %}
-
-{% block ld_json %}
-<link href="{{request.get_host}}{{request.path}}" rel="canonical" />
-{% endblock %}
-
-
-{% block body %}
-    {% load number_converter %}
-    <div class="row">
-        <aside id="sidebar" class="col-md-3 col">
-            <div id="tag-tables" class="col">
-                <div id="tag-table-general" class="mb-3">
-                    <div class="row col">
-                        <span class="font-weight-bold">Tags</span>
-                    </div>
-                    <table class="tag-table table-sm table borderless">
-                        <tbody>
-                            {% for tag in tags_list %}
-                            <tr>
-                                <th class="tag-wiki-link" scope="row">
-                                    <a style="color: #{{tag.category.color}};" href="{% url 'booru:tag_detail' tag.id %}">
-                                        ?
-                                    </a>
-                                </th>
-                                <td class="tag-label">
-                                    <a style="color: #{{tag.category.color}};" href="{{ tag.get_search_url }}">{{tag}}</a>
-                                </td>
-                                <td class="tag-count">{{tag.get_count|number_converter}}</td>
-                            </tr>
-                            {% endfor %}
-                        </tbody>
-                    </table>
-                </div>
-            </div>
-        </aside>
-        <section id="post" class="col">
-            {% if is_safe_only %}
-            <div class="row mb-3">
-                <div class="col">
-                    <div class="alert alert-primary pt-1 pb-1" role="alert">
-                        <small>
-                            <a href="{% url 'account:settings' %}" data-toggle="tooltip" title="Only safe posts will be shown. Search with any tags or disable it in your account.">
-                                <i class="far fa-eye"></i> Safe Only Listing: On
-                            </a>
-                        </small>
-                    </div>
-                </div>
-            </div>
-            {% endif %}
-            <div class="row">
-                <main class="col">
-                    <div class="row">
-                        {% for post in posts %}
-                        <a class="mr-3 mb-3 {% if post.is_deleted %}border border-danger{% elif post.is_hidden %}border border-warning{% endif %}" style="border-width: 3px !important;" href="{{post.get_absolute_url}}"><img src="{{post.preview.url}}" alt="{{ post.tags_mirror }}" title="{{ post.tags_mirror }}"></a>
-                        {% endfor %}
-                    </div>
-                </main>
-            </div>
-            <div class="row">
-                <nav aria-label="..." class="col mt-5">
-                    <ul class="pagination">
-                        {% if page.has_previous %}
-                            <li class="page-item">
-                                <a class="page-link" href="{% url 'booru:post_page_detail' page.previous_page_number %}" tabindex="-1">Previous</a>
-                            </li>
-                        {% else %}
-                            <li class="page-item disabled">
-                                <a class="page-link" href="#" tabindex="-1">Previous</a>
-                            </li>
-                        {% endif %}
-                        {% for i in page.paginator.page_range %}
-                            {% if page.number == i %}
-                            <li class="page-item active">
-                                <a class="page-link" href="{% url 'booru:post_page_detail' i %}">{{i}} <span class="sr-only">(current)</span></a>
-                            </li>
-                            {% elif i > page.number|add:'-3' and i < page.number|add:'3' %}
-                            <li class="page-item">
-                                <a class="page-link" href="{% url 'booru:post_page_detail' i %}">{{i}}</a>
-                            </li>
-                            {% endif %}
-                        {% endfor %}
-                        {% if page.has_next %}
-                            <li class="page-item">
-                                <a class="page-link" href="{% url 'booru:post_page_detail' page.next_page_number %}">Next</a>
-                            </li>
-                        {% else %}
-                            <li class="page-item disabled">
-                                <a class="page-link" href="#">Next</a>
-                            </li>
-                        {% endif %}
-                    </ul>
-                </nav>
-            </div>
-        </section>
-    </div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/post_detail.css' %}"/>
+    {% endblock %}
+
+{% block scripts %}
+<script>
+$(function () {
+    $('[data-toggle="tooltip"]').tooltip()
+})
+</script>
+{% endblock %}
+
+{% block ld_json %}
+<link href="{{request.get_host}}{{request.path}}" rel="canonical" />
+{% endblock %}
+
+
+{% block body %}
+    {% load number_converter %}
+    <div class="row">
+        <aside id="sidebar" class="col-md-3 col">
+            <div id="tag-tables" class="col">
+                <div id="tag-table-general" class="mb-3">
+                    <div class="row col">
+                        <span class="font-weight-bold">Tags</span>
+                    </div>
+                    <table class="tag-table table-sm table borderless">
+                        <tbody>
+                            {% for tag in tags_list %}
+                            <tr>
+                                <th class="tag-wiki-link" scope="row">
+                                    <a style="color: #{{tag.category.color}};" href="{% url 'booru:tag_detail' tag.id %}">
+                                        ?
+                                    </a>
+                                </th>
+                                <td class="tag-label">
+                                    <a style="color: #{{tag.category.color}};" href="{{ tag.get_search_url }}">{{tag}}</a>
+                                </td>
+                                <td class="tag-count">{{tag.get_count|number_converter}}</td>
+                            </tr>
+                            {% endfor %}
+                        </tbody>
+                    </table>
+                </div>
+            </div>
+        </aside>
+        <section id="post" class="col">
+            {% if is_safe_only %}
+            <div class="row mb-3">
+                <div class="col">
+                    <div class="alert alert-primary pt-1 pb-1" role="alert">
+                        <small>
+                            <a href="{% url 'account:settings' %}" data-toggle="tooltip" title="Only safe posts will be shown. Search with any tags or disable it in your account.">
+                                <i class="far fa-eye"></i> Safe Only Listing: On
+                            </a>
+                        </small>
+                    </div>
+                </div>
+            </div>
+            {% endif %}
+            <div class="row">
+                <main class="col">
+                    <div class="row">
+                        {% for post in posts %}
+                        <a class="mr-3 mb-3 {% if post.is_deleted %}border border-danger{% elif post.is_hidden %}border border-warning{% endif %}" style="border-width: 3px !important;" href="{{post.get_absolute_url}}"><img src="{{post.preview.url}}" alt="{{ post.tags_mirror }}" title="{{ post.tags_mirror }}"></a>
+                        {% endfor %}
+                    </div>
+                </main>
+            </div>
+            <div class="row">
+                <nav aria-label="..." class="col mt-5">
+                    <ul class="pagination">
+                        {% if page.has_previous %}
+                            <li class="page-item">
+                                <a class="page-link" href="{% url 'booru:post_page_detail' page.previous_page_number %}" tabindex="-1">Previous</a>
+                            </li>
+                        {% else %}
+                            <li class="page-item disabled">
+                                <a class="page-link" href="#" tabindex="-1">Previous</a>
+                            </li>
+                        {% endif %}
+                        {% for i in page.paginator.page_range %}
+                            {% if page.number == i %}
+                            <li class="page-item active">
+                                <a class="page-link" href="{% url 'booru:post_page_detail' i %}">{{i}} <span class="sr-only">(current)</span></a>
+                            </li>
+                            {% elif i > page.number|add:'-3' and i < page.number|add:'3' %}
+                            <li class="page-item">
+                                <a class="page-link" href="{% url 'booru:post_page_detail' i %}">{{i}}</a>
+                            </li>
+                            {% endif %}
+                        {% endfor %}
+                        {% if page.has_next %}
+                            <li class="page-item">
+                                <a class="page-link" href="{% url 'booru:post_page_detail' page.next_page_number %}">Next</a>
+                            </li>
+                        {% else %}
+                            <li class="page-item disabled">
+                                <a class="page-link" href="#">Next</a>
+                            </li>
+                        {% endif %}
+                    </ul>
+                </nav>
+            </div>
+        </section>
+    </div>
 {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/staff_hash_ban.html` & `Boorunaut-0.5.0/booru/templates/booru/staff_hash_ban.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-{% extends 'booru/base_admin.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block content %}
-{% load crispy_forms_tags %}
-<div class="col-12 text-white bg-primary">
-    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-ban mr-3"></i>Hash Ban</h1>
-</div>
-
-<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
-    <h1>Ban MD5 Hash</h1>
-    <p>Any MD5 hash here will make the corresponding media to be unallowed to be uploaded on the site.</p>
-
-    <form method="post" enctype="multipart/x-www-form-urlencoded">
-        {% csrf_token %}
-        {{ form |crispy }}
-        <button type="submit" class="btn btn-primary">Ban</button>
-    </form>
-    <table class="table table-striped text-center mt-3">
-        <thead>
-            <tr>
-                <th scope="col">#</th>
-                <th scope="col">MD5 Hash</th>
-                <th scope="col">Created</th>
-                <th scope="col">Last Updated</th>
-                <th scope="col">Creator</th>
-                <th scope="col"></th>
-            </tr>
-        </thead>
-        <tbody>
-            {% for banned_hash in banned_hashes %}
-            <tr>
-                <th scope="row">
-                    {{banned_hash.id}}
-                </th>
-                <td>
-                    {{banned_hash.content}}
-                </td>
-                <td>
-                    {{banned_hash.timestamp}}
-                </td>
-                <td>
-                    {{banned_hash.update_timestamp}}
-                </td>
-                <td>
-                    <a href="{{banned_hash.creator.get_absolute_url}}">{{banned_hash.creator}}</a>
-                </td>
-                <td>
-                    <a href="{% url 'core:hash_ban_delete' banned_hash.id %}">Undo</a>
-                </td>
-            </tr>
-            {% endfor %}
-        </tbody>
-    </table>
-</div>
+{% extends 'booru/base_admin.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block content %}
+{% load crispy_forms_tags %}
+<div class="col-12 text-white bg-primary">
+    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-ban mr-3"></i>Hash Ban</h1>
+</div>
+
+<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
+    <h1>Ban MD5 Hash</h1>
+    <p>Any MD5 hash here will make the corresponding media to be unallowed to be uploaded on the site.</p>
+
+    <form method="post" enctype="multipart/x-www-form-urlencoded">
+        {% csrf_token %}
+        {{ form |crispy }}
+        <button type="submit" class="btn btn-primary">Ban</button>
+    </form>
+    <table class="table table-striped text-center mt-3">
+        <thead>
+            <tr>
+                <th scope="col">#</th>
+                <th scope="col">MD5 Hash</th>
+                <th scope="col">Created</th>
+                <th scope="col">Last Updated</th>
+                <th scope="col">Creator</th>
+                <th scope="col"></th>
+            </tr>
+        </thead>
+        <tbody>
+            {% for banned_hash in banned_hashes %}
+            <tr>
+                <th scope="row">
+                    {{banned_hash.id}}
+                </th>
+                <td>
+                    {{banned_hash.content}}
+                </td>
+                <td>
+                    {{banned_hash.timestamp}}
+                </td>
+                <td>
+                    {{banned_hash.update_timestamp}}
+                </td>
+                <td>
+                    <a href="{{banned_hash.creator.get_absolute_url}}">{{banned_hash.creator}}</a>
+                </td>
+                <td>
+                    <a href="{% url 'core:hash_ban_delete' banned_hash.id %}">Undo</a>
+                </td>
+            </tr>
+            {% endfor %}
+        </tbody>
+    </table>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'booru/base_admin.html' %} {% block css %} {% load staticfiles %} {%
+{% extends 'booru/base_admin.html' %} {% block css %} {% load static %} {%
 endblock %} {% block scripts %} {% endblock %} {% block content %} {% load
 crispy_forms_tags %}
 HHaasshh BBaann
 ************ BBaann MMDD55 HHaasshh ************
 Any MD5 hash here will make the corresponding media to be unallowed to be
 uploaded on the site.
 {% csrf_token %} {{ form |crispy }} Ban
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/staff_mass_rename.html` & `Boorunaut-0.5.0/booru/templates/booru/staff_mass_rename.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-{% extends 'booru/base_admin.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-<script>
-    $( document ).ready(function() {
-        $('#id_filter_by').on('input', function() {
-            $('#mass_rename_filter_by').text($(this).val());
-        });
-        $('#id_when').on('input', function() {
-            $('#mass_rename_when').text($(this).val());
-        });
-        $('#id_replace_with').on('input', function() {
-            $('#mass_rename_replace_with').text($(this).val());
-        });
-    });
-</script>
-{% endblock %}
-
-{% block content %}
-{% load crispy_forms_tags %}
-<div class="col-12 text-white bg-primary">
-    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-user-slash mr-3"></i>Mass Rename</h1>
-</div>
-
-<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
-    <h1>Find and replace tags</h1>
-
-    <p>
-        Everytime there is "<span id="mass_rename_filter_by" class="font-weight-bold"></span>", 
-        replace "<span id="mass_rename_when" class="font-weight-bold"></span>" 
-        with "<span id="mass_rename_replace_with" class="font-weight-bold"></span>".
-    </p>
-    <p class="text-muted">
-        Note: "When" also filters when searching. If "Filter by" is empty, it will search for all (with "When" filtering).
-    </p>
-
-    <form method="post" enctype="multipart/x-www-form-urlencoded">
-        {% csrf_token %}
-        {{ form |crispy }}
-        <button type="submit" class="btn btn-primary">Submit</button>
-    </form>
-</div>
+{% extends 'booru/base_admin.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+<script>
+    $( document ).ready(function() {
+        $('#id_filter_by').on('input', function() {
+            $('#mass_rename_filter_by').text($(this).val());
+        });
+        $('#id_when').on('input', function() {
+            $('#mass_rename_when').text($(this).val());
+        });
+        $('#id_replace_with').on('input', function() {
+            $('#mass_rename_replace_with').text($(this).val());
+        });
+    });
+</script>
+{% endblock %}
+
+{% block content %}
+{% load crispy_forms_tags %}
+<div class="col-12 text-white bg-primary">
+    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-user-slash mr-3"></i>Mass Rename</h1>
+</div>
+
+<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
+    <h1>Find and replace tags</h1>
+
+    <p>
+        Everytime there is "<span id="mass_rename_filter_by" class="font-weight-bold"></span>", 
+        replace "<span id="mass_rename_when" class="font-weight-bold"></span>" 
+        with "<span id="mass_rename_replace_with" class="font-weight-bold"></span>".
+    </p>
+    <p class="text-muted">
+        Note: "When" also filters when searching. If "Filter by" is empty, it will search for all (with "When" filtering).
+    </p>
+
+    <form method="post" enctype="multipart/x-www-form-urlencoded">
+        {% csrf_token %}
+        {{ form |crispy }}
+        <button type="submit" class="btn btn-primary">Submit</button>
+    </form>
+</div>
 {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/staff_mod_queue.html` & `Boorunaut-0.5.0/booru/templates/booru/staff_mod_queue.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-{% extends 'booru/base_admin.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block content %}
-{% load markdown_deux_tags %}
-{% load crispy_forms_tags %}
-<div class="col-12 text-white bg-primary">
-    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-tasks mr-3"></i>Moderation Queue</h1>
-</div>
-
-<div class="col bg-white pt-3 pb-3">
-    <div class="row h2 text-center">
-        <div class="col">
-            <i class="fas fa-archive"></i>
-            <a href="{% url 'booru:posts' %}?tags=status:pending">
-                {{pending_posts.count}} posts waiting approval
-            </a>
-        </div>
-        <div class="col">
-            <i class="fas fa-archive"></i>
-            <a href="{% url 'booru:implication-list' %}?status=0">
-                {{pending_implications.count}} pending implications
-            </a>
-        </div>
-    </div>
-    <div class="row pt-5">
-        <h2>Posts flagged for deletion</h2>
-
-        <table class="table table-striped table-hover text-center">
-            <thead class="thead-light">
-                <tr>
-                    <th scope="col">#</th>
-                    <th scope="col">Post</th>
-                    <th scope="col">Reason</th>
-                    <th scope="col">Creator</th>
-                    <th scope="col">Date</th>
-                    <th scope="col">Status</th>
-                    <th scope="col"></th>
-                </tr>
-            </thead>
-            <tbody>
-                {% for flag in post_flags %}
-                <tr>
-                    <th scope="row">{{ flag.id }}</th>
-                    <td>
-                        <a href="{{ flag.post.get_absolute_url }}">{{ flag.post }}</a>
-                    </td>
-                    <td>
-                        {{ flag.reason |markdown }}
-                    </td>
-                    <td><a href="{{ flag.creator.get_absolute_url }}">{{ flag.creator }}</a></td>
-                    <td>{{ flag.timestamp }}</td>
-                    <td>{{ flag.get_status_display }}</td>
-                    <td>
-                        <a href="{% url 'core:mod_queue_resolve' flag.pk %}" class="btn btn-sm btn-primary">
-                            <i class="fas fa-check"></i> Mark as solved
-                        </a>
-                    </td>
-                </tr>
-                {% endfor %}
-            </tbody>
-        </table>
-    </div>
-</div>
+{% extends 'booru/base_admin.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block content %}
+{% load markdownify %}
+{% load crispy_forms_tags %}
+<div class="col-12 text-white bg-primary">
+    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-tasks mr-3"></i>Moderation Queue</h1>
+</div>
+
+<div class="col bg-white pt-3 pb-3">
+    <div class="row h2 text-center">
+        <div class="col">
+            <i class="fas fa-archive"></i>
+            <a href="{% url 'booru:posts' %}?tags=status:pending">
+                {{pending_posts.count}} posts waiting approval
+            </a>
+        </div>
+        <div class="col">
+            <i class="fas fa-archive"></i>
+            <a href="{% url 'booru:implication-list' %}?status=0">
+                {{pending_implications.count}} pending implications
+            </a>
+        </div>
+    </div>
+    <div class="row pt-5">
+        <h2>Posts flagged for deletion</h2>
+
+        <table class="table table-striped table-hover text-center">
+            <thead class="thead-light">
+                <tr>
+                    <th scope="col">#</th>
+                    <th scope="col">Post</th>
+                    <th scope="col">Reason</th>
+                    <th scope="col">Creator</th>
+                    <th scope="col">Date</th>
+                    <th scope="col">Status</th>
+                    <th scope="col"></th>
+                </tr>
+            </thead>
+            <tbody>
+                {% for flag in post_flags %}
+                <tr>
+                    <th scope="row">{{ flag.id }}</th>
+                    <td>
+                        <a href="{{ flag.post.get_absolute_url }}">{{ flag.post }}</a>
+                    </td>
+                    <td>
+                        {{ flag.reason |markdownify }}
+                    </td>
+                    <td><a href="{{ flag.creator.get_absolute_url }}">{{ flag.creator }}</a></td>
+                    <td>{{ flag.timestamp }}</td>
+                    <td>{{ flag.get_status_display }}</td>
+                    <td>
+                        <a href="{% url 'core:mod_queue_resolve' flag.pk %}" class="btn btn-sm btn-primary">
+                            <i class="fas fa-check"></i> Mark as solved
+                        </a>
+                    </td>
+                </tr>
+                {% endfor %}
+            </tbody>
+        </table>
+    </div>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-{% extends 'booru/base_admin.html' %} {% block css %} {% load staticfiles %} {%
+{% extends 'booru/base_admin.html' %} {% block css %} {% load static %} {%
 endblock %} {% block scripts %} {% endblock %} {% block content %} {% load
-markdown_deux_tags %} {% load crispy_forms_tags %}
+markdownify %} {% load crispy_forms_tags %}
 MMooddeerraattiioonn QQuueeuuee
 _{_{_p_e_n_d_i_n_g___p_o_s_t_s_._c_o_u_n_t_}_}_ _p_o_s_t_s_ _w_a_i_t_i_n_g_ _a_p_p_r_o_v_a_l
 _{_{_p_e_n_d_i_n_g___i_m_p_l_i_c_a_t_i_o_n_s_._c_o_u_n_t_}_}_ _p_e_n_d_i_n_g_ _i_m_p_l_i_c_a_t_i_o_n_s
 ********** PPoossttss ffllaaggggeedd ffoorr ddeelleettiioonn **********
-##       PPoosstt      RReeaassoonn      CCrreeaattoorr      DDaattee           SSttaattuuss
-{{       _{         {           _{            {              {
-{{       _{         {           _{            {              {                       _M_a_r_k
-ffllaagg..iidd _f_l_a_g_._p_o_s_t flag.reason _f_l_a_g_._c_r_e_a_t_o_r flag.timestamp flag.get_status_display _a_s
-}}}}      _}_}        |markdown   _}_}           }}             }}                      _s_o_l_v_e_d
+##       PPoosstt      RReeaassoonn       CCrreeaattoorr      DDaattee           SSttaattuuss
+{{       _{         {            _{            {              {
+{{       _{         {            _{            {              {                       _M_a_r_k
+ffllaagg..iidd _f_l_a_g_._p_o_s_t flag.reason  _f_l_a_g_._c_r_e_a_t_o_r flag.timestamp flag.get_status_display _a_s
+}}}}      _}_}        |markdownify _}_}           }}             }}                      _s_o_l_v_e_d
                   }}
 {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/staff_page.html` & `Boorunaut-0.5.0/booru/templates/booru/staff_page.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-{% extends 'booru/base_admin.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block content %}
-<div class="col-12 text-white bg-primary">
-    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-chart-line mr-3"></i>Statistics</h1>
-</div>
-
-<div class="col bg-white align-middle p-4">
-    <div class="row">
-        <div class="col-1 mr-2">
-            <i class="fas fa-users align-top" style="font-size: 4.6875rem;"></i>
-        </div>
-        <div class="col-1 text-center">
-            <div class="col" style="font-size: 2.8125rem; height: 3.09375rem;">
-                {{accounts.count}}
-            </div>
-            <div class="col">
-                <small>Users</small>
-            </div>
-        </div>
-    </div>
-</div>
-
-<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
-    <h1>Registered Users</h1>
-
-    <div class="row mt-4">
-        <table class="table table-striped table-bordered">
-            <thead>
-                <tr>
-                    <th scope="col">Username</th>
-                    <th scope="col">Register Date</th>
-                    <th scope="col">Last Login</th>
-                </tr>
-            </thead>
-            <tbody>
-                {% for account in accounts %}
-                <tr>
-                    <th scope="row"><a href="{{account.get_absolute_url}}">{{account.username}}</a></th>
-                    <td>{{account.date_joined}}</td>
-                    <td>{{account.last_login}}</td>
-                </tr>
-                {% endfor %}
-            </tbody>
-        </table>
-    </div>
-</div>
+{% extends 'booru/base_admin.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block content %}
+<div class="col-12 text-white bg-primary">
+    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-chart-line mr-3"></i>Statistics</h1>
+</div>
+
+<div class="col bg-white align-middle p-4">
+    <div class="row">
+        <div class="col-1 mr-2">
+            <i class="fas fa-users align-top" style="font-size: 4.6875rem;"></i>
+        </div>
+        <div class="col-1 text-center">
+            <div class="col" style="font-size: 2.8125rem; height: 3.09375rem;">
+                {{accounts.count}}
+            </div>
+            <div class="col">
+                <small>Users</small>
+            </div>
+        </div>
+    </div>
+</div>
+
+<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
+    <h1>Registered Users</h1>
+
+    <div class="row mt-4">
+        <table class="table table-striped table-bordered">
+            <thead>
+                <tr>
+                    <th scope="col">Username</th>
+                    <th scope="col">Register Date</th>
+                    <th scope="col">Last Login</th>
+                </tr>
+            </thead>
+            <tbody>
+                {% for account in accounts %}
+                <tr>
+                    <th scope="row"><a href="{{account.get_absolute_url}}">{{account.username}}</a></th>
+                    <td>{{account.date_joined}}</td>
+                    <td>{{account.last_login}}</td>
+                </tr>
+                {% endfor %}
+            </tbody>
+        </table>
+    </div>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'booru/base_admin.html' %} {% block css %} {% load staticfiles %} {%
+{% extends 'booru/base_admin.html' %} {% block css %} {% load static %} {%
 endblock %} {% block scripts %} {% endblock %} {% block content %}
 SSttaattiissttiiccss
 {{accounts.count}}
 Users
 ************ RReeggiisstteerreedd UUsseerrss ************
 UUsseerrnnaammee             RReeggiisstteerr DDaattee           LLaasstt LLooggiinn
 _{{_{{_aa_cc_cc_oo_uu_nn_tt_.._uu_ss_ee_rr_nn_aa_mm_ee_}}_}} {{account.date_joined}} {{account.last_login}}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/staff_site_configuration.html` & `Boorunaut-0.5.0/booru/templates/booru/staff_site_configuration.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-{% extends 'booru/base_admin.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-    <link href="{% static 'booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css' %}" rel="stylesheet">
-{% endblock %}
-
-{% block scripts %}
-    <script src="{% static 'booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js' %}"></script>
-{% endblock %}
-
-{% block content %}
-{% load crispy_forms_tags %}
-<div class="col-12 text-white bg-primary">
-    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-cogs mr-3"></i>Configuration</h1>
-</div>
-
-<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
-    <h1>Customize the booru</h1>
-
-    <form method="post" enctype="multipart/x-www-form-urlencoded">
-        {% csrf_token %}
-        {% for field in form %}
-            {% if field.label != 'Welcome page' %}
-                {{ field|as_crispy_field }}
-            {% else %}
-            <div id="div_id_announcement" class="form-group">
-                <label for="id_announcement" class="col-form-label">{{ field.label }}</label>
-                <div class="">
-                    {{ field }}
-                </div>
-            </div>
-            {% endif %}
-        {% endfor%}
-        <button type="submit" class="btn btn-primary">Submit</button>
-    </form>
-</div>
+{% extends 'booru/base_admin.html' %}
+
+{% block css %}
+    {% load static %}
+    <link href="{% static 'booru/bootstrap-toggle-master/css/bootstrap-toggle.min.css' %}" rel="stylesheet">
+{% endblock %}
+
+{% block scripts %}
+    <script src="{% static 'booru/bootstrap-toggle-master/js/bootstrap-toggle.min.js' %}"></script>
+{% endblock %}
+
+{% block content %}
+{% load crispy_forms_tags %}
+<div class="col-12 text-white bg-primary">
+    <h1 class="h4 text-uppercase p-3 mb-0"><i class="fas fa-cogs mr-3"></i>Configuration</h1>
+</div>
+
+<div class="col bg-white align-middle mt-3 pl-4 pt-3 pb-3 pr-4">
+    <h1>Customize the booru</h1>
+
+    <form method="post" enctype="multipart/x-www-form-urlencoded">
+        {% csrf_token %}
+        {% for field in form %}
+            {% if field.label != 'Welcome page' %}
+                {{ field|as_crispy_field }}
+            {% else %}
+            <div id="div_id_announcement" class="form-group">
+                <label for="id_announcement" class="col-form-label">{{ field.label }}</label>
+                <div class="">
+                    {{ field }}
+                </div>
+            </div>
+            {% endif %}
+        {% endfor%}
+        <button type="submit" class="btn btn-primary">Submit</button>
+    </form>
+</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'booru/base_admin.html' %} {% block css %} {% load staticfiles %}
+{% extends 'booru/base_admin.html' %} {% block css %} {% load static %}
 {% endblock %} {% block scripts %}
 {% endblock %} {% block content %} {% load crispy_forms_tags %}
 CCoonnffiigguurraattiioonn
 ************ CCuussttoommiizzee tthhee bboooorruu ************
 {% csrf_token %} {% for field in form %} {% if field.label != 'Welcome page' %}
 {{ field|as_crispy_field }} {% else %}
 {{ field.label }}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/tag_detail.html` & `Boorunaut-0.5.0/booru/templates/booru/tag_detail.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-    {% load markdown_deux_tags %}
-    {% load permission_tags %}
-    <div class="container">
-        <div class="row">
-            <h1>Tag: <a href="{{ tag.get_search_url }}">{{tag}}</a></h1>
-        </div>
-        <div class="row">
-            <span class="col">
-                <a class="btn btn-sm btn-primary" href="{% url 'booru:tag_edit' tag.id %}">
-                    <i class="fas fa-edit"></i> Edit
-                </a>
-                <a class="btn btn-sm btn-primary" href="{% url 'booru:tag_history' tag.id %}">
-                    <i class="fas fa-history"></i> History
-                </a>
-                {% if user|can:'manage_tags' %}
-                <a class="btn btn-sm btn-danger" href="{% url 'booru:tag-delete' tag.id %}">
-                    <i class="fas fa-trash"></i> Delete
-                </a>
-                {% endif %}
-            </span>
-        </div>
-        <div class="row">
-            <div id="table" class="col mt-3">
-                <table class="table table-sm">
-                    <tbody>
-                        {% if tag.description %}
-                        <tr>
-                            <td><strong>Description:</strong></td>
-                            <td>{{tag.description|markdown}}</td>
-                        </tr>
-                        {% endif %}
-                        <tr>
-                            <td><strong>Category:</strong></td>
-                            <td>{{tag.category}}</td>
-                        </tr>
-                        {% if tag.associated_link %}
-                        <tr>
-                            <td><strong>Associated links:</strong></td>
-                            <td>{{tag.associated_link}}</td>
-                        </tr>
-                        {% endif %}
-                        {% if tag.associated_user %}
-                        <tr>
-                            <td><strong>Associated user:</strong></td>
-                            <td><a href="{% url 'booru:profile' tag.associated_user %}">
-                                    {{tag.associated_user}}
-                                </a>
-                            </td>
-                        </tr>
-                        {% endif %}
-                        {% if tag.timestamp %}
-                        <tr>
-                            <td><strong>Date:</strong></td>
-                            <td>{{tag.timestamp}}</td>
-                        </tr>
-                        {% endif %}
-                        {% if tag.author %}
-                        <tr>
-                            <td><strong>Author:</strong></td>
-                            <td><a href="{{tag.author.get_absolute_url}}">{{tag.author}}</a></td>
-                        </tr>
-                        {% endif %}
-                        {% if tag.aliases %}
-                        <tr>
-                            <td><strong>Aliases:</strong></td>
-                            <td>
-                                {% for tag in tag.aliases.all %}
-                                {{tag}}{% if not forloop.last %},{% endif %}
-                                {% endfor %}
-                            </td>
-                        </tr>
-                        {% endif %}
-                        {% if tag.from_implications.count > 0 %}
-                        <tr>
-                            <td><strong>Implies:</strong></td>
-                            <td>
-                                {% for implication in tag.from_implications.all %}
-                                {% with color='#'|add:implication.to_tag.category.color %}
-                                <a style="color: {{color}};" class="font-weight-bold" href="{% url 'booru:tag_detail' implication.to_tag.id %}">
-                                    ?
-                                </a>
-                                <a style="color: {{color}};" href="{{ implication.to_tag.get_search_url }}">{{implication.to_tag}}</a>
-                                {% endwith %}
-                                {% if not forloop.last %},{% endif %}
-                                {% endfor %}
-                            </td>
-                        </tr>
-                        {% endif %}
-                        {% if tag.to_implications.count > 0 %}
-                        <tr>
-                            <td><strong>Is implied in:</strong></td>
-                            <td>
-                                {% for implication in tag.to_implications.all %}
-                                {% with color='#'|add:implication.from_tag.category.color %}
-                                <a style="color:{{color}};" class="font-weight-bold" href="{% url 'booru:tag_detail' implication.from_tag.id %}">
-                                    ?
-                                </a>
-                                <a style="color:{{color}};" href="{{ implication.from_tag.get_search_url }}">{{implication.from_tag}}</a>
-                                {% endwith %}
-                                {% if not forloop.last %},{% endif %} 
-                                {% endfor %}
-                            </td>
-                        </tr>
-                        {% endif %}
-                    </tbody>
-                </table>
-            </div>
-        </div>
-        <div class="row">
-            {% for post in last_post %}
-            <a href="{{post.get_absolute_url}}"><img src="{{post.preview.url}}" alt=""></a>
-            {% endfor %}
-        </div>
-    </div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+    {% load markdownify %}
+    {% load permission_tags %}
+    <div class="container">
+        <div class="row">
+            <h1>Tag: <a href="{{ tag.get_search_url }}">{{tag}}</a></h1>
+        </div>
+        <div class="row">
+            <span class="col">
+                <a class="btn btn-sm btn-primary" href="{% url 'booru:tag_edit' tag.id %}">
+                    <i class="fas fa-edit"></i> Edit
+                </a>
+                <a class="btn btn-sm btn-primary" href="{% url 'booru:tag_history' tag.id %}">
+                    <i class="fas fa-history"></i> History
+                </a>
+                {% if user|can:'manage_tags' %}
+                <a class="btn btn-sm btn-danger" href="{% url 'booru:tag-delete' tag.id %}">
+                    <i class="fas fa-trash"></i> Delete
+                </a>
+                {% endif %}
+            </span>
+        </div>
+        <div class="row">
+            <div id="table" class="col mt-3">
+                <table class="table table-sm">
+                    <tbody>
+                        {% if tag.description %}
+                        <tr>
+                            <td><strong>Description:</strong></td>
+                            <td>{{tag.description|markdownify}}</td>
+                        </tr>
+                        {% endif %}
+                        <tr>
+                            <td><strong>Category:</strong></td>
+                            <td>{{tag.category}}</td>
+                        </tr>
+                        {% if tag.associated_link %}
+                        <tr>
+                            <td><strong>Associated links:</strong></td>
+                            <td>{{tag.associated_link}}</td>
+                        </tr>
+                        {% endif %}
+                        {% if tag.associated_user %}
+                        <tr>
+                            <td><strong>Associated user:</strong></td>
+                            <td><a href="{% url 'booru:profile' tag.associated_user %}">
+                                    {{tag.associated_user}}
+                                </a>
+                            </td>
+                        </tr>
+                        {% endif %}
+                        {% if tag.timestamp %}
+                        <tr>
+                            <td><strong>Date:</strong></td>
+                            <td>{{tag.timestamp}}</td>
+                        </tr>
+                        {% endif %}
+                        {% if tag.author %}
+                        <tr>
+                            <td><strong>Author:</strong></td>
+                            <td><a href="{{tag.author.get_absolute_url}}">{{tag.author}}</a></td>
+                        </tr>
+                        {% endif %}
+                        {% if tag.aliases %}
+                        <tr>
+                            <td><strong>Aliases:</strong></td>
+                            <td>
+                                {% for tag in tag.aliases.all %}
+                                {{tag}}{% if not forloop.last %},{% endif %}
+                                {% endfor %}
+                            </td>
+                        </tr>
+                        {% endif %}
+                        {% if tag.from_implications.count > 0 %}
+                        <tr>
+                            <td><strong>Implies:</strong></td>
+                            <td>
+                                {% for implication in tag.from_implications.all %}
+                                {% with color='#'|add:implication.to_tag.category.color %}
+                                <a style="color: {{color}};" class="font-weight-bold" href="{% url 'booru:tag_detail' implication.to_tag.id %}">
+                                    ?
+                                </a>
+                                <a style="color: {{color}};" href="{{ implication.to_tag.get_search_url }}">{{implication.to_tag}}</a>
+                                {% endwith %}
+                                {% if not forloop.last %},{% endif %}
+                                {% endfor %}
+                            </td>
+                        </tr>
+                        {% endif %}
+                        {% if tag.to_implications.count > 0 %}
+                        <tr>
+                            <td><strong>Is implied in:</strong></td>
+                            <td>
+                                {% for implication in tag.to_implications.all %}
+                                {% with color='#'|add:implication.from_tag.category.color %}
+                                <a style="color:{{color}};" class="font-weight-bold" href="{% url 'booru:tag_detail' implication.from_tag.id %}">
+                                    ?
+                                </a>
+                                <a style="color:{{color}};" href="{{ implication.from_tag.get_search_url }}">{{implication.from_tag}}</a>
+                                {% endwith %}
+                                {% if not forloop.last %},{% endif %} 
+                                {% endfor %}
+                            </td>
+                        </tr>
+                        {% endif %}
+                    </tbody>
+                </table>
+            </div>
+        </div>
+        <div class="row">
+            {% for post in last_post %}
+            <a href="{{post.get_absolute_url}}"><img src="{{post.preview.url}}" alt=""></a>
+            {% endfor %}
+        </div>
+    </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-{% extends 'booru/base.html' %} {% block css %} {% load staticfiles %} {%
-endblock %} {% block scripts %} {% endblock %} {% block body %} {% load
-markdown_deux_tags %} {% load permission_tags %}
+{% extends 'booru/base.html' %} {% block css %} {% load static %} {% endblock
+%} {% block scripts %} {% endblock %} {% block body %} {% load markdownify %}
+{% load permission_tags %}
 ************ TTaagg:: _{{_{{_tt_aa_gg_}}_}} ************
 _E_d_i_t
 _H_i_s_t_o_r_y
 {% if user|can:'manage_tags' %}
 _D_e_l_e_t_e
 {% endif %}
-DDeessccrriippttiioonn::      {{tag.description|markdown}}
+DDeessccrriippttiioonn::      {{tag.description|markdownify}}
 CCaatteeggoorryy::         {{tag.category}}
 AAssssoocciiaatteedd lliinnkkss:: {{tag.associated_link}}
 AAssssoocciiaatteedd uusseerr::  _{_{_t_a_g_._a_s_s_o_c_i_a_t_e_d___u_s_e_r_}_}
 DDaattee::             {{tag.timestamp}}
 AAuutthhoorr::           _{_{_t_a_g_._a_u_t_h_o_r_}_}
 AAlliiaasseess::          {% for tag in tag.aliases.all %} {{tag}}{% if not
                   forloop.last %},{% endif %} {% endfor %}
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/tag_history.html` & `Boorunaut-0.5.0/booru/templates/booru/post_history.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,106 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-    <div class="container">
-        <div class="row">
-            <h1>Tag: <a href="{% url 'booru:tag_detail' tag.id %}">{{tag}}</a></h1>
-        </div>
-
-        <div class="row mt-3 mb-3">
-            <form class="col" method="get" action="{% url 'booru:tag_revision_diff' tag.id %}" enctype="multipart/form-data">
-                <div id="table">
-                    <table class="table table-striped text-center">
-                        <thead>
-                            <tr>
-                                <th scope="col"> </th>
-                                <th scope="col">Version</th>
-                                <th scope="col">Last edited</th>
-                            </tr>
-                        </thead>
-                        <tbody>
-                            {% for version in page.object_list %}
-                            <tr>
-                                <th scope="row">
-                                    diff
-                                    <input class="" type="radio" name="oldRevision" id="oldRevisionOption{{version.history_id}}" value="{{version.history_id}}" checked>
-                                    <input class="" type="radio" name="newRevision" id="newRevisionOption{{version.history_id}}" value="{{version.history_id}}" checked>
-                                </th>
-                                <td>
-                                    <a href="{% url 'booru:tag_revision_diff' tag.id %}?oldRevision={{version.history_id}}&newRevision={{version.history_id}}">
-                                        {{version.name}}
-                                    </a>
-                                </td>
-                                <td>
-                                    {{version.history_date}} by
-                                    <a href="{% url 'booru:profile' version.history_user %}">{{version.history_user}}</a>
-                                </td>
-                            </tr>
-                            {% endfor %}
-                        </tbody>
-                    </table>
-                </div>
-                <button type="submit" class="btn btn-primary">See differences</button>
-            </form>
-        </div>
-
-        <nav aria-label="..." class="mt-5">
-            <ul class="pagination">
-                {% if page.has_previous %}
-                    <li class="page-item">
-                        <a class="page-link" href="{% url 'booru:tag_history' tag.id page.previous_page_number %}" tabindex="-1">Previous</a>
-                    </li>
-                {% else %}
-                    <li class="page-item disabled">
-                        <a class="page-link" href="#" tabindex="-1">Previous</a>
-                    </li>
-                {% endif %}
-                {% for i in page.paginator.page_range %}
-                    {% if page.number == i %}
-                    <li class="page-item active">
-                        <a class="page-link" href="{% url 'booru:tag_history' tag.id i %}">{{i}} <span class="sr-only">(current)</span></a>
-                    </li>
-                    {% elif i > page.number|add:'-3' and i < page.number|add:'3' %}
-                    <li class="page-item">
-                        <a class="page-link" href="{% url 'booru:tag_history' tag.id i %}">{{i}}</a>
-                    </li>
-                    {% endif %}
-                {% endfor %}
-                {% if page.has_next %}
-                    <li class="page-item">
-                        <a class="page-link" href="{% url 'booru:tag_history' tag.id page.next_page_number %}">Next</a>
-                    </li>
-                {% else %}
-                    <li class="page-item disabled">
-                        <a class="page-link" href="#">Next</a>
-                    </li>
-                {% endif %}
-            </ul>
-        </nav>
-    </div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+    {% load version_comparator %}
+    <div class="container">
+        <div class="row">
+            <h1>Post: <a href="{% url 'booru:post_detail' post.id %}">{{post}}</a></h1>
+        </div>
+
+        <div class="row mt-3 mb-3">
+            <div id="table">
+                <table class="table table-striped text-center">
+                    <thead>
+                        <tr>
+                            <th scope="col">Post</th>
+                            <th scope="col">Date</th>
+                            <th scope="col">User</th>
+                            <th scope="col">Rating</th>
+                            <th scope="col">Parent</th>
+                            <th scope="col">Source</th>
+                            <th scope="col">Tags</th>
+                        </tr>
+                    </thead>
+                    <tbody>
+                        {% for version in page.object_list %}
+                        <tr>
+                            <th scope="row">
+                                <a href="{{post.get_absolute_url}}">
+                                    {{post}}
+                                </a>
+                            </th>
+                            <td>
+                                {{version.history_date}}
+                            </td>
+                            <td>
+                                <a href="{% url 'booru:profile' version.history_user %}">{{version.history_user}}</a>
+                            </td>
+                            <td>
+                                {% if version.rating == 0 %}
+                                None
+                                {% elif version.rating == 1 %}
+                                Safe
+                                {% elif version.rating == 2 %}
+                                Questionable
+                                {% elif version.rating == 3 %}
+                                Explicit
+                                {% endif %}
+                            </td>
+                            <td>
+                                {{version.parent}}
+                            </td>
+                            <td>
+                                {{version.source}}
+                            </td>
+                            <td>
+                                {% version_comparator version "tags_mirror" %}
+                            </td>
+                        </tr>
+                        {% endfor %}
+                    </tbody>
+                </table>
+            </div>
+        </div>
+
+        <nav aria-label="..." class="mt-5">
+            <ul class="pagination">
+                {% if page.has_previous %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:post_history' post.id page.previous_page_number %}" tabindex="-1">Previous</a>
+                    </li>
+                {% else %}
+                    <li class="page-item disabled">
+                        <a class="page-link" href="#" tabindex="-1">Previous</a>
+                    </li>
+                {% endif %}
+                {% for i in page.paginator.page_range %}
+                    {% if page.number == i %}
+                    <li class="page-item active">
+                        <a class="page-link" href="{% url 'booru:post_history' post.id i %}">{{i}} <span class="sr-only">(current)</span></a>
+                    </li>
+                    {% elif i > page.number|add:'-3' and i < page.number|add:'3' %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:post_history' post.id i %}">{{i}}</a>
+                    </li>
+                    {% endif %}
+                {% endfor %}
+                {% if page.has_next %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:post_history' post.id page.next_page_number %}">Next</a>
+                    </li>
+                {% else %}
+                    <li class="page-item disabled">
+                        <a class="page-link" href="#">Next</a>
+                    </li>
+                {% endif %}
+            </ul>
+        </nav>
+    </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,27 @@
-{% extends 'booru/base.html' %} {% block css %} {% load staticfiles %} {%
-endblock %} {% block scripts %} {% endblock %} {% block body %}
-************ TTaagg:: _{{_{{_tt_aa_gg_}}_}} ************
-       VVeerrssiioonn          LLaasstt eeddiitteedd
-ddiiffff#### _{_{_v_e_r_s_i_o_n_._n_a_m_e_}_} {{version.history_date}} by _{_{_v_e_r_s_i_o_n_._h_i_s_t_o_r_y___u_s_e_r_}_}
-See differences
+{% extends 'booru/base.html' %} {% block css %} {% load static %} {% endblock
+%} {% block scripts %} {% endblock %} {% block body %} {% load
+version_comparator %}
+************ PPoosstt:: _{{_{{_pp_oo_ss_tt_}}_}} ************
+PPoosstt    DDaattee                    UUsseerr                    RRaattiinngg         PPaarreenntt            SSoouurrccee            TTaaggss
+                                                        {% if
+                                                        version.rating
+                                                        == 0 %} None
+                                                        {% elif
+                                                        version.rating
+                                                        == 1 %} Safe                                       {%
+_{{       {                       _{                       {% elif        {                 {                 version_comparator
+_{{_pp_oo_ss_tt_}}_}} {version.history_date}} _{_v_e_r_s_i_o_n_._h_i_s_t_o_r_y___u_s_e_r_}_} version.rating {version.parent}} {version.source}} version
+                                                        == 2 %}                                            "tags_mirror" %}
+                                                        Questionable
+                                                        {% elif
+                                                        version.rating
+                                                        == 3 %}
+                                                        Explicit {%
+                                                        endif %}
     * {% if page.has_previous %}
     * _P_r_e_v_i_o_u_s
     * {% else %}
     * _P_r_e_v_i_o_u_s
     * {% endif %} {% for i in page.paginator.page_range %} {% if page.number ==
       i %}
     * _{_{_i_}_}_ _(_c_u_r_r_e_n_t_)
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/tag_list.html` & `Boorunaut-0.5.0/booru/templates/booru/gallery_history.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,87 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-{% endblock %}
-
-{% block body %}
-{% load crispy_forms_tags %}
-<div class="container">
-    <form method="get">
-        {{ form |crispy }}
-        <button type="submit" class="btn btn-sm btn-primary">Search</button>
-    </form>
-
-    <div class="row mt-3">
-        <div id="table" class="col">
-            <table class="table table-striped text-center border">
-                <thead>
-                    <tr>
-                        <th scope="col">#</th>
-                        <th scope="col">Count</th>
-                        <th scope="col">Name</th>
-                        {% if user.is_authenticated %}
-                        <th scope="col"></th>
-                        {% endif %}
-                    </tr>
-                </thead>
-                <tbody>
-                    {% for tag in tags %}
-                    <tr>
-                        <th scope="row">{{ forloop.counter }}</th>
-                        <td>{{tag.get_count}}</td>
-                        <td>
-                            <a class="font-weight-bold" style="color: #{{tag.category.color}};" href="{% url 'booru:tag_detail' tag.id %}">?</a>
-                            <a style="color: #{{tag.category.color}};" href="{{ tag.get_search_url }}">{{tag.name}}</a>
-                        </td>
-                        {% if user.is_authenticated %}
-                        <td scope="col"><a href="{% url 'booru:tag_edit' tag.id %}">Edit</a></td>
-                        {% endif %}
-                    </tr>
-                    {% endfor %}
-                </tbody>
-            </table>
-
-            <nav aria-label="..." class="mt-5">
-                <ul class="pagination">
-                    {% if page.has_previous %}
-                        <li class="page-item">
-                            <a class="page-link" href="{% url 'booru:tags_page_list' page.previous_page_number %}" tabindex="-1">Previous</a>
-                        </li>
-                    {% else %}
-                        <li class="page-item disabled">
-                            <a class="page-link" href="#" tabindex="-1">Previous</a>
-                        </li>
-                    {% endif %}
-                    {% for i in page.paginator.page_range %}
-                        {% if page.number == i %}
-                        <li class="page-item active">
-                            <a class="page-link" href="{% url 'booru:tags_page_list' i %}">{{i}} <span class="sr-only">(current)</span></a>
-                        </li>
-                        {% elif i > page.number|add:'-3' and i < page.number|add:'3' %}
-                        <li class="page-item">
-                            <a class="page-link" href="{% url 'booru:tags_page_list' i %}">{{i}}</a>
-                        </li>
-                        {% endif %}
-                    {% endfor %}
-                    {% if page.has_next %}
-                        <li class="page-item">
-                            <a class="page-link" href="{% url 'booru:tags_page_list' page.next_page_number %}">Next</a>
-                        </li>
-                    {% else %}
-                        <li class="page-item disabled">
-                            <a class="page-link" href="#">Next</a>
-                        </li>
-                    {% endif %}
-                </ul>
-            </nav>
-        </div>
-    </div>
-</div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+    <link rel="stylesheet" type="text/css" href="{% static 'booru/css/index.css' %}"/>
+{% endblock %}
+
+{% block scripts %}
+{% endblock %}
+
+{% block body %}
+    {% load version_comparator %}
+    <div class="container">
+        <div class="row">
+            <h1>Gallery: <a href="{% url 'booru:gallery_detail' gallery.id %}">{{gallery}}</a></h1>
+        </div>
+
+        <div class="mt-3 mb-3">
+            <div id="table">
+                <table class="table table-striped text-center">
+                    <thead>
+                        <tr>
+                            <th scope="col">Gallery</th>
+                            <th scope="col">Tags</th>
+                            <th scope="col">Date</th>
+                            <th scope="col">User</th>
+                        </tr>
+                    </thead>
+                    <tbody>
+                        {% for version in page.object_list %}
+                        <tr>
+                            <th scope="row">
+                                <a href="{{gallery.get_absolute_url}}">
+                                    #{{gallery.id}}
+                                </a>
+                            </th>
+                            <td>
+                                {% version_comparator version "posts_mirror" %}
+                            </td>
+                            <td>
+                                {{version.history_date}}
+                            </td>
+                            <td>
+                                <a href="{% url 'booru:profile' version.history_user %}">{{version.history_user}}</a>
+                            </td>
+                        </tr>
+                        {% endfor %}
+                    </tbody>
+                </table>
+            </div>
+        </div>
+
+        <nav aria-label="..." class="mt-5">
+            <ul class="pagination">
+                {% if page.has_previous %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:gallery_history_page' gallery.id page.previous_page_number %}" tabindex="-1">Previous</a>
+                    </li>
+                {% else %}
+                    <li class="page-item disabled">
+                        <a class="page-link" href="#" tabindex="-1">Previous</a>
+                    </li>
+                {% endif %}
+                {% for i in page.paginator.page_range %}
+                    {% if page.number == i %}
+                    <li class="page-item active">
+                        <a class="page-link" href="{% url 'booru:gallery_history_page' gallery.id i %}">{{i}} <span class="sr-only">(current)</span></a>
+                    </li>
+                    {% elif i > page.number|add:'-3' and i < page.number|add:'3' %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:gallery_history_page' gallery.id i %}">{{i}}</a>
+                    </li>
+                    {% endif %}
+                {% endfor %}
+                {% if page.has_next %}
+                    <li class="page-item">
+                        <a class="page-link" href="{% url 'booru:gallery_history_page' gallery.id page.next_page_number %}">Next</a>
+                    </li>
+                {% else %}
+                    <li class="page-item disabled">
+                        <a class="page-link" href="#">Next</a>
+                    </li>
+                {% endif %}
+            </ul>
+        </nav>
+    </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-{% extends 'booru/base.html' %} {% block css %} {% load staticfiles %} {%
-endblock %} {% block scripts %} {% endblock %} {% block body %} {% load
-crispy_forms_tags %}
-{{ form |crispy }} Search
-##                     CCoouunntt             NNaammee
-{{{{ ffoorrlloooopp..ccoouunntteerr }}}} {{tag.get_count}} _? _{_{_t_a_g_._n_a_m_e_}_} _E_d_i_t
+{% extends 'booru/base.html' %} {% block css %} {% load static %}
+{% endblock %} {% block scripts %} {% endblock %} {% block body %} {% load
+version_comparator %}
+************ GGaalllleerryy:: _{{_{{_gg_aa_ll_ll_ee_rr_yy_}}_}} ************
+GGaalllleerryy       TTaaggss               DDaattee                    UUsseerr
+              {%
+_##_{{            version_comparator {                       _{
+_{{_gg_aa_ll_ll_ee_rr_yy_.._ii_dd_}}_}} version            {version.history_date}} _{_v_e_r_s_i_o_n_._h_i_s_t_o_r_y___u_s_e_r_}_}
+              "posts_mirror" %}
     * {% if page.has_previous %}
     * _P_r_e_v_i_o_u_s
     * {% else %}
     * _P_r_e_v_i_o_u_s
     * {% endif %} {% for i in page.paginator.page_range %} {% if page.number ==
       i %}
     * _{_{_i_}_}_ _(_c_u_r_r_e_n_t_)
```

### Comparing `Boorunaut-0.4.3/booru/templates/booru/upload.html` & `Boorunaut-0.5.0/booru/templates/booru/upload.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-{% extends 'booru/base.html' %}
-
-{% block css %}
-    {% load staticfiles %}
-{% endblock %}
-
-{% block scripts %}
-<script>
-    $(function () {
-        $("#id_media_url").blur(function() {
-            var image_url = $("#id_media_url").val();
-            if (checkURL(image_url)) {
-                $("#image_preview_block").show();
-                $("#image_preview").attr("src", image_url);
-            }
-            else {
-                $("#image_preview_block").hide();
-            }
-        });
-
-        $('.custom-file-input').change(function(e){
-            var file = e.target.files[0];
-            var fileName = file.name;
-
-            if (file){
-                var reader = new FileReader();
-                reader.onload = function (e) {
-                    $("#image_preview").attr("src", e.target.result);
-                };
-                reader.readAsDataURL(file);
-                $("#image_preview_block").show();
-            }
-            else{
-                $("#image_preview_block").hide();
-            }
-        });
-    });
-
-    function checkURL(url) {
-        return(url.match(/\.(jpeg|jpg|gif|png)$/) != null);
-    }
-</script>
-{% endblock %}
-
-{% block body %}
-<div class="container">
-    <div class="row">
-        <div id="upload" class="col">
-            <h1>Upload</h1>
-            
-            <form method="post" enctype="multipart/form-data">
-                {% csrf_token %}
-
-                {% if form.errors %}
-                    {% for field in form %}
-                        {% for error in field.errors %}
-                            <div class="alert alert-danger">
-                                <strong>{{ error|escape }}</strong>
-                            </div>
-                        {% endfor %}
-                    {% endfor %}
-                    {% for error in form.non_field_errors %}
-                        <div class="alert alert-danger">
-                            <strong>{{ error|escape }}</strong>
-                        </div>
-                    {% endfor %}
-                {% endif %}
-
-                <div class="border border-secondary mb-4 p-2">
-                    <div class="form-group row mt-2">
-                        <label class="col-12 col-md-2 col-form-label text-center">{{ form.media.label }}</label>
-                        
-                        <div class="col">
-                            {{form.media}}
-                            <span class="custom-file-control"></span>
-                            <label class="custom-file-label ml-3 mr-3" for="{{ form.media.auto_id }}">
-                                Choose file
-                            </label>
-                        </div>
-
-                        {% if form.media.errors %}
-                        <div class="md-offset-2 col text-danger small">
-                            {{form.media.errors}}
-                        </div>
-                        {% endif %}
-                    </div>
-
-                    <div class="form-group row">
-                        <div class="col offset-5 offset-md-6 font-weight-bold">
-                            OR
-                        </div>
-                    </div>
-                
-                    <div class="form-group row">
-                        <label class="col-12 col-md-2 col-form-label text-center" for="{{ form.media_url.auto_id }}">
-                            {{ form.media_url.label }}
-                        </label>
-                        
-                        <div class="col">
-                            {{form.media_url}}
-                        </div>
-
-                        {% if form.media_url.errors %}
-                        <div class="md-offset-2 col-8 text-danger small">
-                            {{form.media_url.errors}}
-                        </div>
-                        {% endif %}
-                    </div>
-                    <div class="row">
-                        <p class="col offset-md-2 text-muted">
-                            <small>Required: Use one of the methods to upload a file. Use the entire URL (including 'http://' or 'https://'), if chosen.</small>
-                        </p>
-                    </div>
-                </div>
-
-                <div id="image_preview_block" class="row text-center mt-3 mb-3" style="display: none;">
-                    <div class="col border">
-                        <h3>Preview</h3>
-                        <figure>
-                            <img src="#" title="Preview of image" id="image_preview" height="400"/>
-                        </figure>
-                    </div>
-                </div>
-
-                {% for field in form %}
-                {% if field.auto_id != "id_sample" and field.auto_id != "id_preview" and field.auto_id != "id_media" and field.auto_id != "id_media_url" %}
-                <div class="form-group row">
-                    <label for="{{ field.auto_id }}" class="col-12 col-md-2 col-form-label text-center">{{ field.label }}</label>
-                    
-                    <div class="col">
-                        {{field}}
-                    </div>
-                </div>
-                {% if field.errors %}
-                <div class="row text-danger small">
-                    <div class="col">{{field.errors}}</div>
-                </div>
-                {% endif %}
-                {% if field.help_text %}
-                <div class="row">
-                    <p class="col offset-md-2 text-muted">{{field.help_text}}</p>
-                </div>
-                {% endif %}
-                {% endif %}
-                {% endfor %}
-                <button type="submit" class="btn btn-primary btn-lg float-right">Post</button>
-            </form>
-        </div>
-    </div>
-</div>
+{% extends 'booru/base.html' %}
+
+{% block css %}
+    {% load static %}
+{% endblock %}
+
+{% block scripts %}
+<script>
+    $(function () {
+        $("#id_media_url").blur(function() {
+            var image_url = $("#id_media_url").val();
+            if (checkURL(image_url)) {
+                $("#image_preview_block").show();
+                $("#image_preview").attr("src", image_url);
+            }
+            else {
+                $("#image_preview_block").hide();
+            }
+        });
+
+        $('.custom-file-input').change(function(e){
+            var file = e.target.files[0];
+            var fileName = file.name;
+
+            if (file){
+                var reader = new FileReader();
+                reader.onload = function (e) {
+                    $("#image_preview").attr("src", e.target.result);
+                };
+                reader.readAsDataURL(file);
+                $("#image_preview_block").show();
+            }
+            else{
+                $("#image_preview_block").hide();
+            }
+        });
+    });
+
+    function checkURL(url) {
+        return(url.match(/\.(jpeg|jpg|gif|png)$/) != null);
+    }
+</script>
+{% endblock %}
+
+{% block body %}
+<div class="container">
+    <div class="row">
+        <div id="upload" class="col">
+            <h1>Upload</h1>
+            
+            <form method="post" enctype="multipart/form-data">
+                {% csrf_token %}
+
+                {% if form.errors %}
+                    {% for field in form %}
+                        {% for error in field.errors %}
+                            <div class="alert alert-danger">
+                                <strong>{{ error|escape }}</strong>
+                            </div>
+                        {% endfor %}
+                    {% endfor %}
+                    {% for error in form.non_field_errors %}
+                        <div class="alert alert-danger">
+                            <strong>{{ error|escape }}</strong>
+                        </div>
+                    {% endfor %}
+                {% endif %}
+
+                <div class="border border-secondary mb-4 p-2">
+                    <div class="form-group row mt-2">
+                        <label class="col-12 col-md-2 col-form-label text-center">{{ form.media.label }}</label>
+                        
+                        <div class="col">
+                            {{form.media}}
+                            <span class="custom-file-control"></span>
+                            <label class="custom-file-label ml-3 mr-3" for="{{ form.media.auto_id }}">
+                                Choose file
+                            </label>
+                        </div>
+
+                        {% if form.media.errors %}
+                        <div class="md-offset-2 col text-danger small">
+                            {{form.media.errors}}
+                        </div>
+                        {% endif %}
+                    </div>
+
+                    <div class="form-group row">
+                        <div class="col offset-5 offset-md-6 font-weight-bold">
+                            OR
+                        </div>
+                    </div>
+                
+                    <div class="form-group row">
+                        <label class="col-12 col-md-2 col-form-label text-center" for="{{ form.media_url.auto_id }}">
+                            {{ form.media_url.label }}
+                        </label>
+                        
+                        <div class="col">
+                            {{form.media_url}}
+                        </div>
+
+                        {% if form.media_url.errors %}
+                        <div class="md-offset-2 col-8 text-danger small">
+                            {{form.media_url.errors}}
+                        </div>
+                        {% endif %}
+                    </div>
+                    <div class="row">
+                        <p class="col offset-md-2 text-muted">
+                            <small>Required: Use one of the methods to upload a file. Use the entire URL (including 'http://' or 'https://'), if chosen.</small>
+                        </p>
+                    </div>
+                </div>
+
+                <div id="image_preview_block" class="row text-center mt-3 mb-3" style="display: none;">
+                    <div class="col border">
+                        <h3>Preview</h3>
+                        <figure>
+                            <img src="#" title="Preview of image" id="image_preview" height="400"/>
+                        </figure>
+                    </div>
+                </div>
+
+                {% for field in form %}
+                {% if field.auto_id != "id_sample" and field.auto_id != "id_preview" and field.auto_id != "id_media" and field.auto_id != "id_media_url" %}
+                <div class="form-group row">
+                    <label for="{{ field.auto_id }}" class="col-12 col-md-2 col-form-label text-center">{{ field.label }}</label>
+                    
+                    <div class="col">
+                        {{field}}
+                    </div>
+                </div>
+                {% if field.errors %}
+                <div class="row text-danger small">
+                    <div class="col">{{field.errors}}</div>
+                </div>
+                {% endif %}
+                {% if field.help_text %}
+                <div class="row">
+                    <p class="col offset-md-2 text-muted">{{field.help_text}}</p>
+                </div>
+                {% endif %}
+                {% endif %}
+                {% endfor %}
+                <button type="submit" class="btn btn-primary btn-lg float-right">Post</button>
+            </form>
+        </div>
+    </div>
+</div>
 {% endblock %}
```

### Comparing `Boorunaut-0.4.3/booru/tests/tests_booru_clients.py` & `Boorunaut-0.5.0/booru/tests/tests_booru_clients.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# -*- coding: utf-8 -*-
-import tempfile
-from collections import Counter
-from urllib.parse import urlparse
-
-import django
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AnonymousUser, User
-from django.core.files.images import ImageFile
-from django.core.files.uploadedfile import InMemoryUploadedFile
-from django.test import Client, RequestFactory, TestCase
-from django.urls import reverse
-from PIL import Image
-from booru.utils import generate_mock_image
-
-from booru.models import Post
-
-
-class PostClientsTests(TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        cls.factory = RequestFactory()
-        super().setUpClass()
-
-    @classmethod
-    def tearDownClass(cls):
-        super().tearDownClass()
-
-    def create_test_user(self):
-        user = get_user_model().objects.create_user('Test', password="123")
-        user.save()
-        return user
-
-    def create_test_post(self, user, id_number=None):
-        image_file = generate_mock_image(empty=False)
-        image_mock = ImageFile(image_file)
-        tags = ['test1', 'test2']
-        source = "http://example.org"
-        
-        if id_number:
-            test_post = Post.objects.create(id=id_number, uploader=user, media=image_mock,
-                                        source=source, tags=tags)
-        else:
-            test_post = Post.objects.create(uploader=user, media=image_mock,
-                                        source=source, tags=tags)
-        return test_post
-
-    def test_request_index_by_anonymous_client(self):
-        c = Client()
-        response = c.get('/')
-        self.assertEqual(200, response.status_code)
-
-    def test_request_post_list_by_anonymous_client(self):
-        c = Client()
-        post_list = reverse('booru:posts')
-        response = c.get(post_list)
-        self.assertEqual(200, response.status_code)
-
-    def test_request_post_detail_by_anonymous_client(self):
-        user = self.create_test_user()
-        post = self.create_test_post(user, 1)
-
-        c = Client()
-        post = reverse('booru:post_detail', args=(post.id,))
-        response = c.get(post)
-        self.assertEqual(200, response.status_code)
-        del post
-
-    def test_post_was_created_by_logged_client(self):
-        user = self.create_test_user()
-        user.is_staff = True
-        user.save()
-
-        c = Client()
-        c.login(username=user.username, password="123")
-
-        image_file = generate_mock_image()
-
-        data = {"image": image_file,
-                "tags": "test3 test4",
-                "source": "http://example.org/testing"}
-
-        upload_url = reverse('booru:upload')
-        response = c.post(upload_url, data)
-        del image_file
-
-        post_url = reverse('booru:post_detail', args=(1,))
-        self.assertEqual(200, response.status_code)
+# -*- coding: utf-8 -*-
+import tempfile
+from collections import Counter
+from urllib.parse import urlparse
+
+import django
+from django.contrib.auth import get_user_model
+from django.contrib.auth.models import AnonymousUser, User
+from django.core.files.images import ImageFile
+from django.core.files.uploadedfile import InMemoryUploadedFile
+from django.test import Client, RequestFactory, TestCase
+from django.urls import reverse
+from PIL import Image
+from booru.utils import generate_mock_image
+
+from booru.models import Post
+
+
+class PostClientsTests(TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        cls.factory = RequestFactory()
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def create_test_user(self):
+        user = get_user_model().objects.create_user('Test', password="123")
+        user.save()
+        return user
+
+    def create_test_post(self, user, id_number=None):
+        image_file = generate_mock_image(empty=False)
+        image_mock = ImageFile(image_file)
+        tags = ['test1', 'test2']
+        source = "http://example.org"
+        
+        if id_number:
+            test_post = Post.objects.create(id=id_number, uploader=user, media=image_mock,
+                                        source=source, tags=tags)
+        else:
+            test_post = Post.objects.create(uploader=user, media=image_mock,
+                                        source=source, tags=tags)
+        return test_post
+
+    def test_request_index_by_anonymous_client(self):
+        c = Client()
+        response = c.get('/')
+        self.assertEqual(200, response.status_code)
+
+    def test_request_post_list_by_anonymous_client(self):
+        c = Client()
+        post_list = reverse('booru:posts')
+        response = c.get(post_list)
+        self.assertEqual(200, response.status_code)
+
+    def test_request_post_detail_by_anonymous_client(self):
+        user = self.create_test_user()
+        post = self.create_test_post(user, 1)
+
+        c = Client()
+        post = reverse('booru:post_detail', args=(post.id,))
+        response = c.get(post)
+        self.assertEqual(200, response.status_code)
+        del post
+
+    def test_post_was_created_by_logged_client(self):
+        user = self.create_test_user()
+        user.is_staff = True
+        user.save()
+
+        c = Client()
+        c.login(username=user.username, password="123")
+
+        image_file = generate_mock_image()
+
+        data = {"image": image_file,
+                "tags": "test3 test4",
+                "source": "http://example.org/testing"}
+
+        upload_url = reverse('booru:upload')
+        response = c.post(upload_url, data)
+        del image_file
+
+        post_url = reverse('booru:post_detail', args=(1,))
+        self.assertEqual(200, response.status_code)
```

### Comparing `Boorunaut-0.4.3/booru/tests/tests_booru_forms.py` & `Boorunaut-0.5.0/booru/tests/tests_booru_forms.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# -*- coding: utf-8 -*-
-import base64
-import tempfile
-from collections import Counter
-from io import BytesIO
-from urllib.parse import urlparse
-
-import django
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AnonymousUser, User
-from django.core.files.images import ImageFile
-from django.core.files.uploadedfile import InMemoryUploadedFile
-from django.test import Client, RequestFactory, TestCase
-from PIL import Image
-
-from booru.forms import (CreatePostForm, EditPostForm, ImplicationCreateForm,
-                         TagListSearchForm)
-from booru.models import Category
-from booru.utils import generate_mock_image
-
-
-class CreateBooruFormTests(TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-        cls.factory = RequestFactory()
-        super().setUpClass()
-
-    @classmethod
-    def tearDownClass(cls):
-        super().tearDownClass()
-
-    def create_test_image_file(self):
-        im = Image.new(mode='RGB', size=(200, 200))
-        im_io = BytesIO()
-        im.save(im_io, format='JPEG')
-        im_io.seek(0)
-
-        image = InMemoryUploadedFile(
-            im_io, None, 'random-name.jpg', 'image/jpeg', im_io.getbuffer().nbytes, None
-        )
-
-        return image
-
-    def test_create_post_form(self):
-        image_mock = self.create_test_image_file()
-
-        form_data = {'tags': 'test1 test2', 'source': 'http://a.com'}
-        file_data = {'image': image_mock}
-        form = CreatePostForm(form_data, file_data)
-        
-        self.assertTrue(form.is_valid())
-        self.assertEqual('http://a.com', form.cleaned_data['source'])
-        self.assertEqual(['test1', 'test2'], form.cleaned_data['tags'])
-        self.assertEqual(image_mock, form.cleaned_data['image'])
-
-    def test_create_post_form(self):
-        form_data = {'rating': 2, 'parent': 1, 'source': 'http://a.com', 'tags': 'test3 test4'}
-        form = EditPostForm(form_data)
-        
-        self.assertTrue(form.is_valid())
-        self.assertEqual('http://a.com', form.cleaned_data['source'])
-        self.assertEqual(['test3', 'test4'], form.cleaned_data['tags'])
-        self.assertEqual(2, form.cleaned_data['rating'])
-        self.assertEqual(1, form.cleaned_data['parent'])
-    
-    def test_tag_list_search_form(self):
-        category = Category.objects.create(label="general", title_singular="General", title_plural="General")
-
-        form_data = {'category': category.pk, 'tags': 'test5 test6'}
-        form = TagListSearchForm(form_data)
-        
-        self.assertTrue(form.is_valid())
-        self.assertEqual('test5 test6', form.cleaned_data['tags'])
-        self.assertEqual(category, form.cleaned_data['category'])
-
-    def test_implication_create_form(self):
-        form_data = {'from_tag': 'test3', 'to_tag': 'test4'}
-        form = ImplicationCreateForm(form_data)
-        
-        self.assertTrue(form.is_valid())
-        self.assertEqual('test3', form.cleaned_data['from_tag'])
-        self.assertEqual('test4', form.cleaned_data['to_tag'])
-
-    def test_implication_create_form_turns_lowercase(self):
-        form_data = {'from_tag': 'Test3', 'to_tag': 'TesT4_WiTh_UppeRcAse'}
-        form = ImplicationCreateForm(form_data)
-        
-        self.assertTrue(form.is_valid())
-        self.assertEqual('test3', form.cleaned_data['from_tag'])
-        self.assertEqual('test4_with_uppercase', form.cleaned_data['to_tag'])
+# -*- coding: utf-8 -*-
+import base64
+import tempfile
+from collections import Counter
+from io import BytesIO
+from urllib.parse import urlparse
+
+import django
+from django.contrib.auth import get_user_model
+from django.contrib.auth.models import AnonymousUser, User
+from django.core.files.images import ImageFile
+from django.core.files.uploadedfile import InMemoryUploadedFile
+from django.test import Client, RequestFactory, TestCase
+from PIL import Image
+
+from booru.forms import (CreatePostForm, EditPostForm, ImplicationCreateForm,
+                         TagListSearchForm)
+from booru.models import Category
+from booru.utils import generate_mock_image
+
+
+class CreateBooruFormTests(TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        cls.factory = RequestFactory()
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def create_test_image_file(self):
+        im = Image.new(mode='RGB', size=(200, 200))
+        im_io = BytesIO()
+        im.save(im_io, format='JPEG')
+        im_io.seek(0)
+
+        image = InMemoryUploadedFile(
+            im_io, None, 'random-name.jpg', 'image/jpeg', im_io.getbuffer().nbytes, None
+        )
+
+        return image
+
+    def test_create_post_form(self):
+        image_mock = self.create_test_image_file()
+
+        form_data = {'tags': 'test1 test2', 'source': 'http://a.com'}
+        file_data = {'image': image_mock}
+        form = CreatePostForm(form_data, file_data)
+        
+        self.assertTrue(form.is_valid())
+        self.assertEqual('http://a.com', form.cleaned_data['source'])
+        self.assertEqual(['test1', 'test2'], form.cleaned_data['tags'])
+        self.assertEqual(image_mock, form.cleaned_data['image'])
+
+    def test_create_post_form(self):
+        form_data = {'rating': 2, 'parent': 1, 'source': 'http://a.com', 'tags': 'test3 test4'}
+        form = EditPostForm(form_data)
+        
+        self.assertTrue(form.is_valid())
+        self.assertEqual('http://a.com', form.cleaned_data['source'])
+        self.assertEqual(['test3', 'test4'], form.cleaned_data['tags'])
+        self.assertEqual(2, form.cleaned_data['rating'])
+        self.assertEqual(1, form.cleaned_data['parent'])
+    
+    def test_tag_list_search_form(self):
+        category = Category.objects.create(label="general", title_singular="General", title_plural="General")
+
+        form_data = {'category': category.pk, 'tags': 'test5 test6'}
+        form = TagListSearchForm(form_data)
+        
+        self.assertTrue(form.is_valid())
+        self.assertEqual('test5 test6', form.cleaned_data['tags'])
+        self.assertEqual(category, form.cleaned_data['category'])
+
+    def test_implication_create_form(self):
+        form_data = {'from_tag': 'test3', 'to_tag': 'test4'}
+        form = ImplicationCreateForm(form_data)
+        
+        self.assertTrue(form.is_valid())
+        self.assertEqual('test3', form.cleaned_data['from_tag'])
+        self.assertEqual('test4', form.cleaned_data['to_tag'])
+
+    def test_implication_create_form_turns_lowercase(self):
+        form_data = {'from_tag': 'Test3', 'to_tag': 'TesT4_WiTh_UppeRcAse'}
+        form = ImplicationCreateForm(form_data)
+        
+        self.assertTrue(form.is_valid())
+        self.assertEqual('test3', form.cleaned_data['from_tag'])
+        self.assertEqual('test4_with_uppercase', form.cleaned_data['to_tag'])
```

### Comparing `Boorunaut-0.4.3/booru/tests/tests_booru_tags_operators.py` & `Boorunaut-0.5.0/booru/tests/tests_booru_tags_operators.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-# -*- coding: utf-8 -*-
-import base64
-import tempfile
-
-import django
-from django.contrib.auth import get_user_model
-from django.core.files.images import ImageFile
-from django.core.files.uploadedfile import SimpleUploadedFile
-from django.db.models import Q
-from django.test import TestCase
-
-from booru.models import Post, ScoreVote
-from booru.utils import parse_and_filter_tags
-from booru.views import tags_list
-from booru.utils import generate_mock_image
-
-
-def create_test_user(username='Test'):
-    user = get_user_model().objects.create_user(username, password="123")
-    user.save()
-    return user
-
-def create_test_post(user, tags=[], id_number=None):
-    image_file = generate_mock_image(empty=False)
-    image_mock = ImageFile(image_file)
-    source = "http://example.org"
-
-    test_post = None
-    if id_number:
-        test_post = Post.objects.create(id=id_number, uploader=user, media=image_mock, source=source)
-    else:
-        test_post = Post.objects.create(uploader=user, media=image_mock, source=source)
-
-    for tag in tags:
-        test_post.tags.add(tag)
-
-    return test_post
-
-class UtilitiesTests(TestCase):
-    post_one = None
-    post_two = None
-    post_three = None
-
-    @classmethod
-    def setUpClass(cls):
-        mock_user = create_test_user()
-        mock_user_two = create_test_user("Test2")
-
-        cls.post_one = create_test_post(mock_user, ['test1', 'test2', 'test3'], 1)
-        cls.post_two = create_test_post(mock_user, ['test1', 'test2', 'test4', 'test5'], 2)
-        cls.post_three = create_test_post(mock_user, ['test1', 'test4', 'test6'], 3)
-
-        super().setUpClass()
-
-    @classmethod
-    def tearDownClass(cls):
-        super().tearDownClass()
-
-    def test_tag_search_one_result(self):
-        posts = parse_and_filter_tags('test3')
-
-        self.assertEqual(list(posts), [self.post_one])
-
-    def test_tag_search_three_results(self):
-        posts = parse_and_filter_tags('test1')
-
-        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
-
-    def test_tag_search_and_operation_result_none(self):
-        posts = parse_and_filter_tags('test3 test5')
-
-        self.assertEqual(list(posts), [])
-
-    def test_tag_search_and_operation_result_one(self):
-        posts = parse_and_filter_tags('test4 test6')
-
-        self.assertEqual(list(posts), [self.post_three])
-
-    def test_tag_search_and_or_operations_between_two_tags(self):
-        posts = parse_and_filter_tags('test3 ~test5')
-
-        self.assertEqual(list(posts), [])
-
-    def test_tag_search_two_or_operation_between_two_tags(self):
-        posts = parse_and_filter_tags('~test3 ~test6')
-
-        self.assertEqual(list(posts), [self.post_three, self.post_one])
-
-    def test_tag_search_not_operation_between_two_tags(self):
-        posts = parse_and_filter_tags('test1 -test2')
-
-        self.assertEqual(list(posts), [self.post_three])
-
-    def test_tag_search_not_operation_between_three_tags(self):
-        posts = parse_and_filter_tags('test1 -test2 -test6')
-
-        self.assertEqual(list(posts), [])
-
-    def test_tag_search_not_operation_between_three_tags_2(self):
-        posts = parse_and_filter_tags('test1 -test2 -test3')
-
-        self.assertEqual(list(posts), [self.post_three])
-
-    def test_tag_search_no_tags(self):
-        posts = parse_and_filter_tags('')
-
-        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
-
-    def test_tag_search_status_pending(self):
-        posts = parse_and_filter_tags('status:pending')
-        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
-
-    def test_tag_search_status_approved(self):
-        posts = parse_and_filter_tags('status:approved')
-        self.post_two.status = Post.APPROVED
-        self.post_two.save()
-        self.assertEqual(list(posts), [self.post_two])
-
-    def test_tag_search_status_deleted(self):
-        self.post_two.status = Post.DELETED
-        self.post_two.save()
-        posts = parse_and_filter_tags('status:deleted')
-        self.assertEqual(list(posts), [self.post_two])
-    
-    def test_tag_search_status_score_zero(self):
-        posts = parse_and_filter_tags('score:0')
-        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
-
-    def test_tag_search_status_score_one(self):
-        posts = parse_and_filter_tags('score:1')
-        user = get_user_model().objects.get(username="Test")
-        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
-        self.assertEqual(list(posts), [self.post_three])
-    
-    def test_tag_search_status_score_greater_than_zero(self):
-        posts = parse_and_filter_tags('score:>0')
-        user = get_user_model().objects.get(username="Test")
-        ScoreVote.objects.create(account=user, post=self.post_one, point=1)
-        ScoreVote.objects.create(account=user, post=self.post_three, point=0)
-        self.assertEqual(list(posts), [self.post_one])
-
-    def test_tag_search_status_score_greater_than_one(self):
-        posts = parse_and_filter_tags('score:>1')
-        user = get_user_model().objects.get(username="Test")
-        user_two = get_user_model().objects.get(username="Test2")
-        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
-        ScoreVote.objects.create(account=user_two, post=self.post_three, point=1)
-        self.assertEqual(list(posts), [self.post_three])
-    
-    def test_tag_search_status_score_less_than_zero(self):
-        posts = parse_and_filter_tags('score:<0')
-        user = get_user_model().objects.get(username="Test")
-        user_two = get_user_model().objects.get(username="Test2")
-        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
-        ScoreVote.objects.create(account=user_two, post=self.post_two, point=-1)
-        self.assertEqual(list(posts), [self.post_two])
-    
-    def test_tag_search_status_score_less_than_one(self):
-        posts = parse_and_filter_tags('score:<1')
-        user = get_user_model().objects.get(username="Test")
-        user_two = get_user_model().objects.get(username="Test2")
-        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
-        ScoreVote.objects.create(account=user_two, post=self.post_two, point=1)
-        self.assertEqual(list(posts), [self.post_two])
-    
-    def test_tag_search_rating_safe(self):
-        posts = parse_and_filter_tags('rating:safe')
-        posts_abbreviation = parse_and_filter_tags('rating:s')
-        self.post_one.rating = Post.SAFE
-        self.post_one.save()
-        self.assertEqual(list(posts), list(posts_abbreviation))
-        self.assertEqual(list(posts), [self.post_one])
-    
-    def test_tag_search_rating_questionable(self):
-        posts = parse_and_filter_tags('rating:questionable')
-        posts_abbreviation = parse_and_filter_tags('rating:q')
-        self.post_two.rating = Post.QUESTIONABLE
-        self.post_two.save()
-        self.assertEqual(list(posts), list(posts_abbreviation))
-        self.assertEqual(list(posts), [self.post_two])
-    
-    def test_tag_search_rating_explicit(self):
-        posts = parse_and_filter_tags('rating:explicit')
-        posts_abbreviation = parse_and_filter_tags('rating:e')
-        self.post_three.rating = Post.EXPLICIT
-        self.post_three.save()
-        self.assertEqual(list(posts), [self.post_three])
-    
-    def test_tag_search_rating_none(self):
-        posts = parse_and_filter_tags('rating:none')
-        posts_abbreviation = parse_and_filter_tags('rating:n')
-        self.post_three.rating = Post.SAFE
-        self.post_three.save()
-        self.assertEqual(list(posts), list(posts_abbreviation))
-        self.assertEqual(list(posts), [self.post_two, self.post_one])
-    
-    def test_tag_search_order_by_score(self):
-        posts = parse_and_filter_tags('order:score')
-        user = get_user_model().objects.get(username="Test")
-        user_two = get_user_model().objects.get(username="Test2")
-        ScoreVote.objects.create(account=user, post=self.post_one, point=-1)
-        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
-        ScoreVote.objects.create(account=user_two, post=self.post_two, point=1)
-        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
-        ScoreVote.objects.create(account=user_two, post=self.post_three, point=1)
-        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
-
-    def test_tag_search_order_by_score_asc(self):
-        posts = parse_and_filter_tags('order:score_asc')
-        user = get_user_model().objects.get(username="Test")
-        user_two = get_user_model().objects.get(username="Test2")
-        ScoreVote.objects.create(account=user, post=self.post_one, point=-1)
-        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
-        ScoreVote.objects.create(account=user_two, post=self.post_two, point=1)
-        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
-        ScoreVote.objects.create(account=user_two, post=self.post_three, point=1)
-        self.assertEqual(list(posts), [self.post_one, self.post_two, self.post_three])
+# -*- coding: utf-8 -*-
+import base64
+import tempfile
+
+import django
+from django.contrib.auth import get_user_model
+from django.core.files.images import ImageFile
+from django.core.files.uploadedfile import SimpleUploadedFile
+from django.db.models import Q
+from django.test import TestCase
+
+from booru.models import Post, ScoreVote
+from booru.utils import parse_and_filter_tags
+from booru.views import tags_list
+from booru.utils import generate_mock_image
+
+
+def create_test_user(username='Test'):
+    user = get_user_model().objects.create_user(username, password="123")
+    user.save()
+    return user
+
+def create_test_post(user, tags=[], id_number=None):
+    image_file = generate_mock_image(empty=False)
+    image_mock = ImageFile(image_file)
+    source = "http://example.org"
+
+    test_post = None
+    if id_number:
+        test_post = Post.objects.create(id=id_number, uploader=user, media=image_mock, source=source)
+    else:
+        test_post = Post.objects.create(uploader=user, media=image_mock, source=source)
+
+    for tag in tags:
+        test_post.tags.add(tag)
+
+    return test_post
+
+class UtilitiesTests(TestCase):
+    post_one = None
+    post_two = None
+    post_three = None
+
+    @classmethod
+    def setUpClass(cls):
+        mock_user = create_test_user()
+        mock_user_two = create_test_user("Test2")
+
+        cls.post_one = create_test_post(mock_user, ['test1', 'test2', 'test3'], 1)
+        cls.post_two = create_test_post(mock_user, ['test1', 'test2', 'test4', 'test5'], 2)
+        cls.post_three = create_test_post(mock_user, ['test1', 'test4', 'test6'], 3)
+
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def test_tag_search_one_result(self):
+        posts = parse_and_filter_tags('test3')
+
+        self.assertEqual(list(posts), [self.post_one])
+
+    def test_tag_search_three_results(self):
+        posts = parse_and_filter_tags('test1')
+
+        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
+
+    def test_tag_search_and_operation_result_none(self):
+        posts = parse_and_filter_tags('test3 test5')
+
+        self.assertEqual(list(posts), [])
+
+    def test_tag_search_and_operation_result_one(self):
+        posts = parse_and_filter_tags('test4 test6')
+
+        self.assertEqual(list(posts), [self.post_three])
+
+    def test_tag_search_and_or_operations_between_two_tags(self):
+        posts = parse_and_filter_tags('test3 ~test5')
+
+        self.assertEqual(list(posts), [])
+
+    def test_tag_search_two_or_operation_between_two_tags(self):
+        posts = parse_and_filter_tags('~test3 ~test6')
+
+        self.assertEqual(list(posts), [self.post_three, self.post_one])
+
+    def test_tag_search_not_operation_between_two_tags(self):
+        posts = parse_and_filter_tags('test1 -test2')
+
+        self.assertEqual(list(posts), [self.post_three])
+
+    def test_tag_search_not_operation_between_three_tags(self):
+        posts = parse_and_filter_tags('test1 -test2 -test6')
+
+        self.assertEqual(list(posts), [])
+
+    def test_tag_search_not_operation_between_three_tags_2(self):
+        posts = parse_and_filter_tags('test1 -test2 -test3')
+
+        self.assertEqual(list(posts), [self.post_three])
+
+    def test_tag_search_no_tags(self):
+        posts = parse_and_filter_tags('')
+
+        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
+
+    def test_tag_search_status_pending(self):
+        posts = parse_and_filter_tags('status:pending')
+        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
+
+    def test_tag_search_status_approved(self):
+        posts = parse_and_filter_tags('status:approved')
+        self.post_two.status = Post.APPROVED
+        self.post_two.save()
+        self.assertEqual(list(posts), [self.post_two])
+
+    def test_tag_search_status_deleted(self):
+        self.post_two.status = Post.DELETED
+        self.post_two.save()
+        posts = parse_and_filter_tags('status:deleted')
+        self.assertEqual(list(posts), [self.post_two])
+    
+    def test_tag_search_status_score_zero(self):
+        posts = parse_and_filter_tags('score:0')
+        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
+
+    def test_tag_search_status_score_one(self):
+        posts = parse_and_filter_tags('score:1')
+        user = get_user_model().objects.get(username="Test")
+        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
+        self.assertEqual(list(posts), [self.post_three])
+    
+    def test_tag_search_status_score_greater_than_zero(self):
+        posts = parse_and_filter_tags('score:>0')
+        user = get_user_model().objects.get(username="Test")
+        ScoreVote.objects.create(account=user, post=self.post_one, point=1)
+        ScoreVote.objects.create(account=user, post=self.post_three, point=0)
+        self.assertEqual(list(posts), [self.post_one])
+
+    def test_tag_search_status_score_greater_than_one(self):
+        posts = parse_and_filter_tags('score:>1')
+        user = get_user_model().objects.get(username="Test")
+        user_two = get_user_model().objects.get(username="Test2")
+        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
+        ScoreVote.objects.create(account=user_two, post=self.post_three, point=1)
+        self.assertEqual(list(posts), [self.post_three])
+    
+    def test_tag_search_status_score_less_than_zero(self):
+        posts = parse_and_filter_tags('score:<0')
+        user = get_user_model().objects.get(username="Test")
+        user_two = get_user_model().objects.get(username="Test2")
+        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
+        ScoreVote.objects.create(account=user_two, post=self.post_two, point=-1)
+        self.assertEqual(list(posts), [self.post_two])
+    
+    def test_tag_search_status_score_less_than_one(self):
+        posts = parse_and_filter_tags('score:<1')
+        user = get_user_model().objects.get(username="Test")
+        user_two = get_user_model().objects.get(username="Test2")
+        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
+        ScoreVote.objects.create(account=user_two, post=self.post_two, point=1)
+        self.assertEqual(list(posts), [self.post_two])
+    
+    def test_tag_search_rating_safe(self):
+        posts = parse_and_filter_tags('rating:safe')
+        posts_abbreviation = parse_and_filter_tags('rating:s')
+        self.post_one.rating = Post.SAFE
+        self.post_one.save()
+        self.assertEqual(list(posts), list(posts_abbreviation))
+        self.assertEqual(list(posts), [self.post_one])
+    
+    def test_tag_search_rating_questionable(self):
+        posts = parse_and_filter_tags('rating:questionable')
+        posts_abbreviation = parse_and_filter_tags('rating:q')
+        self.post_two.rating = Post.QUESTIONABLE
+        self.post_two.save()
+        self.assertEqual(list(posts), list(posts_abbreviation))
+        self.assertEqual(list(posts), [self.post_two])
+    
+    def test_tag_search_rating_explicit(self):
+        posts = parse_and_filter_tags('rating:explicit')
+        posts_abbreviation = parse_and_filter_tags('rating:e')
+        self.post_three.rating = Post.EXPLICIT
+        self.post_three.save()
+        self.assertEqual(list(posts), [self.post_three])
+    
+    def test_tag_search_rating_none(self):
+        posts = parse_and_filter_tags('rating:none')
+        posts_abbreviation = parse_and_filter_tags('rating:n')
+        self.post_three.rating = Post.SAFE
+        self.post_three.save()
+        self.assertEqual(list(posts), list(posts_abbreviation))
+        self.assertEqual(list(posts), [self.post_two, self.post_one])
+    
+    def test_tag_search_order_by_score(self):
+        posts = parse_and_filter_tags('order:score')
+        user = get_user_model().objects.get(username="Test")
+        user_two = get_user_model().objects.get(username="Test2")
+        ScoreVote.objects.create(account=user, post=self.post_one, point=-1)
+        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
+        ScoreVote.objects.create(account=user_two, post=self.post_two, point=1)
+        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
+        ScoreVote.objects.create(account=user_two, post=self.post_three, point=1)
+        self.assertEqual(list(posts), [self.post_three, self.post_two, self.post_one])
+
+    def test_tag_search_order_by_score_asc(self):
+        posts = parse_and_filter_tags('order:score_asc')
+        user = get_user_model().objects.get(username="Test")
+        user_two = get_user_model().objects.get(username="Test2")
+        ScoreVote.objects.create(account=user, post=self.post_one, point=-1)
+        ScoreVote.objects.create(account=user, post=self.post_two, point=-1)
+        ScoreVote.objects.create(account=user_two, post=self.post_two, point=1)
+        ScoreVote.objects.create(account=user, post=self.post_three, point=1)
+        ScoreVote.objects.create(account=user_two, post=self.post_three, point=1)
+        self.assertEqual(list(posts), [self.post_one, self.post_two, self.post_three])
```

### Comparing `Boorunaut-0.4.3/booru/tests/tests_booru_utilities.py` & `Boorunaut-0.5.0/booru/tests/tests_booru_utilities.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# -*- coding: utf-8 -*-
-import re
-import tempfile
-from collections import Counter
-from urllib.parse import urlparse
-
-import django
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AnonymousUser, User
-from django.test import Client, RequestFactory, TestCase
-from django.test.utils import override_settings
-from booru.utils import space_splitter
-from booru.utils import space_joiner
-from booru.utils import compare_strings
-
-class UtilitiesTests(TestCase):
-    fixtures = []
-
-    @classmethod
-    def setUpClass(cls):
-        super().setUpClass()
-
-    @classmethod
-    def tearDownClass(cls):
-        super().tearDownClass()
-
-    def test_space_splitter_generates_tags_from_string(self):
-        tag_string = "test1 test2 test:test_3 test_4"
-        generated_tags = space_splitter(tag_string)
-        expected_generated_tags = ["test1", "test2", "test:test_3", "test_4"]
-        self.assertEqual(generated_tags, expected_generated_tags)
-
-    def test_history_diff(self):
-        old_string = "test1 test2 test3"
-        new_string = "test2 test3 test4"
-        expected = {"added": ["test4"], "removed": ["test1"], "equal": ["test2", "test3"]}
-
-        result = compare_strings(old_string, new_string)
-        self.assertEqual(sorted(result["added"]), sorted(expected["added"]))
-        self.assertEqual(sorted(result["removed"]), sorted(expected["removed"]))
-        self.assertEqual(sorted(result["equal"]), sorted(expected["equal"]))
+# -*- coding: utf-8 -*-
+import re
+import tempfile
+from collections import Counter
+from urllib.parse import urlparse
+
+import django
+from django.contrib.auth import get_user_model
+from django.contrib.auth.models import AnonymousUser, User
+from django.test import Client, RequestFactory, TestCase
+from django.test.utils import override_settings
+from booru.utils import space_splitter
+from booru.utils import space_joiner
+from booru.utils import compare_strings
+
+class UtilitiesTests(TestCase):
+    fixtures = []
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def test_space_splitter_generates_tags_from_string(self):
+        tag_string = "test1 test2 test:test_3 test_4"
+        generated_tags = space_splitter(tag_string)
+        expected_generated_tags = ["test1", "test2", "test:test_3", "test_4"]
+        self.assertEqual(generated_tags, expected_generated_tags)
+
+    def test_history_diff(self):
+        old_string = "test1 test2 test3"
+        new_string = "test2 test3 test4"
+        expected = {"added": ["test4"], "removed": ["test1"], "equal": ["test2", "test3"]}
+
+        result = compare_strings(old_string, new_string)
+        self.assertEqual(sorted(result["added"]), sorted(expected["added"]))
+        self.assertEqual(sorted(result["removed"]), sorted(expected["removed"]))
+        self.assertEqual(sorted(result["equal"]), sorted(expected["equal"]))
```

### Comparing `Boorunaut-0.4.3/booru/urls.py` & `Boorunaut-0.5.0/booru/urls.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from django.urls import include, path, re_path
-
-import booru.account.views
-import booru.core.views
-
-from . import views
-
-app_name = "booru"
-
-urlpatterns = [
-    re_path(r'^$', views.index, name='index'),
-    re_path(r'^upload/$', views.upload, name='upload'),
-
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/$', views.post_detail, name='post_detail'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/history$', views.post_history, name='post_history'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/history/(?P<page_number>[0-9]+)/$', views.post_history, name='post_history'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/approve$', views.post_approve, name='post_approve'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/hide$', views.post_hide, name='post_hide'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/delete$', views.post_delete, name='post_delete'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/favorite$', views.post_favorite, name='post_favorite'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/vote$', views.post_score_vote, name='post_score_vote'),
-    re_path(r'^post/view/(?P<post_id>[0-9]+)/flag$', booru.core.views.PostFlagCreateView.as_view(), name='post_flag'),
-
-    re_path(r'^post/list/$', views.post_list_detail, name='posts'),
-    re_path(r'^post/list/(?P<page_number>[0-9]+)/$', views.post_list_detail, name='post_page_detail'),
-    
-    re_path(r'^tags/$', views.tags_list, name='tags_list'),
-    re_path(r'^tags/(?P<tag_id>[0-9]+)/$', views.tag_detail, name='tag_detail'),
-    re_path(r'^tags/list/(?P<page_number>[0-9]+)/$', views.tags_list, name='tags_page_list'),
-    re_path(r'^tags/(?P<tag_id>[0-9]+)/edit/$', views.tag_edit, name='tag_edit'),
-    path('tags/<int:pk>/delete/', views.TagDelete.as_view(), name='tag-delete'),
-    re_path(r'^tags/(?P<tag_id>[0-9]+)/history/$', views.tag_history, name='tag_history'),
-    re_path(r'^tags/(?P<tag_id>[0-9]+)/history/(?P<page_number>[0-9]+)/$', views.tag_history, name='tag_history'),
-    re_path(r'^tags/(?P<tag_id>[0-9]+)/revision_difference/$', views.tag_revision_diff, name='tag_revision_diff'),
-
-    path('tag_implications', views.ImplicationListView.as_view(), name='implication-list'),
-    path('tag_implications/<int:pk>/', views.ImplicationDetailView.as_view(), name='implication-detail'),
-
-    re_path(r'^tag_implication_request/$', views.implication_create, name='implication_create'),
-
-    re_path(r'^tag_implications/(?P<implication_id>[0-9]+)/approve/$', views.implication_approve, name='implication_approve'),
-    re_path(r'^tag_implications/(?P<implication_id>[0-9]+)/disapprove/$', views.implication_disapprove, name='implication_disapprove'),
-    
-    re_path(r'^tag_search/$', views.tag_search, name='tag_search'),
-
-    re_path(r'^profile/(?P<account_slug>[\w-]+)/$', booru.account.views.profile, name='profile'),
-    re_path(r'^profile/(?P<account_slug>[\w-]+)/delete$', booru.account.views.DeleteAccountView.as_view(), name='profile_delete'),
-
-    re_path(r'^gallery/list/$', views.gallery_list, name='gallery'),
-    re_path(r'^gallery/list/(?P<page_number>[0-9]+)/$', views.gallery_list, name='gallery_list'),
-    re_path(r'^gallery/new/$', views.gallery_create, name='gallery_create'),
-    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/$', views.gallery_detail, name='gallery_detail'),
-    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/edit$', views.gallery_edit, name='gallery_edit'),
-    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/history/$', views.gallery_history, name='gallery_history'),
-    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/history/(?P<page_number>[0-9]+)/$', views.gallery_history, name='gallery_history_page'),
-    
-    re_path(r'^staff_page/$', views.staff_page, name='staff_page'),
-    re_path(r'^staff_page/mass_rename$', views.staff_mass_rename, name='staff_mass_rename'),
-    re_path(r'^staff_page/configuration$', views.SiteConfigurationView.as_view(), name='staff_site_configuration'),
-    re_path(r'^staff_page/block$', views.StaffBanUser.as_view(), name='staff_block'),
-
-    path('comment/<int:pk>/toggle_view', booru.core.views.StaffCommentToggleHiddenView.as_view(), name='comment-toggle-view'),
-]
+from django.urls import include, path, re_path
+
+import booru.account.views
+import booru.core.views
+
+from . import views
+
+app_name = "booru"
+
+urlpatterns = [
+    re_path(r'^$', views.index, name='index'),
+    re_path(r'^upload/$', views.upload, name='upload'),
+
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/$', views.post_detail, name='post_detail'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/history$', views.post_history, name='post_history'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/history/(?P<page_number>[0-9]+)/$', views.post_history, name='post_history'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/approve$', views.post_approve, name='post_approve'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/hide$', views.post_hide, name='post_hide'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/delete$', views.post_delete, name='post_delete'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/favorite$', views.post_favorite, name='post_favorite'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/vote$', views.post_score_vote, name='post_score_vote'),
+    re_path(r'^post/view/(?P<post_id>[0-9]+)/flag$', booru.core.views.PostFlagCreateView.as_view(), name='post_flag'),
+
+    re_path(r'^post/list/$', views.post_list_detail, name='posts'),
+    re_path(r'^post/list/(?P<page_number>[0-9]+)/$', views.post_list_detail, name='post_page_detail'),
+    
+    re_path(r'^tags/$', views.tags_list, name='tags_list'),
+    re_path(r'^tags/(?P<tag_id>[0-9]+)/$', views.tag_detail, name='tag_detail'),
+    re_path(r'^tags/list/(?P<page_number>[0-9]+)/$', views.tags_list, name='tags_page_list'),
+    re_path(r'^tags/(?P<tag_id>[0-9]+)/edit/$', views.tag_edit, name='tag_edit'),
+    path('tags/<int:pk>/delete/', views.TagDelete.as_view(), name='tag-delete'),
+    re_path(r'^tags/(?P<tag_id>[0-9]+)/history/$', views.tag_history, name='tag_history'),
+    re_path(r'^tags/(?P<tag_id>[0-9]+)/history/(?P<page_number>[0-9]+)/$', views.tag_history, name='tag_history'),
+    re_path(r'^tags/(?P<tag_id>[0-9]+)/revision_difference/$', views.tag_revision_diff, name='tag_revision_diff'),
+
+    path('tag_implications', views.ImplicationListView.as_view(), name='implication-list'),
+    path('tag_implications/<int:pk>/', views.ImplicationDetailView.as_view(), name='implication-detail'),
+
+    re_path(r'^tag_implication_request/$', views.implication_create, name='implication_create'),
+
+    re_path(r'^tag_implications/(?P<implication_id>[0-9]+)/approve/$', views.implication_approve, name='implication_approve'),
+    re_path(r'^tag_implications/(?P<implication_id>[0-9]+)/disapprove/$', views.implication_disapprove, name='implication_disapprove'),
+    
+    re_path(r'^tag_search/$', views.tag_search, name='tag_search'),
+
+    re_path(r'^profile/(?P<account_slug>[\w-]+)/$', booru.account.views.profile, name='profile'),
+    re_path(r'^profile/(?P<account_slug>[\w-]+)/delete$', booru.account.views.DeleteAccountView.as_view(), name='profile_delete'),
+
+    re_path(r'^gallery/list/$', views.gallery_list, name='gallery'),
+    re_path(r'^gallery/list/(?P<page_number>[0-9]+)/$', views.gallery_list, name='gallery_list'),
+    re_path(r'^gallery/new/$', views.gallery_create, name='gallery_create'),
+    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/$', views.gallery_detail, name='gallery_detail'),
+    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/edit$', views.gallery_edit, name='gallery_edit'),
+    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/history/$', views.gallery_history, name='gallery_history'),
+    re_path(r'^gallery/(?P<gallery_id>[0-9]+)/history/(?P<page_number>[0-9]+)/$', views.gallery_history, name='gallery_history_page'),
+    
+    re_path(r'^staff_page/$', views.staff_page, name='staff_page'),
+    re_path(r'^staff_page/mass_rename$', views.staff_mass_rename, name='staff_mass_rename'),
+    re_path(r'^staff_page/configuration$', views.SiteConfigurationView.as_view(), name='staff_site_configuration'),
+    re_path(r'^staff_page/block$', views.StaffBanUser.as_view(), name='staff_block'),
+
+    path('comment/<int:pk>/toggle_view', booru.core.views.StaffCommentToggleHiddenView.as_view(), name='comment-toggle-view'),
+]
```

### Comparing `Boorunaut-0.4.3/booru/utils.py` & `Boorunaut-0.5.0/booru/utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,317 +1,317 @@
-import base64
-import copy
-import hashlib
-import io
-import tempfile
-import time
-import urllib.request
-from io import BytesIO
-
-import diff_match_patch as dmp_module
-import ffmpeg
-import requests
-from django import forms
-from django.apps import apps
-from django.conf import settings
-from django.core.files.base import ContentFile
-from django.core.files.storage import default_storage
-from django.core.files.uploadedfile import InMemoryUploadedFile
-from django.db.models import Count, Sum
-from django.shortcuts import get_object_or_404
-from PIL import Image as ImagePIL
-from rolepermissions.roles import RolesManager
-
-sample_max_resolution = (850, None)
-preview_max_resolution = (150, 150)
-
-def space_splitter(tag_string):
-    return [t.strip().lower() for t in tag_string.split(' ') if t.strip()]
-
-def space_joiner(tags):
-    return ' '.join(t.name for t in tags)
-
-def image_resizer(original_image, size):
-    img_io = io.BytesIO()
-    resized_image = original_image.copy()
-    resized_image.thumbnail(size, ImagePIL.ANTIALIAS)
-    resized_image.convert('RGB').save(img_io, format='JPEG', quality=100)
-    img_content = ContentFile(img_io.getvalue(), original_image.filename)
-    return img_content
-
-def get_video_preview(video):
-    ''' Returns the resized preview image. '''
-    in_filename = video.url[1:]
-    frame_num = 1
-
-    try:
-        out, err = (
-                ffmpeg
-                .input(in_filename)
-                .filter('select', 'gte(n,{})'.format(frame_num))
-                .output('pipe:', vframes=1, format='image2', vcodec='mjpeg')
-                .run(capture_stdout=True)
-        )
-        image = ImagePIL.open(io.BytesIO(out))
-        return get_preview(image)
-    except ffmpeg.Error as e:
-        print(e.stderr)
-
-    return None
-
-def get_pil_image_if_valid(image):
-    ''' Returns a PIL Image if the given image file is valid, returns False otherwise. '''
-    try:
-        return ImagePIL.open(image)
-    except:
-        return False
-
-def check_video_is_valid(video):
-    ''' Returns True if it is a valid video file. Returns False otherwise. '''
-    result = False
-    try:
-        with tempfile.NamedTemporaryFile() as f:
-            f.write(video.file.getbuffer())
-            f.seek(0)
-            probe_result = ffmpeg.probe(f.name)
-
-            if probe_result['format']['probe_score'] == 100:
-                result = True
-    except:
-        pass
-    return result
-
-def get_video_dimensions(video):
-    result = ffmpeg.probe(video.url[1:])
-    video_stream = next((stream for stream in result['streams'] if stream['codec_type'] == 'video'), None)
-    return (video_stream['width'], video_stream['height'])
-
-def convert_to_rgb(pil_image):
-    ''' Converts an image from RGBA to RGB if needed. '''
-
-    # Converting to RBG if RGBA
-    if pil_image.mode == 'RGBA':
-        pil_image.load()
-
-        rgb_image = ImagePIL.new("RGB", pil_image.size, (255, 255, 255))
-        rgb_image.paste(pil_image, mask=pil_image.split()[3]) # 3 is the alpha channel
-
-        return rgb_image
-    else:
-        return pil_image
-
-
-def verify_and_perform_implications(tag_name):
-    Post = apps.get_model('booru', 'Post')
-    Implication = apps.get_model('booru', 'Implication')
-    
-    implication = Implication.objects.filter(from_tag__name=tag_name, status=1).first()
-
-    if implication is not None:
-        from_tag = implication.from_tag
-        to_tag = implication.to_tag
-
-        missing_posts = Post.objects.filter(tags__name__in=[from_tag]).exclude(tags__name__in=[to_tag])
-
-        if missing_posts.exists():
-            for post in missing_posts:
-                post.check_and_update_implications()
-
-def get_diff(field_name, old_revision, new_revision):
-    old_revision_field = old_revision.field_dict[field_name]
-    new_revision_field = new_revision.field_dict[field_name]
-
-    dmp = dmp_module.diff_match_patch()
-    diff_field = dmp.diff_main(old_revision_field, new_revision_field)
-    dmp.diff_cleanupSemantic(diff_field)
-    diff_html = dmp.diff_prettyHtml(diff_field).replace('&para;', '') # Removes paragraph character 
-                                                                      # added by the library.
-
-    return diff_html
-
-def compare_strings(old_string, new_string):
-    """Splits a string by spaces, and compares the lists. Then, returns a dictionary containing the following results:
-
-    `equal` is a list of words in common.
-
-    `removed` is a list of words that ARE in old_string, but ARE NOT in new_string.
-
-    `added` is a list of words that ARE NOT in old_string, but ARE in new_string.
-    """
-    old_string = old_string.split(" ")
-    new_string = new_string.split(" ")
-
-    equal_words = list(set(old_string).intersection(new_string))
-    removed_words = list(set(old_string) - set(new_string))
-    added_words = list(set(new_string) - set(old_string))
-
-    return {"equal": equal_words, "removed": removed_words, "added": added_words}
-
-def parse_tags(tag_string):
-    splitted_tags = space_splitter(tag_string)
-
-    tag_info = {'~': [], '' : [], '-' : [], 'meta': []}
-
-    for tag in splitted_tags:
-        if tag.startswith('~') or tag.startswith('-'):
-            tag_info[tag[0]].append(tag[1:])
-        elif ':' in tag:
-            tag_info['meta'].append(tag)
-        else:
-            tag_info[''].append(tag)
-
-    return tag_info
-
-def filter_posts(tag_list):
-    from booru.models import Post
-    from django.db.models import Q
-    import re
-
-    filtered_posts = Post.objects.all()
-    filtered_posts = filtered_posts.order_by('-id')
-
-    query = Q()
-
-    for tag in tag_list['~']:
-        query = query | Q(tags__name__in=[tag])
-    
-    filtered_posts = filtered_posts.filter(query)
-
-    for tag in tag_list['']:
-        filtered_posts = filtered_posts.filter(Q(tags__name__in=[tag]))
-
-    for tag in tag_list['-']:
-        filtered_posts = filtered_posts.exclude(Q(tags__name__in=[tag]))
-    
-    for tag in tag_list['meta']:
-        score_match = re.match('score:(>|<|>=|<=|)((?:\+|-|)\d+)', tag)
-        if tag == 'status:pending':
-            filtered_posts = filtered_posts.filter(status=Post.PENDING)
-        elif tag == 'status:approved':
-            filtered_posts = filtered_posts.filter(status=Post.APPROVED)
-        elif tag == 'status:hidden':
-            filtered_posts = filtered_posts.filter(status=Post.HIDDEN)
-        elif tag == 'status:deleted':
-            filtered_posts = filtered_posts.filter(status=Post.DELETED)
-        elif tag == 'rating:safe' or tag == 'rating:s':
-            filtered_posts = filtered_posts.filter(rating=Post.SAFE)
-        elif tag == 'rating:questionable' or tag == 'rating:q':
-            filtered_posts = filtered_posts.filter(rating=Post.QUESTIONABLE)
-        elif tag == 'rating:explicit' or tag == 'rating:e':
-            filtered_posts = filtered_posts.filter(rating=Post.EXPLICIT)
-        elif tag == 'rating:none' or tag == 'rating:n':
-            filtered_posts = filtered_posts.filter(rating=Post.NONE)
-        elif score_match:
-            inequality = score_match[1]
-            value = score_match[2]
-            if inequality == '>':
-                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                    .filter(score_sum__gt=value)
-            elif inequality == '>=':
-                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                    .filter(score_sum__gte=value)
-            elif inequality == '<':
-                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                    .filter(score_sum__lt=value)
-            elif inequality == '<=':
-                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                    .filter(score_sum__lte=value)
-            else:
-                if value == '0':
-                    filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                .annotate(scorevote_count=Count('scorevote'))\
-                                                .filter(Q(score_sum=value) | Q(scorevote_count=0))
-                else:
-                    filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                    .filter(score_sum=value)
-        elif tag == 'order:score':
-            filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                    .order_by('-score_sum')
-        elif tag == 'order:score_asc':
-            filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
-                                                    .order_by('score_sum')
-        elif tag == 'order:random':
-            filtered_posts = filtered_posts.order_by('?')
-    return filtered_posts.distinct()
-
-def parse_and_filter_tags(tags):
-    return filter_posts(parse_tags(tags))
-
-def get_file_md5(file_data):
-    hash_md5 = hashlib.md5()
-    for chunk in iter(lambda: file_data.read(4096), b""):
-        hash_md5.update(chunk)
-    return hash_md5.hexdigest()
-
-def get_all_roles():
-    roles_list = enumerate(list(RolesManager.get_roles_names()))
-    roles = []
-    for key, role in roles_list:
-        roles.append((role, role.title()))
-    return tuple(roles)
-
-# Image utils
-def download_and_return_BytesIO(url):
-    r = requests.get(url, stream=True, timeout=settings.BOORUNAUT_INITIAL_UPLOAD_TIMEOUT)
-    r.raise_for_status()
-
-    if int(r.headers.get('Content-Length')) > settings.BOORUNAUT_MAX_SIZE_FILE:
-        max_size_mb = settings.BOORUNAUT_MAX_SIZE_FILE / 1024 / 1024
-        raise forms.ValidationError("Please upload a file with less than {} MB.".format(max_size_mb))
-
-    size = 0
-    start = time.time()
-
-    img_bytesio = io.BytesIO()
-
-    for chunk in r.iter_content(1024):
-        if time.time() - start > settings.BOORUNAUT_MAXIMUM_UPLOAD_TIMEOUT:
-            raise forms.ValidationError("Timeout of connection was reached.")
-
-        size += len(chunk)
-        if size > settings.BOORUNAUT_MAX_SIZE_FILE:
-            raise forms.ValidationError("Please upload a file with less than {} MB.".format(max_size_mb))
-        
-        img_bytesio.write(chunk)
-    return img_bytesio
-
-def BytesIO_to_InMemoryUploadedFile(img_bytesio):
-    img_size = img_bytesio.getbuffer().nbytes
-    img_format = BytesIO_to_PIL(img_bytesio).format.lower()
-    img_name = "tempfile." + img_format
-    img_content_type = "image/" + img_format
-    
-    return InMemoryUploadedFile(
-        img_bytesio,
-        field_name='tempfile',
-        name=img_name,
-        content_type=img_content_type,
-        size=img_size,
-        charset='utf-8',
-    )
-
-def get_remote_image_as_InMemoryUploadedFile(url):
-    image_bytesio = download_and_return_BytesIO(url)
-    return BytesIO_to_InMemoryUploadedFile(image_bytesio)
-
-def BytesIO_to_PIL(img_bytesio):
-    img_copy = copy.copy(img_bytesio)
-    return ImagePIL.open(img_copy)
-
-def generate_mock_image(empty=True):
-    image_base64 = "iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQI12P4//8/w38GIAXDIBKE0DHxgljNBAAO9TXL0Y4OHwAAAABJRU5ErkJggg=="
-    image_bytes = base64.b64decode(image_base64)
-    
-    im = ImagePIL.new(mode='RGB', size=(200, 200))
-    im_io = BytesIO()
-    im.save(im_io, format='JPEG')
-    im_io.seek(0)
-
-    if empty == False:
-        im_io.write(image_bytes)
-        im_io.seek(0)
-
-    image = InMemoryUploadedFile(
-        im_io, None, 'random-name.jpg', 'image/jpeg', im_io.getbuffer().nbytes, None
-    )
-
-    return image
+import base64
+import copy
+import hashlib
+import io
+import tempfile
+import time
+import urllib.request
+from io import BytesIO
+
+import diff_match_patch as dmp_module
+import ffmpeg
+import requests
+from django import forms
+from django.apps import apps
+from django.conf import settings
+from django.core.files.base import ContentFile
+from django.core.files.storage import default_storage
+from django.core.files.uploadedfile import InMemoryUploadedFile
+from django.db.models import Count, Sum
+from django.shortcuts import get_object_or_404
+from PIL import Image as ImagePIL
+from rolepermissions.roles import RolesManager
+
+sample_max_resolution = (850, None)
+preview_max_resolution = (150, 150)
+
+def space_splitter(tag_string):
+    return [t.strip().lower() for t in tag_string.split(' ') if t.strip()]
+
+def space_joiner(tags):
+    return ' '.join(t.name for t in tags)
+
+def image_resizer(original_image, size):
+    img_io = io.BytesIO()
+    resized_image = original_image.copy()
+    resized_image.thumbnail(size, ImagePIL.ANTIALIAS)
+    resized_image.convert('RGB').save(img_io, format='JPEG', quality=100)
+    img_content = ContentFile(img_io.getvalue(), original_image.filename)
+    return img_content
+
+def get_video_preview(video):
+    ''' Returns the resized preview image. '''
+    in_filename = video.url[1:]
+    frame_num = 1
+
+    try:
+        out, err = (
+                ffmpeg
+                .input(in_filename)
+                .filter('select', 'gte(n,{})'.format(frame_num))
+                .output('pipe:', vframes=1, format='image2', vcodec='mjpeg')
+                .run(capture_stdout=True)
+        )
+        image = ImagePIL.open(io.BytesIO(out))
+        return get_preview(image)
+    except ffmpeg.Error as e:
+        print(e.stderr)
+
+    return None
+
+def get_pil_image_if_valid(image):
+    ''' Returns a PIL Image if the given image file is valid, returns False otherwise. '''
+    try:
+        return ImagePIL.open(image)
+    except:
+        return False
+
+def check_video_is_valid(video):
+    ''' Returns True if it is a valid video file. Returns False otherwise. '''
+    result = False
+    try:
+        with tempfile.NamedTemporaryFile() as f:
+            f.write(video.file.getbuffer())
+            f.seek(0)
+            probe_result = ffmpeg.probe(f.name)
+
+            if probe_result['format']['probe_score'] == 100:
+                result = True
+    except:
+        pass
+    return result
+
+def get_video_dimensions(video):
+    result = ffmpeg.probe(video.url[1:])
+    video_stream = next((stream for stream in result['streams'] if stream['codec_type'] == 'video'), None)
+    return (video_stream['width'], video_stream['height'])
+
+def convert_to_rgb(pil_image):
+    ''' Converts an image from RGBA to RGB if needed. '''
+
+    # Converting to RBG if RGBA
+    if pil_image.mode == 'RGBA':
+        pil_image.load()
+
+        rgb_image = ImagePIL.new("RGB", pil_image.size, (255, 255, 255))
+        rgb_image.paste(pil_image, mask=pil_image.split()[3]) # 3 is the alpha channel
+
+        return rgb_image
+    else:
+        return pil_image
+
+
+def verify_and_perform_implications(tag_name):
+    Post = apps.get_model('booru', 'Post')
+    Implication = apps.get_model('booru', 'Implication')
+    
+    implication = Implication.objects.filter(from_tag__name=tag_name, status=1).first()
+
+    if implication is not None:
+        from_tag = implication.from_tag
+        to_tag = implication.to_tag
+
+        missing_posts = Post.objects.filter(tags__name__in=[from_tag]).exclude(tags__name__in=[to_tag])
+
+        if missing_posts.exists():
+            for post in missing_posts:
+                post.check_and_update_implications()
+
+def get_diff(field_name, old_revision, new_revision):
+    old_revision_field = old_revision.field_dict[field_name]
+    new_revision_field = new_revision.field_dict[field_name]
+
+    dmp = dmp_module.diff_match_patch()
+    diff_field = dmp.diff_main(old_revision_field, new_revision_field)
+    dmp.diff_cleanupSemantic(diff_field)
+    diff_html = dmp.diff_prettyHtml(diff_field).replace('&para;', '') # Removes paragraph character 
+                                                                      # added by the library.
+
+    return diff_html
+
+def compare_strings(old_string, new_string):
+    """Splits a string by spaces, and compares the lists. Then, returns a dictionary containing the following results:
+
+    `equal` is a list of words in common.
+
+    `removed` is a list of words that ARE in old_string, but ARE NOT in new_string.
+
+    `added` is a list of words that ARE NOT in old_string, but ARE in new_string.
+    """
+    old_string = old_string.split(" ")
+    new_string = new_string.split(" ")
+
+    equal_words = list(set(old_string).intersection(new_string))
+    removed_words = list(set(old_string) - set(new_string))
+    added_words = list(set(new_string) - set(old_string))
+
+    return {"equal": equal_words, "removed": removed_words, "added": added_words}
+
+def parse_tags(tag_string):
+    splitted_tags = space_splitter(tag_string)
+
+    tag_info = {'~': [], '' : [], '-' : [], 'meta': []}
+
+    for tag in splitted_tags:
+        if tag.startswith('~') or tag.startswith('-'):
+            tag_info[tag[0]].append(tag[1:])
+        elif ':' in tag:
+            tag_info['meta'].append(tag)
+        else:
+            tag_info[''].append(tag)
+
+    return tag_info
+
+def filter_posts(tag_list):
+    from booru.models import Post
+    from django.db.models import Q
+    import re
+
+    filtered_posts = Post.objects.all()
+    filtered_posts = filtered_posts.order_by('-id')
+
+    query = Q()
+
+    for tag in tag_list['~']:
+        query = query | Q(tags__name__in=[tag])
+    
+    filtered_posts = filtered_posts.filter(query)
+
+    for tag in tag_list['']:
+        filtered_posts = filtered_posts.filter(Q(tags__name__in=[tag]))
+
+    for tag in tag_list['-']:
+        filtered_posts = filtered_posts.exclude(Q(tags__name__in=[tag]))
+    
+    for tag in tag_list['meta']:
+        score_match = re.match('score:(>|<|>=|<=|)((?:\+|-|)\d+)', tag)
+        if tag == 'status:pending':
+            filtered_posts = filtered_posts.filter(status=Post.PENDING)
+        elif tag == 'status:approved':
+            filtered_posts = filtered_posts.filter(status=Post.APPROVED)
+        elif tag == 'status:hidden':
+            filtered_posts = filtered_posts.filter(status=Post.HIDDEN)
+        elif tag == 'status:deleted':
+            filtered_posts = filtered_posts.filter(status=Post.DELETED)
+        elif tag == 'rating:safe' or tag == 'rating:s':
+            filtered_posts = filtered_posts.filter(rating=Post.SAFE)
+        elif tag == 'rating:questionable' or tag == 'rating:q':
+            filtered_posts = filtered_posts.filter(rating=Post.QUESTIONABLE)
+        elif tag == 'rating:explicit' or tag == 'rating:e':
+            filtered_posts = filtered_posts.filter(rating=Post.EXPLICIT)
+        elif tag == 'rating:none' or tag == 'rating:n':
+            filtered_posts = filtered_posts.filter(rating=Post.NONE)
+        elif score_match:
+            inequality = score_match[1]
+            value = score_match[2]
+            if inequality == '>':
+                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                    .filter(score_sum__gt=value)
+            elif inequality == '>=':
+                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                    .filter(score_sum__gte=value)
+            elif inequality == '<':
+                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                    .filter(score_sum__lt=value)
+            elif inequality == '<=':
+                filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                    .filter(score_sum__lte=value)
+            else:
+                if value == '0':
+                    filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                .annotate(scorevote_count=Count('scorevote'))\
+                                                .filter(Q(score_sum=value) | Q(scorevote_count=0))
+                else:
+                    filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                    .filter(score_sum=value)
+        elif tag == 'order:score':
+            filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                    .order_by('-score_sum')
+        elif tag == 'order:score_asc':
+            filtered_posts = filtered_posts.annotate(score_sum=Sum('scorevote__point'))\
+                                                    .order_by('score_sum')
+        elif tag == 'order:random':
+            filtered_posts = filtered_posts.order_by('?')
+    return filtered_posts.distinct()
+
+def parse_and_filter_tags(tags):
+    return filter_posts(parse_tags(tags))
+
+def get_file_md5(file_data):
+    hash_md5 = hashlib.md5()
+    for chunk in iter(lambda: file_data.read(4096), b""):
+        hash_md5.update(chunk)
+    return hash_md5.hexdigest()
+
+def get_all_roles():
+    roles_list = enumerate(list(RolesManager.get_roles_names()))
+    roles = []
+    for key, role in roles_list:
+        roles.append((role, role.title()))
+    return tuple(roles)
+
+# Image utils
+def download_and_return_BytesIO(url):
+    r = requests.get(url, stream=True, timeout=settings.BOORUNAUT_INITIAL_UPLOAD_TIMEOUT)
+    r.raise_for_status()
+
+    if int(r.headers.get('Content-Length')) > settings.BOORUNAUT_MAX_SIZE_FILE:
+        max_size_mb = settings.BOORUNAUT_MAX_SIZE_FILE / 1024 / 1024
+        raise forms.ValidationError("Please upload a file with less than {} MB.".format(max_size_mb))
+
+    size = 0
+    start = time.time()
+
+    img_bytesio = io.BytesIO()
+
+    for chunk in r.iter_content(1024):
+        if time.time() - start > settings.BOORUNAUT_MAXIMUM_UPLOAD_TIMEOUT:
+            raise forms.ValidationError("Timeout of connection was reached.")
+
+        size += len(chunk)
+        if size > settings.BOORUNAUT_MAX_SIZE_FILE:
+            raise forms.ValidationError("Please upload a file with less than {} MB.".format(max_size_mb))
+        
+        img_bytesio.write(chunk)
+    return img_bytesio
+
+def BytesIO_to_InMemoryUploadedFile(img_bytesio):
+    img_size = img_bytesio.getbuffer().nbytes
+    img_format = BytesIO_to_PIL(img_bytesio).format.lower()
+    img_name = "tempfile." + img_format
+    img_content_type = "image/" + img_format
+    
+    return InMemoryUploadedFile(
+        img_bytesio,
+        field_name='tempfile',
+        name=img_name,
+        content_type=img_content_type,
+        size=img_size,
+        charset='utf-8',
+    )
+
+def get_remote_image_as_InMemoryUploadedFile(url):
+    image_bytesio = download_and_return_BytesIO(url)
+    return BytesIO_to_InMemoryUploadedFile(image_bytesio)
+
+def BytesIO_to_PIL(img_bytesio):
+    img_copy = copy.copy(img_bytesio)
+    return ImagePIL.open(img_copy)
+
+def generate_mock_image(empty=True):
+    image_base64 = "iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAAHElEQVQI12P4//8/w38GIAXDIBKE0DHxgljNBAAO9TXL0Y4OHwAAAABJRU5ErkJggg=="
+    image_bytes = base64.b64decode(image_base64)
+    
+    im = ImagePIL.new(mode='RGB', size=(200, 200))
+    im_io = BytesIO()
+    im.save(im_io, format='JPEG')
+    im_io.seek(0)
+
+    if empty == False:
+        im_io.write(image_bytes)
+        im_io.seek(0)
+
+    image = InMemoryUploadedFile(
+        im_io, None, 'random-name.jpg', 'image/jpeg', im_io.getbuffer().nbytes, None
+    )
+
+    return image
```

### Comparing `Boorunaut-0.4.3/booru/views.py` & `Boorunaut-0.5.0/booru/views.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,611 +1,611 @@
-import json
-
-import diff_match_patch as dmp_module
-from django.apps import apps
-from django.conf import settings
-from django.contrib.admin.views.decorators import staff_member_required
-from django.contrib.auth import REDIRECT_FIELD_NAME, authenticate
-from django.contrib.auth.decorators import login_required
-from django.core.paginator import EmptyPage, Paginator
-from django.db.models import Count, Q
-from django.forms.models import model_to_dict
-from django.http import HttpResponse
-from django.shortcuts import get_object_or_404, redirect, render
-from django.urls import reverse, reverse_lazy
-from django.utils.decorators import method_decorator
-from django.views import generic
-from django.views.decorators.csrf import csrf_protect
-from django.views.generic import FormView
-from django.views.generic.edit import DeleteView
-from rolepermissions.checkers import has_permission
-
-from booru.account.decorators import user_is_not_blocked
-from booru.account.models import Account, Privilege, Timeout
-
-from . import utils
-from .forms import (BanUserForm, CreatePostForm, EditPostForm,
-                    GalleryCreateForm, GalleryEditForm, GalleryListSearchForm,
-                    ImplicationCreateForm, ImplicationFilterForm,
-                    MassRenameForm, SiteConfigurationForm, TagEditForm,
-                    TagListSearchForm)
-from .models import (Comment, Configuration, Favorite, Gallery, Implication,
-                     Post, PostTag, ScoreVote, TaggedPost)
-
-
-@user_is_not_blocked
-def index(request):
-    welcome_page = bool(int(Configuration.objects.get(code_name='welcome_page').value))
-
-    if welcome_page:
-        post_count = Post.objects.not_deleted().count()
-        return render(request, 'booru/index.html', {'post_count': post_count})
-    else:
-        return redirect('booru:posts')
-
-@user_is_not_blocked
-def post_detail(request, post_id):
-    post = get_object_or_404(Post, id=post_id)
-    form = EditPostForm(request.POST or None, request.FILES or None, instance=post)
-    
-    is_favorited = False
-    has_comment_priv = False
-    current_vote = 0
-    
-    if request.user.is_authenticated:
-        is_favorited = Favorite.objects.filter(account=request.user, post=post).exists()
-        current_vote = ScoreVote.objects.filter(account=request.user, post=post)
-        has_comment_priv = request.user.has_priv("can_comment")
-
-        if current_vote.exists():
-            current_vote = current_vote.first().point
-        else:
-            current_vote = 0
-    
-    if request.method == "POST":
-        if not request.user.is_authenticated:
-            return redirect('account:login')
-        
-        newCommentTextarea = request.POST.get("newCommentTextarea")
-
-        if form.is_valid(): # Post editing (post_edit)
-            post = form.save(commit=False)
-            form.save_m2m()
-            post.check_and_update_implications()
-            post.save()
-            return redirect('booru:post_detail', post_id=post.id)
-        elif newCommentTextarea and has_comment_priv: # Comment creating
-            comment_content = newCommentTextarea
-            Comment.objects.create(content=comment_content, author=request.user, content_object=post)
-            return redirect('booru:post_detail', post_id=post.id)
-
-    previous_post = Post.objects.filter(id__lt=post.id).exclude(status=2).exclude(status=3).last() or None
-    next_post = Post.objects.filter(id__gt=post.id).exclude(status=2).exclude(status=3).first() or None
-
-    ordered_tags = post.get_ordered_tags()
-
-    SHOW_ADS = (post.rating == Post.QUESTIONABLE and settings.BOORUNAUT_ADS_ON_QUESTIONABLE or
-                post.rating == Post.EXPLICIT and settings.BOORUNAUT_ADS_ON_EXPLICIT or
-                post.rating == Post.SAFE)
-
-    return render(  request=request, template_name='booru/post_detail.html',
-                    context={"post": post, "ordered_tags": ordered_tags, "form": form,
-                        "previous_post": previous_post, "next_post": next_post,
-                        "is_favorited":is_favorited, "current_vote": current_vote,
-                        "can_comment": has_comment_priv, "SHOW_ADS": SHOW_ADS})
-
-@user_is_not_blocked
-def post_history(request, post_id, page_number = 1):
-    post = get_object_or_404(Post, id=post_id)
-    page_limit = 20
-
-    p = Paginator(post.history.all(), page_limit)
-    page = p.page(page_number)
-
-    return render(request, 'booru/post_history.html', {"page": page, "post": post})
-
-@login_required
-@user_is_not_blocked
-def upload(request): # post_create
-    form = CreatePostForm(request.POST or None, request.FILES or None)
-    
-    if form.is_valid():
-        post = form.save(commit=False)
-        post.uploader = request.user
-        post.save_without_historical_record()
-        form.save_m2m()
-        post.check_and_update_implications()
-        post.save()
-        return redirect('booru:post_detail', post_id=post.id)
-
-    return render(request, 'booru/upload.html', {"form": form})
-
-@user_is_not_blocked
-def post_list_detail(request, page_number = 1):
-    tags = request.GET.get("tags", "")
-    
-    posts = utils.parse_and_filter_tags(tags)
-    if not has_permission(request.user, 'change_status'):
-        posts = posts.exclude(status=Post.HIDDEN).exclude(status=Post.DELETED)
-
-    # Check if user enabled safe only
-    # TODO: transform these tag operations into a class
-    is_safe_only = False
-    if (request.user.is_authenticated and request.user.safe_only) or (not request.user.is_authenticated and tags == ""):
-        posts = posts.exclude(rating=Post.QUESTIONABLE).exclude(rating=Post.EXPLICIT)
-        is_safe_only = True
-    
-    page_limit = 20
-    p = Paginator(posts, page_limit)
-    page = p.page(page_number)
-    post_list = page.object_list
-
-    tags_list = Post.tags.most_common().filter(id__in=post_list)[:25]
-    
-    return render(request, 'booru/posts.html', {"posts": post_list, "page": page, "tags_list": tags_list,
-                                                "SHOW_ADS": True, "is_safe_only": is_safe_only})
-
-@user_is_not_blocked
-def tags_list(request, page_number = 1):
-    searched_tag = request.GET.get("tags", "")
-    category = request.GET.get("category", "")
-
-    try:
-        category = int(category)
-    except:
-        category = 0
-
-    form = TagListSearchForm(request.GET or None)
-
-    tags = PostTag.objects.all()
-
-    if searched_tag != "":
-        tags = tags.filter(name=searched_tag)
-
-    if category != 0:
-        tags = tags.filter(category=category)
-
-    tags = tags.order_by('id')
-    
-    page_limit = 10
-    p = Paginator(tags, page_limit)
-    
-    try:
-        page = p.page(page_number)
-    except EmptyPage:
-        url = reverse('booru:tags_list') + '?tags={}&category={}'.format(searched_tag, category)
-        return redirect(url, page_number=1)
-    
-    tags_list = page.object_list
-    return render(request, 'booru/tag_list.html', {"tags": tags_list, "page": page, "form": form})
-
-@login_required
-@user_is_not_blocked
-def tag_edit(request, tag_id):
-    tag = get_object_or_404(PostTag, pk=tag_id)
-    tag_dict = model_to_dict(tag)
-
-    if tag.associated_user_id:
-        associated_user = get_object_or_404(Account.objects.active(), id=tag.associated_user_id)
-        tag_dict['associated_user_name'] = associated_user.slug
-
-    form = TagEditForm(request.POST or None, instance=tag, initial=tag_dict)
-    if form.is_valid() and request.POST:
-        tag = form.save(commit=False)
-        tag.author = request.user
-        if form.cleaned_data['associated_user_name']:
-            associated_user = get_object_or_404(Account.objects.active(), slug=form.cleaned_data['associated_user_name'])
-            tag.associated_user = associated_user
-        tag.save()
-        form.save_m2m()
-        return redirect('booru:tag_detail', tag.id)
-        
-    return render(request, 'booru/tag_edit.html', {"tag": tag, "form": form})
-
-@user_is_not_blocked
-def tag_detail(request, tag_id):
-    tag = get_object_or_404(PostTag, pk=tag_id)
-    last_posts = Post.objects.filter(tags__name__in=[tag.name])[:6]
-    return render(request, 'booru/tag_detail.html', {"tag": tag, "last_post": last_posts})
-
-@user_is_not_blocked
-def tag_history(request, tag_id, page_number = 1):
-    tag = get_object_or_404(PostTag, pk=tag_id)
-    page_limit = 20
-
-    p = Paginator(tag.history.all(), page_limit)
-    page = p.page(page_number)
-    return render(request, 'booru/tag_history.html', {"page": page, "tag": tag})
-
-class TagDelete(DeleteView):
-    model = PostTag
-    success_url = reverse_lazy('booru:tags_list')
-    template_name = 'booru/tag_confirm_delete.html'
-
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated or not has_permission(request.user, 'manage_tags'):
-            return redirect('account:login')
-        return super().dispatch(request, *args, **kwargs)
-
-@user_is_not_blocked
-def tag_revision_diff(request, tag_id):
-    tag = get_object_or_404(PostTag, pk=tag_id)
-
-    old_version = tag.history.filter(history_id=request.GET.get('oldRevision')).first()
-    new_version = tag.history.filter(history_id=request.GET.get('newRevision')).first()
-
-    delta = new_version.diff_against(old_version)
-
-    context = {"tag": tag, "changes": delta.changes,
-               "old_version": old_version, "new_version": new_version}
-    
-    return render(request, 'booru/tag_revision_diff.html', context)
-
-class ImplicationListView(generic.ListView):
-    model = Implication
-    paginate_by = 20
-
-    def get_queryset(self):
-        queryset = Implication.objects.all()
-
-        if self.request.GET.get('name'):
-            queryset = queryset.filter( Q(from_tag__name=self.request.GET.get('name'))|
-                                        Q(to_tag__name=self.request.GET.get('name')))
-        
-        status = self.request.GET.get('status')
-        if status:
-            try:
-                status = int(status)
-                queryset = queryset.filter(status=status)
-            except ValueError:
-                pass
-        return queryset
-
-    def get_context_data(self, **kwargs):
-        context = super(ImplicationListView, self).get_context_data(**kwargs)
-        context['form'] = ImplicationFilterForm(self.request.GET)
-        return context
-    
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        return super().dispatch(request, *args, **kwargs)
-
-class ImplicationDetailView(generic.DetailView):
-    model = Implication
-
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        return super().dispatch(request, *args, **kwargs)
-
-@login_required
-@user_is_not_blocked
-def implication_create(request):
-    form = ImplicationCreateForm(data=request.POST)
-    
-    if form.is_valid():
-        from_tag_name = form.cleaned_data['from_tag']
-        to_tag_name = form.cleaned_data['to_tag']
-
-        from_tag, from_tag_created = PostTag.objects.get_or_create(name=from_tag_name)
-        to_tag, from_tag_created = PostTag.objects.get_or_create(name=to_tag_name)
-
-        implication, implication_created = Implication.objects.get_or_create(from_tag=from_tag, to_tag=to_tag)
-        implication.author = request.user
-        implication.save()
-        return redirect('booru:implication-detail', implication.id)
-
-    return render(request, 'booru/implication_create.html', { "form": form })
-
-@staff_member_required
-@user_is_not_blocked
-def implication_approve(request, implication_id):
-    implication = Implication.objects.get(id=implication_id)
-
-    if implication.status != 1:
-        implication.status = 1
-        implication.approver = request.user
-        implication.save()
-    
-    utils.verify_and_perform_implications(implication.from_tag)
-    return redirect('booru:implication-detail', implication.id)
-
-@staff_member_required
-@user_is_not_blocked
-def implication_disapprove(request, implication_id):
-    implication = Implication.objects.get(id=implication_id)
-    implication.status = 2
-    implication.save()
-    return redirect('booru:implication-detail', implication.id)
-
-@staff_member_required
-@user_is_not_blocked
-def staff_page(request):
-    Account = apps.get_model('account', 'Account')
-    accounts = Account.objects.active().order_by("-id")
-
-    context = {
-        'accounts': accounts
-    }
-
-    return render(request, 'booru/staff_page.html', context)
-
-@user_is_not_blocked
-def tag_search(request):
-    term = request.GET.get("term", "")
-    operator = ""
-    value = term
-
-    if term.startswith("-") or term.startswith("~"):
-        operator = term[0]
-        value = term[1:]
-
-    tag_results = PostTag.objects.filter(Q(name__istartswith=value) | Q(aliases__name__istartswith=value)).distinct()
-    tag_results = tag_results[:10]
-
-    results = []
-    for tag in tag_results:
-        name = operator + tag.name
-        if tag.name.startswith(value):
-            results.append({'id': tag.pk, 'label': name, 'value': name})
-        else:
-            results.append({'id': tag.pk, 'label': "{} ({})".format(name, term), 'value': name})
-    return HttpResponse(json.dumps(results), content_type='application/json')
-
-@user_is_not_blocked
-def post_approve(request, post_id):
-    post = Post.objects.get(id=post_id)
-
-    if has_permission(request.user, "change_status") and post.status != 1:
-        post.status = 1
-        post.save()
-    return redirect('booru:post_detail', post_id=post.id)
-
-@user_is_not_blocked
-def post_hide(request, post_id):
-    post = Post.objects.get(id=post_id)
-
-    if has_permission(request.user, "change_status") and post.status != 2:
-        post.status = 2
-        post.save()
-    return redirect('booru:post_detail', post_id=post.id)
-
-@user_is_not_blocked
-def post_delete(request, post_id):
-    post = Post.objects.get(id=post_id)
-
-    if has_permission(request.user, "change_status") and post.status != 3:
-        post.status = 3
-        post.save()
-    return redirect('booru:post_detail', post_id=post.id)
-
-@login_required
-@user_is_not_blocked
-def post_favorite(request, post_id):
-    post = Post.objects.get(id=post_id)
-    favorite = Favorite.objects.filter(post=post, account=request.user).first()
-
-    if favorite:
-        favorite.delete()
-    else:
-        Favorite.objects.create(post=post, account=request.user)
-    
-    return redirect('booru:post_detail', post_id=post.id)
-
-@login_required
-@user_is_not_blocked
-def post_score_vote(request, post_id):
-    post = Post.objects.get(id=post_id)
-    score_vote = ScoreVote.objects.filter(post=post, account=request.user).first()
-
-    value = int(request.GET.get("point", 0))
-    if value > 1: value = 1
-    if value < -1: value = -1
-
-    if score_vote:
-        if score_vote.point == value:
-            score_vote.point = 0
-        else:
-            score_vote.point = value
-
-        score_vote.save()
-    else:
-        score_vote = ScoreVote.objects.create(post=post, account=request.user, point=value)
-    
-    results = {'value': score_vote.point, "current_points": post.get_score_count()}
-    return HttpResponse(json.dumps(results), content_type='application/json')
-
-@user_is_not_blocked
-def staff_mass_rename(request):
-    form = MassRenameForm(request.POST or None, request.FILES or None)
-
-    if has_permission(request.user, "mass_rename"):
-        if form.is_valid():
-            filter_by = form.cleaned_data['filter_by']
-            when = form.cleaned_data['when']
-            replace_with = form.cleaned_data['replace_with']
-
-            posts = utils.parse_and_filter_tags(filter_by)
-
-            when = utils.space_splitter(when)
-            replace_with = utils.space_splitter(replace_with)
-
-            posts = posts.filter(tags__name__in=when)
-
-            for post in posts:
-                post.tags.remove(*when)
-                post.tags.add(*replace_with)
-                post.save()
-                
-            return redirect('booru:staff_mass_rename')
-        return render(request, 'booru/staff_mass_rename.html', {"form": form})
-    return redirect('booru:index')
-
-@user_is_not_blocked
-def gallery_list(request, page_number = 1):
-    searched_gallery = request.GET.get("name", "")
-    form = GalleryListSearchForm(request.GET or None)
-
-    galleries = Gallery.objects.all().order_by('-id')
-    if searched_gallery != "":
-        galleries = galleries.filter(name__icontains=searched_gallery)
-    
-    page_limit = 10
-    p = Paginator(galleries, page_limit)
-    page = p.page(page_number)
-    gallery_list = page.object_list
-    
-    return render(request, 'booru/gallery_list.html', {"galleries": gallery_list, "page": page, "form": form})
-
-@user_is_not_blocked
-def gallery_history(request, gallery_id, page_number = 1):
-    gallery = get_object_or_404(Gallery, id=gallery_id)
-    page_limit = 20
-
-    p = Paginator(gallery.history.all(), page_limit)
-    page = p.page(page_number)
-
-    object_enum = enumerate(page.object_list)
-
-    return render(request, 'booru/gallery_history.html', {"page": page, "gallery": gallery})
-
-@login_required
-@user_is_not_blocked
-def gallery_edit(request, gallery_id):
-    gallery = get_object_or_404(Gallery, pk=gallery_id)
-
-    gallery_dict = model_to_dict(gallery)
-    gallery_dict['posts_ids'] = '\n'.join([str(post_id['id']) for post_id in gallery.posts.values('id')])
-    form = GalleryEditForm(request.POST or None, instance=gallery, initial=gallery_dict)
-
-    if form.is_valid():
-        posts_ids = form.cleaned_data['posts_ids'].splitlines()
-        gallery = form.save(commit=False)
-        gallery.posts.clear()
-        gallery.posts_mirror = " ".join(form.cleaned_data['posts_ids'].splitlines())
-        gallery.save()
-        posts = Post.objects.filter(id__in=posts_ids)
-        gallery.posts.add(*posts)
-        form.save_m2m()
-        return redirect('booru:gallery_detail', gallery_id=gallery.id)
-        
-    return render(request, 'booru/gallery_edit.html', {"form": form, "gallery": gallery})
-
-@login_required
-@user_is_not_blocked
-def gallery_create(request):    
-    form = GalleryCreateForm(request.POST or None, request.FILES or None)
-    
-    if form.is_valid():
-        posts_text = form.cleaned_data['posts_ids']
-        posts_ids = posts_text.splitlines()
-        
-        gallery = form.save(commit=False)
-        gallery.posts_mirror = " ".join(posts_ids)
-        gallery.save()
-        posts = Post.objects.filter(id__in=posts_ids)
-        gallery.posts.add(*posts)
-        form.save_m2m()
-        return redirect('booru:gallery_detail', gallery_id=gallery.id)
-    return render(request, 'booru/gallery_create.html', {"form": form})
-
-@user_is_not_blocked
-def gallery_detail(request, gallery_id):
-    page_number = int(request.GET.get('page', '1'))
-    page_limit = 20
-
-    gallery = Gallery.objects.get(id=gallery_id)
-    posts = gallery.posts.all()
-
-    p = Paginator(posts, page_limit)
-    page = p.page(page_number)
-
-    return render(request, 'booru/gallery_detail.html', {"gallery": gallery, "page": page})
-
-class StaffBanUser(FormView):
-    """
-    Provides a form for staff members to configure their booru.
-    """
-    success_url = '.'
-    form_class = BanUserForm
-    redirect_field_name = REDIRECT_FIELD_NAME
-    template_name = "booru/staff_user_tools.html"
-
-    def form_valid(self, form):
-        reason = form.cleaned_data['reason']
-        expiration = form.cleaned_data['expiration']
-        revoked = Privilege.objects.get(codename="can_login")
-        target_user = Account.objects.get(username=form.cleaned_data['username'])
-        author = self.request.user
-
-        if not has_role(target_user, 'administrator'): # Can't ban admins
-            if (has_role(target_user, 'moderator') and has_permission(request.user, 'booru.ban_mod')
-                or not has_role(target_user, 'moderator')):
-                instance = Timeout.objects.create(  author=author, target_user=target_user, 
-                                                    expiration=expiration, reason=reason)
-                instance.revoked.add(revoked)
-        return super().form_valid(form)
-
-    @method_decorator(csrf_protect)
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated or not has_permission(request.user, 'booru.ban_user'):
-            return redirect('account:login')
-        return super().dispatch(request, *args, **kwargs)
-
-class SiteConfigurationView(FormView):
-    """
-    Provides a form for staff members to configure their booru.
-    """
-    success_url = '.'
-    form_class = SiteConfigurationForm
-    redirect_field_name = REDIRECT_FIELD_NAME
-    template_name = "booru/staff_site_configuration.html"
-
-    def get_initial(self):
-        """
-        Returns the initial data to use for forms on this view.
-        """
-        initial = super().get_initial()
-
-        initial['site_title'] = Configuration.objects.get(code_name='site_title').value
-        initial['site_description'] = Configuration.objects.get(code_name='site_description').value
-        initial['terms_of_service'] = Configuration.objects.get(code_name='terms_of_service').value
-        initial['privacy_policy'] = Configuration.objects.get(code_name='privacy_policy').value
-        initial['announcement'] = Configuration.objects.get(code_name='announcement').value
-        initial['welcome_page'] = bool(int(Configuration.objects.get(code_name='welcome_page').value))
-        return initial
-
-    def form_valid(self, form):
-        site_title = Configuration.objects.get(code_name='site_title')
-        site_title.value = form.cleaned_data.get('site_title')
-        site_title.save()
-
-        site_description = Configuration.objects.get(code_name='site_description')
-        site_description.value = form.cleaned_data.get('site_description')
-        site_description.save()
-
-        terms_of_service = Configuration.objects.get(code_name='terms_of_service')
-        terms_of_service.value = form.cleaned_data.get('terms_of_service')
-        terms_of_service.save()
-
-        privacy_policy = Configuration.objects.get(code_name='privacy_policy')
-        privacy_policy.value = form.cleaned_data.get('privacy_policy')
-        privacy_policy.save()
-
-        announcement = Configuration.objects.get(code_name='announcement')
-        announcement.value = form.cleaned_data.get('announcement')
-        announcement.save()
-
-        welcome_page = Configuration.objects.get(code_name='welcome_page')
-        welcome_page.value = int(form.cleaned_data.get('welcome_page') == True)
-        welcome_page.save()
-
-        return super().form_valid(form)
-
-    @method_decorator(csrf_protect)
-    @user_is_not_blocked
-    def dispatch(self, request, *args, **kwargs):
-        if not request.user.is_authenticated or not has_permission(request.user,'change_configurations'):
-            return redirect('account:login')
-
-        return super().dispatch(request, *args, **kwargs)
+import json
+
+import diff_match_patch as dmp_module
+from django.apps import apps
+from django.conf import settings
+from django.contrib.admin.views.decorators import staff_member_required
+from django.contrib.auth import REDIRECT_FIELD_NAME, authenticate
+from django.contrib.auth.decorators import login_required
+from django.core.paginator import EmptyPage, Paginator
+from django.db.models import Count, Q
+from django.forms.models import model_to_dict
+from django.http import HttpResponse
+from django.shortcuts import get_object_or_404, redirect, render
+from django.urls import reverse, reverse_lazy
+from django.utils.decorators import method_decorator
+from django.views import generic
+from django.views.decorators.csrf import csrf_protect
+from django.views.generic import FormView
+from django.views.generic.edit import DeleteView
+from rolepermissions.checkers import has_permission
+
+from booru.account.decorators import user_is_not_blocked
+from booru.account.models import Account, Privilege, Timeout
+
+from . import utils
+from .forms import (BanUserForm, CreatePostForm, EditPostForm,
+                    GalleryCreateForm, GalleryEditForm, GalleryListSearchForm,
+                    ImplicationCreateForm, ImplicationFilterForm,
+                    MassRenameForm, SiteConfigurationForm, TagEditForm,
+                    TagListSearchForm)
+from .models import (Comment, Configuration, Favorite, Gallery, Implication,
+                     Post, PostTag, ScoreVote, TaggedPost)
+
+
+@user_is_not_blocked
+def index(request):
+    welcome_page = bool(int(Configuration.objects.get(code_name='welcome_page').value))
+
+    if welcome_page:
+        post_count = Post.objects.not_deleted().count()
+        return render(request, 'booru/index.html', {'post_count': post_count})
+    else:
+        return redirect('booru:posts')
+
+@user_is_not_blocked
+def post_detail(request, post_id):
+    post = get_object_or_404(Post, id=post_id)
+    form = EditPostForm(request.POST or None, request.FILES or None, instance=post)
+    
+    is_favorited = False
+    has_comment_priv = False
+    current_vote = 0
+    
+    if request.user.is_authenticated:
+        is_favorited = Favorite.objects.filter(account=request.user, post=post).exists()
+        current_vote = ScoreVote.objects.filter(account=request.user, post=post)
+        has_comment_priv = request.user.has_priv("can_comment")
+
+        if current_vote.exists():
+            current_vote = current_vote.first().point
+        else:
+            current_vote = 0
+    
+    if request.method == "POST":
+        if not request.user.is_authenticated:
+            return redirect('account:login')
+        
+        newCommentTextarea = request.POST.get("newCommentTextarea")
+
+        if form.is_valid(): # Post editing (post_edit)
+            post = form.save(commit=False)
+            form.save_m2m()
+            post.check_and_update_implications()
+            post.save()
+            return redirect('booru:post_detail', post_id=post.id)
+        elif newCommentTextarea and has_comment_priv: # Comment creating
+            comment_content = newCommentTextarea
+            Comment.objects.create(content=comment_content, author=request.user, content_object=post)
+            return redirect('booru:post_detail', post_id=post.id)
+
+    previous_post = Post.objects.filter(id__lt=post.id).exclude(status=2).exclude(status=3).last() or None
+    next_post = Post.objects.filter(id__gt=post.id).exclude(status=2).exclude(status=3).first() or None
+
+    ordered_tags = post.get_ordered_tags()
+
+    SHOW_ADS = (post.rating == Post.QUESTIONABLE and settings.BOORUNAUT_ADS_ON_QUESTIONABLE or
+                post.rating == Post.EXPLICIT and settings.BOORUNAUT_ADS_ON_EXPLICIT or
+                post.rating == Post.SAFE)
+
+    return render(  request=request, template_name='booru/post_detail.html',
+                    context={"post": post, "ordered_tags": ordered_tags, "form": form,
+                        "previous_post": previous_post, "next_post": next_post,
+                        "is_favorited":is_favorited, "current_vote": current_vote,
+                        "can_comment": has_comment_priv, "SHOW_ADS": SHOW_ADS})
+
+@user_is_not_blocked
+def post_history(request, post_id, page_number = 1):
+    post = get_object_or_404(Post, id=post_id)
+    page_limit = 20
+
+    p = Paginator(post.history.all(), page_limit)
+    page = p.page(page_number)
+
+    return render(request, 'booru/post_history.html', {"page": page, "post": post})
+
+@login_required
+@user_is_not_blocked
+def upload(request): # post_create
+    form = CreatePostForm(request.POST or None, request.FILES or None)
+    
+    if form.is_valid():
+        post = form.save(commit=False)
+        post.uploader = request.user
+        post.save_without_historical_record()
+        form.save_m2m()
+        post.check_and_update_implications()
+        post.save()
+        return redirect('booru:post_detail', post_id=post.id)
+
+    return render(request, 'booru/upload.html', {"form": form})
+
+@user_is_not_blocked
+def post_list_detail(request, page_number = 1):
+    tags = request.GET.get("tags", "")
+    
+    posts = utils.parse_and_filter_tags(tags)
+    if not has_permission(request.user, 'change_status'):
+        posts = posts.exclude(status=Post.HIDDEN).exclude(status=Post.DELETED)
+
+    # Check if user enabled safe only
+    # TODO: transform these tag operations into a class
+    is_safe_only = False
+    if (request.user.is_authenticated and request.user.safe_only) or (not request.user.is_authenticated and tags == ""):
+        posts = posts.exclude(rating=Post.QUESTIONABLE).exclude(rating=Post.EXPLICIT)
+        is_safe_only = True
+    
+    page_limit = 20
+    p = Paginator(posts, page_limit)
+    page = p.page(page_number)
+    post_list = page.object_list
+
+    tags_list = Post.tags.most_common().filter(id__in=post_list)[:25]
+    
+    return render(request, 'booru/posts.html', {"posts": post_list, "page": page, "tags_list": tags_list,
+                                                "SHOW_ADS": True, "is_safe_only": is_safe_only})
+
+@user_is_not_blocked
+def tags_list(request, page_number = 1):
+    searched_tag = request.GET.get("tags", "")
+    category = request.GET.get("category", "")
+
+    try:
+        category = int(category)
+    except:
+        category = 0
+
+    form = TagListSearchForm(request.GET or None)
+
+    tags = PostTag.objects.all()
+
+    if searched_tag != "":
+        tags = tags.filter(name=searched_tag)
+
+    if category != 0:
+        tags = tags.filter(category=category)
+
+    tags = tags.order_by('id')
+    
+    page_limit = 10
+    p = Paginator(tags, page_limit)
+    
+    try:
+        page = p.page(page_number)
+    except EmptyPage:
+        url = reverse('booru:tags_list') + '?tags={}&category={}'.format(searched_tag, category)
+        return redirect(url, page_number=1)
+    
+    tags_list = page.object_list
+    return render(request, 'booru/tag_list.html', {"tags": tags_list, "page": page, "form": form})
+
+@login_required
+@user_is_not_blocked
+def tag_edit(request, tag_id):
+    tag = get_object_or_404(PostTag, pk=tag_id)
+    tag_dict = model_to_dict(tag)
+
+    if tag.associated_user_id:
+        associated_user = get_object_or_404(Account.objects.active(), id=tag.associated_user_id)
+        tag_dict['associated_user_name'] = associated_user.slug
+
+    form = TagEditForm(request.POST or None, instance=tag, initial=tag_dict)
+    if form.is_valid() and request.POST:
+        tag = form.save(commit=False)
+        tag.author = request.user
+        if form.cleaned_data['associated_user_name']:
+            associated_user = get_object_or_404(Account.objects.active(), slug=form.cleaned_data['associated_user_name'])
+            tag.associated_user = associated_user
+        tag.save()
+        form.save_m2m()
+        return redirect('booru:tag_detail', tag.id)
+        
+    return render(request, 'booru/tag_edit.html', {"tag": tag, "form": form})
+
+@user_is_not_blocked
+def tag_detail(request, tag_id):
+    tag = get_object_or_404(PostTag, pk=tag_id)
+    last_posts = Post.objects.filter(tags__name__in=[tag.name])[:6]
+    return render(request, 'booru/tag_detail.html', {"tag": tag, "last_post": last_posts})
+
+@user_is_not_blocked
+def tag_history(request, tag_id, page_number = 1):
+    tag = get_object_or_404(PostTag, pk=tag_id)
+    page_limit = 20
+
+    p = Paginator(tag.history.all(), page_limit)
+    page = p.page(page_number)
+    return render(request, 'booru/tag_history.html', {"page": page, "tag": tag})
+
+class TagDelete(DeleteView):
+    model = PostTag
+    success_url = reverse_lazy('booru:tags_list')
+    template_name = 'booru/tag_confirm_delete.html'
+
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated or not has_permission(request.user, 'manage_tags'):
+            return redirect('account:login')
+        return super().dispatch(request, *args, **kwargs)
+
+@user_is_not_blocked
+def tag_revision_diff(request, tag_id):
+    tag = get_object_or_404(PostTag, pk=tag_id)
+
+    old_version = tag.history.filter(history_id=request.GET.get('oldRevision')).first()
+    new_version = tag.history.filter(history_id=request.GET.get('newRevision')).first()
+
+    delta = new_version.diff_against(old_version)
+
+    context = {"tag": tag, "changes": delta.changes,
+               "old_version": old_version, "new_version": new_version}
+    
+    return render(request, 'booru/tag_revision_diff.html', context)
+
+class ImplicationListView(generic.ListView):
+    model = Implication
+    paginate_by = 20
+
+    def get_queryset(self):
+        queryset = Implication.objects.all()
+
+        if self.request.GET.get('name'):
+            queryset = queryset.filter( Q(from_tag__name=self.request.GET.get('name'))|
+                                        Q(to_tag__name=self.request.GET.get('name')))
+        
+        status = self.request.GET.get('status')
+        if status:
+            try:
+                status = int(status)
+                queryset = queryset.filter(status=status)
+            except ValueError:
+                pass
+        return queryset
+
+    def get_context_data(self, **kwargs):
+        context = super(ImplicationListView, self).get_context_data(**kwargs)
+        context['form'] = ImplicationFilterForm(self.request.GET)
+        return context
+    
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        return super().dispatch(request, *args, **kwargs)
+
+class ImplicationDetailView(generic.DetailView):
+    model = Implication
+
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        return super().dispatch(request, *args, **kwargs)
+
+@login_required
+@user_is_not_blocked
+def implication_create(request):
+    form = ImplicationCreateForm(data=request.POST)
+    
+    if form.is_valid():
+        from_tag_name = form.cleaned_data['from_tag']
+        to_tag_name = form.cleaned_data['to_tag']
+
+        from_tag, from_tag_created = PostTag.objects.get_or_create(name=from_tag_name)
+        to_tag, from_tag_created = PostTag.objects.get_or_create(name=to_tag_name)
+
+        implication, implication_created = Implication.objects.get_or_create(from_tag=from_tag, to_tag=to_tag)
+        implication.author = request.user
+        implication.save()
+        return redirect('booru:implication-detail', implication.id)
+
+    return render(request, 'booru/implication_create.html', { "form": form })
+
+@staff_member_required
+@user_is_not_blocked
+def implication_approve(request, implication_id):
+    implication = Implication.objects.get(id=implication_id)
+
+    if implication.status != 1:
+        implication.status = 1
+        implication.approver = request.user
+        implication.save()
+    
+    utils.verify_and_perform_implications(implication.from_tag)
+    return redirect('booru:implication-detail', implication.id)
+
+@staff_member_required
+@user_is_not_blocked
+def implication_disapprove(request, implication_id):
+    implication = Implication.objects.get(id=implication_id)
+    implication.status = 2
+    implication.save()
+    return redirect('booru:implication-detail', implication.id)
+
+@staff_member_required
+@user_is_not_blocked
+def staff_page(request):
+    Account = apps.get_model('account', 'Account')
+    accounts = Account.objects.active().order_by("-id")
+
+    context = {
+        'accounts': accounts
+    }
+
+    return render(request, 'booru/staff_page.html', context)
+
+@user_is_not_blocked
+def tag_search(request):
+    term = request.GET.get("term", "")
+    operator = ""
+    value = term
+
+    if term.startswith("-") or term.startswith("~"):
+        operator = term[0]
+        value = term[1:]
+
+    tag_results = PostTag.objects.filter(Q(name__istartswith=value) | Q(aliases__name__istartswith=value)).distinct()
+    tag_results = tag_results[:10]
+
+    results = []
+    for tag in tag_results:
+        name = operator + tag.name
+        if tag.name.startswith(value):
+            results.append({'id': tag.pk, 'label': name, 'value': name})
+        else:
+            results.append({'id': tag.pk, 'label': "{} ({})".format(name, term), 'value': name})
+    return HttpResponse(json.dumps(results), content_type='application/json')
+
+@user_is_not_blocked
+def post_approve(request, post_id):
+    post = Post.objects.get(id=post_id)
+
+    if has_permission(request.user, "change_status") and post.status != 1:
+        post.status = 1
+        post.save()
+    return redirect('booru:post_detail', post_id=post.id)
+
+@user_is_not_blocked
+def post_hide(request, post_id):
+    post = Post.objects.get(id=post_id)
+
+    if has_permission(request.user, "change_status") and post.status != 2:
+        post.status = 2
+        post.save()
+    return redirect('booru:post_detail', post_id=post.id)
+
+@user_is_not_blocked
+def post_delete(request, post_id):
+    post = Post.objects.get(id=post_id)
+
+    if has_permission(request.user, "change_status") and post.status != 3:
+        post.status = 3
+        post.save()
+    return redirect('booru:post_detail', post_id=post.id)
+
+@login_required
+@user_is_not_blocked
+def post_favorite(request, post_id):
+    post = Post.objects.get(id=post_id)
+    favorite = Favorite.objects.filter(post=post, account=request.user).first()
+
+    if favorite:
+        favorite.delete()
+    else:
+        Favorite.objects.create(post=post, account=request.user)
+    
+    return redirect('booru:post_detail', post_id=post.id)
+
+@login_required
+@user_is_not_blocked
+def post_score_vote(request, post_id):
+    post = Post.objects.get(id=post_id)
+    score_vote = ScoreVote.objects.filter(post=post, account=request.user).first()
+
+    value = int(request.GET.get("point", 0))
+    if value > 1: value = 1
+    if value < -1: value = -1
+
+    if score_vote:
+        if score_vote.point == value:
+            score_vote.point = 0
+        else:
+            score_vote.point = value
+
+        score_vote.save()
+    else:
+        score_vote = ScoreVote.objects.create(post=post, account=request.user, point=value)
+    
+    results = {'value': score_vote.point, "current_points": post.get_score_count()}
+    return HttpResponse(json.dumps(results), content_type='application/json')
+
+@user_is_not_blocked
+def staff_mass_rename(request):
+    form = MassRenameForm(request.POST or None, request.FILES or None)
+
+    if has_permission(request.user, "mass_rename"):
+        if form.is_valid():
+            filter_by = form.cleaned_data['filter_by']
+            when = form.cleaned_data['when']
+            replace_with = form.cleaned_data['replace_with']
+
+            posts = utils.parse_and_filter_tags(filter_by)
+
+            when = utils.space_splitter(when)
+            replace_with = utils.space_splitter(replace_with)
+
+            posts = posts.filter(tags__name__in=when)
+
+            for post in posts:
+                post.tags.remove(*when)
+                post.tags.add(*replace_with)
+                post.save()
+                
+            return redirect('booru:staff_mass_rename')
+        return render(request, 'booru/staff_mass_rename.html', {"form": form})
+    return redirect('booru:index')
+
+@user_is_not_blocked
+def gallery_list(request, page_number = 1):
+    searched_gallery = request.GET.get("name", "")
+    form = GalleryListSearchForm(request.GET or None)
+
+    galleries = Gallery.objects.all().order_by('-id')
+    if searched_gallery != "":
+        galleries = galleries.filter(name__icontains=searched_gallery)
+    
+    page_limit = 10
+    p = Paginator(galleries, page_limit)
+    page = p.page(page_number)
+    gallery_list = page.object_list
+    
+    return render(request, 'booru/gallery_list.html', {"galleries": gallery_list, "page": page, "form": form})
+
+@user_is_not_blocked
+def gallery_history(request, gallery_id, page_number = 1):
+    gallery = get_object_or_404(Gallery, id=gallery_id)
+    page_limit = 20
+
+    p = Paginator(gallery.history.all(), page_limit)
+    page = p.page(page_number)
+
+    object_enum = enumerate(page.object_list)
+
+    return render(request, 'booru/gallery_history.html', {"page": page, "gallery": gallery})
+
+@login_required
+@user_is_not_blocked
+def gallery_edit(request, gallery_id):
+    gallery = get_object_or_404(Gallery, pk=gallery_id)
+
+    gallery_dict = model_to_dict(gallery)
+    gallery_dict['posts_ids'] = '\n'.join([str(post_id['id']) for post_id in gallery.posts.values('id')])
+    form = GalleryEditForm(request.POST or None, instance=gallery, initial=gallery_dict)
+
+    if form.is_valid():
+        posts_ids = form.cleaned_data['posts_ids'].splitlines()
+        gallery = form.save(commit=False)
+        gallery.posts.clear()
+        gallery.posts_mirror = " ".join(form.cleaned_data['posts_ids'].splitlines())
+        gallery.save()
+        posts = Post.objects.filter(id__in=posts_ids)
+        gallery.posts.add(*posts)
+        form.save_m2m()
+        return redirect('booru:gallery_detail', gallery_id=gallery.id)
+        
+    return render(request, 'booru/gallery_edit.html', {"form": form, "gallery": gallery})
+
+@login_required
+@user_is_not_blocked
+def gallery_create(request):    
+    form = GalleryCreateForm(request.POST or None, request.FILES or None)
+    
+    if form.is_valid():
+        posts_text = form.cleaned_data['posts_ids']
+        posts_ids = posts_text.splitlines()
+        
+        gallery = form.save(commit=False)
+        gallery.posts_mirror = " ".join(posts_ids)
+        gallery.save()
+        posts = Post.objects.filter(id__in=posts_ids)
+        gallery.posts.add(*posts)
+        form.save_m2m()
+        return redirect('booru:gallery_detail', gallery_id=gallery.id)
+    return render(request, 'booru/gallery_create.html', {"form": form})
+
+@user_is_not_blocked
+def gallery_detail(request, gallery_id):
+    page_number = int(request.GET.get('page', '1'))
+    page_limit = 20
+
+    gallery = Gallery.objects.get(id=gallery_id)
+    posts = gallery.posts.all()
+
+    p = Paginator(posts, page_limit)
+    page = p.page(page_number)
+
+    return render(request, 'booru/gallery_detail.html', {"gallery": gallery, "page": page})
+
+class StaffBanUser(FormView):
+    """
+    Provides a form for staff members to configure their booru.
+    """
+    success_url = '.'
+    form_class = BanUserForm
+    redirect_field_name = REDIRECT_FIELD_NAME
+    template_name = "booru/staff_user_tools.html"
+
+    def form_valid(self, form):
+        reason = form.cleaned_data['reason']
+        expiration = form.cleaned_data['expiration']
+        revoked = Privilege.objects.get(codename="can_login")
+        target_user = Account.objects.get(username=form.cleaned_data['username'])
+        author = self.request.user
+
+        if not has_role(target_user, 'administrator'): # Can't ban admins
+            if (has_role(target_user, 'moderator') and has_permission(request.user, 'booru.ban_mod')
+                or not has_role(target_user, 'moderator')):
+                instance = Timeout.objects.create(  author=author, target_user=target_user, 
+                                                    expiration=expiration, reason=reason)
+                instance.revoked.add(revoked)
+        return super().form_valid(form)
+
+    @method_decorator(csrf_protect)
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated or not has_permission(request.user, 'booru.ban_user'):
+            return redirect('account:login')
+        return super().dispatch(request, *args, **kwargs)
+
+class SiteConfigurationView(FormView):
+    """
+    Provides a form for staff members to configure their booru.
+    """
+    success_url = '.'
+    form_class = SiteConfigurationForm
+    redirect_field_name = REDIRECT_FIELD_NAME
+    template_name = "booru/staff_site_configuration.html"
+
+    def get_initial(self):
+        """
+        Returns the initial data to use for forms on this view.
+        """
+        initial = super().get_initial()
+
+        initial['site_title'] = Configuration.objects.get(code_name='site_title').value
+        initial['site_description'] = Configuration.objects.get(code_name='site_description').value
+        initial['terms_of_service'] = Configuration.objects.get(code_name='terms_of_service').value
+        initial['privacy_policy'] = Configuration.objects.get(code_name='privacy_policy').value
+        initial['announcement'] = Configuration.objects.get(code_name='announcement').value
+        initial['welcome_page'] = bool(int(Configuration.objects.get(code_name='welcome_page').value))
+        return initial
+
+    def form_valid(self, form):
+        site_title = Configuration.objects.get(code_name='site_title')
+        site_title.value = form.cleaned_data.get('site_title')
+        site_title.save()
+
+        site_description = Configuration.objects.get(code_name='site_description')
+        site_description.value = form.cleaned_data.get('site_description')
+        site_description.save()
+
+        terms_of_service = Configuration.objects.get(code_name='terms_of_service')
+        terms_of_service.value = form.cleaned_data.get('terms_of_service')
+        terms_of_service.save()
+
+        privacy_policy = Configuration.objects.get(code_name='privacy_policy')
+        privacy_policy.value = form.cleaned_data.get('privacy_policy')
+        privacy_policy.save()
+
+        announcement = Configuration.objects.get(code_name='announcement')
+        announcement.value = form.cleaned_data.get('announcement')
+        announcement.save()
+
+        welcome_page = Configuration.objects.get(code_name='welcome_page')
+        welcome_page.value = int(form.cleaned_data.get('welcome_page') == True)
+        welcome_page.save()
+
+        return super().form_valid(form)
+
+    @method_decorator(csrf_protect)
+    @user_is_not_blocked
+    def dispatch(self, request, *args, **kwargs):
+        if not request.user.is_authenticated or not has_permission(request.user,'change_configurations'):
+            return redirect('account:login')
+
+        return super().dispatch(request, *args, **kwargs)
```

### Comparing `Boorunaut-0.4.3/setup.py` & `Boorunaut-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import os, io
-from setuptools import find_packages, setup
-
-BASE_DIR = os.path.join(os.path.dirname(__file__))
-
-with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
-    README = readme.read()
-
-with io.open(os.path.join(BASE_DIR, 'requirements.txt'), encoding='utf-8') as fh:
-    REQUIREMENTS = fh.read()
-
-# allow setup.py to be run from any path
-os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-
-setup(
-    name='Boorunaut',
-    version='0.4.3',
-    packages=find_packages(),
-    include_package_data=True,
-    license='MIT License',
-    description='A taggable imageboard built in Django.',
-    long_description=README,
-    long_description_content_type='text/markdown',
-    url='https://github.com/Boorunaut/Boorunaut',
-    author='Luk3M, NogardRyuu',
-    author_email='luk3@hotmail.com.br, thiago_dragon_@hotmail.com',
-    entry_points={'console_scripts': [
-        'boorunaut=booru.setup.start_project:main',
-    ]},
-    classifiers=[
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Internet :: WWW/HTTP',
-        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
-    ],
-    install_requires=REQUIREMENTS,
+import os, io
+from setuptools import find_packages, setup
+
+BASE_DIR = os.path.join(os.path.dirname(__file__))
+
+with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
+    README = readme.read()
+
+with io.open(os.path.join(BASE_DIR, 'requirements.txt'), encoding='utf-8') as fh:
+    REQUIREMENTS = fh.read()
+
+# allow setup.py to be run from any path
+os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
+
+setup(
+    name='Boorunaut',
+    version='0.5.0',
+    packages=find_packages(),
+    include_package_data=True,
+    license='MIT License',
+    description='A taggable imageboard built in Django.',
+    long_description=README,
+    long_description_content_type='text/markdown',
+    url='https://github.com/Boorunaut/Boorunaut',
+    author='LucasCTN, ThiagoCamposTN',
+    author_email='lucascampostn@gmail.com, thiagocampostn@gmail.com',
+    entry_points={'console_scripts': [
+        'boorunaut=booru.setup.start_project:main',
+    ]},
+    classifiers=[
+        'Environment :: Web Environment',
+        'Framework :: Django',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Topic :: Internet :: WWW/HTTP',
+        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
+    ],
+    install_requires=REQUIREMENTS,
 )
```

