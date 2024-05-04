# Comparing `tmp/nl_matcher-0.0.1.tar.gz` & `tmp/nl_matcher-0.0.2.tar.gz`

## Comparing `nl_matcher-0.0.1.tar` & `nl_matcher-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/main.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/requirements_dev.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/src/nl_matcher/__init__.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/src/nl_matcher/location_matcher.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/src/nl_matcher/rules/cfg
--rw-r--r--   0        0        0   703364 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/src/nl_matcher/rules/patterns.jsonl
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/tests/test_location_matcher.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/.gitignore
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/README.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 nl_matcher-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/main.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/requirements_dev.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/__init__.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/location_matcher.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/rules/cfg
+-rw-r--r--   0        0        0   703364 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/src/nl_matcher/rules/patterns.jsonl
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/tests/test_location_matcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/.gitignore
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/README.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 nl_matcher-0.0.2/PKG-INFO
```

### Comparing `nl_matcher-0.0.1/src/nl_matcher/location_matcher.py` & `nl_matcher-0.0.2/src/nl_matcher/location_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import spacy
 from spacy.tokens import Span
 from spacy.matcher import Matcher
+from pathlib import Path
 import re
 
 
 def LocationMatcher():
     # Exclude all but essencial pipelines to improve performance.
     exclude = [
         # 'ner',
@@ -22,15 +23,15 @@
         'senter',
         'sentencizer',
         'transformer',
     ]
 
     nlp = spacy.load('nl_core_news_lg', exclude=exclude)
     ruler = nlp.add_pipe('entity_ruler', before='ner')
-    ruler.from_disk('./rules')
+    ruler.from_disk((Path(__file__).parent / "./rules").resolve())
 
     patterns = [
         ([
             {"TEXT": "oversteekplaats"},
             {"TEXT": "tussen"},
             {"TEXT": "de"},
             {"ENT_TYPE": {"IN": ["GPE", "FAC", "LOC", "ORG"]}, "OP": "+"},
```

### Comparing `nl_matcher-0.0.1/src/nl_matcher/rules/patterns.jsonl` & `nl_matcher-0.0.2/src/nl_matcher/rules/patterns.jsonl`

 * *Files identical despite different names*

### Comparing `nl_matcher-0.0.1/tests/test_location_matcher.py` & `nl_matcher-0.0.2/tests/test_location_matcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 import pytest
-from location_matcher import LocationMatcher
+from nl_matcher import LocationMatcher
 
 location_matcher = LocationMatcher()
 
 testdata = [
     (
-        """Al ruim twee jaar rookt bij elke frisse dag de houtkachel aan de Fluitekamp in Hoogland.""",
+        "Al ruim twee jaar rookt bij elke frisse dag de houtkachel aan de "
+        "Fluitekamp in Hoogland.",
+
         'Fluitekamp in Hoogland'
     ),
 
     (
-        """Terwijl dit gesprek door gaat, komt een man de Hema in Montfoort binnen en rekent twee powerbanks af met de pas van het slachtoffer.""",
+        "Terwijl dit gesprek door gaat, komt een man de Hema in Montfoort "
+        "binnen en rekent twee powerbanks af met de pas van het slachtoffer.",
+
         'Hema in Montfoort'
     ),
 
     (
-        """Was u getuige van de aanval in de Maarssense wijk Zwanenkamp op woensdag 1 februari? Bel dan met de tiplijn: 0800 - 6070 of bel Meld Misdaad Anoniem: 0800 - 7000. Beelden waarop de dader te zien is kunt u uploaden via politie.nl/upload""",
+        "Was u getuige van de aanval in de Maarssense wijk Zwanenkamp op "
+        "woensdag 1 februari? Bel dan met de tiplijn: 0800 - 6070 of bel "
+        "Meld Misdaad Anoniem: 0800 - 7000. Beelden waarop de dader te "
+        "zien is kunt u uploaden via politie.nl/upload",
+
         'Maarssense wijk Zwanenkamp'
     ),
 
     (
-        """Er is veel chemie op de werkvloer, de cultuur is hier heel goed.""  VERJAARDAG MET DE KONING EN MINISTER YESILGÖZ  Het 75-jarige jubileum van de vrijwillige politie werd vandaag gevierd bij evenementenlocatie Mereveld in Utrecht.""",
+        "Het 75-jarige jubileum van de vrijwillige politie werd vandaag "
+        "gevierd bij evenementenlocatie Mereveld in Utrecht.",
         'Mereveld in Utrecht'
     ),
 
     (
         """Vleuten - Zondagavond 12 maart rond 22.30 uur was er een explosie bij een woning aan de Moersbergen in Vleuten.""",
         'Moersbergen in Vleuten'
     ),
 
     (
-        """Utrecht - Straatafval, drugshandel, geluidoverlast en intimidatie. Bewoners van een flat aan de Marco Pololaan in de Utrechtse wijk Kanaleneiland zijn naar eigen zeggen al jaren met politie en gemeente in de weer om de overlast van een groep hangjongeren en volwassen mannen in hun straat te weren, vooralsnog zonder resultaat.""",
-        'Marco Pololaan in de Utrechtse wijk Kanaleneiland'
-    ),
+        """Utrecht - Straatafval, drugshandel, geluidoverlast en intimidatie. Bewoners van een flat aan de Marco Pololaan in de Utrechtse wijk Kanaleneiland zijn naar eigen zeggen al jaren met politie en gemeente in de weer om de overlast van een groep hangjongeren en volwassen mannen in hun straat te weren, vooralsnog zonder resultaat.""", 'Marco Pololaan in de Utrechtse wijk Kanaleneiland'),
 
     (
         """Vleuten - Zondagavond 12 maart rond 22.30 uur was er een explosie bij een woning aan de Moersbergen in Vleuten.""",
         'Moersbergen in Vleuten'
     ),
 
     (
```

### Comparing `nl_matcher-0.0.1/pyproject.toml` & `nl_matcher-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nl-matcher"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Diego Da'Silva", email="smartcrashomg@gmail.com" },
 ]
 description = "A simple library to match locations in text using SpaCy"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nl_matcher-0.0.1/PKG-INFO` & `nl_matcher-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nl-matcher
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple library to match locations in text using SpaCy
 Project-URL: Homepage, https://github.com/smartcrash/nlmatcher
 Project-URL: Issues, https://github.com/smartcrash/nlmatcher/issues
 Author-email: Diego Da'Silva <smartcrashomg@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

