# Comparing `tmp/vital-ai-domain-0.1.1.tar.gz` & `tmp/vital-ai-domain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-domain-0.1.1.tar", last modified: Thu Feb  8 13:03:49 2024, max compression
+gzip compressed data, was "vital-ai-domain-0.1.3.tar", last modified: Sat May  4 20:50:22 2024, max compression
```

## Comparing `vital-ai-domain-0.1.1.tar` & `vital-ai-domain-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,159 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:03:49.868727 vital-ai-domain-0.1.1/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-02-02 13:30:17.000000 vital-ai-domain-0.1.1/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      536 2024-02-08 13:03:49.868507 vital-ai-domain-0.1.1/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       17 2024-02-06 19:31:37.000000 vital-ai-domain-0.1.1/README.md
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-02-08 13:03:49.868775 vital-ai-domain-0.1.1/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      716 2024-02-08 13:02:50.000000 vital-ai-domain-0.1.1/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:03:49.867599 vital-ai-domain-0.1.1/vital_ai_domain/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 19:32:01.000000 vital-ai-domain-0.1.1/vital_ai_domain/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-02-08 13:03:49.868258 vital-ai-domain-0.1.1/vital_ai_domain.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      536 2024-02-08 13:03:49.000000 vital-ai-domain-0.1.1/vital_ai_domain.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-02-08 13:03:49.000000 vital-ai-domain-0.1.1/vital_ai_domain.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-02-08 13:03:49.000000 vital-ai-domain-0.1.1/vital_ai_domain.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       20 2024-02-08 13:03:49.000000 vital-ai-domain-0.1.1/vital_ai_domain.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       16 2024-02-08 13:03:49.000000 vital-ai-domain-0.1.1/vital_ai_domain.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:50:22.093542 vital-ai-domain-0.1.3/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-02-02 13:30:17.000000 vital-ai-domain-0.1.3/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      543 2024-05-04 20:50:22.093261 vital-ai-domain-0.1.3/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       17 2024-02-06 19:31:37.000000 vital-ai-domain-0.1.3/README.md
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 20:50:22.093631 vital-ai-domain-0.1.3/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      891 2024-05-04 20:50:03.000000 vital-ai-domain-0.1.3/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:50:22.069730 vital-ai-domain-0.1.3/vital_ai_domain/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-02-05 19:32:01.000000 vital-ai-domain-0.1.3/vital_ai_domain/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:50:22.085165 vital-ai-domain-0.1.3/vital_ai_domain/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1830 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Account.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Account.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/AdminLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/AdminLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/BusinessOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/BusinessOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1457 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/CredentialsLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/CredentialsLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1223 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Currency.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       97 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Currency.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1350 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/DatascriptInfo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/DatascriptInfo.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1643 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/DatascriptRun.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/DatascriptRun.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1223 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Duration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       97 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Duration.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasLoginAuth.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasLoginAuth.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasNextElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasNextElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasUserLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasUserLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasUserSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Edge_hasUserSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/EmailAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/EmailAddress.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1434 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/ErrorFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/ErrorFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2000 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/FileNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      301 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/FileNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/GeographicRegion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      105 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/GeographicRegion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/GovernmentOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/GovernmentOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/HyperEdge_hasFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/HyperEdge_hasFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/HyperEdge_hasHyperAnnotation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/HyperEdge_hasHyperAnnotation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/HyperEdge_hasReason.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/HyperEdge_hasReason.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Identifier_Locator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      107 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Identifier_Locator.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1931 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Job.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      310 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Job.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/ListElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/ListElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Location.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Location.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1345 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Login.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Login.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1443 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/LoginAuth.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/LoginAuth.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1214 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Media.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       94 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Media.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1217 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Number.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       95 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Number.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1235 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Organization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      101 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Organization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1241 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Person.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Person.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/PhoneNumber.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/PhoneNumber.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1238 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/PhysicalThing.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/PhysicalThing.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/PrivateOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/PrivateOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1244 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Product.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Product.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1233 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Thing.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Thing.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1211 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Time.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       93 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/Time.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/URI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/URI.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/URL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/URL.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1636 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/UserLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/UserLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1646 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/UserSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/UserSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VITAL_Annotation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VITAL_Annotation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1360 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VITAL_Fact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VITAL_Fact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VITAL_Reason.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VITAL_Reason.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2071 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VitalDataScript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      342 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VitalDataScript.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1429 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VitalRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VitalRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VitalRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/VitalRuleSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-19 22:12:17.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:50:22.092935 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasAccountAccessURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasAccountID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasAccountLoginSuffix.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasAccountOwnerURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasCertainty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasCronExpression.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasDegree.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasEmailAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasErrorMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasErrorType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasExpirationDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasFileLength.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasFileName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasFileScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasFileType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasFileURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      190 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasInfo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasInterval.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasIntervalTimeUnit.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasJobID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasJobStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasLastCompilationError.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasLastExecutionTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasLastModifiedDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasLocalLoginsType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasLoginOwnerURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasNextExecutionTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasPageRank.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasProfileURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasRuleBody.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasScriptPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasVerificationCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_hasVitalDataScriptBody.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isAdminScript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isCallable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isEmailVerified.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isFactEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isFirstElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isLocalLoginsValidated.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isLocked.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isPaused.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isRegularScript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isRetired.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 20:36:09.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/Property_isServiceLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-19 22:12:17.000000 vital-ai-domain-0.1.3/vital_ai_domain/model/properties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 20:50:22.070772 vital-ai-domain-0.1.3/vital_ai_domain.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      543 2024-05-04 20:50:22.000000 vital-ai-domain-0.1.3/vital_ai_domain.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)     6753 2024-05-04 20:50:22.000000 vital-ai-domain-0.1.3/vital_ai_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 20:50:22.000000 vital-ai-domain-0.1.3/vital_ai_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       56 2024-05-04 20:50:22.000000 vital-ai-domain-0.1.3/vital_ai_domain.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       27 2024-05-04 20:50:22.000000 vital-ai-domain-0.1.3/vital_ai_domain.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       16 2024-05-04 20:50:22.000000 vital-ai-domain-0.1.3/vital_ai_domain.egg-info/top_level.txt
```

### Comparing `vital-ai-domain-0.1.1/LICENSE` & `vital-ai-domain-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vital-ai-domain-0.1.1/PKG-INFO` & `vital-ai-domain-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vital-ai-domain
-Version: 0.1.1
+Version: 0.1.3
 Summary: VitalSigns vital domain
 Home-page: https://github.com/vital-ai/vitalhome-knowledge-graph
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns
+Requires-Dist: vital-ai-vitalsigns==0.1.3
 
 # vital-ai-domain
```

### Comparing `vital-ai-domain-0.1.1/setup.py` & `vital-ai-domain-0.1.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-domain',
-    version='0.1.1',
+    version='0.1.3',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns vital domain',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vitalhome-knowledge-graph',
     packages=find_packages(),
+    entry_points={
+        'vitalsigns_packages': [
+            'vital_ai_domain = vital_ai_domain'
+        ]
+    },
+    package_data={
+         '': ['*.pyi'],
+    },
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-vitalsigns',
+            'vital-ai-vitalsigns==0.1.3',
         ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
-)
+)
```

### Comparing `vital-ai-domain-0.1.1/vital_ai_domain.egg-info/PKG-INFO` & `vital-ai-domain-0.1.3/vital_ai_domain.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: vital-ai-domain
-Version: 0.1.1
+Version: 0.1.3
 Summary: VitalSigns vital domain
 Home-page: https://github.com/vital-ai/vitalhome-knowledge-graph
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-vitalsigns
+Requires-Dist: vital-ai-vitalsigns==0.1.3
 
 # vital-ai-domain
```

