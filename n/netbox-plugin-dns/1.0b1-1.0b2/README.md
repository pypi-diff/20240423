# Comparing `tmp/netbox_plugin_dns-1.0b1.tar.gz` & `tmp/netbox_plugin_dns-1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_dns-1.0b1.tar", max compression
+gzip compressed data, was "netbox_plugin_dns-1.0b2.tar", max compression
```

## Comparing `netbox_plugin_dns-1.0b1.tar` & `netbox_plugin_dns-1.0b2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1076 2024-04-03 13:17:52.207418 netbox_plugin_dns-1.0b1/LICENSE
--rw-r--r--   0        0        0     3697 2024-04-03 13:17:52.207418 netbox_plugin_dns-1.0b1/README.md
--rw-r--r--   0        0        0     1053 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/__init__.py
--rw-r--r--   0        0        0     2145 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/nested_serializers.py
--rw-r--r--   0        0        0      249 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers.py
--rw-r--r--   0        0        0        0 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/__init__.py
--rw-r--r--   0        0        0      929 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/contact.py
--rw-r--r--   0        0        0     1093 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/nameserver.py
--rw-r--r--   0        0        0     2284 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/record.py
--rw-r--r--   0        0        0      805 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/registrar.py
--rw-r--r--   0        0        0      798 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/view.py
--rw-r--r--   0        0        0     4759 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/zone.py
--rw-r--r--   0        0        0      575 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/urls.py
--rw-r--r--   0        0        0     3566 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/views.py
--rw-r--r--   0        0        0      151 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/apps.py
--rw-r--r--   0        0        0       69 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/__init__.py
--rw-r--r--   0        0        0     1494 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/address.py
--rw-r--r--   0        0        0     3606 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/network.py
--rw-r--r--   0        0        0     2518 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/rfc2317.py
--rw-r--r--   0        0        0      136 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/__init__.py
--rw-r--r--   0        0        0     1057 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/contact.py
--rwxr-xr-x   0        0        0     1110 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/nameserver.py
--rwxr-xr-x   0        0        0     3687 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/record.py
--rw-r--r--   0        0        0      941 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/registrar.py
--rw-r--r--   0        0        0      505 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/view.py
--rwxr-xr-x   0        0        0     6564 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/zone.py
--rw-r--r--   0        0        0      136 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/__init__.py
--rw-r--r--   0        0        0     5220 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/contact.py
--rwxr-xr-x   0        0        0     2361 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/nameserver.py
--rwxr-xr-x   0        0        0     6272 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/record.py
--rw-r--r--   0        0        0     3638 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/registrar.py
--rw-r--r--   0        0        0     1932 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/view.py
--rwxr-xr-x   0        0        0    22627 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/zone.py
--rw-r--r--   0        0        0      358 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/filters.py
--rw-r--r--   0        0        0     1915 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/schema.py
--rw-r--r--   0        0        0     4207 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/types.py
--rw-r--r--   0        0        0     5960 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_database.py
--rw-r--r--   0        0        0     2029 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_rrset_ttl.py
--rw-r--r--   0        0        0     4556 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/setup_coupling.py
--rw-r--r--   0        0        0      660 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/update_soa.py
--rw-r--r--   0        0        0    10283 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
--rw-r--r--   0        0        0    20243 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_22.py
--rw-r--r--   0        0        0      583 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0002_contact_description_registrar_description.py
--rw-r--r--   0        0        0     1271 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0020_netbox_3_4.py
--rw-r--r--   0        0        0     3243 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0021_record_ip_address.py
--rw-r--r--   0        0        0      172 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0022_search.py
--rw-r--r--   0        0        0      378 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0023_alter_record_value.py
--rw-r--r--   0        0        0     1745 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0024_tenancy.py
--rw-r--r--   0        0        0      620 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0025_ipam_coupling_cf.py
--rw-r--r--   0        0        0     5796 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0026_domain_registration.py
--rw-r--r--   0        0        0      404 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0027_alter_registrar_iana_id.py
--rw-r--r--   0        0        0     1364 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0028_rfc2317_fields.py
--rw-r--r--   0        0        0      808 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0029_record_fqdn.py
--rw-r--r--   0        0        0        0 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/__init__.py
--rw-r--r--   0        0        0      182 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/__init__.py
--rw-r--r--   0        0        0     2958 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/contact.py
--rw-r--r--   0        0        0     3021 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/nameserver.py
--rw-r--r--   0        0        0    23740 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/record.py
--rw-r--r--   0        0        0     1502 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/registrar.py
--rw-r--r--   0        0        0      920 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/view.py
--rw-r--r--   0        0        0    26519 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/models/zone.py
--rw-r--r--   0        0        0     4062 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/navigation.py
--rw-r--r--   0        0        0        0 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/signals/__init__.py
--rw-r--r--   0        0        0     5595 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/signals/ipam_coupling.py
--rw-r--r--   0        0        0      136 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/__init__.py
--rw-r--r--   0        0        0      774 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/contact.py
--rw-r--r--   0        0        0      767 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/nameserver.py
--rw-r--r--   0        0        0     3162 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/record.py
--rw-r--r--   0        0        0      648 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/registrar.py
--rw-r--r--   0        0        0      501 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/view.py
--rw-r--r--   0        0        0     1886 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/zone.py
--rw-r--r--   0        0        0     3805 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/template_content.py
--rw-r--r--   0        0        0     2855 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/contact.html
--rw-r--r--   0        0        0     1554 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/nameserver.html
--rw-r--r--   0        0        0       89 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record/managed.html
--rw-r--r--   0        0        0      742 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record/related.html
--rw-r--r--   0        0        0     5481 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record.html
--rw-r--r--   0        0        0     2152 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/registrar.html
--rw-r--r--   0        0        0      806 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/related_dns_objects.html
--rw-r--r--   0        0        0     1321 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/view.html
--rw-r--r--   0        0        0      495 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/base.html
--rw-r--r--   0        0        0     2147 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/child.html
--rw-r--r--   0        0        0      514 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/managed_record.html
--rw-r--r--   0        0        0     2194 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/record.html
--rw-r--r--   0        0        0     1151 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/registration.html
--rw-r--r--   0        0        0      517 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html
--rw-r--r--   0        0        0     6717 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone.html
--rw-r--r--   0        0        0     9172 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/urls.py
--rw-r--r--   0        0        0     1835 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/utilities/__init__.py
--rw-r--r--   0        0        0     3441 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/utilities/ipam_coupling.py
--rw-r--r--   0        0        0       47 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/validators/__init__.py
--rw-r--r--   0        0        0     2097 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/validators/dns_name.py
--rw-r--r--   0        0        0      501 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/validators/rfc2317.py
--rw-r--r--   0        0        0      136 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/__init__.py
--rw-r--r--   0        0        0     2253 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/contact.py
--rw-r--r--   0        0        0     3011 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/nameserver.py
--rw-r--r--   0        0        0     4928 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/record.py
--rw-r--r--   0        0        0     2090 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/registrar.py
--rw-r--r--   0        0        0     1913 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/view.py
--rw-r--r--   0        0        0     4591 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/zone.py
--rw-r--r--   0        0        0      732 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/pyproject.toml
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 netbox_plugin_dns-1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-22 22:58:00.339468 netbox_plugin_dns-1.0b2/LICENSE
+-rw-r--r--   0        0        0     5227 2024-04-22 22:58:00.339468 netbox_plugin_dns-1.0b2/README.md
+-rw-r--r--   0        0        0     1053 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/__init__.py
+-rw-r--r--   0        0        0     2145 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/nested_serializers.py
+-rw-r--r--   0        0        0      249 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/contact.py
+-rw-r--r--   0        0        0     1093 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/nameserver.py
+-rw-r--r--   0        0        0     2284 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/record.py
+-rw-r--r--   0        0        0      805 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/registrar.py
+-rw-r--r--   0        0        0      798 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/view.py
+-rw-r--r--   0        0        0     4351 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/zone.py
+-rw-r--r--   0        0        0      575 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/urls.py
+-rw-r--r--   0        0        0     3566 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/api/views.py
+-rw-r--r--   0        0        0      151 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/apps.py
+-rw-r--r--   0        0        0       69 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/fields/__init__.py
+-rw-r--r--   0        0        0     1494 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/fields/address.py
+-rw-r--r--   0        0        0     3606 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/fields/network.py
+-rw-r--r--   0        0        0     2518 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/fields/rfc2317.py
+-rw-r--r--   0        0        0      136 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/filtersets/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/filtersets/contact.py
+-rwxr-xr-x   0        0        0     1110 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/filtersets/nameserver.py
+-rwxr-xr-x   0        0        0     3687 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/filtersets/record.py
+-rw-r--r--   0        0        0      941 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/filtersets/registrar.py
+-rw-r--r--   0        0        0      505 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/filtersets/view.py
+-rwxr-xr-x   0        0        0     6564 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/filtersets/zone.py
+-rw-r--r--   0        0        0      136 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/forms/__init__.py
+-rw-r--r--   0        0        0     5220 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/forms/contact.py
+-rwxr-xr-x   0        0        0     2361 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/forms/nameserver.py
+-rwxr-xr-x   0        0        0     6272 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/forms/record.py
+-rw-r--r--   0        0        0     3638 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/forms/registrar.py
+-rw-r--r--   0        0        0     1932 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/forms/view.py
+-rwxr-xr-x   0        0        0    22627 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/forms/zone.py
+-rw-r--r--   0        0        0      358 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/graphql/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/graphql/filters.py
+-rw-r--r--   0        0        0     1915 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/graphql/schema.py
+-rw-r--r--   0        0        0     4207 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/graphql/types.py
+-rw-r--r--   0        0        0     5960 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/management/commands/cleanup_database.py
+-rw-r--r--   0        0        0     2029 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/management/commands/cleanup_rrset_ttl.py
+-rw-r--r--   0        0        0     4556 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/management/commands/setup_coupling.py
+-rw-r--r--   0        0        0      660 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/management/commands/update_soa.py
+-rw-r--r--   0        0        0    10283 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
+-rw-r--r--   0        0        0    20243 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0001_squashed_netbox_dns_0_22.py
+-rw-r--r--   0        0        0      583 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0002_contact_description_registrar_description.py
+-rw-r--r--   0        0        0     1271 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0020_netbox_3_4.py
+-rw-r--r--   0        0        0     3243 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0021_record_ip_address.py
+-rw-r--r--   0        0        0      172 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0022_search.py
+-rw-r--r--   0        0        0      378 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0023_alter_record_value.py
+-rw-r--r--   0        0        0     1745 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0024_tenancy.py
+-rw-r--r--   0        0        0      620 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0025_ipam_coupling_cf.py
+-rw-r--r--   0        0        0     5796 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0026_domain_registration.py
+-rw-r--r--   0        0        0      404 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0027_alter_registrar_iana_id.py
+-rw-r--r--   0        0        0     1364 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0028_rfc2317_fields.py
+-rw-r--r--   0        0        0      808 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/0029_record_fqdn.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/migrations/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/models/__init__.py
+-rw-r--r--   0        0        0     2958 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/models/contact.py
+-rw-r--r--   0        0        0     3021 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/models/nameserver.py
+-rw-r--r--   0        0        0    23763 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/models/record.py
+-rw-r--r--   0        0        0     1502 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/models/registrar.py
+-rw-r--r--   0        0        0      920 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/models/view.py
+-rw-r--r--   0        0        0    26519 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/models/zone.py
+-rw-r--r--   0        0        0     4062 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/navigation.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/signals/__init__.py
+-rw-r--r--   0        0        0     5595 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/signals/ipam_coupling.py
+-rw-r--r--   0        0        0      136 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/tables/__init__.py
+-rw-r--r--   0        0        0      774 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/tables/contact.py
+-rw-r--r--   0        0        0      767 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/tables/nameserver.py
+-rw-r--r--   0        0        0     3162 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/tables/record.py
+-rw-r--r--   0        0        0      648 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/tables/registrar.py
+-rw-r--r--   0        0        0      501 2024-04-22 22:58:00.371467 netbox_plugin_dns-1.0b2/netbox_dns/tables/view.py
+-rw-r--r--   0        0        0     1886 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/tables/zone.py
+-rw-r--r--   0        0        0     3805 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/template_content.py
+-rw-r--r--   0        0        0     2855 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/contact.html
+-rw-r--r--   0        0        0     1554 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/nameserver.html
+-rw-r--r--   0        0        0       89 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/record/managed.html
+-rw-r--r--   0        0        0      742 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/record/related.html
+-rw-r--r--   0        0        0     5481 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/record.html
+-rw-r--r--   0        0        0     2152 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/registrar.html
+-rw-r--r--   0        0        0      806 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/related_dns_objects.html
+-rw-r--r--   0        0        0     1321 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/view.html
+-rw-r--r--   0        0        0      495 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/base.html
+-rw-r--r--   0        0        0     2147 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/child.html
+-rw-r--r--   0        0        0      514 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/managed_record.html
+-rw-r--r--   0        0        0     2194 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/record.html
+-rw-r--r--   0        0        0     1151 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/registration.html
+-rw-r--r--   0        0        0      517 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html
+-rw-r--r--   0        0        0     6717 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone.html
+-rw-r--r--   0        0        0     9172 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/urls.py
+-rw-r--r--   0        0        0     1835 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/utilities/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/utilities/ipam_coupling.py
+-rw-r--r--   0        0        0       47 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/validators/__init__.py
+-rw-r--r--   0        0        0     2097 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/validators/dns_name.py
+-rw-r--r--   0        0        0      501 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/validators/rfc2317.py
+-rw-r--r--   0        0        0      136 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/views/__init__.py
+-rw-r--r--   0        0        0     2253 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/views/contact.py
+-rw-r--r--   0        0        0     3011 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/views/nameserver.py
+-rw-r--r--   0        0        0     4616 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/views/record.py
+-rw-r--r--   0        0        0     2090 2024-04-22 22:58:00.375467 netbox_plugin_dns-1.0b2/netbox_dns/views/registrar.py
+-rw-r--r--   0        0        0     1913 2024-04-22 22:58:00.379468 netbox_plugin_dns-1.0b2/netbox_dns/views/view.py
+-rw-r--r--   0        0        0     4591 2024-04-22 22:58:00.379468 netbox_plugin_dns-1.0b2/netbox_dns/views/zone.py
+-rw-r--r--   0        0        0      732 2024-04-22 22:58:00.379468 netbox_plugin_dns-1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 netbox_plugin_dns-1.0b2/PKG-INFO
```

### Comparing `netbox_plugin_dns-1.0b1/LICENSE` & `netbox_plugin_dns-1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/__init__.py` & `netbox_plugin_dns-1.0b2/netbox_dns/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from netbox.plugins import PluginConfig
 
-__version__ = "1.0-beta1"
+__version__ = "1.0-beta2"
 
 
 class DNSConfig(PluginConfig):
     name = "netbox_dns"
     verbose_name = "NetBox DNS"
     description = "NetBox plugin for DNS data"
     min_version = "4.0-beta1"
```

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/nested_serializers.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/contact.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/nameserver.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/record.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/registrar.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/view.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/zone.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/serializers_/zone.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,14 @@
 from netbox_dns.api.serializers_.contact import ContactSerializer
 from netbox_dns.api.nested_serializers import NestedZoneSerializer
 
 from netbox_dns.models import Zone
 
 
 class ZoneSerializer(NetBoxModelSerializer):
-    # +
-    # This is a hack to avoid the exception raised by the UniqueTogetherValidator
-    # after NetBox commit https://github.com/netbox-community/netbox/commit/78e284c
-    #
-    # See https://github.com/netbox-community/netbox/issues/15351 for details.
-    # -
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        if self.nested:
-            self.validators = []
-
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_dns-api:zone-detail"
     )
     view = ViewSerializer(
         nested=True,
         many=False,
         read_only=False,
```

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/urls.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/api/views.py` & `netbox_plugin_dns-1.0b2/netbox_dns/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/fields/address.py` & `netbox_plugin_dns-1.0b2/netbox_dns/fields/address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/fields/network.py` & `netbox_plugin_dns-1.0b2/netbox_dns/fields/network.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/fields/rfc2317.py` & `netbox_plugin_dns-1.0b2/netbox_dns/fields/rfc2317.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/contact.py` & `netbox_plugin_dns-1.0b2/netbox_dns/filtersets/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/nameserver.py` & `netbox_plugin_dns-1.0b2/netbox_dns/filtersets/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/record.py` & `netbox_plugin_dns-1.0b2/netbox_dns/filtersets/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/registrar.py` & `netbox_plugin_dns-1.0b2/netbox_dns/filtersets/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/zone.py` & `netbox_plugin_dns-1.0b2/netbox_dns/filtersets/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/forms/contact.py` & `netbox_plugin_dns-1.0b2/netbox_dns/forms/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/forms/nameserver.py` & `netbox_plugin_dns-1.0b2/netbox_dns/forms/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/forms/record.py` & `netbox_plugin_dns-1.0b2/netbox_dns/forms/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/forms/registrar.py` & `netbox_plugin_dns-1.0b2/netbox_dns/forms/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/forms/view.py` & `netbox_plugin_dns-1.0b2/netbox_dns/forms/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/forms/zone.py` & `netbox_plugin_dns-1.0b2/netbox_dns/forms/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/graphql/filters.py` & `netbox_plugin_dns-1.0b2/netbox_dns/graphql/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/graphql/schema.py` & `netbox_plugin_dns-1.0b2/netbox_dns/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/graphql/types.py` & `netbox_plugin_dns-1.0b2/netbox_dns/graphql/types.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_database.py` & `netbox_plugin_dns-1.0b2/netbox_dns/management/commands/cleanup_database.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_rrset_ttl.py` & `netbox_plugin_dns-1.0b2/netbox_dns/management/commands/cleanup_rrset_ttl.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         self.stdout.write("RRSet cleanup completed.")
 
     def cleanup_rrset_ttl(self, **options):
         ttl_records = (
             Record.objects.filter(ttl__isnull=False)
             .exclude(type=RecordTypeChoices.SOA)
-            .exclude(type=RecordTypeChoices.PTR, maanged=True)
+            .exclude(type=RecordTypeChoices.PTR, managed=True)
         )
         for record in ttl_records:
             records = Record.objects.filter(
                 name=record.name,
                 zone=record.zone,
                 type=record.type,
             ).exclude(type=RecordTypeChoices.PTR, maanged=True)
```

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/setup_coupling.py` & `netbox_plugin_dns-1.0b2/netbox_dns/management/commands/setup_coupling.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/update_soa.py` & `netbox_plugin_dns-1.0b2/netbox_dns/management/commands/update_soa.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_22.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0001_squashed_netbox_dns_0_22.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0002_contact_description_registrar_description.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0002_contact_description_registrar_description.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0020_netbox_3_4.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0020_netbox_3_4.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0021_record_ip_address.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0021_record_ip_address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0024_tenancy.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0024_tenancy.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0025_ipam_coupling_cf.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0025_ipam_coupling_cf.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0026_domain_registration.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0026_domain_registration.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0028_rfc2317_fields.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0028_rfc2317_fields.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0029_record_fqdn.py` & `netbox_plugin_dns-1.0b2/netbox_dns/migrations/0029_record_fqdn.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/models/contact.py` & `netbox_plugin_dns-1.0b2/netbox_dns/models/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/models/nameserver.py` & `netbox_plugin_dns-1.0b2/netbox_dns/models/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/models/record.py` & `netbox_plugin_dns-1.0b2/netbox_dns/models/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,12 +750,13 @@
             zone.update_serial(save_zone_serial=save_zone_serial)
 
 
 @register_search
 class RecordIndex(SearchIndex):
     model = Record
     fields = (
-        ("name", 100),
+        ("fqdn", 100),
+        ("name", 120),
         ("value", 150),
         ("zone", 200),
         ("type", 200),
     )
```

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/models/registrar.py` & `netbox_plugin_dns-1.0b2/netbox_dns/models/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/models/view.py` & `netbox_plugin_dns-1.0b2/netbox_dns/models/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/models/zone.py` & `netbox_plugin_dns-1.0b2/netbox_dns/models/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/navigation.py` & `netbox_plugin_dns-1.0b2/netbox_dns/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/signals/ipam_coupling.py` & `netbox_plugin_dns-1.0b2/netbox_dns/signals/ipam_coupling.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/tables/contact.py` & `netbox_plugin_dns-1.0b2/netbox_dns/tables/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/tables/nameserver.py` & `netbox_plugin_dns-1.0b2/netbox_dns/tables/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/tables/record.py` & `netbox_plugin_dns-1.0b2/netbox_dns/tables/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/tables/registrar.py` & `netbox_plugin_dns-1.0b2/netbox_dns/tables/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/tables/zone.py` & `netbox_plugin_dns-1.0b2/netbox_dns/tables/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/template_content.py` & `netbox_plugin_dns-1.0b2/netbox_dns/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/contact.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/contact.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/nameserver.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/nameserver.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record/related.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/record/related.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/registrar.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/registrar.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/related_dns_objects.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/related_dns_objects.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/view.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/view.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/child.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/child.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/managed_record.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/managed_record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/record.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/record.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/registration.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/registration.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone.html` & `netbox_plugin_dns-1.0b2/netbox_dns/templates/netbox_dns/zone.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/urls.py` & `netbox_plugin_dns-1.0b2/netbox_dns/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/utilities/__init__.py` & `netbox_plugin_dns-1.0b2/netbox_dns/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/utilities/ipam_coupling.py` & `netbox_plugin_dns-1.0b2/netbox_dns/utilities/ipam_coupling.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/validators/dns_name.py` & `netbox_plugin_dns-1.0b2/netbox_dns/validators/dns_name.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/views/contact.py` & `netbox_plugin_dns-1.0b2/netbox_dns/views/contact.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/views/nameserver.py` & `netbox_plugin_dns-1.0b2/netbox_dns/views/nameserver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/views/record.py` & `netbox_plugin_dns-1.0b2/netbox_dns/views/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,30 +37,23 @@
     template_name = "netbox_dns/record/managed.html"
 
 
 class RecordView(generic.ObjectView):
     queryset = Record.objects.all().prefetch_related("zone", "ptr_record")
 
     def get_value_records(self, instance):
-        value_fqdn = dns_name.from_text(instance.value_fqdn)
-        value_zone_names = [
-            value_fqdn.split(length)[1].to_text().rstrip(".")
-            for length in range(2, len(value_fqdn) + 1)
-        ]
-
-        value_zone = (
-            Zone.objects.filter(instance.zone.view_filter, name__in=value_zone_names)
-            .order_by(Length("name").desc())
-            .first()
+        view_filter = (
+            Q(zone__view__isnull=True)
+            if instance.zone.view is None
+            else Q(zone__view=instance.zone.view)
         )
-        if not value_zone:
-            return None
 
-        value_name = value_fqdn.relativize(dns_name.from_text(value_zone.name))
-        cname_targets = Record.objects.filter(zone=value_zone, name=value_name)
+        value_fqdn = dns_name.from_text(instance.value_fqdn)
+
+        cname_targets = Record.objects.filter(view_filter, fqdn=value_fqdn)
 
         if cname_targets:
             return RelatedRecordTable(
                 data=cname_targets,
             )
 
         return None
```

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/views/registrar.py` & `netbox_plugin_dns-1.0b2/netbox_dns/views/registrar.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/views/view.py` & `netbox_plugin_dns-1.0b2/netbox_dns/views/view.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/netbox_dns/views/zone.py` & `netbox_plugin_dns-1.0b2/netbox_dns/views/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-1.0b1/pyproject.toml` & `netbox_plugin_dns-1.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-plugin-dns"
-version = "1.0-beta1"
+version = "1.0-beta2"
 description = "NetBox DNS is a NetBox plugin for managing DNS data."
 authors = ["Peter Eckel <pete@netbox-dns.org>"]
 homepage = "https://github.com/peteeckel/netbox-plugin-dns"
 repository = "https://github.com/peteeckel/netbox-plugin-dns"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "netbox_dns"}]
```

