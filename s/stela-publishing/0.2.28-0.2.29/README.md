# Comparing `tmp/stela_publishing-0.2.28.tar.gz` & `tmp/stela_publishing-0.2.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stela_publishing-0.2.28.tar", last modified: Tue Apr 23 17:35:08 2024, max compression
+gzip compressed data, was "stela_publishing-0.2.29.tar", last modified: Tue Apr 23 17:43:17 2024, max compression
```

## Comparing `stela_publishing-0.2.28.tar` & `stela_publishing-0.2.29.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.920922 stela_publishing-0.2.28/
--rw-rw-rw-   0        0        0    35803 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/LICENSE
--rw-rw-rw-   0        0        0      133 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/MANIFEST.in
--rw-rw-rw-   0        0        0     3241 2024-04-23 17:35:08.887313 stela_publishing-0.2.28/PKG-INFO
--rw-rw-rw-   0        0        0     2058 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.005783 stela_publishing-0.2.28/accounts/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/admin.py
--rw-rw-rw-   0        0        0      154 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/apps.py
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/forms.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.013333 stela_publishing-0.2.28/accounts/migrations/
--rw-rw-rw-   0        0        0     4062 2024-01-29 16:48:12.000000 stela_publishing-0.2.28/accounts/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:12.000000 stela_publishing-0.2.28/accounts/migrations/__init__.py
--rw-rw-rw-   0        0        0     4733 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/tests.py
--rw-rw-rw-   0        0        0      370 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/token.py
--rw-rw-rw-   0        0        0     1836 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/urls.py
--rw-rw-rw-   0        0        0    10979 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/accounts/views.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.079735 stela_publishing-0.2.28/cloud/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/cloud/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/cloud/admin.py
--rw-rw-rw-   0        0        0      148 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/cloud/apps.py
--rw-rw-rw-   0        0        0     3456 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/cloud/cart.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.085886 stela_publishing-0.2.28/cloud/migrations/
--rw-rw-rw-   0        0        0     5564 2024-01-29 16:48:24.000000 stela_publishing-0.2.28/cloud/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:24.000000 stela_publishing-0.2.28/cloud/migrations/__init__.py
--rw-rw-rw-   0        0        0     3508 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/cloud/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/cloud/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/cloud/views.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.106083 stela_publishing-0.2.28/geolocation/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/geolocation/__init__.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/geolocation/admin.py
--rw-rw-rw-   0        0        0      160 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/geolocation/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.113080 stela_publishing-0.2.28/geolocation/migrations/
--rw-rw-rw-   0        0        0     6403 2024-01-29 16:48:36.000000 stela_publishing-0.2.28/geolocation/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:36.000000 stela_publishing-0.2.28/geolocation/migrations/__init__.py
--rw-rw-rw-   0        0        0      582 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/geolocation/models.py
--rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/geolocation/tests.py
--rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.28/geolocation/views.py
--rw-rw-rw-   0        0        0       42 2024-04-23 17:35:08.920922 stela_publishing-0.2.28/setup.cfg
--rw-rw-rw-   0        0        0     1394 2024-04-23 17:34:32.000000 stela_publishing-0.2.28/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.398901 stela_publishing-0.2.28/stela_control/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/__init__.py
--rw-rw-rw-   0        0        0       34 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/admin.py
--rw-rw-rw-   0        0        0      163 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/apps.py
--rw-rw-rw-   0        0        0     7541 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/cart.py
--rw-rw-rw-   0        0        0      164 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/context_processors.py
--rw-rw-rw-   0        0        0      316 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/cron.py
--rw-rw-rw-   0        0        0    74694 2024-04-23 17:02:31.000000 stela_publishing-0.2.28/stela_control/forms.py
--rw-rw-rw-   0        0        0      181 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.188693 stela_publishing-0.2.28/stela_control/locale/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.188693 stela_publishing-0.2.28/stela_control/locale/es/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.581730 stela_publishing-0.2.28/stela_control/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0    59691 2024-02-12 17:42:58.000000 stela_publishing-0.2.28/stela_control/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0   376901 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:50.845051 stela_publishing-0.2.28/stela_control/migrations/
--rw-rw-rw-   0        0        0    85798 2024-01-29 16:48:50.000000 stela_publishing-0.2.28/stela_control/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     7914 2024-02-07 18:48:34.000000 stela_publishing-0.2.28/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py
--rw-rw-rw-   0        0        0     7300 2024-02-10 15:04:52.000000 stela_publishing-0.2.28/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py
--rw-rw-rw-   0        0        0     6916 2024-02-10 16:34:10.000000 stela_publishing-0.2.28/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     5651 2024-02-10 16:49:33.000000 stela_publishing-0.2.28/stela_control/migrations/0005_rename_description_team_content_and_more.py
--rw-rw-rw-   0        0        0     6881 2024-02-13 00:43:29.000000 stela_publishing-0.2.28/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6174 2024-02-13 00:46:55.000000 stela_publishing-0.2.28/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6925 2024-02-20 21:45:50.000000 stela_publishing-0.2.28/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6664 2024-02-26 16:53:17.000000 stela_publishing-0.2.28/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5955 2024-02-28 16:33:58.000000 stela_publishing-0.2.28/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6006 2024-02-28 16:39:48.000000 stela_publishing-0.2.28/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6714 2024-02-28 16:47:02.000000 stela_publishing-0.2.28/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6809 2024-02-28 16:55:43.000000 stela_publishing-0.2.28/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5972 2024-02-28 17:37:52.000000 stela_publishing-0.2.28/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     6686 2024-02-28 19:01:16.000000 stela_publishing-0.2.28/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
--rw-rw-rw-   0        0        0     5617 2024-02-28 19:16:55.000000 stela_publishing-0.2.28/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6432 2024-02-28 19:17:57.000000 stela_publishing-0.2.28/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     7209 2024-04-23 16:47:22.000000 stela_publishing-0.2.28/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py
--rw-rw-rw-   0        0        0     6726 2024-04-23 17:33:11.000000 stela_publishing-0.2.28/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py
--rw-rw-rw-   0        0        0        0 2024-01-29 16:48:50.000000 stela_publishing-0.2.28/stela_control/migrations/__init__.py
--rw-rw-rw-   0        0        0    68561 2024-04-23 17:32:02.000000 stela_publishing-0.2.28/stela_control/models.py
--rw-rw-rw-   0        0        0     2943 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/routers.py
--rw-rw-rw-   0        0        0   144613 2024-04-20 17:01:45.000000 stela_publishing-0.2.28/stela_control/superfunctions.py
--rw-rw-rw-   0        0        0      410 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/tasks.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.215787 stela_publishing-0.2.28/stela_control/templates/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:53.360702 stela_publishing-0.2.28/stela_control/templates/stela_control/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:53.458228 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/
--rw-rw-rw-   0        0        0      497 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/base.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:53.748595 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/registration/
--rw-rw-rw-   0        0        0      227 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
--rw-rw-rw-   0        0        0       21 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
--rw-rw-rw-   0        0        0     1373 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
--rw-rw-rw-   0        0        0     3071 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/registration/register.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:54.033963 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/
--rw-rw-rw-   0        0        0     1364 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/delete_user.html
--rw-rw-rw-   0        0        0     2813 2024-02-04 17:29:27.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/login.html
--rw-rw-rw-   0        0        0     2692 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
--rw-rw-rw-   0        0        0     2043 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_done.html
--rw-rw-rw-   0        0        0      629 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_email.html
--rw-rw-rw-   0        0        0     2424 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:54.218847 stela_publishing-0.2.28/stela_control/templates/stela_control/analytics/
--rw-rw-rw-   0        0        0      757 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/analytics/analytics.html
--rw-rw-rw-   0        0        0      527 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/analytics/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:54.283362 stela_publishing-0.2.28/stela_control/templates/stela_control/api/
--rw-rw-rw-   0        0        0     5932 2024-01-15 04:03:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/api/main.html
--rw-rw-rw-   0        0        0     2817 2024-02-13 00:06:24.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/base.html
--rw-rw-rw-   0        0        0     4402 2024-02-07 14:19:14.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/base_content.html
--rw-rw-rw-   0        0        0     6768 2024-02-07 14:19:37.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/base_list.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:54.378303 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/
--rw-rw-rw-   0        0        0   240584 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/homebrew.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:58.171949 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/
--rw-rw-rw-   0        0        0     2186 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
--rw-rw-rw-   0        0        0    30854 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/checkout.html
--rw-rw-rw-   0        0        0      906 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/data-customer.html
--rw-rw-rw-   0        0        0    56802 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/invoice-copy.html
--rw-rw-rw-   0        0        0    56693 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/invoice.html
--rw-rw-rw-   0        0        0     2875 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/order-placed.html
--rw-rw-rw-   0        0        0    48008 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/preview-recipt.html
--rw-rw-rw-   0        0        0     2750 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
--rw-rw-rw-   0        0        0     3336 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/recipt-detail.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:58.342984 stela_publishing-0.2.28/stela_control/templates/stela_control/chatstela/
--rw-rw-rw-   0        0        0    30842 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/chatstela/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:58.845953 stela_publishing-0.2.28/stela_control/templates/stela_control/content/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.038470 stela_publishing-0.2.28/stela_control/templates/stela_control/content/comments/
--rw-rw-rw-   0        0        0     7574 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/content/comments/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.156124 stela_publishing-0.2.28/stela_control/templates/stela_control/content/docs/
--rw-rw-rw-   0        0        0    15755 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/content/docs/main.html
--rw-rw-rw-   0        0        0     7448 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/content/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.230506 stela_publishing-0.2.28/stela_control/templates/stela_control/content/main/
--rw-rw-rw-   0        0        0     1003 2024-02-28 11:49:02.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/content/main/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.312986 stela_publishing-0.2.28/stela_control/templates/stela_control/content/staff/
--rw-rw-rw-   0        0        0     7608 2024-02-10 16:45:07.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/content/staff/index.html
--rw-rw-rw-   0        0        0    26830 2024-02-23 18:59:08.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/content/stelastory.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.454491 stela_publishing-0.2.28/stela_control/templates/stela_control/developer/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.778638 stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/
--rw-rw-rw-   0        0        0      933 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal1.html
--rw-rw-rw-   0        0        0      898 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal2.html
--rw-rw-rw-   0        0        0      900 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal3.html
--rw-rw-rw-   0        0        0      875 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal4.html
--rw-rw-rw-   0        0        0    46793 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/developer/home.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.366633 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.840910 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/accounts/
--rw-rw-rw-   0        0        0      413 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:59.918751 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/billing/
--rw-rw-rw-   0        0        0    21938 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
--rw-rw-rw-   0        0        0    21903 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/billing/invoice.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:00.205109 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/
--rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/message_notification.html
--rw-rw-rw-   0        0        0    29872 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/message_response.html
--rw-rw-rw-   0        0        0     8454 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/support_notification.html
--rw-rw-rw-   0        0        0    21428 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/update_support.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:00.263193 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/marketing/
--rw-rw-rw-   0        0        0    60992 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:00.332014 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/newsletter/
--rw-rw-rw-   0        0        0    21461 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
--rw-rw-rw-   0        0        0    21883 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/newsletter/success.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:00.516566 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/
--rw-rw-rw-   0        0        0    10226 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
--rw-rw-rw-   0        0        0    10337 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html
--rw-rw-rw-   0        0        0    57366 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html
--rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html
--rw-rw-rw-   0        0        0    57320 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html
--rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:00.826007 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/
--rw-rw-rw-   0        0        0    27770 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
--rw-rw-rw-   0        0        0     6930 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/charges.html
--rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
--rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
--rw-rw-rw-   0        0        0     7266 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
--rw-rw-rw-   0        0        0     7166 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:00.906951 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/support/
--rw-rw-rw-   0        0        0    20072 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/support/support_notification.html
--rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/support/support_response.html
--rw-rw-rw-   0        0        0    22210 2024-02-23 18:58:52.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/home.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:00.945299 stela_publishing-0.2.28/stela_control/templates/stela_control/inbox/
--rw-rw-rw-   0        0        0     7530 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/inbox/index.html
--rw-rw-rw-   0        0        0     8900 2024-02-10 15:38:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.407398 stela_publishing-0.2.28/stela_control/templates/stela_control/inventory/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:01.049412 stela_publishing-0.2.28/stela_control/templates/stela_control/inventory/journals/
--rw-rw-rw-   0        0        0     6289 2024-02-08 17:58:31.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/inventory/journals/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:01.433144 stela_publishing-0.2.28/stela_control/templates/stela_control/inventory/publishing/
--rw-rw-rw-   0        0        0     6897 2024-02-26 22:43:48.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/inventory/publishing/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.117184 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.128178 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutemmerut/
--rw-rw-rw-   0        0        0     1694 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.162892 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutsecondary/
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.176194 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutstela/
--rw-rw-rw-   0        0        0     1381 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.188189 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/appstela/
--rw-rw-rw-   0        0        0     1806 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/appstela/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.544563 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.206218 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/pw_reset/
--rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
--rw-rw-rw-   0        0        0      171 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.249239 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/signup/
--rw-rw-rw-   0        0        0      794 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
--rw-rw-rw-   0        0        0      269 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
--rw-rw-rw-   0        0        0     3005 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/blog-feed.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.276896 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/categories/
--rw-rw-rw-   0        0        0      834 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/categories/modal4.html
--rw-rw-rw-   0        0        0      826 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/chatbox.html
--rw-rw-rw-   0        0        0      925 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/chatbox2.html
--rw-rw-rw-   0        0        0      143 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/city_data.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.363899 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/colors/
--rw-rw-rw-   0        0        0      857 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/colors/modal2.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.399498 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/contact/
--rw-rw-rw-   0        0        0     1606 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/contact/modal.html
--rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/dynamic-formset.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.413494 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutfooter/
--rw-rw-rw-   0        0        0     2233 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.500138 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutservices/
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
--rw-rw-rw-   0        0        0      841 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/form-base.html
--rw-rw-rw-   0        0        0       64 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/form-errors.html
--rw-rw-rw-   0        0        0       45 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/form.html
--rw-rw-rw-   0        0        0      924 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/formset-base-services.html
--rw-rw-rw-   0        0        0     1790 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/formset-base.html
--rw-rw-rw-   0        0        0      816 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/formset.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.580366 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/handlers/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.558504 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/handlers/blog/
--rw-rw-rw-   0        0        0     1488 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html
--rw-rw-rw-   0        0        0      128 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
--rw-rw-rw-   0        0        0      265 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/handlers/blog/empy-blog.html
--rw-rw-rw-   0        0        0      103 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/hashtags.html
--rw-rw-rw-   0        0        0      587 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/instagram-alert.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.665824 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/inventory/
--rw-rw-rw-   0        0        0     2029 2024-02-27 00:20:27.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
--rw-rw-rw-   0        0        0      777 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/inventory/simple-form.html
--rw-rw-rw-   0        0        0     1578 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/inventory/simple-formset.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.704359 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/job-application/
--rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:02.736357 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/linkzoneupdates/
--rw-rw-rw-   0        0        0      848 2024-01-15 04:03:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.603376 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:03.710131 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/
--rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2477 2024-02-23 18:05:57.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:06:42.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.031435 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/
--rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
--rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2737 2024-02-23 18:05:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
--rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
--rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.518076 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/
--rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
--rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
--rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
--rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
--rw-rw-rw-   0        0        0     2815 2024-02-23 18:07:00.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
--rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
--rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
--rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
--rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
--rw-rw-rw-   0        0        0     2489 2024-02-23 18:07:28.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
--rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
--rw-rw-rw-   0        0        0     2803 2024-02-23 18:07:38.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.666087 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.682053 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/community/
--rw-rw-rw-   0        0        0      818 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/community/formdata.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.691051 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/content-pro-media/
--rw-rw-rw-   0        0        0     3209 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.720032 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/content-pro-update/
--rw-rw-rw-   0        0        0       83 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
--rw-rw-rw-   0        0        0       84 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
--rw-rw-rw-   0        0        0      986 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.737022 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ic-update/
--rw-rw-rw-   0        0        0      469 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
--rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.937782 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/
--rw-rw-rw-   0        0        0    25077 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
--rw-rw-rw-   0        0        0     1667 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
--rw-rw-rw-   0        0        0     1530 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
--rw-rw-rw-   0        0        0     1849 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
--rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
--rw-rw-rw-   0        0        0     4485 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
--rw-rw-rw-   0        0        0     5787 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:04.955769 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/meta-assets/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
--rw-rw-rw-   0        0        0      628 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.047997 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/page-analythics/
--rw-rw-rw-   0        0        0     1755 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
--rw-rw-rw-   0        0        0     1960 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
--rw-rw-rw-   0        0        0     1428 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.061984 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/smart-boost/
--rw-rw-rw-   0        0        0     2129 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.075977 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/stela-sight/
--rw-rw-rw-   0        0        0      268 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.092331 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/newcomer/
--rw-rw-rw-   0        0        0     3796 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/newcomer/form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.125731 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/post/
--rw-rw-rw-   0        0        0      846 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/post/list-modal.html
--rw-rw-rw-   0        0        0      850 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/post/main-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.183396 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/
--rw-rw-rw-   0        0        0     1824 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/catalog-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.469034 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/
--rw-rw-rw-   0        0        0      933 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
--rw-rw-rw-   0        0        0      872 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/category-form.html
--rw-rw-rw-   0        0        0      888 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/color-form.html
--rw-rw-rw-   0        0        0     1024 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/product-form.html
--rw-rw-rw-   0        0        0      855 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/size-form.html
--rw-rw-rw-   0        0        0      115 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/variant-form.html
--rw-rw-rw-   0        0        0      805 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/product-modal.html
--rw-rw-rw-   0        0        0      848 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/size-modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.571207 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/
--rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
--rw-rw-rw-   0        0        0      287 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/category-form.html
--rw-rw-rw-   0        0        0      230 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/color-form.html
--rw-rw-rw-   0        0        0     1008 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/product-form.html
--rw-rw-rw-   0        0        0      228 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/size-form.html
--rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/variant-form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.593333 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/profile/
--rw-rw-rw-   0        0        0     1306 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
--rw-rw-rw-   0        0        0      200 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/profile/single-form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.604325 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/projects/
--rw-rw-rw-   0        0        0     1698 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/projects/modal.html
--rw-rw-rw-   0        0        0      260 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/remove-complete.html
--rw-rw-rw-   0        0        0      212 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/single-form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.800747 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.628310 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.664287 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_forms/
--rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.731799 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/forms/
--rw-rw-rw-   0        0        0     1269 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
--rw-rw-rw-   0        0        0     1097 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
--rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.754784 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/update_forms/
--rw-rw-rw-   0        0        0     1156 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
--rw-rw-rw-   0        0        0     1320 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.768558 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/staff/
--rw-rw-rw-   0        0        0     1947 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/staff/form.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.815832 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stela_story/
--rw-rw-rw-   0        0        0     3404 2024-02-21 12:50:07.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
--rw-rw-rw-   0        0        0     2001 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.826779 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelafooter/
--rw-rw-rw-   0        0        0     2176 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelafooter/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.925758 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelamedia/
--rw-rw-rw-   0        0        0     1695 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelamedia/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.942369 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelapath/
--rw-rw-rw-   0        0        0     1337 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelapath/modal.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:05.998400 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/youtube/
--rw-rw-rw-   0        0        0      157 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/youtube/video-preview.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.811744 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:06.125753 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/
--rw-rw-rw-   0        0        0     2345 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
--rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html
--rw-rw-rw-   0        0        0     1917 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/new_email.html
--rw-rw-rw-   0        0        0      976 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/update_email.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:06.306210 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/
--rw-rw-rw-   0        0        0    10789 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:49.837724 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:06.920828 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
--rw-rw-rw-   0        0        0    13445 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:07.227429 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
--rw-rw-rw-   0        0        0    23333 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:07.306091 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
--rw-rw-rw-   0        0        0    34272 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:07.386050 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:07.476272 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/community/
--rw-rw-rw-   0        0        0    14156 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:07.638438 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
--rw-rw-rw-   0        0        0    30243 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
--rw-rw-rw-   0        0        0      248 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:07.706923 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
--rw-rw-rw-   0        0        0     3162 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
--rw-rw-rw-   0        0        0    12633 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
--rw-rw-rw-   0        0        0    17640 2024-02-12 17:40:18.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/newcomer.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:07.925011 stela_publishing-0.2.28/stela_control/templates/stela_control/orders/
--rw-rw-rw-   0        0        0     6171 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/orders/list_view.html
--rw-rw-rw-   0        0        0     8860 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/orders/order_update.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.184386 stela_publishing-0.2.28/stela_control/templates/stela_control/payments/
--rw-rw-rw-   0        0        0    43167 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/payments/homebrew.html
--rw-rw-rw-   0        0        0     2687 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/payments/register-wallet.html
--rw-rw-rw-   0        0        0     4322 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/payments/wallet-list.html
--rw-rw-rw-   0        0        0     2831 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/payments/withdraw.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.200260 stela_publishing-0.2.28/stela_control/templates/stela_control/prostela/
--rw-rw-rw-   0        0        0      153 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/prostela/chatbox.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.211254 stela_publishing-0.2.28/stela_control/templates/stela_control/prostela-expert/
--rw-rw-rw-   0        0        0    34014 2024-01-15 04:03:12.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/prostela-expert/index.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.323316 stela_publishing-0.2.28/stela_control/templates/stela_control/reviews/
--rw-rw-rw-   0        0        0     3170 2024-01-15 04:03:13.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/reviews/reviews_list.html
--rw-rw-rw-   0        0        0     1325 2024-01-15 04:03:13.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/reviews/update_review.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.346172 stela_publishing-0.2.28/stela_control/templates/stela_control/support/
--rw-rw-rw-   0        0        0     2061 2024-01-15 04:03:13.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/support/list.html
--rw-rw-rw-   0        0        0     7093 2024-01-15 04:03:13.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/support/update.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.732803 stela_publishing-0.2.28/stela_control/templates/stela_control/users/
--rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/users/generic-user-handler.html
--rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/users/profile.html
--rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/users/users-control.html
--rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_publishing-0.2.28/stela_control/templates/stela_control/users/users.html
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.837014 stela_publishing-0.2.28/stela_control/templatetags/
--rw-rw-rw-   0        0        0        0 2024-01-15 04:03:13.000000 stela_publishing-0.2.28/stela_control/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1277 2024-01-19 05:09:17.000000 stela_publishing-0.2.28/stela_control/templatetags/stelatags.py
--rw-rw-rw-   0        0        0      507 2024-01-15 04:03:13.000000 stela_publishing-0.2.28/stela_control/tests.py
--rw-rw-rw-   0        0        0     1131 2024-01-15 04:03:13.000000 stela_publishing-0.2.28/stela_control/tokenize.py
--rw-rw-rw-   0        0        0     5281 2024-02-20 00:45:02.000000 stela_publishing-0.2.28/stela_control/urls.py
--rw-rw-rw-   0        0        0   211317 2024-02-20 00:48:27.000000 stela_publishing-0.2.28/stela_control/views.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:35:08.882315 stela_publishing-0.2.28/stela_publishing.egg-info/
--rw-rw-rw-   0        0        0     3241 2024-04-23 17:34:47.000000 stela_publishing-0.2.28/stela_publishing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    20793 2024-04-23 17:34:47.000000 stela_publishing-0.2.28/stela_publishing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:34:47.000000 stela_publishing-0.2.28/stela_publishing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      355 2024-04-23 17:34:47.000000 stela_publishing-0.2.28/stela_publishing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2024-04-23 17:34:47.000000 stela_publishing-0.2.28/stela_publishing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:17.247522 stela_publishing-0.2.29/
+-rw-rw-rw-   0        0        0    35803 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/LICENSE
+-rw-rw-rw-   0        0        0      133 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/MANIFEST.in
+-rw-rw-rw-   0        0        0     3241 2024-04-23 17:43:17.244523 stela_publishing-0.2.29/PKG-INFO
+-rw-rw-rw-   0        0        0     2058 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.207257 stela_publishing-0.2.29/accounts/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/admin.py
+-rw-rw-rw-   0        0        0      154 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/apps.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/forms.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.233817 stela_publishing-0.2.29/accounts/migrations/
+-rw-rw-rw-   0        0        0     4062 2024-01-29 16:48:12.000000 stela_publishing-0.2.29/accounts/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:12.000000 stela_publishing-0.2.29/accounts/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4733 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/tests.py
+-rw-rw-rw-   0        0        0      370 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/token.py
+-rw-rw-rw-   0        0        0     1836 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/urls.py
+-rw-rw-rw-   0        0        0    10979 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/accounts/views.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.253809 stela_publishing-0.2.29/cloud/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/cloud/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/cloud/admin.py
+-rw-rw-rw-   0        0        0      148 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/cloud/apps.py
+-rw-rw-rw-   0        0        0     3456 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/cloud/cart.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.292812 stela_publishing-0.2.29/cloud/migrations/
+-rw-rw-rw-   0        0        0     5564 2024-01-29 16:48:24.000000 stela_publishing-0.2.29/cloud/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:24.000000 stela_publishing-0.2.29/cloud/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/cloud/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/cloud/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/cloud/views.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.309610 stela_publishing-0.2.29/geolocation/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/geolocation/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/geolocation/admin.py
+-rw-rw-rw-   0        0        0      160 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/geolocation/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.324875 stela_publishing-0.2.29/geolocation/migrations/
+-rw-rw-rw-   0        0        0     6403 2024-01-29 16:48:36.000000 stela_publishing-0.2.29/geolocation/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:36.000000 stela_publishing-0.2.29/geolocation/migrations/__init__.py
+-rw-rw-rw-   0        0        0      582 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/geolocation/models.py
+-rw-rw-rw-   0        0        0       63 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/geolocation/tests.py
+-rw-rw-rw-   0        0        0       66 2024-01-15 04:03:09.000000 stela_publishing-0.2.29/geolocation/views.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 17:43:17.248520 stela_publishing-0.2.29/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2024-04-23 17:42:51.000000 stela_publishing-0.2.29/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.576386 stela_publishing-0.2.29/stela_control/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/__init__.py
+-rw-rw-rw-   0        0        0       34 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/admin.py
+-rw-rw-rw-   0        0        0      163 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/apps.py
+-rw-rw-rw-   0        0        0     7541 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/cart.py
+-rw-rw-rw-   0        0        0      164 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/context_processors.py
+-rw-rw-rw-   0        0        0      316 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/cron.py
+-rw-rw-rw-   0        0        0    74844 2024-04-23 17:42:35.000000 stela_publishing-0.2.29/stela_control/forms.py
+-rw-rw-rw-   0        0        0      181 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:07.939554 stela_publishing-0.2.29/stela_control/locale/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:07.940552 stela_publishing-0.2.29/stela_control/locale/es/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.612357 stela_publishing-0.2.29/stela_control/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    59691 2024-02-12 17:42:58.000000 stela_publishing-0.2.29/stela_control/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0   376901 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:09.859875 stela_publishing-0.2.29/stela_control/migrations/
+-rw-rw-rw-   0        0        0    85798 2024-01-29 16:48:50.000000 stela_publishing-0.2.29/stela_control/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     7914 2024-02-07 18:48:34.000000 stela_publishing-0.2.29/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py
+-rw-rw-rw-   0        0        0     7300 2024-02-10 15:04:52.000000 stela_publishing-0.2.29/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py
+-rw-rw-rw-   0        0        0     6916 2024-02-10 16:34:10.000000 stela_publishing-0.2.29/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     5651 2024-02-10 16:49:33.000000 stela_publishing-0.2.29/stela_control/migrations/0005_rename_description_team_content_and_more.py
+-rw-rw-rw-   0        0        0     6881 2024-02-13 00:43:29.000000 stela_publishing-0.2.29/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6174 2024-02-13 00:46:55.000000 stela_publishing-0.2.29/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6925 2024-02-20 21:45:50.000000 stela_publishing-0.2.29/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6664 2024-02-26 16:53:17.000000 stela_publishing-0.2.29/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5955 2024-02-28 16:33:58.000000 stela_publishing-0.2.29/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6006 2024-02-28 16:39:48.000000 stela_publishing-0.2.29/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6714 2024-02-28 16:47:02.000000 stela_publishing-0.2.29/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6809 2024-02-28 16:55:43.000000 stela_publishing-0.2.29/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5972 2024-02-28 17:37:52.000000 stela_publishing-0.2.29/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     6686 2024-02-28 19:01:16.000000 stela_publishing-0.2.29/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py
+-rw-rw-rw-   0        0        0     5617 2024-02-28 19:16:55.000000 stela_publishing-0.2.29/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6432 2024-02-28 19:17:57.000000 stela_publishing-0.2.29/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     7209 2024-04-23 16:47:22.000000 stela_publishing-0.2.29/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py
+-rw-rw-rw-   0        0        0     6726 2024-04-23 17:33:11.000000 stela_publishing-0.2.29/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-01-29 16:48:50.000000 stela_publishing-0.2.29/stela_control/migrations/__init__.py
+-rw-rw-rw-   0        0        0    68561 2024-04-23 17:32:02.000000 stela_publishing-0.2.29/stela_control/models.py
+-rw-rw-rw-   0        0        0     2943 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/routers.py
+-rw-rw-rw-   0        0        0   144613 2024-04-20 17:01:45.000000 stela_publishing-0.2.29/stela_control/superfunctions.py
+-rw-rw-rw-   0        0        0      410 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/tasks.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:07.942551 stela_publishing-0.2.29/stela_control/templates/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:10.176075 stela_publishing-0.2.29/stela_control/templates/stela_control/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:10.241604 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/
+-rw-rw-rw-   0        0        0      497 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/base.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:10.330551 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/registration/
+-rw-rw-rw-   0        0        0      227 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/registration/account_activation_email.html
+-rw-rw-rw-   0        0        0       21 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/registration/activation_invalid.html
+-rw-rw-rw-   0        0        0     1373 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/registration/confirmation_email.html
+-rw-rw-rw-   0        0        0     3071 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/registration/register.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:10.454087 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/
+-rw-rw-rw-   0        0        0     1364 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/delete_user.html
+-rw-rw-rw-   0        0        0     2813 2024-02-04 17:29:27.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/login.html
+-rw-rw-rw-   0        0        0     2692 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html
+-rw-rw-rw-   0        0        0     2043 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_done.html
+-rw-rw-rw-   0        0        0      629 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_email.html
+-rw-rw-rw-   0        0        0     2424 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:10.473073 stela_publishing-0.2.29/stela_control/templates/stela_control/analytics/
+-rw-rw-rw-   0        0        0      757 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/analytics/analytics.html
+-rw-rw-rw-   0        0        0      527 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/analytics/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:10.486067 stela_publishing-0.2.29/stela_control/templates/stela_control/api/
+-rw-rw-rw-   0        0        0     5932 2024-01-15 04:03:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/api/main.html
+-rw-rw-rw-   0        0        0     2817 2024-02-13 00:06:24.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/base.html
+-rw-rw-rw-   0        0        0     4402 2024-02-07 14:19:14.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/base_content.html
+-rw-rw-rw-   0        0        0     6768 2024-02-07 14:19:37.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/base_list.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:10.530039 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/
+-rw-rw-rw-   0        0        0   240584 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/homebrew.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.201865 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/
+-rw-rw-rw-   0        0        0     2186 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/bill-data-customer.html
+-rw-rw-rw-   0        0        0    30854 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/checkout.html
+-rw-rw-rw-   0        0        0      906 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/data-customer.html
+-rw-rw-rw-   0        0        0    56802 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/invoice-copy.html
+-rw-rw-rw-   0        0        0    56693 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/invoice.html
+-rw-rw-rw-   0        0        0     2875 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/order-placed.html
+-rw-rw-rw-   0        0        0    48008 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/preview-recipt.html
+-rw-rw-rw-   0        0        0     2750 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html
+-rw-rw-rw-   0        0        0     3336 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/recipt-detail.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.212857 stela_publishing-0.2.29/stela_control/templates/stela_control/chatstela/
+-rw-rw-rw-   0        0        0    30842 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/chatstela/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.310401 stela_publishing-0.2.29/stela_control/templates/stela_control/content/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.335145 stela_publishing-0.2.29/stela_control/templates/stela_control/content/comments/
+-rw-rw-rw-   0        0        0     7574 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/content/comments/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.391548 stela_publishing-0.2.29/stela_control/templates/stela_control/content/docs/
+-rw-rw-rw-   0        0        0    15755 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/content/docs/main.html
+-rw-rw-rw-   0        0        0     7448 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/content/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.431556 stela_publishing-0.2.29/stela_control/templates/stela_control/content/main/
+-rw-rw-rw-   0        0        0     1003 2024-02-28 11:49:02.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/content/main/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.449506 stela_publishing-0.2.29/stela_control/templates/stela_control/content/staff/
+-rw-rw-rw-   0        0        0     7608 2024-02-10 16:45:07.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/content/staff/index.html
+-rw-rw-rw-   0        0        0    26830 2024-02-23 18:59:08.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/content/stelastory.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.499475 stela_publishing-0.2.29/stela_control/templates/stela_control/developer/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.596416 stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/
+-rw-rw-rw-   0        0        0      933 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal1.html
+-rw-rw-rw-   0        0        0      898 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal2.html
+-rw-rw-rw-   0        0        0      900 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal3.html
+-rw-rw-rw-   0        0        0      875 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal4.html
+-rw-rw-rw-   0        0        0    46793 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/developer/home.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:07.962155 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.607410 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/accounts/
+-rw-rw-rw-   0        0        0      413 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/accounts/password_reset_email.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.654124 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/billing/
+-rw-rw-rw-   0        0        0    21938 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html
+-rw-rw-rw-   0        0        0    21903 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/billing/invoice.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.865381 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/
+-rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/message_notification.html
+-rw-rw-rw-   0        0        0    29872 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/message_response.html
+-rw-rw-rw-   0        0        0     8454 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/support_notification.html
+-rw-rw-rw-   0        0        0    21428 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/update_support.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:11.896363 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/marketing/
+-rw-rw-rw-   0        0        0    60992 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:12.001297 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/newsletter/
+-rw-rw-rw-   0        0        0    21461 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html
+-rw-rw-rw-   0        0        0    21883 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/newsletter/success.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:12.133240 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/
+-rw-rw-rw-   0        0        0    10226 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html
+-rw-rw-rw-   0        0        0    10337 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html
+-rw-rw-rw-   0        0        0    57366 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html
+-rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html
+-rw-rw-rw-   0        0        0    57320 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html
+-rw-rw-rw-   0        0        0    57419 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:12.302693 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/
+-rw-rw-rw-   0        0        0    27770 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/billing_payment.html
+-rw-rw-rw-   0        0        0     6930 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/charges.html
+-rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/payment_notification.html
+-rw-rw-rw-   0        0        0    20151 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/sale_notification.html
+-rw-rw-rw-   0        0        0     7266 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html
+-rw-rw-rw-   0        0        0     7166 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/withdrawals.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:12.346668 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/support/
+-rw-rw-rw-   0        0        0    20072 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/support/support_notification.html
+-rw-rw-rw-   0        0        0    20096 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/support/support_response.html
+-rw-rw-rw-   0        0        0    22210 2024-02-23 18:58:52.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/home.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:12.384642 stela_publishing-0.2.29/stela_control/templates/stela_control/inbox/
+-rw-rw-rw-   0        0        0     7530 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/inbox/index.html
+-rw-rw-rw-   0        0        0     8900 2024-02-10 15:38:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:07.965153 stela_publishing-0.2.29/stela_control/templates/stela_control/inventory/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:12.420300 stela_publishing-0.2.29/stela_control/templates/stela_control/inventory/journals/
+-rw-rw-rw-   0        0        0     6289 2024-02-08 17:58:31.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/inventory/journals/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:12.652158 stela_publishing-0.2.29/stela_control/templates/stela_control/inventory/publishing/
+-rw-rw-rw-   0        0        0     6897 2024-02-26 22:43:48.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/inventory/publishing/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.191157 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.206147 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutemmerut/
+-rw-rw-rw-   0        0        0     1694 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.256059 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutsecondary/
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.271049 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutstela/
+-rw-rw-rw-   0        0        0     1381 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.283043 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/appstela/
+-rw-rw-rw-   0        0        0     1806 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/appstela/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.012694 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.302030 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/pw_reset/
+-rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/pw_reset/form_errors.html
+-rw-rw-rw-   0        0        0      171 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/pw_reset/password_reset_form.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.318020 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/signup/
+-rw-rw-rw-   0        0        0      794 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html
+-rw-rw-rw-   0        0        0      269 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/signup/success_register.html
+-rw-rw-rw-   0        0        0     3005 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/blog-feed.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.323017 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/categories/
+-rw-rw-rw-   0        0        0      834 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/categories/modal4.html
+-rw-rw-rw-   0        0        0      826 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/chatbox.html
+-rw-rw-rw-   0        0        0      925 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/chatbox2.html
+-rw-rw-rw-   0        0        0      143 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/city_data.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.336010 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/colors/
+-rw-rw-rw-   0        0        0      857 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/colors/modal2.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.408256 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/contact/
+-rw-rw-rw-   0        0        0     1606 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/contact/modal.html
+-rw-rw-rw-   0        0        0     1638 2024-01-22 20:05:28.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/dynamic-formset.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.418793 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutfooter/
+-rw-rw-rw-   0        0        0     2233 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.453018 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutservices/
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html
+-rw-rw-rw-   0        0        0      841 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/form-base.html
+-rw-rw-rw-   0        0        0       64 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/form-errors.html
+-rw-rw-rw-   0        0        0       45 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/form.html
+-rw-rw-rw-   0        0        0      924 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/formset-base-services.html
+-rw-rw-rw-   0        0        0     1790 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/formset-base.html
+-rw-rw-rw-   0        0        0      816 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/formset.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.018643 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/handlers/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.499364 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/handlers/blog/
+-rw-rw-rw-   0        0        0     1488 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html
+-rw-rw-rw-   0        0        0      128 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/handlers/blog/empty-blog.html
+-rw-rw-rw-   0        0        0      265 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/handlers/blog/empy-blog.html
+-rw-rw-rw-   0        0        0      103 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/hashtags.html
+-rw-rw-rw-   0        0        0      587 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/instagram-alert.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.588307 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/inventory/
+-rw-rw-rw-   0        0        0     2029 2024-02-27 00:20:27.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html
+-rw-rw-rw-   0        0        0      777 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/inventory/simple-form.html
+-rw-rw-rw-   0        0        0     1578 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/inventory/simple-formset.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.605298 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/job-application/
+-rw-rw-rw-   0        0        0       45 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/job-application/error-form-v1.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:13.611294 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/linkzoneupdates/
+-rw-rw-rw-   0        0        0      848 2024-01-15 04:03:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.023640 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.002587 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/
+-rw-rw-rw-   0        0        0     1067 2024-02-23 15:58:42.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1467 2024-02-23 16:29:50.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1650 2024-02-23 18:05:44.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     2732 2024-02-23 18:06:01.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2477 2024-02-23 18:05:57.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:06.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     1712 2024-02-23 18:06:10.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2887 2024-02-23 18:06:18.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2593 2024-02-23 18:06:24.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2296 2024-02-23 18:06:30.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1639 2024-02-23 18:06:35.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:06:42.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.242464 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/
+-rw-rw-rw-   0        0        0     1614 2024-02-23 18:04:43.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3292 2024-02-23 18:04:45.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     3051 2024-02-23 18:04:50.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1936 2024-02-23 18:04:55.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2198 2024-02-23 18:05:01.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     2866 2024-02-23 18:05:07.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2737 2024-02-23 18:05:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2418 2024-02-23 18:05:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1412 2024-02-23 18:07:47.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:05:27.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html
+-rw-rw-rw-   0        0        0     1297 2024-02-23 15:56:06.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html
+-rw-rw-rw-   0        0        0     1778 2024-02-23 16:29:34.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.419566 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/
+-rw-rw-rw-   0        0        0     1069 2024-02-23 15:58:34.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html
+-rw-rw-rw-   0        0        0     1464 2024-02-23 16:29:44.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html
+-rw-rw-rw-   0        0        0     1962 2024-02-23 18:06:50.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html
+-rw-rw-rw-   0        0        0     3022 2024-02-23 18:06:54.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html
+-rw-rw-rw-   0        0        0     2815 2024-02-23 18:07:00.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html
+-rw-rw-rw-   0        0        0     1740 2024-02-23 18:07:07.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html
+-rw-rw-rw-   0        0        0     2080 2024-02-23 18:07:11.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html
+-rw-rw-rw-   0        0        0     3148 2024-02-23 18:07:16.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html
+-rw-rw-rw-   0        0        0     2631 2024-02-23 18:07:22.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html
+-rw-rw-rw-   0        0        0     2489 2024-02-23 18:07:28.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html
+-rw-rw-rw-   0        0        0     1929 2024-02-23 18:07:33.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html
+-rw-rw-rw-   0        0        0     2803 2024-02-23 18:07:38.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.529500 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.545488 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/community/
+-rw-rw-rw-   0        0        0      818 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/community/formdata.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.551484 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/content-pro-media/
+-rw-rw-rw-   0        0        0     3209 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.576471 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/content-pro-update/
+-rw-rw-rw-   0        0        0       83 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/content-pro-update/content.html
+-rw-rw-rw-   0        0        0       84 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/content-pro-update/schedule.html
+-rw-rw-rw-   0        0        0      986 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.593458 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ic-update/
+-rw-rw-rw-   0        0        0      469 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ic-update/content.html
+-rw-rw-rw-   0        0        0     1379 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.729375 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/
+-rw-rw-rw-   0        0        0    25077 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html
+-rw-rw-rw-   0        0        0     1667 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html
+-rw-rw-rw-   0        0        0     1530 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html
+-rw-rw-rw-   0        0        0     1849 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html
+-rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html
+-rw-rw-rw-   0        0        0     4485 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html
+-rw-rw-rw-   0        0        0     5787 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.743365 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/meta-assets/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page-alert.html
+-rw-rw-rw-   0        0        0      628 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.781344 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/page-analythics/
+-rw-rw-rw-   0        0        0     1755 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html
+-rw-rw-rw-   0        0        0     1960 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html
+-rw-rw-rw-   0        0        0     1428 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.816324 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/smart-boost/
+-rw-rw-rw-   0        0        0     2129 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.830313 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/stela-sight/
+-rw-rw-rw-   0        0        0      268 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/stela-sight/data.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.836309 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/newcomer/
+-rw-rw-rw-   0        0        0     3796 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/newcomer/form.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.879283 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/post/
+-rw-rw-rw-   0        0        0      846 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/post/list-modal.html
+-rw-rw-rw-   0        0        0      850 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/post/main-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.917258 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/
+-rw-rw-rw-   0        0        0     1824 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/catalog-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:14.988215 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/
+-rw-rw-rw-   0        0        0      933 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/catalog-form.html
+-rw-rw-rw-   0        0        0      872 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/category-form.html
+-rw-rw-rw-   0        0        0      888 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/color-form.html
+-rw-rw-rw-   0        0        0     1024 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/product-form.html
+-rw-rw-rw-   0        0        0      855 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/size-form.html
+-rw-rw-rw-   0        0        0      115 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/variant-form.html
+-rw-rw-rw-   0        0        0      805 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/product-modal.html
+-rw-rw-rw-   0        0        0      848 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/size-modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.061169 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/
+-rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/catalog-form.html
+-rw-rw-rw-   0        0        0      287 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/category-form.html
+-rw-rw-rw-   0        0        0      230 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/color-form.html
+-rw-rw-rw-   0        0        0     1008 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/product-form.html
+-rw-rw-rw-   0        0        0      228 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/size-form.html
+-rw-rw-rw-   0        0        0      234 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/variant-form.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.084157 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/profile/
+-rw-rw-rw-   0        0        0     1306 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/profile/dynamic-form.html
+-rw-rw-rw-   0        0        0      200 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/profile/single-form.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.094150 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/projects/
+-rw-rw-rw-   0        0        0     1698 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/projects/modal.html
+-rw-rw-rw-   0        0        0      260 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/remove-complete.html
+-rw-rw-rw-   0        0        0      212 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/single-form.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.079177 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.165107 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.192089 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_forms/
+-rw-rw-rw-   0        0        0     1099 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.230067 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/forms/
+-rw-rw-rw-   0        0        0     1269 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html
+-rw-rw-rw-   0        0        0     1097 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html
+-rw-rw-rw-   0        0        0     1265 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.253927 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/update_forms/
+-rw-rw-rw-   0        0        0     1156 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html
+-rw-rw-rw-   0        0        0     1320 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.268917 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/staff/
+-rw-rw-rw-   0        0        0     1947 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/staff/form.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.375850 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stela_story/
+-rw-rw-rw-   0        0        0     3404 2024-02-21 12:50:07.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stela_story/feed-item.html
+-rw-rw-rw-   0        0        0     2001 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.389844 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelafooter/
+-rw-rw-rw-   0        0        0     2176 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelafooter/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.402834 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelamedia/
+-rw-rw-rw-   0        0        0     1695 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelamedia/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.435405 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelapath/
+-rw-rw-rw-   0        0        0     1337 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelapath/modal.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.446400 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/youtube/
+-rw-rw-rw-   0        0        0      157 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/youtube/video-preview.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.121181 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.491372 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/
+-rw-rw-rw-   0        0        0     2345 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/email_list.html
+-rw-rw-rw-   0        0        0     1774 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html
+-rw-rw-rw-   0        0        0     1917 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/new_email.html
+-rw-rw-rw-   0        0        0      976 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/update_email.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.503364 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/
+-rw-rw-rw-   0        0        0    10789 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:08.125179 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.965571 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/
+-rw-rw-rw-   0        0        0    13445 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:15.998549 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/
+-rw-rw-rw-   0        0        0    23333 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.022534 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/
+-rw-rw-rw-   0        0        0    34272 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.245197 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.297068 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/community/
+-rw-rw-rw-   0        0        0    14156 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.426637 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/
+-rw-rw-rw-   0        0        0    30243 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html
+-rw-rw-rw-   0        0        0      248 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/update.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.457099 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/
+-rw-rw-rw-   0        0        0     3162 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html
+-rw-rw-rw-   0        0        0    12633 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html
+-rw-rw-rw-   0        0        0    17640 2024-02-12 17:40:18.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/newcomer.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.567577 stela_publishing-0.2.29/stela_control/templates/stela_control/orders/
+-rw-rw-rw-   0        0        0     6171 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/orders/list_view.html
+-rw-rw-rw-   0        0        0     8860 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/orders/order_update.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.742196 stela_publishing-0.2.29/stela_control/templates/stela_control/payments/
+-rw-rw-rw-   0        0        0    43167 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/payments/homebrew.html
+-rw-rw-rw-   0        0        0     2687 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/payments/register-wallet.html
+-rw-rw-rw-   0        0        0     4322 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/payments/wallet-list.html
+-rw-rw-rw-   0        0        0     2831 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/payments/withdraw.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.754190 stela_publishing-0.2.29/stela_control/templates/stela_control/prostela/
+-rw-rw-rw-   0        0        0      153 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/prostela/chatbox.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.762184 stela_publishing-0.2.29/stela_control/templates/stela_control/prostela-expert/
+-rw-rw-rw-   0        0        0    34014 2024-01-15 04:03:12.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/prostela-expert/index.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.821148 stela_publishing-0.2.29/stela_control/templates/stela_control/reviews/
+-rw-rw-rw-   0        0        0     3170 2024-01-15 04:03:13.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/reviews/reviews_list.html
+-rw-rw-rw-   0        0        0     1325 2024-01-15 04:03:13.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/reviews/update_review.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:16.845134 stela_publishing-0.2.29/stela_control/templates/stela_control/support/
+-rw-rw-rw-   0        0        0     2061 2024-01-15 04:03:13.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/support/list.html
+-rw-rw-rw-   0        0        0     7093 2024-01-15 04:03:13.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/support/update.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:17.143989 stela_publishing-0.2.29/stela_control/templates/stela_control/users/
+-rw-rw-rw-   0        0        0      339 2024-01-18 10:28:40.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/users/generic-user-handler.html
+-rw-rw-rw-   0        0        0    11181 2024-01-22 21:22:30.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/users/profile.html
+-rw-rw-rw-   0        0        0    12343 2024-02-06 16:52:33.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/users/users-control.html
+-rw-rw-rw-   0        0        0     6472 2024-02-06 15:00:39.000000 stela_publishing-0.2.29/stela_control/templates/stela_control/users/users.html
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:17.174972 stela_publishing-0.2.29/stela_control/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-01-15 04:03:13.000000 stela_publishing-0.2.29/stela_control/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1277 2024-01-19 05:09:17.000000 stela_publishing-0.2.29/stela_control/templatetags/stelatags.py
+-rw-rw-rw-   0        0        0      507 2024-01-15 04:03:13.000000 stela_publishing-0.2.29/stela_control/tests.py
+-rw-rw-rw-   0        0        0     1131 2024-01-15 04:03:13.000000 stela_publishing-0.2.29/stela_control/tokenize.py
+-rw-rw-rw-   0        0        0     5281 2024-02-20 00:45:02.000000 stela_publishing-0.2.29/stela_control/urls.py
+-rw-rw-rw-   0        0        0   211317 2024-02-20 00:48:27.000000 stela_publishing-0.2.29/stela_control/views.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:43:17.241525 stela_publishing-0.2.29/stela_publishing.egg-info/
+-rw-rw-rw-   0        0        0     3241 2024-04-23 17:43:07.000000 stela_publishing-0.2.29/stela_publishing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    20793 2024-04-23 17:43:07.000000 stela_publishing-0.2.29/stela_publishing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 17:43:07.000000 stela_publishing-0.2.29/stela_publishing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      355 2024-04-23 17:43:07.000000 stela_publishing-0.2.29/stela_publishing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2024-04-23 17:43:07.000000 stela_publishing-0.2.29/stela_publishing.egg-info/top_level.txt
```

### Comparing `stela_publishing-0.2.28/LICENSE` & `stela_publishing-0.2.29/LICENSE`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/PKG-INFO` & `stela_publishing-0.2.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_publishing
-Version: 0.2.28
+Version: 0.2.29
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_publishing-0.2.28/README.md` & `stela_publishing-0.2.29/README.md`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/accounts/migrations/0001_initial.py` & `stela_publishing-0.2.29/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/accounts/models.py` & `stela_publishing-0.2.29/accounts/models.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/accounts/urls.py` & `stela_publishing-0.2.29/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/accounts/views.py` & `stela_publishing-0.2.29/accounts/views.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/cloud/cart.py` & `stela_publishing-0.2.29/cloud/cart.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/cloud/migrations/0001_initial.py` & `stela_publishing-0.2.29/cloud/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/cloud/models.py` & `stela_publishing-0.2.29/cloud/models.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/geolocation/migrations/0001_initial.py` & `stela_publishing-0.2.29/geolocation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/geolocation/models.py` & `stela_publishing-0.2.29/geolocation/models.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/setup.py` & `stela_publishing-0.2.29/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 excluded_packages = [
     'core', 'core.*', 
     'linkzone', 'linkzone.*', 
 ]
 setup(
     name='stela_publishing',
-    version='0.2.28',
+    version='0.2.29',
     packages=find_packages(exclude=excluded_packages),
     include_package_data=True,
     license='MIT',
     description='All apps in one for business.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

### Comparing `stela_publishing-0.2.28/stela_control/cart.py` & `stela_publishing-0.2.29/stela_control/cart.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/forms.py` & `stela_publishing-0.2.29/stela_control/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -979,15 +979,15 @@
         model = Inventory
         exclude = ('slug','owner','type','price','qty', 'sku', 'lang', 'id')
         fields = '__all__'
 
 class WorksForm(forms.ModelForm):
     class Meta:
         model = Inventory
-        fields = ['status', 'title', 'condition', 'description', 'image', 'price', 'url', 'published_date']
+        fields = ['status', 'title', 'condition', 'description', 'image', 'price', 'url', 'published_date', 'amazon_published_date']
         widgets = {
             'status': forms.Select(attrs={
                 'placeholder': 'Choose status...',
                 'class': 'form-control',  
             }),
             'condition': forms.Select(attrs={
                 'placeholder': 'Select...',
@@ -1008,14 +1008,17 @@
             'url': forms.URLInput(attrs={
                 'placeholder': 'http://example.com',
                 'class': 'form-control',
             }),
             'published_date': DateInput(attrs={
                 'placeholder': _('Select a date'),
             }),
+            'amazon_published_date': DateInput(attrs={
+                'placeholder': _('Select a date'),
+            }),
         }
         labels = {
             'status': '',
             'title': '',
             'description': '',
             'url': '',
         }
```

### Comparing `stela_publishing-0.2.28/stela_control/locale/es/LC_MESSAGES/django.mo` & `stela_publishing-0.2.29/stela_control/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/locale/es/LC_MESSAGES/django.po` & `stela_publishing-0.2.29/stela_control/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0001_initial.py` & `stela_publishing-0.2.29/stela_control/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0002_rename_response_chatsupport_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0003_rename_logo_company_alter_logo_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0004_content_video_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0005_rename_description_team_content_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0005_rename_description_team_content_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0006_content_cover_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0007_content_fecade_url_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0008_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0009_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0010_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0011_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0012_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0013_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0014_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0015_alter_billingrecipt_option_alter_company_business_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0016_remove_sociallinks_url_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0017_sociallinks_social_url_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0018_inventory_condition_alter_billingrecipt_option_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py` & `stela_publishing-0.2.29/stela_control/migrations/0019_inventory_amazon_published_date_and_more.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/models.py` & `stela_publishing-0.2.29/stela_control/models.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/routers.py` & `stela_publishing-0.2.29/stela_control/routers.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/superfunctions.py` & `stela_publishing-0.2.29/stela_control/superfunctions.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/registration/confirmation_email.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/registration/confirmation_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/registration/register.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/registration/register.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/delete_user.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/delete_user.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/login.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/login.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_done.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_email.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/accounts/user/password_reset_form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/accounts/user/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/analytics/analytics.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/analytics/analytics.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/analytics/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/analytics/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/api/main.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/api/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/base.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/base.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/base_content.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/base_content.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/base_list.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/base_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/homebrew.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/bill-data-customer.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/bill-data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/checkout.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/checkout.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/data-customer.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/data-customer.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/invoice-copy.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/invoice.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/order-placed.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/order-placed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/preview-recipt.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/preview-recipt.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/recipt-detail-ves.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/billing/sections/recipt-detail.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/billing/sections/recipt-detail.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/chatstela/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/chatstela/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/content/comments/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/content/comments/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/content/docs/main.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/content/docs/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/content/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/content/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/content/main/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/content/main/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/content/staff/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/content/staff/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/content/stelastory.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/content/stelastory.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal1.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal1.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal2.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal3.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal3.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/developer/data-update/modal4.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/developer/data-update/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/developer/home.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/developer/home.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/billing/invoice-copy.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/billing/invoice.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/billing/invoice.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/message_notification.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/message_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/message_response.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/message_response.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/support_notification.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/contact/update_support.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/contact/update_support.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/marketing/content-planner-email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/newsletter/stela-notify.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/newsletter/success.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/newsletter/success.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_credentials.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_express_placed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/orders/stela_order_placed_ves2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/billing_payment.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/billing_payment.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/charges.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/charges.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/payment_notification.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/payment_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/sale_notification.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/sale_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/withdraw_success.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/payments/withdrawals.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/payments/withdrawals.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/support/support_notification.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/support/support_notification.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/emails-template/support/support_response.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/emails-template/support/support_response.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/home.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/home.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/inbox/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/inbox/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/inventory/journals/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/inventory/journals/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/inventory/publishing/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/inventory/publishing/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutemmerut/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutsecondary/formset-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/aboutstela/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/aboutstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/appstela/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/appstela/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/auth/signup/register_errors_v1.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/blog-feed.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/blog-feed.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/categories/modal4.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/categories/modal4.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/chatbox.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/chatbox.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/chatbox2.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/chatbox2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/colors/modal2.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/colors/modal2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/contact/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/contact/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/dynamic-formset.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutfooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutservices/formset1.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutservices/formset2.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/emmerutservices/formset3.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/form-base.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/form-base.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/formset-base-services.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/formset-base-services.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/formset-base.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/formset-base.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/formset.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/handlers/blog/blog-pages.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/instagram-alert.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/instagram-alert.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/inventory/dynamic-formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/inventory/simple-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/inventory/simple-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/inventory/simple-formset.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/inventory/simple-formset.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/linkzoneupdates/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/error_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/forms/blog_form_video.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormImage.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/BlogFormVideo.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/BulletSimpleForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentDynamicForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/GalleryForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ImageContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/RedirectContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/SimpleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/StickerContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/TitleContentForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/maincontent/update_forms/ValuesForm.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/community/formdata.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/community/formdata.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/content-pro-media/media.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/fb-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ic-update/hashtags.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/content-render.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-carousels.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-post.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-reels.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-analythics/table-metric-stories.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-new-page-grid.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/ig-new-pages.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/meta-assets/remove-page.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/page-analythics/page-select.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/page-analythics/post-select.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/page-analythics/video-select.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/meta/smart-boost/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/newcomer/form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/newcomer/form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/post/list-modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/post/list-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/post/main-modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/post/main-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/catalog-modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/catalog-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/catalog-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/catalog-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/category-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/category-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/color-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/color-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/product-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/new/size-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/new/size-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/product-modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/product-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/size-modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/size-modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/products/update/product-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/products/update/product-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/profile/dynamic-form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/profile/dynamic-form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/projects/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/projects/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_empty_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/error_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/forms/bio_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/update_forms/faq_form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/site_docs/update_forms/terms.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/staff/form.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/staff/form.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stela_story/feed-item.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stela_story/feed-item.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stela_story/table-blog-filter.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelafooter/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelafooter/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelamedia/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelamedia/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/load-data/stelapath/modal.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/load-data/stelapath/modal.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/email_list.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/email_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/emails_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/new_email.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/new_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/email-marketing/update_email.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/email-marketing/update_email.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/grid/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/ig-analyzer/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/instagram/insight-creative/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/community/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/content-pro/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/page-analythics/main.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/marketing/meta_business/page/page-detail.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/newcomer.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/newcomer.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/orders/list_view.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/orders/list_view.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/orders/order_update.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/orders/order_update.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/payments/homebrew.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/payments/homebrew.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/payments/register-wallet.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/payments/register-wallet.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/payments/wallet-list.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/payments/wallet-list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/payments/withdraw.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/payments/withdraw.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/prostela-expert/index.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/prostela-expert/index.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/reviews/reviews_list.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/reviews/reviews_list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/reviews/update_review.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/reviews/update_review.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/support/list.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/support/list.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/support/update.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/support/update.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/users/profile.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/users/profile.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/users/users-control.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/users/users-control.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templates/stela_control/users/users.html` & `stela_publishing-0.2.29/stela_control/templates/stela_control/users/users.html`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/templatetags/stelatags.py` & `stela_publishing-0.2.29/stela_control/templatetags/stelatags.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/tokenize.py` & `stela_publishing-0.2.29/stela_control/tokenize.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/urls.py` & `stela_publishing-0.2.29/stela_control/urls.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_control/views.py` & `stela_publishing-0.2.29/stela_control/views.py`

 * *Files identical despite different names*

### Comparing `stela_publishing-0.2.28/stela_publishing.egg-info/PKG-INFO` & `stela_publishing-0.2.29/stela_publishing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stela_publishing
-Version: 0.2.28
+Version: 0.2.29
 Summary: All apps in one for business.
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `stela_publishing-0.2.28/stela_publishing.egg-info/SOURCES.txt` & `stela_publishing-0.2.29/stela_publishing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

