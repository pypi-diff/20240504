# Comparing `tmp/netbox-contract-2.0.8.tar.gz` & `tmp/netbox-contract-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-contract-2.0.8.tar", last modified: Sun Sep  3 11:05:21 2023, max compression
+gzip compressed data, was "netbox-contract-2.0.9.tar", last modified: Fri Dec 15 21:42:05 2023, max compression
```

## Comparing `netbox-contract-2.0.8.tar` & `netbox-contract-2.0.9.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.987323 netbox-contract-2.0.8/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.8/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.8/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4712 2023-09-03 11:05:21.987323 netbox-contract-2.0.8/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4173 2023-09-03 07:35:01.000000 netbox-contract-2.0.8/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-09-03 07:35:01.000000 netbox-contract-2.0.8/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-09-03 11:05:21.987323 netbox-contract-2.0.8/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.8/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.963322 netbox-contract-2.0.8/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.967322 netbox-contract-2.0.8/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-09-03 07:35:01.000000 netbox-contract-2.0.8/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.975323 netbox-contract-2.0.8/src/netbox_contract/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4431 2023-09-03 08:33:50.000000 netbox-contract-2.0.8/src/netbox_contract/api/serializers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.8/src/netbox_contract/api/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      983 2023-06-18 15:21:49.000000 netbox-contract-2.0.8/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1434 2023-09-03 10:41:24.000000 netbox-contract-2.0.8/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7131 2023-09-03 10:41:30.000000 netbox-contract-2.0.8/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.983323 netbox-contract-2.0.8/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0015_contractassignement.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      630 2023-06-18 15:21:49.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0016_contract_parent.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-06-18 16:08:41.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5692 2023-06-18 16:08:41.000000 netbox-contract-2.0.8/src/netbox_contract/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2240 2023-06-18 13:35:02.000000 netbox-contract-2.0.8/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.8/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4292 2023-08-23 20:51:29.000000 netbox-contract-2.0.8/src/netbox_contract/tables.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2763 2023-09-03 11:03:34.000000 netbox-contract-2.0.8/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.983323 netbox-contract-2.0.8/src/netbox_contract/templates/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2566 2023-06-25 09:18:53.000000 netbox-contract-2.0.8/src/netbox_contract/templates/contact_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-18 13:30:49.000000 netbox-contract-2.0.8/src/netbox_contract/templates/contract_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-18 13:30:49.000000 netbox-contract-2.0.8/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.987323 netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4648 2023-09-03 08:33:50.000000 netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/contract_assignement.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2334 2023-09-03 08:33:50.000000 netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1136 2023-06-25 09:18:53.000000 netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3871 2023-06-21 19:25:05.000000 netbox-contract-2.0.8/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8640 2023-09-03 09:47:56.000000 netbox-contract-2.0.8/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-03 11:05:21.971322 netbox-contract-2.0.8/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4712 2023-09-03 11:05:21.000000 netbox-contract-2.0.8/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2339 2023-09-03 11:05:21.000000 netbox-contract-2.0.8/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-09-03 11:05:21.000000 netbox-contract-2.0.8/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-21 12:00:44.000000 netbox-contract-2.0.8/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-09-03 11:05:21.000000 netbox-contract-2.0.8/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-09-03 11:05:21.000000 netbox-contract-2.0.8/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.089381 netbox-contract-2.0.9/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.9/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.9/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-12-15 21:42:05.085381 netbox-contract-2.0.9/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4920 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-12-15 21:42:05.089381 netbox-contract-2.0.9/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.053381 netbox-contract-2.0.9/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.061381 netbox-contract-2.0.9/src/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.065381 netbox-contract-2.0.9/src/netbox_contract/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5036 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      388 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      979 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/api/views.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      185 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/constants.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1320 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/filtersets.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10398 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/forms.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.077381 netbox-contract-2.0.9/src/netbox_contract/migrations/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6090 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      856 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1578 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      600 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      583 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      562 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      402 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      385 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      427 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      493 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      603 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      338 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      548 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      421 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2103 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      629 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0016_contract_parent.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      415 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1386 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0018_contract_external_partie_object_id_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1382 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0019_auto_20230924_1813.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      623 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0020_alter_contract_external_partie.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      662 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0021_alter_contract_external_partie.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-12-15 21:38:43.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/0022_alter_contract_internal_partie_alter_contract_parent.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.9/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5642 2023-12-15 21:27:05.000000 netbox-contract-2.0.9/src/netbox_contract/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2192 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/search.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5365 2023-12-15 21:27:24.000000 netbox-contract-2.0.9/src/netbox_contract/tables.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3364 2023-12-15 21:11:25.000000 netbox-contract-2.0.9/src/netbox_contract/template_content.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.077381 netbox-contract-2.0.9/src/netbox_contract/templates/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2566 2023-06-25 09:18:53.000000 netbox-contract-2.0.9/src/netbox_contract/templates/contact_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-18 13:30:49.000000 netbox-contract-2.0.9/src/netbox_contract/templates/contract_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-18 13:30:49.000000 netbox-contract-2.0.9/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.085381 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4818 2023-12-15 21:28:15.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract_assignement.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2334 2023-09-03 08:33:50.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1136 2023-06-25 09:18:53.000000 netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4662 2023-12-15 20:52:55.000000 netbox-contract-2.0.9/src/netbox_contract/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9803 2023-12-15 21:38:42.000000 netbox-contract-2.0.9/src/netbox_contract/views.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-15 21:42:05.085381 netbox-contract-2.0.9/src/netbox_contract.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5490 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2745 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-11-12 14:38:39.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-12-15 21:42:05.000000 netbox-contract-2.0.9/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox-contract-2.0.8/LICENSE` & `netbox-contract-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.8/PKG-INFO` & `netbox-contract-2.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.8
+Version: 2.0.9
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
@@ -47,21 +48,26 @@
 Customize the location of the plugin's menu:
 
 
 ```python
 # configuration.py
 PLUGINS_CONFIG = {
     'netbox_contract': {
-        'top_level_menu': True
+        'top_level_menu': True,
+        'default_accounting_dimensions':{
+            "account": "", 
+            "project": "", 
+            "cost center": ""
+        }
     }
 }
 
 ```
 
-Customize the internal partie field.  
+Customize fields choices.  
 Internal partie reference the legal entity of your organization that is a partie to the contract.  
 
 ```python
 # configuration.py
 FIELD_CHOICES = {
     'netbox_contract.Contract.internal_partie': (
         ('Nagravision SARL', 'Nagravision SARL', 'green'),
@@ -127,7 +133,15 @@
 #### version 2.0.6
 * [#80](https://github.com/mlebreuil/netbox-contract/issues/80) Fix missing fields in the API.
 
 #### version 2.0.7
 * [#85](https://github.com/mlebreuil/netbox-contract/issues/85) Fix missing fields contract and invoice import and export forms.
 
 #### version 2.0.8
+* [#91](https://github.com/mlebreuil/netbox-contract/issues/91) Replace deprecated ( in netbox version 3.6) MultipleChoiceField.  
+* [48](https://github.com/mlebreuil/netbox-contract/issues/48) Allow other plugin to inject visual in contract and invoice forms.  
+* [89] (https://github.com/mlebreuil/netbox-contract/issues/89) Add contract assignement to virtual machines.
+
+#### version 2.0.9
+* [42](https://github.com/mlebreuil/netbox-contract/issues/42) Allow the selection of either providers or Service providers as contract third partie.
+* Removed all reference to the direct assignement of circuits to contracts
+
```

### Comparing `netbox-contract-2.0.8/README.md` & `netbox-contract-2.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -33,21 +33,26 @@
 Customize the location of the plugin's menu:
 
 
 ```python
 # configuration.py
 PLUGINS_CONFIG = {
     'netbox_contract': {
-        'top_level_menu': True
+        'top_level_menu': True,
+        'default_accounting_dimensions':{
+            "account": "", 
+            "project": "", 
+            "cost center": ""
+        }
     }
 }
 
 ```
 
-Customize the internal partie field.  
+Customize fields choices.  
 Internal partie reference the legal entity of your organization that is a partie to the contract.  
 
 ```python
 # configuration.py
 FIELD_CHOICES = {
     'netbox_contract.Contract.internal_partie': (
         ('Nagravision SARL', 'Nagravision SARL', 'green'),
@@ -113,7 +118,15 @@
 #### version 2.0.6
 * [#80](https://github.com/mlebreuil/netbox-contract/issues/80) Fix missing fields in the API.
 
 #### version 2.0.7
 * [#85](https://github.com/mlebreuil/netbox-contract/issues/85) Fix missing fields contract and invoice import and export forms.
 
 #### version 2.0.8
+* [#91](https://github.com/mlebreuil/netbox-contract/issues/91) Replace deprecated ( in netbox version 3.6) MultipleChoiceField.  
+* [48](https://github.com/mlebreuil/netbox-contract/issues/48) Allow other plugin to inject visual in contract and invoice forms.  
+* [89] (https://github.com/mlebreuil/netbox-contract/issues/89) Add contract assignement to virtual machines.
+
+#### version 2.0.9
+* [42](https://github.com/mlebreuil/netbox-contract/issues/42) Allow the selection of either providers or Service providers as contract third partie.
+* Removed all reference to the direct assignement of circuits to contracts
+
```

### Comparing `netbox-contract-2.0.8/pyproject.toml` & `netbox-contract-2.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netbox-contract"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -26,8 +26,14 @@
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["*"]
-namespaces = false
+namespaces = false
+
+[tool.black]
+skip-string-normalization = true
+
+[tool.isort]
+profile = "black"
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/api/views.py` & `netbox-contract-2.0.9/src/netbox_contract/api/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import filtersets, models
-from .serializers import ContractSerializer, InvoiceSerializer, ServiceProviderSerializer, ContractAssignementSerializer
+from .serializers import (
+    ContractAssignementSerializer,
+    ContractSerializer,
+    InvoiceSerializer,
+    ServiceProviderSerializer,
+)
+
 
 class ContractViewSet(NetBoxModelViewSet):
-    queryset = models.Contract.objects.prefetch_related(
-        'parent','circuit','tags'
-        )
+    queryset = models.Contract.objects.prefetch_related('parent', 'circuit', 'tags')
     serializer_class = ContractSerializer
 
+
 class InvoiceViewSet(NetBoxModelViewSet):
-    queryset = models.Invoice.objects.prefetch_related(
-        'contracts', 'tags'
-    )
+    queryset = models.Invoice.objects.prefetch_related('contracts', 'tags')
     serializer_class = InvoiceSerializer
     filterset_class = filtersets.InvoiceFilterSet
 
+
 class ServiceProviderViewSet(NetBoxModelViewSet):
     queryset = models.ServiceProvider.objects.prefetch_related('tags')
     serializer_class = ServiceProviderSerializer
 
+
 class ContractAssignementViewSet(NetBoxModelViewSet):
-    queryset = models.ContractAssignement.objects.prefetch_related('contract','tags')
+    queryset = models.ContractAssignement.objects.prefetch_related('contract', 'tags')
     serializer_class = ContractAssignementSerializer
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/filtersets.py` & `netbox-contract-2.0.9/src/netbox_contract/filtersets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-
 from django.db.models import Q
 from netbox.filtersets import NetBoxModelFilterSet
-from .models import Contract,Invoice,ServiceProvider,ContractAssignement
 
-class ContractFilterSet(NetBoxModelFilterSet):
+from .models import Contract, ContractAssignement, Invoice, ServiceProvider
+
 
+class ContractFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = Contract
-        fields = ('id', 'external_partie', 'internal_partie', 'status','parent')
+        fields = ('id', 'internal_partie', 'status', 'parent')
 
     def search(self, queryset, name, value):
-        return queryset.filter( Q(name__icontains=value)
-                               | Q(external_partie__name__icontains=value)
-                               | Q(external_reference__icontains=value)
-                               | Q(comments__icontains=value))
+        return queryset.filter(
+            Q(name__icontains=value)
+            | Q(external_reference__icontains=value)
+            | Q(comments__icontains=value)
+        )
 
-class InvoiceFilterSet(NetBoxModelFilterSet):
 
+class InvoiceFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = Invoice
         fields = ('id', 'contracts')
 
     def search(self, queryset, name, value):
-        return queryset.filter(Q(number__icontains=value)
-                               | Q(contracts__name__icontains=value))
+        return queryset.filter(
+            Q(number__icontains=value) | Q(contracts__name__icontains=value)
+        )
 
-class ServiceProviderFilterSet(NetBoxModelFilterSet):
 
+class ServiceProviderFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = ServiceProvider
-        fields = ('id','name')
+        fields = ('id', 'name')
 
     def search(self, queryset, name, value):
         return queryset.filter(name__icontains=value)
 
-class ContractAssignementFilterSet(NetBoxModelFilterSet):
 
+class ContractAssignementFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = ContractAssignement
-        fields = ('id','contract')
+        fields = ('id', 'contract')
 
     def search(self, queryset, name, value):
         return queryset.filter(Q(contract__name__icontains=value))
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0001_initial.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,165 @@
 # Generated by Django 4.0.8 on 2023-01-03 21:49
 
 import django.core.serializers.json
-from django.db import migrations, models
 import django.db.models.deletion
 import taggit.managers
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ('extras', '0077_customlink_extend_text_and_url'),
         ('circuits', '0038_cabling_cleanup'),
         ('tenancy', '0007_contact_link'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Contract',
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
+                (
+                    'id',
+                    models.BigAutoField(
+                        auto_created=True, primary_key=True, serialize=False
+                    ),
+                ),
                 ('created', models.DateTimeField(auto_now_add=True, null=True)),
                 ('last_updated', models.DateTimeField(auto_now=True, null=True)),
-                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
+                (
+                    'custom_field_data',
+                    models.JSONField(
+                        blank=True,
+                        default=dict,
+                        encoder=django.core.serializers.json.DjangoJSONEncoder,
+                    ),
+                ),
                 ('name', models.CharField(max_length=100)),
                 ('internal_partie', models.CharField(default='Active', max_length=50)),
                 ('status', models.CharField(default='Active', max_length=50)),
                 ('start_date', models.DateField()),
                 ('initial_term', models.IntegerField(default=12)),
                 ('renewal_term', models.IntegerField(default=12)),
                 ('mrc', models.DecimalField(decimal_places=2, max_digits=10)),
-                ('nrc', models.DecimalField(decimal_places=2, default=0, max_digits=10)),
+                (
+                    'nrc',
+                    models.DecimalField(decimal_places=2, default=0, max_digits=10),
+                ),
                 ('invoice_frequency', models.IntegerField(default=1)),
                 ('comments', models.TextField(blank=True)),
-                ('circuit', models.ManyToManyField(related_name='contract', to='circuits.circuit')),
+                (
+                    'circuit',
+                    models.ManyToManyField(
+                        related_name='contract', to='circuits.circuit'
+                    ),
+                ),
             ],
             options={
                 'ordering': ('name',),
             },
         ),
         migrations.CreateModel(
             name='ServiceProvider',
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
+                (
+                    'id',
+                    models.BigAutoField(
+                        auto_created=True, primary_key=True, serialize=False
+                    ),
+                ),
                 ('created', models.DateTimeField(auto_now_add=True, null=True)),
                 ('last_updated', models.DateTimeField(auto_now=True, null=True)),
-                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
+                (
+                    'custom_field_data',
+                    models.JSONField(
+                        blank=True,
+                        default=dict,
+                        encoder=django.core.serializers.json.DjangoJSONEncoder,
+                    ),
+                ),
                 ('name', models.CharField(max_length=100)),
                 ('slug', models.SlugField(max_length=100, unique=True)),
                 ('portal_url', models.URLField(blank=True)),
                 ('comments', models.TextField(blank=True)),
-                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
+                (
+                    'tags',
+                    taggit.managers.TaggableManager(
+                        through='extras.TaggedItem', to='extras.Tag'
+                    ),
+                ),
             ],
             options={
                 'ordering': ('name',),
             },
         ),
         migrations.CreateModel(
             name='Invoice',
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
+                (
+                    'id',
+                    models.BigAutoField(
+                        auto_created=True, primary_key=True, serialize=False
+                    ),
+                ),
                 ('created', models.DateTimeField(auto_now_add=True, null=True)),
                 ('last_updated', models.DateTimeField(auto_now=True, null=True)),
-                ('custom_field_data', models.JSONField(blank=True, default=dict, encoder=django.core.serializers.json.DjangoJSONEncoder)),
+                (
+                    'custom_field_data',
+                    models.JSONField(
+                        blank=True,
+                        default=dict,
+                        encoder=django.core.serializers.json.DjangoJSONEncoder,
+                    ),
+                ),
                 ('number', models.CharField(max_length=100)),
                 ('period_start', models.DateField()),
                 ('period_end', models.DateField()),
                 ('amount', models.DecimalField(decimal_places=2, max_digits=10)),
-                ('contract', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='invoice', to='netbox_contract.contract')),
-                ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
+                (
+                    'contract',
+                    models.ForeignKey(
+                        on_delete=django.db.models.deletion.CASCADE,
+                        related_name='invoice',
+                        to='netbox_contract.contract',
+                    ),
+                ),
+                (
+                    'tags',
+                    taggit.managers.TaggableManager(
+                        through='extras.TaggedItem', to='extras.Tag'
+                    ),
+                ),
             ],
             options={
                 'ordering': ('-period_start',),
             },
         ),
         migrations.AddField(
             model_name='contract',
             name='external_partie',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='contract', to='netbox_contract.serviceprovider'),
+            field=models.ForeignKey(
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name='contract',
+                to='netbox_contract.serviceprovider',
+            ),
         ),
         migrations.AddField(
             model_name='contract',
             name='tags',
-            field=taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag'),
+            field=taggit.managers.TaggableManager(
+                through='extras.TaggedItem', to='extras.Tag'
+            ),
         ),
         migrations.AddField(
             model_name='contract',
             name='tenant',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='contracts', to='tenancy.tenant'),
+            field=models.ForeignKey(
+                blank=True,
+                null=True,
+                on_delete=django.db.models.deletion.PROTECT,
+                related_name='contracts',
+                to='tenancy.tenant',
+            ),
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0016_contract_parent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-# Generated by Django 4.0.8 on 2023-01-03 23:22
+# Generated by Django 4.1.9 on 2023-06-18 14:45
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('circuits', '0038_cabling_cleanup'),
-        ('netbox_contract', '0001_initial'),
+        ('netbox_contract', '0015_contractassignement'),
     ]
 
     operations = [
-        migrations.AlterField(
-            model_name='contract',
-            name='circuit',
-            field=models.ManyToManyField(related_name='contracts', to='circuits.circuit'),
-        ),
-        migrations.AlterField(
+        migrations.AddField(
             model_name='contract',
-            name='external_partie',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='contracts', to='netbox_contract.serviceprovider'),
+            name='parent',
+            field=models.ForeignKey(
+                blank=True,
+                null=True,
+                on_delete=django.db.models.deletion.CASCADE,
+                related_name='child',
+                to='netbox_contract.contract',
+            ),
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 # Generated by Django 4.1.5 on 2023-01-15 09:18
 
-from django.db import migrations, models
 import utilities.json
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("netbox_contract", "0002_alter_contract_circuit_and_more"),
+        ('netbox_contract', '0002_alter_contract_circuit_and_more'),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name="contract",
-            name="custom_field_data",
+            model_name='contract',
+            name='custom_field_data',
             field=models.JSONField(
                 blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder
             ),
         ),
         migrations.AlterField(
-            model_name="contract",
-            name="initial_term",
+            model_name='contract',
+            name='initial_term',
             field=models.IntegerField(blank=True, default=12, null=True),
         ),
         migrations.AlterField(
-            model_name="contract",
-            name="renewal_term",
+            model_name='contract',
+            name='renewal_term',
             field=models.IntegerField(blank=True, default=12, null=True),
         ),
         migrations.AlterField(
-            model_name="contract",
-            name="start_date",
+            model_name='contract',
+            name='start_date',
             field=models.DateField(blank=True, null=True),
         ),
         migrations.AlterField(
-            model_name="invoice",
-            name="custom_field_data",
+            model_name='invoice',
+            name='custom_field_data',
             field=models.JSONField(
                 blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder
             ),
         ),
         migrations.AlterField(
-            model_name="serviceprovider",
-            name="custom_field_data",
+            model_name='serviceprovider',
+            name='custom_field_data',
             field=models.JSONField(
                 blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder
             ),
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Generated by Django 4.1.5 on 2023-01-15 09:57
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("netbox_contract", "0003_alter_contract_custom_field_data_and_more"),
+        ('netbox_contract', '0003_alter_contract_custom_field_data_and_more'),
     ]
 
     operations = [
         migrations.AddField(
-            model_name="contract",
-            name="currency",
-            field=models.CharField(default="usd", max_length=3),
+            model_name='contract',
+            name='currency',
+            field=models.CharField(default='usd', max_length=3),
         ),
         migrations.AddField(
-            model_name="invoice",
-            name="currency",
-            field=models.CharField(default="usd", max_length=3),
+            model_name='invoice',
+            name='currency',
+            field=models.CharField(default='usd', max_length=3),
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Generated by Django 4.1.5 on 2023-01-15 10:32
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("netbox_contract", "0004_contract_currency_invoice_currency"),
+        ('netbox_contract', '0004_contract_currency_invoice_currency'),
     ]
 
     operations = [
         migrations.AddField(
-            model_name="contract",
-            name="accounting_dimensions",
+            model_name='contract',
+            name='accounting_dimensions',
             field=models.JSONField(null=True),
         ),
         migrations.AddField(
-            model_name="invoice",
-            name="accounting_dimensions",
+            model_name='invoice',
+            name='accounting_dimensions',
             field=models.JSONField(null=True),
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Generated by Django 4.1.5 on 2023-01-22 09:49
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("circuits", "0041_standardize_description_comments"),
-        ("netbox_contract", "0005_contract_accounting_dimensions_and_more"),
+        ('circuits', '0041_standardize_description_comments'),
+        ('netbox_contract', '0005_contract_accounting_dimensions_and_more'),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name="contract",
-            name="circuit",
+            model_name='contract',
+            name='circuit',
             field=models.ManyToManyField(
-                blank=True, related_name="contracts", to="circuits.circuit"
+                blank=True, related_name='contracts', to='circuits.circuit'
             ),
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Generated by Django 4.1.5 on 2023-01-22 21:12
 
 from django.db import migrations
 
+
 def make_many_contracts(apps, schema_editor):
     """
-        Adds the Contract object in Invoice.contract to the
-        many-to-many relationship in Invoice.contracts
+    Adds the Contract object in Invoice.contract to the
+    many-to-many relationship in Invoice.contracts
     """
     Invoice = apps.get_model('netbox_contract', 'Invoice')
 
     for invoice in Invoice.objects.all():
         invoice.contracts.add(invoice.contract)
 
-class Migration(migrations.Migration):
 
+class Migration(migrations.Migration):
     dependencies = [
-        ("netbox_contract", "0010_invoice_contracts"),
+        ('netbox_contract', '0010_invoice_contracts'),
     ]
 
     operations = [
         migrations.RunPython(make_many_contracts),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Generated by Django 4.1.5 on 2023-01-30 21:06
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("netbox_contract", "0012_remove_invoice_contract"),
+        ('netbox_contract', '0012_remove_invoice_contract'),
     ]
 
     operations = [
         migrations.AddField(
-            model_name="contract",
-            name="documents",
+            model_name='contract',
+            name='documents',
             field=models.URLField(blank=True),
         ),
         migrations.AddField(
-            model_name="invoice",
-            name="documents",
+            model_name='invoice',
+            name='documents',
             field=models.URLField(blank=True),
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/migrations/0015_contractassignement.py` & `netbox-contract-2.0.9/src/netbox_contract/migrations/0015_contractassignement.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 # Generated by Django 4.1.7 on 2023-05-13 17:53
 
-from django.db import migrations, models
 import django.db.models.deletion
 import taggit.managers
 import utilities.json
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ("extras", "0084_staging"),
-        ("contenttypes", "0002_remove_content_type_name"),
-        ("netbox_contract", "0014_contract_end_date"),
+        ('extras', '0084_staging'),
+        ('contenttypes', '0002_remove_content_type_name'),
+        ('netbox_contract', '0014_contract_end_date'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name="ContractAssignement",
+            name='ContractAssignement',
             fields=[
                 (
-                    "id",
+                    'id',
                     models.BigAutoField(
                         auto_created=True, primary_key=True, serialize=False
                     ),
                 ),
-                ("created", models.DateTimeField(auto_now_add=True, null=True)),
-                ("last_updated", models.DateTimeField(auto_now=True, null=True)),
+                ('created', models.DateTimeField(auto_now_add=True, null=True)),
+                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
                 (
-                    "custom_field_data",
+                    'custom_field_data',
                     models.JSONField(
                         blank=True,
                         default=dict,
                         encoder=utilities.json.CustomFieldJSONEncoder,
                     ),
                 ),
-                ("object_id", models.PositiveBigIntegerField()),
+                ('object_id', models.PositiveBigIntegerField()),
                 (
-                    "content_type",
+                    'content_type',
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE,
-                        to="contenttypes.contenttype",
+                        to='contenttypes.contenttype',
                     ),
                 ),
                 (
-                    "contract",
+                    'contract',
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="assignments",
-                        to="netbox_contract.contract",
+                        related_name='assignments',
+                        to='netbox_contract.contract',
                     ),
                 ),
                 (
-                    "tags",
+                    'tags',
                     taggit.managers.TaggableManager(
-                        through="extras.TaggedItem", to="extras.Tag"
+                        through='extras.TaggedItem', to='extras.Tag'
                     ),
                 ),
             ],
             options={
-                "ordering": ("contract",),
+                'ordering': ('contract',),
             },
         ),
     ]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/models.py` & `netbox-contract-2.0.9/src/netbox_contract/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,233 +1,178 @@
-from django.contrib.postgres.fields import ArrayField
+from circuits.models import Circuit
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.contrib.contenttypes.models import ContentType
-from django.urls import reverse
 from django.db import models
-from utilities.choices import ChoiceSet
+from django.urls import reverse
 from netbox.models import NetBoxModel
-from circuits.models import Circuit
+from utilities.choices import ChoiceSet
+
 
 class StatusChoices(ChoiceSet):
     key = 'Contract.status'
 
     STATUS_ACTIVE = 'Active'
     STATUS_CANCELED = 'Cancled'
 
     CHOICES = [
         (STATUS_ACTIVE, 'Active', 'green'),
         (STATUS_CANCELED, 'Canceled', 'red'),
     ]
 
+
 class InternalEntityChoices(ChoiceSet):
     key = 'Contract.internal_partie'
 
     ENTITY = 'Default entity'
 
     CHOICES = [
         (ENTITY, 'Default entity', 'green'),
     ]
 
+
 class CurrencyChoices(ChoiceSet):
     key = 'Contract.currency'
     CURRENCY_USD = 'usd'
 
     CHOICES = [
         (CURRENCY_USD, 'USD'),
         ('eur', 'EUR'),
         ('chf', 'CHF'),
     ]
 
+
 class ServiceProvider(NetBoxModel):
-    name = models.CharField(
-        max_length=100
-    )
-    slug = models.SlugField(
-        max_length=100,
-        unique=True
-    )
-    contacts = GenericRelation(
-        to='tenancy.ContactAssignment'
-    )
-    portal_url = models.URLField(
-        blank=True,
-        verbose_name='Portal URL'
-    )
-    comments = models.TextField(
-        blank=True
-    )
+    name = models.CharField(max_length=100)
+    slug = models.SlugField(max_length=100, unique=True)
+    contacts = GenericRelation(to='tenancy.ContactAssignment')
+    portal_url = models.URLField(blank=True, verbose_name='Portal URL')
+    comments = models.TextField(blank=True)
 
     class Meta:
         ordering = ('name',)
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_contract:serviceprovider', args=[self.pk])
 
+
 class ContractAssignement(NetBoxModel):
-    content_type = models.ForeignKey(
-        to=ContentType,
-        on_delete=models.CASCADE
-    )
+    content_type = models.ForeignKey(to=ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveBigIntegerField()
-    content_object = GenericForeignKey(
-        ct_field='content_type',
-        fk_field='object_id'
-    )
+    content_object = GenericForeignKey(ct_field='content_type', fk_field='object_id')
     contract = models.ForeignKey(
-        to='Contract',
-        on_delete=models.PROTECT,
-        related_name='assignments'
+        to='Contract', on_delete=models.PROTECT, related_name='assignments'
     )
-    clone_fields = ('content_type', 'object_id','contract')
+    clone_fields = ('content_type', 'object_id', 'contract')
 
     class Meta:
         ordering = ('contract',)
+        indexes = [
+            models.Index(fields=['content_type', 'object_id']),
+        ]
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_contract:contractassignement', args=[self.pk])
 
+
 class Contract(NetBoxModel):
-    name = models.CharField(
-        max_length=100
-    )
+    name = models.CharField(max_length=100)
     external_partie = models.ForeignKey(
         to=ServiceProvider,
         on_delete=models.CASCADE,
-        related_name='contracts'
-    )
-    external_reference = models.CharField(
-        max_length=100,
+        related_name='contracts',
         blank=True,
-        null=True
+        null=True,
     )
+
+    external_partie_object_type = models.ForeignKey(
+        to=ContentType, on_delete=models.CASCADE, blank=True, null=True
+    )
+    external_partie_object_id = models.PositiveBigIntegerField(blank=True, null=True)
+    external_partie_object = GenericForeignKey(
+        ct_field='external_partie_object_type', fk_field='external_partie_object_id'
+    )
+
+    external_reference = models.CharField(max_length=100, blank=True, null=True)
     internal_partie = models.CharField(
         max_length=50,
         choices=InternalEntityChoices,
-        default=StatusChoices.STATUS_ACTIVE
     )
     tenant = models.ForeignKey(
         to='tenancy.Tenant',
         on_delete=models.PROTECT,
         related_name='contracts',
         blank=True,
-        null=True
+        null=True,
     )
     status = models.CharField(
-        max_length=50,
-        choices=StatusChoices,
-        default=StatusChoices.STATUS_ACTIVE
-    )
-    start_date = models.DateField(
-        blank=True,
-        null=True
-    )
-    end_date = models.DateField(
-        blank=True,
-        null=True
+        max_length=50, choices=StatusChoices, default=StatusChoices.STATUS_ACTIVE
     )
+    start_date = models.DateField(blank=True, null=True)
+    end_date = models.DateField(blank=True, null=True)
     initial_term = models.IntegerField(
-        help_text = "In month",
-        default = 12,
-        blank=True,
-        null=True
+        help_text='In month', default=12, blank=True, null=True
     )
     renewal_term = models.IntegerField(
-        help_text = "In month",
-        default = 12,
-        blank=True,
-        null=True
+        help_text='In month', default=12, blank=True, null=True
     )
     currency = models.CharField(
-        max_length=3,
-        choices=CurrencyChoices,
-        default=CurrencyChoices.CURRENCY_USD
-    )
-    accounting_dimensions = models.JSONField(
-        null=True,
-        blank=True
+        max_length=3, choices=CurrencyChoices, default=CurrencyChoices.CURRENCY_USD
     )
+    accounting_dimensions = models.JSONField(null=True, blank=True)
     mrc = models.DecimalField(
-        verbose_name = "Monthly recuring cost",
-        max_digits = 10,
-        decimal_places= 2
+        verbose_name='Monthly recuring cost', max_digits=10, decimal_places=2
     )
     nrc = models.DecimalField(
-        verbose_name = "None recuring cost",
-        default = 0,
-        max_digits = 10,
-        decimal_places= 2
+        verbose_name='None recuring cost', default=0, max_digits=10, decimal_places=2
     )
     invoice_frequency = models.IntegerField(
-        help_text = "The frequency of invoices in month",
-        default = 1
-    )
-    circuit = models.ManyToManyField(Circuit,
-        related_name='contracts',
-        blank=True
-    )
-    documents = models.URLField(
-        blank=True
-    )
-    comments = models.TextField(
-        blank=True
+        help_text='The frequency of invoices in month', default=1
     )
+    circuit = models.ManyToManyField(Circuit, related_name='contracts', blank=True)
+    documents = models.URLField(blank=True)
+    comments = models.TextField(blank=True)
     parent = models.ForeignKey(
-        'self',
-        on_delete=models.CASCADE,
-        related_name='child',
-        null=True,
-        blank=True
+        'self', on_delete=models.CASCADE, related_name='childs', null=True, blank=True
     )
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_contract:contract', args=[self.pk])
 
     class Meta:
         ordering = ('name',)
+        indexes = [
+            models.Index(
+                fields=['external_partie_object_type', 'external_partie_object_id']
+            ),
+        ]
 
     def __str__(self):
         return self.name
 
 
 class Invoice(NetBoxModel):
-    number = models.CharField(
-        max_length=100
-    )
-    date = models.DateField(
-        blank=True,
-        null=True
-    )
+    number = models.CharField(max_length=100)
+    date = models.DateField(blank=True, null=True)
     contracts = models.ManyToManyField(
         Contract,
         related_name='invoices',
         blank=True,
     )
     period_start = models.DateField()
     period_end = models.DateField()
     currency = models.CharField(
-        max_length=3,
-        choices=CurrencyChoices,
-        default=CurrencyChoices.CURRENCY_USD
-    )
-    accounting_dimensions = models.JSONField(
-        null=True
-    )
-    amount = models.DecimalField(
-        max_digits = 10,
-        decimal_places= 2
-    )
-    documents = models.URLField(
-        blank=True
-    )
-    comments = models.TextField(
-        blank=True
+        max_length=3, choices=CurrencyChoices, default=CurrencyChoices.CURRENCY_USD
     )
+    accounting_dimensions = models.JSONField(null=True)
+    amount = models.DecimalField(max_digits=10, decimal_places=2)
+    documents = models.URLField(blank=True)
+    comments = models.TextField(blank=True)
 
     class Meta:
         ordering = ('-period_start',)
 
     def __str__(self):
         return self.number
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/navigation.py` & `netbox-contract-2.0.9/src/netbox_contract/navigation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,77 @@
 from django.conf import settings
 from extras.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
 from utilities.choices import ButtonColorChoices
 
-plugin_settings = settings.PLUGINS_CONFIG["netbox_contract"]
+plugin_settings = settings.PLUGINS_CONFIG['netbox_contract']
 
 contract_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:contract_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN,
-        permissions=['netbox_contract.add_contract']
+        permissions=['netbox_contract.add_contract'],
     )
 ]
 
 invoice_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:invoice_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN,
-        permissions=['netbox_contract.add_invoice']
+        permissions=['netbox_contract.add_invoice'],
     )
 ]
 
 serviceprovider_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:serviceprovider_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN,
-        permissions=['netbox_contract.add_serviceprovider']
+        permissions=['netbox_contract.add_serviceprovider'],
     )
 ]
 
 contract_menu_item = PluginMenuItem(
-        link='plugins:netbox_contract:contract_list',
-        link_text='Contracts',
-        buttons=contract_buttons,
-        permissions=['netbox_contract.view_contract']
-    )
+    link='plugins:netbox_contract:contract_list',
+    link_text='Contracts',
+    buttons=contract_buttons,
+    permissions=['netbox_contract.view_contract'],
+)
 
 invoices_menu_item = PluginMenuItem(
-        link='plugins:netbox_contract:invoice_list',
-        link_text='Invoices',
-        buttons=invoice_buttons,
-        permissions=['netbox_contract.view_invoice']
-    )
+    link='plugins:netbox_contract:invoice_list',
+    link_text='Invoices',
+    buttons=invoice_buttons,
+    permissions=['netbox_contract.view_invoice'],
+)
 
 service_provider_menu_item = PluginMenuItem(
-        link='plugins:netbox_contract:serviceprovider_list',
-        link_text='Service Providers',
-        buttons=serviceprovider_buttons,
-        permissions=['netbox_contract.view_serviceprovider']
-    )
+    link='plugins:netbox_contract:serviceprovider_list',
+    link_text='Service Providers',
+    buttons=serviceprovider_buttons,
+    permissions=['netbox_contract.view_serviceprovider'],
+)
 contract_assignemnt_menu_item = PluginMenuItem(
-        link='plugins:netbox_contract:contractassignement_list',
-        link_text='Contract assignements',
-        permissions=['netbox_contract.view_contractassignement']
-    )
-
-items = (contract_menu_item,invoices_menu_item,service_provider_menu_item, contract_assignemnt_menu_item)
+    link='plugins:netbox_contract:contractassignement_list',
+    link_text='Contract assignements',
+    permissions=['netbox_contract.view_contractassignement'],
+)
+
+items = (
+    contract_menu_item,
+    invoices_menu_item,
+    service_provider_menu_item,
+    contract_assignemnt_menu_item,
+)
 
-if plugin_settings.get("top_level_menu"):
+if plugin_settings.get('top_level_menu'):
     menu = PluginMenu(
-        label="Contracts",
-        groups=(("Contracts", items),),
-        icon_class="mdi mdi-file-sign",
+        label='Contracts',
+        groups=(('Contracts', items),),
+        icon_class='mdi mdi-file-sign',
     )
 else:
     menu_items = items
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/search.py` & `netbox-contract-2.0.9/src/netbox_contract/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from netbox.search import SearchIndex, register_search
-from .models import ServiceProvider, Contract, Invoice
+
+from .models import Contract, Invoice, ServiceProvider
+
 
 @register_search
 class ServiceProviderIndex(SearchIndex):
     model = ServiceProvider
     fields = (
         ('name', 100),
         ('comments', 5000),
     )
 
+
 @register_search
 class ContractIndex(SearchIndex):
     model = Contract
     fields = (
         ('name', 100),
         ('comments', 5000),
     )
 
+
 @register_search
 class InvoiceIndex(SearchIndex):
     model = Invoice
     fields = (
         ('number', 100),
         ('comments', 5000),
     )
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/template_content.py` & `netbox-contract-2.0.9/src/netbox_contract/template_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,104 @@
+from circuits.models import Circuit
+from dcim.models import Device, Site
 from django.contrib.contenttypes.models import ContentType
 from extras.plugins import PluginTemplateExtension
-from circuits.models import Circuit
-from dcim.models import Device
 from virtualization.models import VirtualMachine
-from .models import ContractAssignement
-from . import tables
-
-class CircuitContracts(PluginTemplateExtension):
-    model = 'circuits.circuit'
 
-    def full_width_page(self):
-        circuit = self.context['object']
-        table = tables.ContractListBottomTable(circuit.contracts.all())
-        table.configure(self.context['request'])
+from . import tables
+from .models import ContractAssignement
 
-        return self.render('contract_list_bottom.html', extra_context={
-            'contracts_table': table,
-        })
 
 class CircuitContractAssignements(PluginTemplateExtension):
     model = 'circuits.circuit'
 
     def full_width_page(self):
         circuit = self.context['object']
         circuit_type = ContentType.objects.get_for_model(Circuit)
-        contract_assignements = ContractAssignement.objects.filter(content_type__pk=circuit_type.id, object_id=circuit.id)
-        assignements_table = tables.ContractAssignementObjectTable(contract_assignements)
+        contract_assignements = ContractAssignement.objects.filter(
+            content_type__pk=circuit_type.id, object_id=circuit.id
+        )
+        assignements_table = tables.ContractAssignementObjectTable(
+            contract_assignements
+        )
         assignements_table.configure(self.context['request'])
 
-        return self.render('contract_assignements_bottom.html', extra_context={
-            'assignements_table': assignements_table,
-        })
+        return self.render(
+            'contract_assignements_bottom.html',
+            extra_context={
+                'assignements_table': assignements_table,
+            },
+        )
+
 
 class DeviceContractAssignements(PluginTemplateExtension):
     model = 'dcim.device'
 
     def full_width_page(self):
         device = self.context['object']
         device_type = ContentType.objects.get_for_model(Device)
-        contract_assignements = ContractAssignement.objects.filter(content_type__pk=device_type.id, object_id=device.id)
-        assignements_table = tables.ContractAssignementObjectTable(contract_assignements)
+        contract_assignements = ContractAssignement.objects.filter(
+            content_type__pk=device_type.id, object_id=device.id
+        )
+        assignements_table = tables.ContractAssignementObjectTable(
+            contract_assignements
+        )
         assignements_table.configure(self.context['request'])
 
-        return self.render('contract_assignements_bottom.html', extra_context={
-            'assignements_table': assignements_table,
-        })
+        return self.render(
+            'contract_assignements_bottom.html',
+            extra_context={
+                'assignements_table': assignements_table,
+            },
+        )
+
 
 class VMContractAssignements(PluginTemplateExtension):
     model = 'virtualization.virtualmachine'
 
     def full_width_page(self):
-        device = self.context['object']
-        device_type = ContentType.objects.get_for_model(VirtualMachine)
-        contract_assignements = ContractAssignement.objects.filter(content_type__pk=device_type.id, object_id=device.id)
-        assignements_table = tables.ContractAssignementObjectTable(contract_assignements)
+        vm = self.context['object']
+        vm_type = ContentType.objects.get_for_model(VirtualMachine)
+        contract_assignements = ContractAssignement.objects.filter(
+            content_type__pk=vm_type.id, object_id=vm.id
+        )
+        assignements_table = tables.ContractAssignementObjectTable(
+            contract_assignements
+        )
+        assignements_table.configure(self.context['request'])
+
+        return self.render(
+            'contract_assignements_bottom.html',
+            extra_context={
+                'assignements_table': assignements_table,
+            },
+        )
+
+
+class SiteContractAssignements(PluginTemplateExtension):
+    model = 'dcim.site'
+
+    def full_width_page(self):
+        site = self.context['object']
+        site_type = ContentType.objects.get_for_model(Site)
+        contract_assignements = ContractAssignement.objects.filter(
+            content_type__pk=site_type.id, object_id=site.id
+        )
+        assignements_table = tables.ContractAssignementObjectTable(
+            contract_assignements
+        )
         assignements_table.configure(self.context['request'])
 
-        return self.render('contract_assignements_bottom.html', extra_context={
-            'assignements_table': assignements_table,
-        })
+        return self.render(
+            'contract_assignements_bottom.html',
+            extra_context={
+                'assignements_table': assignements_table,
+            },
+        )
+
 
-template_extensions = [ CircuitContracts, CircuitContractAssignements, DeviceContractAssignements, VMContractAssignements]
+template_extensions = [
+    CircuitContractAssignements,
+    DeviceContractAssignements,
+    VMContractAssignements,
+    SiteContractAssignements,
+]
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/templates/contact_assignements_bottom.html` & `netbox-contract-2.0.9/src/netbox_contract/templates/contact_assignements_bottom.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.8/src/netbox_contract/templates/contract_assignements_bottom.html` & `netbox-contract-2.0.9/src/netbox_contract/templates/contract_assignements_bottom.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,22 @@
         <h5 class="card-header">Contract</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
+                <tr>
+              <th scope="row">External partie type</th>
+              <td>{{ object.external_partie_object_type }}</td>
+            </tr>
             <tr>
               <th scope="row">External partie</th>
               <td>
-                <a href="{{ object.external_partie.get_absolute_url }}">{{ object.external_partie.name }}</a>
+                <a href="{{ object.external_partie_object.get_absolute_url }}">{{ object.external_partie_object.name }}</a>
               </td>
             </tr>
             <tr>
               <th scope="row">Status</th>
               <td>{{ object.status }}</td>
             </tr>
             <tr>
@@ -97,27 +101,27 @@
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Circuits</h5>
+        <h5 class="card-header">Assignements</h5>
         <div class="card-body table-responsive">
-          {% render_table circuit_table %}
+          {% render_table assignements_table %}
         </div>
       </div>
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Assignements</h5>
+        <h5 class="card-header">childs</h5>
         <div class="card-body table-responsive">
-          {% render_table assignements_table %}
+          {% render_table childs_table %}
         </div>
       </div>
     </div>
   </div>
   {% if perms.netbox_contract.view_invoice %}
   <div class="row">
     <div class="col col-md-12">
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends 'generic/object.html' %} {% load plugins %} {% load render_table
 from django_tables2 %} {% block breadcrumbs %} {{ block.super }}
 _{_{_ _o_b_j_e_c_t_._e_x_t_e_r_n_a_l___p_a_r_t_i_e_ _}_}
 {% endblock %} {% block content %}
 **** CCoonnttrraacctt ****
 NNaammee                   {{ object.name }}
-EExxtteerrnnaall ppaarrttiiee        _{_{_ _o_b_j_e_c_t_._e_x_t_e_r_n_a_l___p_a_r_t_i_e_._n_a_m_e_ _}_}
+EExxtteerrnnaall ppaarrttiiee ttyyppee   {{ object.external_partie_object_type }}
+EExxtteerrnnaall ppaarrttiiee        _{_{_ _o_b_j_e_c_t_._e_x_t_e_r_n_a_l___p_a_r_t_i_e___o_b_j_e_c_t_._n_a_m_e_ _}_}
 SSttaattuuss                 {{ object.status }}
 EExxtteerrnnaall rreeffeerreennccee     {{ object.external_reference }}
 IInntteerrnnaall ppaarrttiiee        {{ object.internal_partie }}
 TTeennaanntt                 {{ object.tenant }}
 SSttaarrtt ddaattee             {{ object.start_date }}
 EEnndd ddaattee               {{ object.end_date }}
 IInniittiiaall tteerrmm           {{ object.initial_term }}
@@ -18,18 +19,18 @@
 MMoonntthhllyy rreeccuurriinngg ccoossttss {{ object.mrc }}
 NNoonn rreeccuurriinngg ccoossttss     {{ object.nrc }}
 IInnvvooiiccee ffrreeqquueennccyy      {{ object.invoice_frequency }}
 PPaarreenntt                 _{_{_ _o_b_j_e_c_t_._p_a_r_e_n_t_._n_a_m_e_ _}_}
 DDooccuummeennttss              _D_o_c_u_m_e_n_t_s
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
-**** CCiirrccuuiittss ****
-{% render_table circuit_table %}
 **** AAssssiiggnneemmeennttss ****
 {% render_table assignements_table %}
+**** cchhiillddss ****
+{% render_table childs_table %}
 {% if perms.netbox_contract.view_invoice %}
 **** IInnvvooiicceess ****
 {% render_table invoices_table %}
 {% if perms.netbox_contract.add_invoice %}
 _A_d_d_ _a_n_ _i_n_v_o_i_c_e
 {% endif %}
 {% endif %} {% plugin_right_page object %} {% endblock content %}
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/contract_assignement.html` & `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/contract_assignement.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/invoice.html` & `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/invoice.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.8/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox-contract-2.0.9/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.8/src/netbox_contract/views.py` & `netbox-contract-2.0.9/src/netbox_contract/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,225 @@
-from datetime import timedelta, date
+from datetime import date, timedelta
+
+from circuits.models import Circuit
 from dateutil.relativedelta import relativedelta
-from django.core.exceptions import ObjectDoesNotExist
 from django.contrib.contenttypes.models import ContentType
-from django.shortcuts import render, get_object_or_404
+from django.core.exceptions import ObjectDoesNotExist
+from django.shortcuts import get_object_or_404, render
 from netbox.views import generic
-from tenancy.views import ObjectContactsView
 from netbox.views.generic.utils import get_prerequisite_model
-from utilities.utils import count_related, normalize_querydict
 from utilities.forms import restrict_form_fields
-from utilities.views import ViewTab, register_model_view
-from circuits.models import Circuit
-from .models import ServiceProvider, ContractAssignement, Contract, Invoice
-from . import forms, tables, filtersets
+from utilities.utils import count_related, normalize_querydict
+
+from . import filtersets, forms, tables
+from .models import Contract, ContractAssignement, Invoice, ServiceProvider
 
 # ServiceProvider views
 
+
 class ServiceProviderView(generic.ObjectView):
     queryset = ServiceProvider.objects.all()
 
+
 class ServiceProviderListView(generic.ObjectListView):
     queryset = ServiceProvider.objects.all()
     table = tables.ServiceProviderListTable
     filterset = filtersets.ServiceProviderFilterSet
     filterset_form = forms.ServiceProviderFilterSetForm
 
+
 class ServiceProviderEditView(generic.ObjectEditView):
     queryset = ServiceProvider.objects.all()
     form = forms.ServiceProviderForm
 
+
 class ServiceProviderDeleteView(generic.ObjectDeleteView):
     queryset = ServiceProvider.objects.all()
 
+
 class ServiceProviderBulkImportView(generic.BulkImportView):
     queryset = ServiceProvider.objects.all()
     model_form = forms.ServiceProviderCSVForm
     table = tables.ServiceProviderListTable
 
+
 class ServiceProviderBulkEditView(generic.BulkEditView):
     queryset = ServiceProvider.objects.annotate()
     filterset = filtersets.ServiceProviderFilterSet
     table = tables.ServiceProviderListTable
     form = forms.ServiceProviderBulkEditForm
 
+
 class ServiceProviderBulkDeleteView(generic.BulkDeleteView):
     queryset = ServiceProvider.objects.annotate()
     filterset = filtersets.ServiceProviderFilterSet
     table = tables.ServiceProviderListTable
 
+
 # Contract assignement view
 
+
 class ContractAssignementView(generic.ObjectView):
     queryset = ContractAssignement.objects.all()
 
+
 class ContractAssignementListView(generic.ObjectListView):
     queryset = ContractAssignement.objects.all()
     table = tables.ContractAssignementListTable
     filterset = filtersets.ContractAssignementFilterSet
     filterset_form = forms.ContractAssignementFilterSetForm
-    actions = ['import', 'export', ]
+    actions = [
+        'import',
+        'export',
+    ]
+
 
 class ContractAssignementEditView(generic.ObjectEditView):
     queryset = ContractAssignement.objects.all()
     form = forms.ContractAssignementForm
 
     def alter_object(self, instance, request, args, kwargs):
         if not instance.pk and kwargs:
             # Assign the object based on URL kwargs
-            content_type = get_object_or_404(ContentType, pk=request.GET.get('content_type'))
-            instance.object = get_object_or_404(content_type.model_class(), pk=request.GET.get('object_id'))
+            content_type = get_object_or_404(
+                ContentType, pk=request.GET.get('content_type')
+            )
+            instance.object = get_object_or_404(
+                content_type.model_class(), pk=request.GET.get('object_id')
+            )
         return instance
 
     def get_extra_addanother_params(self, request):
         return {
             'content_type': request.GET.get('content_type'),
             'object_id': request.GET.get('object_id'),
         }
 
+
 class ContractAssignementDeleteView(generic.ObjectDeleteView):
     queryset = ContractAssignement.objects.all()
 
+
 class ContractAssignementBulkImportView(generic.BulkImportView):
     queryset = ContractAssignement.objects.all()
     model_form = forms.ContractAssignementImportForm
     table = tables.ContractAssignementListTable
 
+
 # Contract views
 
+
 class ContractView(generic.ObjectView):
     queryset = Contract.objects.all()
 
     def get_extra_context(self, request, instance):
         invoices_table = tables.InvoiceListTable(instance.invoices.all())
         invoices_table.configure(request)
-        circuit_table = tables.ContractCircuitListTable(instance.circuit.all())
-        circuit_table.configure(request)
-        assignements_table = tables.ContractAssignementContractTable(instance.assignments.all())
+        assignements_table = tables.ContractAssignementContractTable(
+            instance.assignments.all()
+        )
         assignements_table.configure(request)
+        childs_table = tables.ContractListBottomTable(instance.childs.all())
+        childs_table.configure(request)
 
         return {
             'invoices_table': invoices_table,
-            'circuit_table': circuit_table,
             'assignements_table': assignements_table,
+            'childs_table': childs_table,
         }
 
+
 class ContractListView(generic.ObjectListView):
     queryset = Contract.objects.all()
     table = tables.ContractListTable
     filterset = filtersets.ContractFilterSet
     filterset_form = forms.ContractFilterSetForm
 
+
 class ContractEditView(generic.ObjectEditView):
     queryset = Contract.objects.all()
     form = forms.ContractForm
 
+    def alter_object(self, obj, request, url_args, url_kwargs):
+        """
+        When this method is called after a Post,
+        it is used here to set the external partie object id for exiting objects,
+        In any case, this happens before the form is instanciated.
+
+        Args:
+            obj: The object being edited
+            request: The current request
+            url_args: URL path args
+            url_kwargs: URL path kwargs
+        """
+
+        if request.method == 'POST':
+            data = normalize_querydict(request.POST)
+            obj.external_partie_object_id = data['external_partie_object']
+            external_partie_object_type_id = data['external_partie_object_type']
+            obj.external_partie_object_type = ContentType.objects.get(
+                id=external_partie_object_type_id
+            )
+            external_partie_object_type = obj.external_partie_object_type
+            obj.external_partie_object = (
+                external_partie_object_type.get_object_for_this_type(
+                    id=obj.external_partie_object_id
+                )
+            )
+
+        return obj
+
+
 class ContractDeleteView(generic.ObjectDeleteView):
     queryset = Contract.objects.all()
 
+
 class ContractBulkImportView(generic.BulkImportView):
     queryset = Contract.objects.all()
     model_form = forms.ContractCSVForm
     table = tables.ContractListTable
 
+
 class ContractBulkEditView(generic.BulkEditView):
-    queryset = Contract.objects.annotate(
-        count_circuits=count_related(Circuit, 'contracts')
-    )
+    queryset = Contract.objects.all()
     filterset = filtersets.ContractFilterSet
     table = tables.ContractListTable
     form = forms.ContractBulkEditForm
 
+
 class ContractBulkDeleteView(generic.BulkDeleteView):
     queryset = Contract.objects.annotate(
         count_circuits=count_related(Circuit, 'contracts')
     )
     filterset = filtersets.ContractFilterSet
     table = tables.ContractListTable
 
+
 # Invoice views
 
+
 class InvoiceView(generic.ObjectView):
     queryset = Invoice.objects.all()
 
     def get_extra_context(self, request, instance):
         contracts_table = tables.ContractListTable(instance.contracts.all())
         contracts_table.configure(request)
 
         return {
             'contracts_table': contracts_table,
         }
 
+
 class InvoiceListView(generic.ObjectListView):
     queryset = Invoice.objects.all()
     table = tables.InvoiceListTable
     filterset = filtersets.InvoiceFilterSet
     filterset_form = forms.InvoiceFilterSetForm
 
+
 class InvoiceEditView(generic.ObjectEditView):
     queryset = Invoice.objects.all()
     form = forms.InvoiceForm
 
     def get(self, request, *args, **kwargs):
         """
         GET request handler
@@ -177,53 +238,61 @@
         if 'contracts' in initial_data.keys():
             contract = Contract.objects.get(pk=initial_data['contracts'])
 
             try:
                 last_invoice = contract.invoices.latest('period_end')
                 new_period_start = last_invoice.period_end + timedelta(days=1)
             except ObjectDoesNotExist:
-                if contract.start_date :
+                if contract.start_date:
                     new_period_start = contract.start_date
                 else:
                     new_period_start = None
 
-            if new_period_start :
+            if new_period_start:
                 initial_data['period_start'] = new_period_start
                 delta = relativedelta(months=contract.invoice_frequency)
                 new_period_end = new_period_start + delta - timedelta(days=1)
                 initial_data['period_end'] = new_period_end
 
             initial_data['amount'] = contract.mrc * contract.invoice_frequency
             initial_data['currency'] = contract.currency
-            if contract.accounting_dimensions :
+            if contract.accounting_dimensions:
                 initial_data['accounting_dimensions'] = contract.accounting_dimensions
 
         form = self.form(instance=obj, initial=initial_data)
         restrict_form_fields(form, request.user)
 
-        return render(request, self.template_name, {
-            'model': model,
-            'object': obj,
-            'form': form,
-            'return_url': self.get_return_url(request, obj),
-            'prerequisite_model': get_prerequisite_model(self.queryset),
-            **self.get_extra_context(request, obj),
-        })
+        return render(
+            request,
+            self.template_name,
+            {
+                'model': model,
+                'object': obj,
+                'form': form,
+                'return_url': self.get_return_url(request, obj),
+                'prerequisite_model': get_prerequisite_model(self.queryset),
+                **self.get_extra_context(request, obj),
+            },
+        )
+
 
 class InvoiceDeleteView(generic.ObjectDeleteView):
     queryset = Invoice.objects.all()
 
+
 class InvoiceBulkImportView(generic.BulkImportView):
     queryset = Invoice.objects.all()
     model_form = forms.InvoiceCSVForm
     table = tables.InvoiceListTable
 
+
 class InvoiceBulkEditView(generic.BulkEditView):
     queryset = Invoice.objects.all()
     filterset = filtersets.InvoiceFilterSet
     table = tables.InvoiceListTable
     form = forms.InvoiceBulkEditForm
 
+
 class InvoiceBulkDeleteView(generic.BulkDeleteView):
     queryset = Invoice.objects.all()
     filterset = filtersets.InvoiceFilterSet
     table = tables.InvoiceListTable
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract.egg-info/PKG-INFO` & `netbox-contract-2.0.9/src/netbox_contract.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.8
+Version: 2.0.9
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dateutil
 
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
@@ -47,21 +48,26 @@
 Customize the location of the plugin's menu:
 
 
 ```python
 # configuration.py
 PLUGINS_CONFIG = {
     'netbox_contract': {
-        'top_level_menu': True
+        'top_level_menu': True,
+        'default_accounting_dimensions':{
+            "account": "", 
+            "project": "", 
+            "cost center": ""
+        }
     }
 }
 
 ```
 
-Customize the internal partie field.  
+Customize fields choices.  
 Internal partie reference the legal entity of your organization that is a partie to the contract.  
 
 ```python
 # configuration.py
 FIELD_CHOICES = {
     'netbox_contract.Contract.internal_partie': (
         ('Nagravision SARL', 'Nagravision SARL', 'green'),
@@ -127,7 +133,15 @@
 #### version 2.0.6
 * [#80](https://github.com/mlebreuil/netbox-contract/issues/80) Fix missing fields in the API.
 
 #### version 2.0.7
 * [#85](https://github.com/mlebreuil/netbox-contract/issues/85) Fix missing fields contract and invoice import and export forms.
 
 #### version 2.0.8
+* [#91](https://github.com/mlebreuil/netbox-contract/issues/91) Replace deprecated ( in netbox version 3.6) MultipleChoiceField.  
+* [48](https://github.com/mlebreuil/netbox-contract/issues/48) Allow other plugin to inject visual in contract and invoice forms.  
+* [89] (https://github.com/mlebreuil/netbox-contract/issues/89) Add contract assignement to virtual machines.
+
+#### version 2.0.9
+* [42](https://github.com/mlebreuil/netbox-contract/issues/42) Allow the selection of either providers or Service providers as contract third partie.
+* Removed all reference to the direct assignement of circuits to contracts
+
```

### Comparing `netbox-contract-2.0.8/src/netbox_contract.egg-info/SOURCES.txt` & `netbox-contract-2.0.9/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/netbox_contract/__init__.py
+src/netbox_contract/constants.py
 src/netbox_contract/filtersets.py
 src/netbox_contract/forms.py
 src/netbox_contract/models.py
 src/netbox_contract/navigation.py
 src/netbox_contract/search.py
 src/netbox_contract/tables.py
 src/netbox_contract/template_content.py
@@ -36,14 +37,19 @@
 src/netbox_contract/migrations/0011_auto_20230122_2112.py
 src/netbox_contract/migrations/0012_remove_invoice_contract.py
 src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
 src/netbox_contract/migrations/0014_contract_end_date.py
 src/netbox_contract/migrations/0015_contractassignement.py
 src/netbox_contract/migrations/0016_contract_parent.py
 src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
+src/netbox_contract/migrations/0018_contract_external_partie_object_id_and_more.py
+src/netbox_contract/migrations/0019_auto_20230924_1813.py
+src/netbox_contract/migrations/0020_alter_contract_external_partie.py
+src/netbox_contract/migrations/0021_alter_contract_external_partie.py
+src/netbox_contract/migrations/0022_alter_contract_internal_partie_alter_contract_parent.py
 src/netbox_contract/migrations/__init__.py
 src/netbox_contract/templates/contact_assignements_bottom.html
 src/netbox_contract/templates/contract_assignements_bottom.html
 src/netbox_contract/templates/contract_list_bottom.html
 src/netbox_contract/templates/netbox_contract/contract.html
 src/netbox_contract/templates/netbox_contract/contract_assignement.html
 src/netbox_contract/templates/netbox_contract/invoice.html
```

