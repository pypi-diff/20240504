# Comparing `tmp/hnt_nf_jira_library-0.4.6.tar.gz` & `tmp/hnt_nf_jira_library-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.4.6.tar", last modified: Wed May  1 13:21:01 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.4.7.tar", last modified: Fri May  3 21:36:12 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.4.6.tar` & `hnt_nf_jira_library-0.4.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 13:21:01.983433 hnt_nf_jira_library-0.4.6/
--rw-rw-rw-   0        0        0      183 2024-05-01 13:21:01.982920 hnt_nf_jira_library-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 13:21:01.953866 hnt_nf_jira_library-0.4.6/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      183 2024-05-01 13:21:01.000000 hnt_nf_jira_library-0.4.6/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-05-01 13:21:01.000000 hnt_nf_jira_library-0.4.6/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 13:21:01.000000 hnt_nf_jira_library-0.4.6/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-01 13:21:01.000000 hnt_nf_jira_library-0.4.6/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-01 13:21:01.000000 hnt_nf_jira_library-0.4.6/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-01 13:21:01.956501 hnt_nf_jira_library-0.4.6/nf_jira/
--rw-rw-rw-   0        0        0       41 2024-04-26 20:27:31.000000 hnt_nf_jira_library-0.4.6/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 13:21:01.976710 hnt_nf_jira_library-0.4.6/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-23 21:17:37.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      131 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-05-01 13:21:01.981887 hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-22 11:49:00.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     3672 2024-04-30 11:22:42.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     7667 2024-04-30 11:22:42.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0      774 2024-04-26 20:18:01.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     3613 2024-04-30 11:22:42.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      593 2024-04-30 12:58:26.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      480 2024-04-30 16:57:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      793 2024-04-30 11:37:21.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      419 2024-04-30 16:35:09.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      485 2024-04-30 12:50:47.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      460 2024-04-30 16:56:32.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0     1167 2024-04-30 16:34:56.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 12:03:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-04-14 18:48:57.000000 hnt_nf_jira_library-0.4.6/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    16173 2024-04-30 16:55:31.000000 hnt_nf_jira_library-0.4.6/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-05-01 13:21:01.983947 hnt_nf_jira_library-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      468 2024-04-30 17:04:52.000000 hnt_nf_jira_library-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:36:12.825362 hnt_nf_jira_library-0.4.7/
+-rw-rw-rw-   0        0        0      240 2024-05-03 21:36:12.823360 hnt_nf_jira_library-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:36:12.821361 hnt_nf_jira_library-0.4.7/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      240 2024-05-03 21:36:12.000000 hnt_nf_jira_library-0.4.7/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-05-03 21:36:12.000000 hnt_nf_jira_library-0.4.7/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:36:12.000000 hnt_nf_jira_library-0.4.7/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-03 21:36:12.000000 hnt_nf_jira_library-0.4.7/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-03 21:36:12.000000 hnt_nf_jira_library-0.4.7/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 21:36:12.753502 hnt_nf_jira_library-0.4.7/nf_jira/
+-rw-rw-rw-   0        0        0       41 2024-04-30 14:47:20.000000 hnt_nf_jira_library-0.4.7/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:36:12.804979 hnt_nf_jira_library-0.4.7/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      131 2024-04-19 19:08:56.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:36:12.816929 hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-05-03 19:41:15.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     3672 2024-05-03 19:41:15.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2023 2024-05-03 21:34:52.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     7667 2024-05-03 19:41:15.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0      774 2024-04-30 14:47:20.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     3613 2024-05-03 19:41:15.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      593 2024-05-03 19:45:08.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      480 2024-05-03 19:45:08.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      793 2024-05-03 19:45:08.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      419 2024-05-03 19:45:08.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      485 2024-05-03 19:45:08.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      460 2024-05-03 19:45:08.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0     1167 2024-05-03 19:45:08.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.4.7/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    16173 2024-05-03 21:31:47.000000 hnt_nf_jira_library-0.4.7/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:36:12.826280 hnt_nf_jira_library-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      468 2024-05-03 21:35:56.000000 hnt_nf_jira_library-0.4.7/setup.py
```

### Comparing `hnt_nf_jira_library-0.4.6/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.4.7/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/issue_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         jira_fields_from_keys = {}
 
         for field_key in form_jira_keys:
 
             jira_key = form_jira_keys[field_key]
     
             if jira_key is not None:
-                field_value = jira_fields[jira_key]
+                field_value = jira_fields.get(jira_key)
                 if 'value' in field_value:
                     field_value = field_value['value']
             else:
                 field_value = None
 
             jira_fields_from_keys[field_key] = field_value if field_value else None
```

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/dados_basicos_fatura.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/dados_basicos_fatura.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/fatura.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/fatura.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/entities/nota_pedido.py` & `hnt_nf_jira_library-0.4.7/nf_jira/entities/nota_pedido.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.4.6/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.4.7/nf_jira/wrapper_nf_jira.py`

 * *Files identical despite different names*

