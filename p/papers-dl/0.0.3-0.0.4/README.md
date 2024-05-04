# Comparing `tmp/papers_dl-0.0.3.tar.gz` & `tmp/papers_dl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papers_dl-0.0.3.tar", last modified: Tue Apr 16 21:30:08 2024, max compression
+gzip compressed data, was "papers_dl-0.0.4.tar", last modified: Sat May  4 19:22:27 2024, max compression
```

## Comparing `papers_dl-0.0.3.tar` & `papers_dl-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.009233 papers_dl-0.0.3/
--rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.3/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     2264 2024-04-16 21:30:08.009002 papers_dl-0.0.3/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1131 2024-04-16 19:39:30.000000 papers_dl-0.0.3/README.md
--rw-r--r--   0 ben        (501) staff       (20)      972 2024-04-16 21:30:05.000000 papers_dl-0.0.3/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-04-16 21:30:08.009284 papers_dl-0.0.3/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.006910 papers_dl-0.0.3/src/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.008713 papers_dl-0.0.3/src/papers_dl.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2264 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      257 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)      225 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       13 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      577 2024-04-16 19:15:05.000000 papers_dl-0.0.3/src/parse.py
--rw-r--r--   0 ben        (501) staff       (20)    10448 2024-04-16 19:18:52.000000 papers_dl-0.0.3/src/scihub.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.007872 papers_dl-0.0.3/tests/
--rw-r--r--   0 ben        (501) staff       (20)     2130 2024-04-15 17:59:50.000000 papers_dl-0.0.3/tests/test.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.048978 papers_dl-0.0.4/
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.4/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     2450 2024-05-04 19:22:27.048654 papers_dl-0.0.4/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1131 2024-04-16 22:48:35.000000 papers_dl-0.0.4/README.md
+-rw-r--r--   0 ben        (501) staff       (20)     1158 2024-05-04 19:21:22.000000 papers_dl-0.0.4/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-04 19:22:27.049041 papers_dl-0.0.4/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.046033 papers_dl-0.0.4/src/
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.048227 papers_dl-0.0.4/src/papers_dl.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2450 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      318 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       23 2024-05-04 19:22:27.000000 papers_dl-0.0.4/src/papers_dl.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)     3562 2024-05-04 19:19:41.000000 papers_dl-0.0.4/src/papers_dl.py
+-rw-r--r--   0 ben        (501) staff       (20)     2384 2024-05-04 19:19:49.000000 papers_dl-0.0.4/src/parse.py
+-rw-r--r--   0 ben        (501) staff       (20)     7881 2024-05-04 19:19:49.000000 papers_dl-0.0.4/src/scihub.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-04 19:22:27.047929 papers_dl-0.0.4/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     1714 2024-05-04 19:19:41.000000 papers_dl-0.0.4/tests/test_cli.py
+-rw-r--r--   0 ben        (501) staff       (20)      825 2024-05-04 19:19:41.000000 papers_dl-0.0.4/tests/test_fetch.py
+-rw-r--r--   0 ben        (501) staff       (20)     2347 2024-05-04 19:19:41.000000 papers_dl-0.0.4/tests/test_parse.py
```

### Comparing `papers_dl-0.0.3/LICENSE` & `papers_dl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.3/PKG-INFO` & `papers_dl-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4
-Requires-Dist: bs4
-Requires-Dist: certifi
-Requires-Dist: cffi
-Requires-Dist: charset-normalizer
-Requires-Dist: cryptography
-Requires-Dist: easygui
-Requires-Dist: feedparser
-Requires-Dist: google
-Requires-Dist: idna
-Requires-Dist: pdf2doi
-Requires-Dist: pdfminer.six
-Requires-Dist: pdftitle
-Requires-Dist: pycparser
-Requires-Dist: PyMuPDF
-Requires-Dist: PyMuPDFb
-Requires-Dist: PyPDF2
-Requires-Dist: pyperclip
-Requires-Dist: requests
-Requires-Dist: retrying
-Requires-Dist: sgmllib3k
-Requires-Dist: six
-Requires-Dist: soupsieve
-Requires-Dist: urllib3
-Requires-Dist: w3lib
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: bs4==0.0.2
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: cffi==1.16.0
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cryptography==42.0.5
+Requires-Dist: easygui==0.98.3
+Requires-Dist: feedparser==6.0.11
+Requires-Dist: google==3.0.0
+Requires-Dist: idna==3.6
+Requires-Dist: pdf2doi==1.5.1
+Requires-Dist: pdfminer.six==20221105
+Requires-Dist: pdftitle==0.11
+Requires-Dist: pycparser==2.21
+Requires-Dist: PyMuPDF==1.23.26
+Requires-Dist: PyMuPDFb==1.23.22
+Requires-Dist: PyPDF2==2.0.0
+Requires-Dist: pyperclip==1.8.2
+Requires-Dist: requests==2.31.0
+Requires-Dist: retrying==1.3.4
+Requires-Dist: sgmllib3k==1.0.0
+Requires-Dist: six==1.16.0
+Requires-Dist: soupsieve==2.5
+Requires-Dist: urllib3==2.2.1
+Requires-Dist: w3lib==2.1.2
 
 # Overview
 `papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 ```
 usage: papers-dl.py [-h] {fetch,parse} ...
```

### Comparing `papers_dl-0.0.3/README.md` & `papers_dl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.3/pyproject.toml` & `papers_dl-0.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "papers-dl"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ben Muthalaly", email="benmuthalaly@gmail.com" },
 ]
 description = "A command line application for downloading scientific papers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "beautifulsoup4",
-  "bs4",
-  "certifi",
-  "cffi",
-  "charset-normalizer",
-  "cryptography",
-  "easygui",
-  "feedparser",
-  "google",
-  "idna",
-  "pdf2doi",
-  "pdfminer.six",
-  "pdftitle",
-  "pycparser",
-  "PyMuPDF",
-  "PyMuPDFb",
-  "PyPDF2",
-  "pyperclip",
-  "requests",
-  "retrying",
-  "sgmllib3k",
-  "six",
-  "soupsieve",
-  "urllib3",
-  "w3lib",
+  "beautifulsoup4==4.12.3",
+  "bs4==0.0.2",
+  "certifi==2024.2.2",
+  "cffi==1.16.0",
+  "charset-normalizer==3.3.2",
+  "cryptography==42.0.5",
+  "easygui==0.98.3",
+  "feedparser==6.0.11",
+  "google==3.0.0",
+  "idna==3.6",
+  "pdf2doi==1.5.1",
+  "pdfminer.six==20221105",
+  "pdftitle==0.11",
+  "pycparser==2.21",
+  "PyMuPDF==1.23.26",
+  "PyMuPDFb==1.23.22",
+  "PyPDF2==2.0.0",
+  "pyperclip==1.8.2",
+  "requests==2.31.0",
+  "retrying==1.3.4",
+  "sgmllib3k==1.0.0",
+  "six==1.16.0",
+  "soupsieve==2.5",
+  "urllib3==2.2.1",
+  "w3lib==2.1.2",
 ]
 
 [project.urls]
 Homepage = "https://github.com/benmuth/papers-dl"
 Issues = "https://github.com/benmuth/papers-dl/issues"
```

### Comparing `papers_dl-0.0.3/src/papers_dl.egg-info/PKG-INFO` & `papers_dl-0.0.4/src/papers_dl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.3
+Version: 0.0.4
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4
-Requires-Dist: bs4
-Requires-Dist: certifi
-Requires-Dist: cffi
-Requires-Dist: charset-normalizer
-Requires-Dist: cryptography
-Requires-Dist: easygui
-Requires-Dist: feedparser
-Requires-Dist: google
-Requires-Dist: idna
-Requires-Dist: pdf2doi
-Requires-Dist: pdfminer.six
-Requires-Dist: pdftitle
-Requires-Dist: pycparser
-Requires-Dist: PyMuPDF
-Requires-Dist: PyMuPDFb
-Requires-Dist: PyPDF2
-Requires-Dist: pyperclip
-Requires-Dist: requests
-Requires-Dist: retrying
-Requires-Dist: sgmllib3k
-Requires-Dist: six
-Requires-Dist: soupsieve
-Requires-Dist: urllib3
-Requires-Dist: w3lib
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: bs4==0.0.2
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: cffi==1.16.0
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cryptography==42.0.5
+Requires-Dist: easygui==0.98.3
+Requires-Dist: feedparser==6.0.11
+Requires-Dist: google==3.0.0
+Requires-Dist: idna==3.6
+Requires-Dist: pdf2doi==1.5.1
+Requires-Dist: pdfminer.six==20221105
+Requires-Dist: pdftitle==0.11
+Requires-Dist: pycparser==2.21
+Requires-Dist: PyMuPDF==1.23.26
+Requires-Dist: PyMuPDFb==1.23.22
+Requires-Dist: PyPDF2==2.0.0
+Requires-Dist: pyperclip==1.8.2
+Requires-Dist: requests==2.31.0
+Requires-Dist: retrying==1.3.4
+Requires-Dist: sgmllib3k==1.0.0
+Requires-Dist: six==1.16.0
+Requires-Dist: soupsieve==2.5
+Requires-Dist: urllib3==2.2.1
+Requires-Dist: w3lib==2.1.2
 
 # Overview
 `papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 ```
 usage: papers-dl.py [-h] {fetch,parse} ...
```

### Comparing `papers_dl-0.0.3/src/scihub.py` & `papers_dl-0.0.4/src/scihub.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-# -*- coding: utf-8 -*-
-
-# I modified this in a few ways from the `scihub.py` GH repo:
-# - the user agent is changed to work on my Mac
-# - it will now search through all Sci-Hub links from sci-hub.now.sh for the source PDF
-# instead of giving up after the first one
-# - I added a specific exception for when no identifier matches in any base Sci-Hub url
-
-"""
-Sci-API Unofficial API
-[Search|Download] research papers from [scholar.google.com|sci-hub.io].
-
-@author zaytoun
-"""
-
 from collections.abc import MutableMapping
 import re
 import hashlib
 import logging
 import os
 
 import requests
@@ -27,30 +12,22 @@
 import enum
 
 # log config
 logging.basicConfig()
 logger = logging.getLogger("Sci-Hub")
 logger.setLevel(logging.DEBUG)
 
-#
 urllib3.disable_warnings()
 
-
 # URL-DIRECT - openly accessible paper
 # URL-NON-DIRECT - pay-walled paper
 # PMID - PubMed ID
 # DOI - digital object identifier
 IDClass = enum.Enum("identifier", ["URL-DIRECT", "URL-NON-DIRECT", "PMD", "DOI"])
 
-# constants
-SCHOLARS_BASE_URL = "https://scholar.google.com/scholar"
-HEADERS: MutableMapping = {
-    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3 Safari/605.1.15"
-}
-
 
 class IdentifierNotFoundError(Exception):
     pass
 
 
 class SiteAccessError(Exception):
     pass
@@ -62,17 +39,19 @@
 
 class SciHub(object):
     """
     SciHub class can search for papers on Google Scholar
     and fetch/download papers from sci-hub.io
     """
 
-    def __init__(self):
+    def __init__(self, user_agent):
         self.sess = requests.Session()
-        self.sess.headers = HEADERS
+        self.sess.headers = {
+            "User-Agent": user_agent,
+        }
         self.available_base_url_list = self._get_available_scihub_urls()
 
         self.base_url = self.available_base_url_list[0] + "/"
 
     def _get_available_scihub_urls(self):
         """
         Finds available scihub urls via https://sci-hub.now.sh/
@@ -104,134 +83,78 @@
             self.sess.proxies = {
                 "http": proxy,
                 "https": proxy,
             }
 
     def _change_base_url(self):
         if not self.available_base_url_list:
-            logger.critical("Ran out of valid sci-hub urls")
+            logger.error("Ran out of valid sci-hub urls")
             raise IdentifierNotFoundError()
         del self.available_base_url_list[0]
         self.base_url = self.available_base_url_list[0] + "/"
         logger.info("I'm changing to {}".format(self.available_base_url_list[0]))
 
-    def search(self, query, limit=10, download=False):
-        """
-        Performs a query on scholar.google.com, and returns a dictionary
-        of results in the form {'papers': ...}. Unfortunately, as of now,
-        captchas can potentially prevent searches after a certain limit.
-        """
-        start = 0
-        results = {"papers": []}
-
-        while True:
-            try:
-                res = self.sess.get(
-                    SCHOLARS_BASE_URL, params={"q": query, "start": start}
-                )
-            except requests.exceptions.RequestException as e:
-                logger.error(
-                    "Failed to complete search with query %s (connection error)", query
-                )
-                raise e
-
-            s = self._get_soup(res.content)
-            papers = s.find_all("div", class_="gs_r")
-
-            if not papers:
-                if "CAPTCHA" in str(res.content):
-                    logger.error(
-                        "Failed to complete search with query %s (captcha)", query
-                    )
-                    raise SiteAccessError
-
-            for paper in papers:
-                if not paper.find("table"):
-                    source = None
-                    pdf = paper.find("div", class_="gs_ggs gs_fl")
-                    link = paper.find("h3", class_="gs_rt")
-
-                    if pdf:
-                        source = pdf.find("a")["href"]
-                    elif link.find("a"):
-                        source = link.find("a")["href"]
-                    else:
-                        continue
-
-                    results["papers"].append({"name": link.text, "url": source})
-
-                    if len(results["papers"]) >= limit:
-                        return results
-
-            start += 10
-
-    @retry(wait_random_min=100, wait_random_max=1000, stop_max_attempt_number=10)
-    def download(self, identifier, destination="", path=None) -> dict[str, bytes | str] | None:
+    def download(self, identifier, destination="", path=None) -> dict[str, str] | None:
         """
         Downloads a paper from sci-hub given an indentifier (DOI, PMID, URL).
         Currently, this can potentially be blocked by a captcha if a certain
         limit has been reached.
         """
         data = self.fetch(identifier)
 
         # TODO: allow for passing in name
         if data:
             self._save(
-                data["pdf"], os.path.join(destination, path if path else data["name"])
+                data["pdf"],
+                os.path.join(destination, path if path else data["name"]),
             )
         return data
 
-    def fetch(self, identifier) -> dict[str, bytes | str] | None:
+    @retry(wait_random_min=100, wait_random_max=1000, stop_max_attempt_number=20)
+    def fetch(self, identifier) -> dict[str, str | bytes | None] | None:
         """
         Fetches the paper by first retrieving the direct link to the pdf.
         If the indentifier is a DOI, PMID, or URL pay-wall, then use Sci-Hub
         to access and download paper. Otherwise, just download paper directly.
         """
         url = None
         try:
+            # find the url to the pdf for a given identifier
             url = self._get_direct_url(identifier)
-            if not url:
-                raise ValueError("No URL found")
+            logger.info("Found potential source at %s", identifier)
+
             # verify=False is dangerous but sci-hub.io
             # requires intermediate certificates to verify
             # and requests doesn't know how to download them.
             # as a hacky fix, you can add them to your store
             # and verifying would work. will fix this later.
             # NOTE(ben): see this SO answer: https://stackoverflow.com/questions/27068163/python-requests-not-handling-missing-intermediate-certificate-only-from-one-mach
             res = self.sess.get(url, verify=True)
 
             if res.headers["Content-Type"] != "application/pdf":
-                logger.info(
-                    "Failed to fetch pdf with identifier %s (resolved url %s) due to captcha",
+                logger.error(
+                    "Failed to fetch PDF with identifier %s (resolved url %s) due to captcha, changing url...",
                     identifier,
                     url,
                 )
                 self._change_base_url()
-                raise SiteAccessError()
+                raise CaptchaNeededError("Failed to fetch PDF due to captcha")
             else:
                 return {
                     "pdf": res.content,
                     "url": url,
                     "name": self._generate_name(res),
                 }
 
-        except requests.exceptions.ConnectionError as e:
+        except Exception as e:
             logger.info(
-                "Cannot access %s, changing url", self.available_base_url_list[0]
+                "Cannot access %s: %s, changing url...", self.available_base_url_list[0], e
             )
             self._change_base_url()
-            raise e
-
-        except requests.exceptions.RequestException as e:
-            logger.error(
-                "Failed to fetch pdf with identifier %s (resolved url %s) due to request exception.",
-                identifier,
-                url,
-            )
-            return None
+            raise SiteAccessError("Failed to access site")
 
     def _get_direct_url(self, identifier: str) -> str | None:
         """
         Finds the direct source url for a given identifier.
         """
         id_type = self._classify(identifier)
 
@@ -285,15 +208,15 @@
         """
         Save a file give data and a path.
         """
         try:
             with open(path, "wb") as f:
                 f.write(data)
         except Exception as e:
-            logger.info("Failed to write to %s (%s)", path, e.__str__)
+            logger.error("Failed to write to %s (%s)", path, e.__str__)
             raise e
 
     def _get_soup(self, html):
         """
         Return html soup.
         """
         return BeautifulSoup(html, "html.parser")
```

