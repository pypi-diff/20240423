# Comparing `tmp/hnt_nf_jira_library-0.4.0.tar.gz` & `tmp/hnt_nf_jira_library-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.4.0.tar", last modified: Fri Apr 19 19:19:40 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.4.1.tar", last modified: Tue Apr 23 12:58:44 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.4.0.tar` & `hnt_nf_jira_library-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 19:19:40.149881 hnt_nf_jira_library-0.4.0/
--rw-rw-rw-   0        0        0      286 2024-04-19 19:19:40.145882 hnt_nf_jira_library-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 19:19:40.142881 hnt_nf_jira_library-0.4.0/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-19 19:19:39.000000 hnt_nf_jira_library-0.4.0/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-19 19:19:39.000000 hnt_nf_jira_library-0.4.0/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 19:19:39.000000 hnt_nf_jira_library-0.4.0/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-19 19:19:39.000000 hnt_nf_jira_library-0.4.0/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 19:19:39.000000 hnt_nf_jira_library-0.4.0/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 19:19:40.066876 hnt_nf_jira_library-0.4.0/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.4.0/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 19:19:40.123878 hnt_nf_jira_library-0.4.0/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      131 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-19 19:19:40.139880 hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     4338 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     5454 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     3411 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      234 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      354 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.0/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    15563 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.0/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-19 19:19:40.149881 hnt_nf_jira_library-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-19 19:09:21.000000 hnt_nf_jira_library-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.127407 hnt_nf_jira_library-0.4.1/
+-rw-rw-rw-   0        0        0      183 2024-04-23 12:58:44.127407 hnt_nf_jira_library-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.100893 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      183 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-04-23 12:58:44.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 12:58:43.000000 hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.102892 hnt_nf_jira_library-0.4.1/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-02-26 12:03:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.121892 hnt_nf_jira_library-0.4.1/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      131 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:58:44.126408 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     4338 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     5454 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     3411 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      234 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      448 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      354 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 12:03:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.1/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    15563 2024-04-23 12:55:45.000000 hnt_nf_jira_library-0.4.1/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 12:58:44.127407 hnt_nf_jira_library-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-23 12:58:04.000000 hnt_nf_jira_library-0.4.1/setup.py
```

### Comparing `hnt_nf_jira_library-0.4.0/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.4.1/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.0/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.4.1/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.0/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.4.1/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.0/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.4.1/nf_jira/wrapper_nf_jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
 
     def _prepare_ref(self, issue):
 
         data_ref = datetime.strptime(issue['json_data'][DATA_DE_REFERÊNCIA], "%m/%Y").strftime("%b/%y").upper()
 
         if issue['json_data'][COMPLEMENTO_DE_ÁGUA] is not None:
             
-            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataleituraAnterior'] is not None else None
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'] is not None else None
             leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'] is not None else None
         elif issue['json_data'][COMPLEMENTO_DE_ENERGIA] is not None:
             leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'] is not None else None
             leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'] is not None else None
         elif issue['json_data'][COMPLEMENTO_DE_GÁS] is not None:
             leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper() if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'] is not None else None
             leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()  if issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'] is not None else None
```

