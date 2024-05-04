# Comparing `tmp/sonatoki-0.1.0.tar.gz` & `tmp/sonatoki-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonatoki-0.1.0.tar", last modified: Thu May  2 20:45:18 2024, max compression
+gzip compressed data, was "sonatoki-0.1.1.tar", last modified: Fri May  3 21:55:45 2024, max compression
```

## Comparing `sonatoki-0.1.0.tar` & `sonatoki-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34523 2024-04-23 19:07:55.795668 sonatoki-0.1.0/LICENSE
--rw-r--r--   0        0        0     2872 2024-05-02 20:36:51.015963 sonatoki-0.1.0/README.md
--rw-r--r--   0        0        0     2013 2024-05-02 20:45:18.821799 sonatoki-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-04-20 18:49:02.963236 sonatoki-0.1.0/src/sonatoki/Cleaners.py
--rw-r--r--   0        0        0     4093 2024-05-02 20:35:15.738238 sonatoki-0.1.0/src/sonatoki/Filters.py
--rw-r--r--   0        0        0     3431 2024-04-24 18:37:20.174610 sonatoki-0.1.0/src/sonatoki/Preprocessors.py
--rw-r--r--   0        0        0     3690 2024-05-02 20:35:18.981607 sonatoki-0.1.0/src/sonatoki/Scorers.py
--rw-r--r--   0        0        0     1628 2024-04-23 21:03:01.388273 sonatoki-0.1.0/src/sonatoki/Tokenizers.py
--rw-r--r--   0        0        0        0 2024-04-14 02:56:25.653492 sonatoki-0.1.0/src/sonatoki/__init__.py
--rw-r--r--   0        0        0       82 2024-04-20 18:48:59.589895 sonatoki-0.1.0/src/sonatoki/__main__.py
--rw-r--r--   0        0        0     1320 2024-04-20 18:50:32.233508 sonatoki-0.1.0/src/sonatoki/constants.py
--rw-r--r--   0        0        0     3482 2024-05-02 20:35:17.581592 sonatoki-0.1.0/src/sonatoki/ilo.py
--rw-r--r--   0        0        0   270928 2024-04-15 22:25:04.757856 sonatoki-0.1.0/src/sonatoki/linku.json
--rw-r--r--   0        0        0        0 2024-03-09 04:40:19.049987 sonatoki-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-02 20:35:53.578656 sonatoki-0.1.0/tests/test_cleaners.py
--rw-r--r--   0        0        0     2536 2024-05-02 20:35:54.652001 sonatoki-0.1.0/tests/test_filters.py
--rw-r--r--   0        0        0     1566 2024-05-02 20:35:55.625346 sonatoki-0.1.0/tests/test_ilo.py
--rw-r--r--   0        0        0     2808 2024-05-02 20:35:56.852026 sonatoki-0.1.0/tests/test_preprocessors.py
--rw-r--r--   0        0        0      986 2024-05-02 20:35:58.425377 sonatoki-0.1.0/tests/test_scorers.py
--rw-r--r--   0        0        0     2997 2024-05-02 20:35:59.512055 sonatoki-0.1.0/tests/test_tokenize.py
--rw-r--r--   0        0        0      821 2024-05-02 20:36:00.588734 sonatoki-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0      151 2024-04-12 22:41:28.463028 sonatoki-0.1.0/tests/tokenize_cases/tokenize_sentences.yml
--rw-r--r--   0        0        0      429 2024-04-12 22:44:39.979114 sonatoki-0.1.0/tests/tokenize_cases/tokenize_sentences_tok.yml
--rw-r--r--   0        0        0      536 2024-04-12 22:41:14.139489 sonatoki-0.1.0/tests/tokenize_cases/tokenize_words.yml
--rw-r--r--   0        0        0     1143 2024-04-23 21:06:36.351195 sonatoki-0.1.0/tests/tokenize_cases/tokenize_words_tok.yml
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 sonatoki-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-03 21:55:32.367514 sonatoki-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4560 2024-05-03 21:55:32.367514 sonatoki-0.1.1/README.md
+-rw-r--r--   0        0        0     2013 2024-05-03 21:55:45.023626 sonatoki-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1160 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/Cleaners.py
+-rw-r--r--   0        0        0     4093 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/Filters.py
+-rw-r--r--   0        0        0     3431 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/Preprocessors.py
+-rw-r--r--   0        0        0     3678 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/Scorers.py
+-rw-r--r--   0        0        0     1628 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/Tokenizers.py
+-rw-r--r--   0        0        0        0 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/__main__.py
+-rw-r--r--   0        0        0     1320 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/constants.py
+-rw-r--r--   0        0        0     4278 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/ilo.py
+-rw-r--r--   0        0        0   270928 2024-05-03 21:55:32.367514 sonatoki-0.1.1/src/sonatoki/linku.json
+-rw-r--r--   0        0        0        0 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/test_cleaners.py
+-rw-r--r--   0        0        0     2536 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/test_filters.py
+-rw-r--r--   0        0        0     2277 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/test_ilo.py
+-rw-r--r--   0        0        0     2808 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/test_preprocessors.py
+-rw-r--r--   0        0        0      986 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/test_scorers.py
+-rw-r--r--   0        0        0     2997 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/test_tokenize.py
+-rw-r--r--   0        0        0      821 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0      151 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/tokenize_cases/tokenize_sentences.yml
+-rw-r--r--   0        0        0      429 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/tokenize_cases/tokenize_sentences_tok.yml
+-rw-r--r--   0        0        0      536 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/tokenize_cases/tokenize_words.yml
+-rw-r--r--   0        0        0     1354 2024-05-03 21:55:32.367514 sonatoki-0.1.1/tests/tokenize_cases/tokenize_words_tok.yml
+-rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 sonatoki-0.1.1/PKG-INFO
```

### Comparing `sonatoki-0.1.0/LICENSE` & `sonatoki-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/README.md` & `sonatoki-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -26,45 +26,68 @@
     Numerics,
     Syllabic,
     NimiLinku,
     Alphabetic,
     ProperName,
     Punctuations,
 )
-from sonatoki.Scorers import Scaling
+from sonatoki.Scorers import SoftScaling
 from sonatoki.Cleaners import ConsecutiveDuplicates
 from sonatoki.Tokenizers import word_tokenize_tok
 from sonatoki.Preprocessors import URLs, DiscordEmotes
 
 def main():
     ilo = Ilo(
         preprocessors=[URLs, DiscordEmotes],
         ignoring_filters=[Numerics, Punctuations],
         scoring_filters=[NimiLinku, Syllabic, ProperName, Alphabetic],
         cleaners=[ConsecutiveDuplicates],
-        scorer=Scaling,
+        scorer=SoftScaling,
         tokenizer=word_tokenize_tok,
     )
     ilo.is_toki_pona("imagine how is touch the sky")  # False
     ilo.is_toki_pona("o pilin insa e ni: sina pilin e sewi")  # True
+    ilo.is_toki_pona("I Think I Can Evade Detection")  # False
 
 if __name__ == "__main__":
     main()
 ```
 
-`Ilo` is highly configurable by design, so I recommend exploring the `Preprocessors`, `Filters`, and `Scorers` modules. The `Cleaners` module only contains one cleaner, which I highly recommend. The `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the
+`Ilo` is highly configurable by design, so I recommend exploring the `Preprocessors`, `Filters`, and `Scorers` modules. The `Cleaners` module only contains one cleaner, which I recommend using. The `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the dedicated Toki Pona tokenizer `word_tokenize_tok`.
 
 ## Development
 
 1. Install [pdm](https://github.com/pdm-project/pdm)
-1. `pdm sync --dev`
+1. `pdm install --dev`
 1. Open any file you like!
 
 ## FAQ
 
 ### Why isn't this README/library written in Toki Pona?
 
 The intent is to show our methodology to the Unicode Consortium, particularly to the Script Encoding Working Group (previously the Script Ad Hoc Group). As far as we're aware, zero members of the committee know Toki Pona, which unfortunately means we fall back on English.
 
 After our proposal has been examined and a result given by the committee, I will translate this file and library into Toki Pona, with a note left behind for those who do not understand it.
 
-### Why aren't any of the specific
+### What's the deal with the tokenizers?
+
+The Toki Pona tokenizer `word_tokenize_tok` is very specific in always separating writing characters from punctuation, and leaving contiguous punctuation as contiguous- this is a level of precision that NLTK's English tokenizer does not want for several reasons, such as that English words can have "punctuation" characters in them.
+
+Toki Pona doesn't have any mid-word symbols when rendered in the Latin alphabet, so a more aggressive tokenizer is highly desirable.
+
+The other tokenizers are provided as a comparison case more than anything. I do not recommend their use.
+
+### Aren't there a lot of false positives?
+
+Yes. It's up to you to use this tool responsibly on input you've done your best to clean, and better, use stronger filters before weaker ones. For now though, here's a list of relevant false positives:
+
+- `ProperName` will errantly match text in languages without a capital/lowercase distinction, artificially inflating the scores.
+- `Alphabetic` will match a _lot_ of undesirable text- it essentially allows 14 letters of the English alphabet.
+
+### Don't some of the cleaners/filters conflict?
+
+Yes. Some do so
+
+- `ConsecutiveDuplicates` may errantly change a word's validity. For example, "manna" is phonotactically invalid in Toki Pona, but would become "mana" which is valid.
+- `ConsecutiveDuplicates` will not work correctly with syllabaries (alphabets, but representing a pair of consonant and vowel).
+
+You'll notice a _lot_ of these are troubles regarding the application of latin alphabet filters to non-latin text. Working on it!
```

### Comparing `sonatoki-0.1.0/pyproject.toml` & `sonatoki-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sonatoki"
-version = "0.1.0"
+version = "0.1.1"
 description = "ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?"
 authors = [
     { name = "jan Kekan San (@gregdan3)", email = "gregory.danielson3@gmail.com" },
 ]
 dependencies = [
     "unidecode>=1.3.6",
     "regex>=2023.12.25",
```

### Comparing `sonatoki-0.1.0/src/sonatoki/Cleaners.py` & `sonatoki-0.1.1/src/sonatoki/Cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/src/sonatoki/Filters.py` & `sonatoki-0.1.1/src/sonatoki/Filters.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/src/sonatoki/Preprocessors.py` & `sonatoki-0.1.1/src/sonatoki/Preprocessors.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/src/sonatoki/Tokenizers.py` & `sonatoki-0.1.1/src/sonatoki/Tokenizers.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/src/sonatoki/constants.py` & `sonatoki-0.1.1/src/sonatoki/constants.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/src/sonatoki/ilo.py` & `sonatoki-0.1.1/src/sonatoki/Scorers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,123 @@
 # STL
-from typing import List, Type
+import math
+import logging
+from abc import ABC, abstractmethod
+from typing import Dict, List, Type, Union
+
+# PDM
+from typing_extensions import override
 
 # LOCAL
 from sonatoki.Filters import Filter
-from sonatoki.Scorers import Number, Scorer
-from sonatoki.Cleaners import Cleaner
-from sonatoki.Tokenizers import Tokenizer
-from sonatoki.Preprocessors import Preprocessor
-
-
-class Ilo:
-    __preprocessors: List[Type[Preprocessor]]
-    __cleaners: List[Type[Cleaner]]
-    __ignoring_filters: List[Type[Filter]]
-    __scoring_filters: List[Type[Filter]]
-    __scorer: Type[Scorer]
-    __tokenize: Tokenizer
-    __passing_score: Number
-    debug: bool = False
-
-    def __init__(
-        self,
-        preprocessors: List[Type[Preprocessor]],
-        cleaners: List[Type[Cleaner]],
-        ignoring_filters: List[Type[Filter]],
-        scoring_filters: List[Type[Filter]],
-        scorer: Type[Scorer],
-        tokenizer: Tokenizer,  # NOTE: no wrapper needed?
-        passing_score: Number,
-    ):
-        super().__init__()
-        # avoid keeping a ref to user's list just in case
-        self.__preprocessors = [*preprocessors]
-        self.__cleaners = [*cleaners]
-        self.__ignoring_filters = [*ignoring_filters]
-        self.__scoring_filters = [*scoring_filters]
-        self.__scorer = scorer
-        self.__tokenize = tokenizer
-        self.__passing_score = passing_score
-
-    def __preprocess(self, msg: str) -> str:
-        for p in self.__preprocessors:
-            msg = p.process(msg)
-        return msg
-
-    def __clean_token(self, token: str) -> str:
-        for c in self.__cleaners:
-            token = c.clean(token)
-        return token
-
-    def __clean_tokens(self, tokens: List[str]) -> List[str]:
-        # NOTE: tested, making a new list with a for loop *is* faster than
-        # - list comps
-        # - generator comps
-        # - in-place replacement/removal
-        # - in place replacement with result of generator comp
-        cleaned_tokens: List[str] = list()
+
+LOG = logging.getLogger(__name__)
+
+Number = Union[int, float]
+Weights = Dict[str, Number]
+
+
+class Scorer(ABC):
+    @classmethod
+    @abstractmethod
+    def score(cls, tokens: List[str], filters: List[Type[Filter]]) -> Number:
+        raise NotImplementedError
+
+
+class PassFail(Scorer):
+    """The token passes any filter or fails all of them, scoring 1 or 0 respectively."""
+
+    @classmethod
+    def __score(cls, token: str, filters: List[Type[Filter]]) -> Number:
+        for f in filters:
+            if f.filter(token):
+                score = 1
+                LOG.debug(
+                    "%12s.%s('%s') = %.2f", cls.__name__, f.__name__, token, score
+                )
+                return score
+        LOG.debug("%12s('%s') = 0.00", cls.__name__, token)
+        return 0
+
+    @classmethod
+    @override
+    def score(cls, tokens: List[str], filters: List[Type[Filter]]) -> Number:
+        if not tokens:
+            return 1
+
+        total_score = 0
+        len_tokens = len(tokens)
         for token in tokens:
-            cleaned_token = self.__clean_token(token)
-            if not cleaned_token:
-                # TODO: warn user?
-                continue
-            cleaned_tokens.append(cleaned_token)
-        return cleaned_tokens
+            total_score += cls.__score(token, filters)
+        return total_score / len_tokens if len_tokens else 0
+
 
-    def __filter_token(self, token: str) -> bool:
-        for f in self.__ignoring_filters:
+class Scaling(Scorer):
+    """
+    The sooner a token matches a filter, the higher its score.
+    In other words, filter order matters, weighing earlier listed filters higher than later ones.
+    This is desirable to avoid messages which would only match weaker filters, as these are less likely to be Toki Pona.
+    """
+
+    @classmethod
+    def score_token(cls, token: str, filters: List[Type[Filter]], scale: int):
+        for i, f in enumerate(filters):
             if f.filter(token):
-                return True
-        return False
+                score = scale - i
+                LOG.debug(
+                    "%12s.%s('%s') = %.2f", cls.__name__, f.__name__, token, score
+                )
+                return score
+        LOG.debug("%12s('%s') = 0.00", cls.__name__, token)
+        return 0
+
+    @classmethod
+    @override
+    def score(cls, tokens: List[str], filters: List[Type[Filter]]) -> Number:
+        if not tokens:
+            return 1
+
+        total_score = 0
+        len_filters = len(filters)
+        max_score = len(tokens) * len_filters
+        for token in tokens:
+            total_score += cls.score_token(token, filters, len_filters)
+        return total_score / max_score if max_score else 0
+
+
+class SoftScaling(Scaling):
+    """Shorter messages are subject to less harsh scoring
+    by mapping the token count to [0.5, 1.0] via the sigmoid function,
+    then raising the score to the resultant power.
+    For example, a single token scoring 0.64 will now score 0.8.
+    """
+
+    @staticmethod
+    def sigmoid(n: int) -> Number:
+        return 1 / (1 + math.exp(-(0.30 * (n - 1))))
+        # n-1 makes sigmoid(1) == 0.5
+        # 0.30 softens scaling in favor of short input
+        # return n / (1+abs(n))   # too weak in 0.7+
+
+    @classmethod
+    @override
+    def score(cls, tokens: List[str], filters: List[Type[Filter]]) -> Number:
+        if not tokens:
+            return 1
+
+        total_score = 0
+        len_filters = len(filters)
+        len_tokens = len(tokens)
 
-    def __filter_tokens(self, tokens: List[str]) -> List[str]:
-        filtered_tokens: List[str] = []
+        max_score = len_tokens * len_filters
         for token in tokens:
-            if self.__filter_token(token):
-                continue
-            # the ignoring filter is true if the token matches
-            # the user wants to ignore these so keep non-matching tokens
-            filtered_tokens.append(token)
-        return filtered_tokens
-
-    def __score_tokens(self, tokens: List[str]) -> float:
-        return self.__scorer.score(tokens, self.__scoring_filters)
-
-    def is_toki_pona(self, message: str) -> bool:
-        preprocessed = self.__preprocess(message)
-        tokenized = self.__tokenize(preprocessed)
-        filtered = self.__filter_tokens(tokenized)
-        cleaned = self.__clean_tokens(filtered)
-        score = self.__score_tokens(cleaned)
-
-        if self.debug:
-            print("msg: %.2f  %s" % (score, repr(message)))
-            print("Preproc:   %s" % repr(preprocessed))
-            print("Tokenized: %s" % tokenized)
-            print("Filtered:  %s" % filtered)
-            print("Cleaned:   %s" % cleaned)
-            print()
+            total_score += cls.score_token(token, filters, len_filters)
+
+        percentage = total_score / max_score if max_score else 0
+        percentage **= cls.sigmoid(len_tokens)
+        return percentage
+
+
+class Logarithmic(Scorer): ...
+
 
-        return score >= self.__passing_score
+__all__ = ["PassFail", "Scaling", "SoftScaling"]
```

### Comparing `sonatoki-0.1.0/src/sonatoki/linku.json` & `sonatoki-0.1.1/src/sonatoki/linku.json`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/test_cleaners.py` & `sonatoki-0.1.1/tests/test_cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/test_filters.py` & `sonatoki-0.1.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/test_ilo.py` & `sonatoki-0.1.1/tests/test_ilo.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,22 +32,42 @@
         ignoring_filters=[Numerics, Punctuations],
         scoring_filters=[NimiLinku, Syllabic, ProperName, Alphabetic],
         cleaners=[ConsecutiveDuplicates],
         scorer=SoftScaling,
         tokenizer=word_tokenize_tok,
         passing_score=0.8,
     )
-    ilo.debug = True
-    assert not ilo.is_toki_pona("super bruh moment 64")
+    # ilo._logging_threshold = 0.8
     assert ilo.is_toki_pona("mi unpa e mama sina")
-    assert ilo.is_toki_pona("mama sina li mu tan mi")
-    assert ilo.is_toki_pona("toki. sike li pona ala. o anpa.")
+    # toki pona
+    assert ilo.is_toki_pona("mama sina li lon seme? mi wile toki tawa ona")
+    assert ilo.is_toki_pona("sina sike pakala")
+    # names
     assert ilo.is_toki_pona("musi Homestuck li ike tawa mi")
+    # typoes
     assert ilo.is_toki_pona("mi mtue o kama sona")
+    assert ilo.is_toki_pona("mi mute o kma son")
+    # phonotactically valid
     assert ilo.is_toki_pona("ni li tenpo penpo")
+    # alphabetically valid
     assert ilo.is_toki_pona("ni li tptpt")
+    # a single
+    assert ilo.is_toki_pona("sipisi")
+
+    # soft scaling with syllablic filter at 2/4 will pass up to 5 syllablic words
+    assert ilo.is_toki_pona("walawa malama walama malama mupi")
+    # but fail 6 or more
+    assert not ilo.is_toki_pona("manama manama namana namana majani makala")
 
-    assert not ilo.is_toki_pona("I'm Trying To Evade The Filter")
+    # TODO: should soft scaling save an alphabetically valid single word?
+    assert not ilo.is_toki_pona("tok")
+    assert not ilo.is_toki_pona("mtue")
+
+    # just english
+    assert not ilo.is_toki_pona("bong")
+    assert not ilo.is_toki_pona("super bruh moment 64")
+    # all names
+    assert not ilo.is_toki_pona("I Want To Evade The Filter")
+    # all alphabetic
     assert not ilo.is_toki_pona(
-        """aaa i non-saw usa's most multiple element-set
-it's as asinine as in `e`-less speak"""
+        "aaa i non-saw usa's most multiple element-set. it's as asinine as in `e`-less speak"
     )
```

### Comparing `sonatoki-0.1.0/tests/test_preprocessors.py` & `sonatoki-0.1.1/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/test_scorers.py` & `sonatoki-0.1.1/tests/test_scorers.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/test_tokenize.py` & `sonatoki-0.1.1/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/test_utils.py` & `sonatoki-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/tokenize_cases/tokenize_words.yml` & `sonatoki-0.1.1/tests/tokenize_cases/tokenize_words.yml`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.0/tests/tokenize_cases/tokenize_words_tok.yml` & `sonatoki-0.1.1/tests/tokenize_cases/tokenize_words_tok.yml`

 * *Files 18% similar despite different names*

```diff
@@ -69,7 +69,22 @@
     - ":"
     - "'"
     - "single"
     - "quotes"
     - "are"
     - "boring"
     - "'"
+- name: "discovered case 1"
+  input: "***__U T A L A__   __M U N__***"
+  output:
+    - "***__"
+    - "U"
+    - "T"
+    - "A"
+    - "L"
+    - "A"
+    - "__"
+    - "__"
+    - "M"
+    - "U"
+    - "N"
+    - "__***"
```

### Comparing `sonatoki-0.1.0/PKG-INFO` & `sonatoki-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonatoki
-Version: 0.1.0
+Version: 0.1.1
 Summary: ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?
 Author-Email: "jan Kekan San (@gregdan3)" <gregory.danielson3@gmail.com>
 License: AGPL-3.0-or-later
 Requires-Python: >=3.8
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: regex>=2023.12.25
 Requires-Dist: typing-extensions>=4.11.0
@@ -40,45 +40,68 @@
     Numerics,
     Syllabic,
     NimiLinku,
     Alphabetic,
     ProperName,
     Punctuations,
 )
-from sonatoki.Scorers import Scaling
+from sonatoki.Scorers import SoftScaling
 from sonatoki.Cleaners import ConsecutiveDuplicates
 from sonatoki.Tokenizers import word_tokenize_tok
 from sonatoki.Preprocessors import URLs, DiscordEmotes
 
 def main():
     ilo = Ilo(
         preprocessors=[URLs, DiscordEmotes],
         ignoring_filters=[Numerics, Punctuations],
         scoring_filters=[NimiLinku, Syllabic, ProperName, Alphabetic],
         cleaners=[ConsecutiveDuplicates],
-        scorer=Scaling,
+        scorer=SoftScaling,
         tokenizer=word_tokenize_tok,
     )
     ilo.is_toki_pona("imagine how is touch the sky")  # False
     ilo.is_toki_pona("o pilin insa e ni: sina pilin e sewi")  # True
+    ilo.is_toki_pona("I Think I Can Evade Detection")  # False
 
 if __name__ == "__main__":
     main()
 ```
 
-`Ilo` is highly configurable by design, so I recommend exploring the `Preprocessors`, `Filters`, and `Scorers` modules. The `Cleaners` module only contains one cleaner, which I highly recommend. The `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the
+`Ilo` is highly configurable by design, so I recommend exploring the `Preprocessors`, `Filters`, and `Scorers` modules. The `Cleaners` module only contains one cleaner, which I recommend using. The `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the dedicated Toki Pona tokenizer `word_tokenize_tok`.
 
 ## Development
 
 1. Install [pdm](https://github.com/pdm-project/pdm)
-1. `pdm sync --dev`
+1. `pdm install --dev`
 1. Open any file you like!
 
 ## FAQ
 
 ### Why isn't this README/library written in Toki Pona?
 
 The intent is to show our methodology to the Unicode Consortium, particularly to the Script Encoding Working Group (previously the Script Ad Hoc Group). As far as we're aware, zero members of the committee know Toki Pona, which unfortunately means we fall back on English.
 
 After our proposal has been examined and a result given by the committee, I will translate this file and library into Toki Pona, with a note left behind for those who do not understand it.
 
-### Why aren't any of the specific
+### What's the deal with the tokenizers?
+
+The Toki Pona tokenizer `word_tokenize_tok` is very specific in always separating writing characters from punctuation, and leaving contiguous punctuation as contiguous- this is a level of precision that NLTK's English tokenizer does not want for several reasons, such as that English words can have "punctuation" characters in them.
+
+Toki Pona doesn't have any mid-word symbols when rendered in the Latin alphabet, so a more aggressive tokenizer is highly desirable.
+
+The other tokenizers are provided as a comparison case more than anything. I do not recommend their use.
+
+### Aren't there a lot of false positives?
+
+Yes. It's up to you to use this tool responsibly on input you've done your best to clean, and better, use stronger filters before weaker ones. For now though, here's a list of relevant false positives:
+
+- `ProperName` will errantly match text in languages without a capital/lowercase distinction, artificially inflating the scores.
+- `Alphabetic` will match a _lot_ of undesirable text- it essentially allows 14 letters of the English alphabet.
+
+### Don't some of the cleaners/filters conflict?
+
+Yes. Some do so
+
+- `ConsecutiveDuplicates` may errantly change a word's validity. For example, "manna" is phonotactically invalid in Toki Pona, but would become "mana" which is valid.
+- `ConsecutiveDuplicates` will not work correctly with syllabaries (alphabets, but representing a pair of consonant and vowel).
+
+You'll notice a _lot_ of these are troubles regarding the application of latin alphabet filters to non-latin text. Working on it!
```

