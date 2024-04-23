# Comparing `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3.tar.gz` & `tmp/odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3.tar", last modified: Wed Apr 17 10:57:46 2024, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4.tar", last modified: Tue Apr 23 07:52:59 2024, max compression
```

## Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3.tar` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-17 10:57:46.031855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    30218 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)    29753 2024-04-17 10:57:46.028855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/photovoltaic_mgmt_extended.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/account_allocation.py
--rw-rw-rw-   0 root         (0) root         (0)     1214 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/contract_participation.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/participant_liquidations.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/photovoltaic_power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/res_partner_interest.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/security/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-17 10:57:46.029855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/account_allocation.xml
--rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/contract_participation.xml
--rw-rw-rw-   0 root         (0) root         (0)     2052 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/photovoltaic_power_station.xml
--rw-rw-rw-   0 root         (0) root         (0)      716 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner.xml
--rw-rw-rw-   0 root         (0) root         (0)     2325 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner_interest.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/
--rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-17 10:57:46.030855 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-23 07:52:59.101391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-23 07:52:59.097391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2024-04-23 07:52:59.097391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    30218 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)    29753 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/i18n/photovoltaic_mgmt_extended.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/account_allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/contract_participation.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-23 07:52:59.098391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/participant_liquidations.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/photovoltaic_power_energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/photovoltaic_power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/res_partner_interest.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/security/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/account_allocation.xml
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-23 07:52:59.099391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/contract_participation.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/photovoltaic_power_station.xml
+-rw-rw-rw-   0 root         (0) root         (0)      716 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/res_partner.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/res_partner_interest.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/wizard/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/wizard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/wizard/account_allocation_state_update_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-23 07:52:59.100391 odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/wizard/account_allocation_state_update_wizard_view.xml
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/__manifest__.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': "Photovoltaic Management Extended",
-    'version': '13.0.1.1.3',
+    'version': '13.0.1.1.4',
     'depends': [
         'photovoltaic_mgmt',
         'photovoltaic_participant_liquidations',
         'stock'
     ],
     'author': "Librecoop",
     'category': 'Sales',
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/es.po` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/i18n/photovoltaic_mgmt_extended.pot` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/i18n/photovoltaic_mgmt_extended.pot`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/models/photovoltaic_power_station.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/models/photovoltaic_power_station.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from odoo import models, fields
+from odoo import models, fields, tools
 
 
 class PhotovoltaicPowerStation(models.Model):
     _inherit = "photovoltaic.power.station"
 
     tecnical_memory_link = fields.Char(string="Enlace memoria técnica")
 
@@ -31,7 +31,18 @@
                 record.stock_quants = []
 
     def toggle_short_term(self):
         self.short_term_investment = not self.short_term_investment
 
     def toggle_long_term(self):
         self.long_term_investment = not self.long_term_investment
+
+    @tools.ormcache()
+    def _compute_installed_power(self):
+        plants = self.env['photovoltaic.power.station'].sudo().search([('name','!=','SDL')])
+        return round(sum(plants.mapped('peak_power')) / 1000, 2)
+
+    @tools.ormcache()
+    def _compute_plants_with_reservation(self):
+        plants_with_reservation = self.env['photovoltaic.power.station'].sudo().search(
+            [('reservation', '>=', 0)])
+        return len(plants_with_reservation)
```

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/account_allocation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/account_allocation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/contract_participation.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/contract_participation.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/photovoltaic_power_station.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/photovoltaic_power_station.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/res_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/views/res_partner_interest.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/views/res_partner_interest.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard.py` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/wizard/account_allocation_state_update_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.3/wizard/account_allocation_state_update_wizard_view.xml` & `odoo13-addon-photovoltaic_mgmt_extended-13.0.1.1.4/wizard/account_allocation_state_update_wizard_view.xml`

 * *Files identical despite different names*

