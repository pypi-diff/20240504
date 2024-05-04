# Comparing `tmp/edgarquery-0.0.59.tar.gz` & `tmp/edgarquery-0.0.60.tar.gz`

## Comparing `edgarquery-0.0.59.tar` & `edgarquery-0.0.60.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 edgarquery-0.0.59/genusage.sh
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.59/notes.txt
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.59/scripts/edgarquery.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.59/scripts/edgartickerstocsv.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/__about__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/__init__.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/concepts.sh
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/ebquery.py
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcikperson.py
--rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyconcepttocsv.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsshow.py
--rwxr-xr-x   0        0        0     5961 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyfactstocsv.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsziptocsv.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarlatest10K.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarlatestsubmissions.py
--rwxr-xr-x   0        0        0    15138 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarquery.py
--rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarsubmissions.py
--rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarsubmissionsziptocsv.py
--rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgartickerstocsv.py
--rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/edgarxbrlframestocsv.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/sedfile
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.59/src/edgarquery/tickerd.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/__init__.py
--rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/p.sh
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/s.sh
--rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/x.sh
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.59/tests/y.sh
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.59/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.59/LICENSE.txt
--rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 edgarquery-0.0.59/README.md
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 edgarquery-0.0.59/pyproject.toml
--rw-r--r--   0        0        0     9421 2020-02-02 00:00:00.000000 edgarquery-0.0.59/PKG-INFO
+-rwxr-xr-x   0        0        0      621 2020-02-02 00:00:00.000000 edgarquery-0.0.60/genusage.sh
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.60/notes.txt
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.60/scripts/edgarquery.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.60/scripts/edgartickerstocsv.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/__about__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/__init__.py
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/concepts.sh
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/ebquery.py
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcikperson.py
+-rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyconcepttocsv.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsshow.py
+-rwxr-xr-x   0        0        0     5961 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyfactstocsv.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsziptocsv.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarlatest10K.py
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarlatestsubmission.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarlatestsubmissions.py
+-rwxr-xr-x   0        0        0    15138 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarquery.py
+-rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarsubmissions.py
+-rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarsubmissionsziptocsv.py
+-rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgartickerstocsv.py
+-rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/edgarxbrlframestocsv.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/sedfile
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.60/src/edgarquery/tickerd.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/__init__.py
+-rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/p.sh
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/s.sh
+-rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/x.sh
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.60/tests/y.sh
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.60/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.60/LICENSE.txt
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 edgarquery-0.0.60/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 edgarquery-0.0.60/pyproject.toml
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 edgarquery-0.0.60/PKG-INFO
```

### Comparing `edgarquery-0.0.59/notes.txt` & `edgarquery-0.0.60/notes.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/scripts/edgarquery.py` & `edgarquery-0.0.60/scripts/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/ebquery.py` & `edgarquery-0.0.60/src/edgarquery/ebquery.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
                 resp = urllib.request.urlopen(req)
                 return resp
             except urllib.error.URLError as e:
                 print("Error %s(%s): %s" % ('query', url, e.reason),
                               file=sys.stderr )
                 if e.reason == 'Not Found':
                     return None
+                if e.reason == 'Forbidden':
+                    return None
                 if tries < ntries:
                     print('retrying in %d seconds' % (pause),
                         file=sys.stderr)
                     time.sleep(pause)
                     tries = tries + 1
                     pause = pause * 2
                     continue
```

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarcikperson.py` & `edgarquery-0.0.60/src/edgarquery/edgarcikperson.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarcompanyconcepttocsv.py` & `edgarquery-0.0.60/src/edgarquery/edgarcompanyconcepttocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsshow.py` & `edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsshow.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarcompanyfactstocsv.py` & `edgarquery-0.0.60/src/edgarquery/edgarcompanyfactstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarcompanyfactsziptocsv.py` & `edgarquery-0.0.60/src/edgarquery/edgarcompanyfactsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarlatest10K.py` & `edgarquery-0.0.60/src/edgarquery/edgarlatest10K.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarlatestsubmissions.py` & `edgarquery-0.0.60/src/edgarquery/edgarlatestsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarquery.py` & `edgarquery-0.0.60/src/edgarquery/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarsubmissions.py` & `edgarquery-0.0.60/src/edgarquery/edgarsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarsubmissionsziptocsv.py` & `edgarquery-0.0.60/src/edgarquery/edgarsubmissionsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgartickerstocsv.py` & `edgarquery-0.0.60/src/edgarquery/edgartickerstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/edgarxbrlframestocsv.py` & `edgarquery-0.0.60/src/edgarquery/edgarxbrlframestocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/src/edgarquery/tickerd.py` & `edgarquery-0.0.60/src/edgarquery/tickerd.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/tests/p.sh` & `edgarquery-0.0.60/tests/p.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/tests/x.sh` & `edgarquery-0.0.60/tests/x.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/LICENSE.txt` & `edgarquery-0.0.60/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.59/README.md` & `edgarquery-0.0.60/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ## Usage
 
 <br/>
 ##<br/>
 ## edgarcikperson<br/>
 ##<br/>
-usage: edgarcikperson [-h] [--cikpersondb CIKPERSONDB] [--file FILE]<br/>
+usage: cikperson [-h] [--cikpersondb CIKPERSONDB] [--file FILE]<br/>
 <br/>
 extract CIK and person names from form345 zip files<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cikpersondb CIKPERSONDB<br/>
 full path to the sqlite3 database - default in memory<br/>
@@ -88,16 +88,16 @@
 --directory DIRECTORY<br/>
 where to deposit the csv fileѕ<br/>
 <br/>
 <br/>
 ##<br/>
 ## edgarcompanyfactsziptocsv<br/>
 ##<br/>
-usage: edgarcompanyfactsziptocsv [-h] --zipfile ZIPFILE [--directory DIRECTORY]<br/>
-[--files FILES]<br/>
+usage: edgarcompanyfactsziptocsv [-h] --zipfile ZIPFILE<br/>
+[--directory DIRECTORY] [--files FILES]<br/>
 <br/>
 Extract one or more json files from an SEC EDGAR companyfacts.zip file and<br/>
 convert to CSV<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --zipfile ZIPFILE     submissions.zip file to process. Іt can be downloadæd<br/>
@@ -105,70 +105,50 @@
 --directory DIRECTORY<br/>
 where to deposit the output<br/>
 --files FILES         comma separated(no spaces) content file(s) to process<br/>
 a subset of the files in the zip file<br/>
 <br/>
 <br/>
 ##<br/>
-## edgarquery<br/>
+## edgarlatest10K<br/>
 ##<br/>
-usage: edgarquery [-h] [--cik CIK] [--ticker TICKER] [--cy CY] [--frame FRAME]<br/>
-[--units UNITS] [--fact FACT] [--directory DIRECTORY]<br/>
-[--file FILE] [--companyconcept] [--companyfacts]<br/>
-[--xbrlframes] [--companyfactsarchivezip] [--submissionszip]<br/>
-[--financialstatementandnotesdataset]<br/>
+usage: edgarlatest10K [-h] [--cik CIK] [--ticker TICKER] [--link]<br/>
+[--directory DIRECTORY] [--show]<br/>
 <br/>
-query SEC EDGAR site NOTE thæt EQEMAIL env variable is required and must<br/>
-contain a valid User-Agent such as your email address<br/>
+find the most recent 10-K for cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
---ticker TICKER       company stock ticker<br/>
---cy CY               calendar year e.g. CY2023, CY2023Q1, CY2023Q4I<br/>
---frame FRAME         reporting frame e.g us-gaap, ifrs-full, dei, srt<br/>
---units UNITS         USD or shares<br/>
---fact FACT           fact to collect e.g AccountsPayableCurrent, USD-per-<br/>
-shares<br/>
+--ticker TICKER       company ticker symbol<br/>
+--link                return the url for the latest 10-K<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
---file FILE           file in which to store the output argument allowed for<br/>
-each query type if --directory is not provided, it<br/>
-should be the full path<br/>
---companyconcept      returns all the XBRL disclosures from a single company<br/>
---cik or --ticker required --frame - default us-gaap --fact -<br/>
-default USD-per-shares<br/>
---companyfacts        aggregates one fact for each reporting entity that is<br/>
-last filed that most closely fits the calendrical<br/>
-period requested --cik <br/>
---xbrlframes          returns all the company concepts data for a CIK --cy<br/>
-required<br/>
---companyfactsarchivezip<br/>
-returns daily companyfacts index in a zip file<br/>
---submissionszip      returns daily index of submissions in a zip file<br/>
---financialstatementandnotesdataset<br/>
-returns zip file with financial statement and notes<br/>
-summaries --cy required<br/>
+--show                show the 10-K stored in directory to your browser<br/>
 <br/>
 <br/>
 ##<br/>
-## edgarlatest10K<br/>
+## edgarlatestsubmission<br/>
 ##<br/>
-usage: edgarlatest10K [-h] [--cik CIK] [--ticker TICKER] [--link]<br/>
-[--directory DIRECTORY]<br/>
+usage: edgarlatestsubmission [-h] [--cik CIK] [--ticker TICKER]<br/>
+[--submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}]<br/>
+[--link] [--directory DIRECTORY] [--show]<br/>
 <br/>
-find the most recent 10-K for cik<br/>
+find the most recent X-K for cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
---link                return the url for the latest 10-K<br/>
+--submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}<br/>
+X-K submission type<br/>
+--link                return the url for the latest X-K<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
+--show                show the X-K stored in directory to your browser<br/>
 <br/>
 <br/>
 ##<br/>
 ## edgarlatestsubmissions<br/>
 ##<br/>
 usage: edgarlatestsubmissions [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--directory DIRECTORY] [--file FILE]<br/>
@@ -181,14 +161,57 @@
 --ticker TICKER       company ticker symbol<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
 --file FILE           where to store the output<br/>
 <br/>
 <br/>
 ##<br/>
+## edgarquery<br/>
+##<br/>
+usage: edgarquery [-h] [--cik CIK] [--ticker TICKER] [--cy CY]<br/>
+[--frame FRAME] [--units UNITS] [--fact FACT]<br/>
+[--directory DIRECTORY] [--file FILE] [--companyconcept]<br/>
+[--companyfacts] [--xbrlframes]<br/>
+[--companyfactsarchivezip] [--submissionszip]<br/>
+[--financialstatementandnotesdataset]<br/>
+<br/>
+query SEC EDGAR site NOTE thæt EQEMAIL env variable is required and must<br/>
+contain a valid User-Agent such as your email address<br/>
+<br/>
+options:<br/>
+-h, --help            show this help message and exit<br/>
+--cik CIK             10-digit Central Index Key<br/>
+--ticker TICKER       company stock ticker<br/>
+--cy CY               calendar year e.g. CY2023, CY2023Q1, CY2023Q4I<br/>
+--frame FRAME         reporting frame e.g us-gaap, ifrs-full, dei, srt<br/>
+--units UNITS         USD or shares<br/>
+--fact FACT           fact to collect e.g AccountsPayableCurrent, USD-per-<br/>
+shares<br/>
+--directory DIRECTORY<br/>
+directory to store the output<br/>
+--file FILE           file in which to store the output argument allowed for<br/>
+each query type if --directory is not provided, it<br/>
+should be the full path<br/>
+--companyconcept      returns all the XBRL disclosures from a single company<br/>
+--cik required --frame - default us-gaap --fact -<br/>
+default USD-per-shares<br/>
+--companyfacts        aggregates one fact for each reporting entity that is<br/>
+last filed that most closely fits the calendrical<br/>
+period requested --cik required<br/>
+--xbrlframes          returns all the company concepts data for a CIK --cy<br/>
+required<br/>
+--companyfactsarchivezip<br/>
+returns daily companyfacts index in a zip file<br/>
+--submissionszip      returns daily index of submissions in a zip file<br/>
+--financialstatementandnotesdataset<br/>
+returns zip file with financial statement and notes<br/>
+summaries --cy required<br/>
+<br/>
+<br/>
+##<br/>
 ## edgarsubmissions<br/>
 ##<br/>
 usage: edgarsubmissions [-h] [--cik CIK] [--ticker TICKER] [--year YEAR]<br/>
 [--file FILE] [--directory DIRECTORY]<br/>
 <br/>
 find the most recent submissions for cik<br/>
 <br/>
@@ -201,16 +224,16 @@
 --directory DIRECTORY<br/>
 store the output in this directory<br/>
 <br/>
 <br/>
 ##<br/>
 ## edgarsubmissionsziptocsv<br/>
 ##<br/>
-usage: edgarsubmissionsziptocsv [-h] [--zipfile ZIPFILE] [--directory DIRECTORY]<br/>
-[--files FILES]<br/>
+usage: edgarsubmissionsziptocsv [-h] [--zipfile ZIPFILE]<br/>
+[--directory DIRECTORY] [--files FILES]<br/>
 <br/>
 Extract one or more json files from an SEC EDGAR submissions.zip file and<br/>
 convert to CSV<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --zipfile ZIPFILE     submissions.zip file to process - required<br/>
```

### Comparing `edgarquery-0.0.59/pyproject.toml` & `edgarquery-0.0.60/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 edgarcompanyconcepttocsv = "edgarquery.edgarcompanyconcepttocsv:main"
 edgarcompanyfactstocsv = "edgarquery.edgarcompanyfactstocsv:main"
 edgarcompanyfactsshow = "edgarquery.edgarcompanyfactsshow:main"
 edgarcompanyfactsziptocsv = "edgarquery.edgarcompanyfactsziptocsv:main"
 edgarcikperson = "edgarquery.edgarcikperson:main"
 edgarquery = "edgarquery.edgarquery:main"
 edgarlatest10K = "edgarquery.edgarlatest10K:main"
+edgarlatestsubmission = "edgarquery.edgarlatestsubmission:main"
 edgarlatestsubmissions = "edgarquery.edgarlatestsubmissions:main"
 edgarsubmissions = "edgarquery.edgarsubmissions:main"
 edgarsubmissionsziptocsv = "edgarquery.edgarsubmissionsziptocsv:main"
 edgartickerstocsv = "edgarquery.edgartickerstocsv:main"
 edgarxbrlframestocsv = "edgarquery.edgarxbrlframestocsv:main"
 
 #scripts/__pycache__:
```

### Comparing `edgarquery-0.0.59/PKG-INFO` & `edgarquery-0.0.60/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgarquery
-Version: 0.0.59
+Version: 0.0.60
 Summary: Downloads various SEC EDGAR files by CIK or ticker.  companyfactsshow displays company facts in your browser
 Project-URL: Documentation, https://github.com/dfwcnj/edgarquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/edgarquery/issues
 Project-URL: Source, https://github.com/dfwcnj/edgarquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -50,15 +50,15 @@
 
 ## Usage
 
 <br/>
 ##<br/>
 ## edgarcikperson<br/>
 ##<br/>
-usage: edgarcikperson [-h] [--cikpersondb CIKPERSONDB] [--file FILE]<br/>
+usage: cikperson [-h] [--cikpersondb CIKPERSONDB] [--file FILE]<br/>
 <br/>
 extract CIK and person names from form345 zip files<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cikpersondb CIKPERSONDB<br/>
 full path to the sqlite3 database - default in memory<br/>
@@ -110,16 +110,16 @@
 --directory DIRECTORY<br/>
 where to deposit the csv fileѕ<br/>
 <br/>
 <br/>
 ##<br/>
 ## edgarcompanyfactsziptocsv<br/>
 ##<br/>
-usage: edgarcompanyfactsziptocsv [-h] --zipfile ZIPFILE [--directory DIRECTORY]<br/>
-[--files FILES]<br/>
+usage: edgarcompanyfactsziptocsv [-h] --zipfile ZIPFILE<br/>
+[--directory DIRECTORY] [--files FILES]<br/>
 <br/>
 Extract one or more json files from an SEC EDGAR companyfacts.zip file and<br/>
 convert to CSV<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --zipfile ZIPFILE     submissions.zip file to process. Іt can be downloadæd<br/>
@@ -127,70 +127,50 @@
 --directory DIRECTORY<br/>
 where to deposit the output<br/>
 --files FILES         comma separated(no spaces) content file(s) to process<br/>
 a subset of the files in the zip file<br/>
 <br/>
 <br/>
 ##<br/>
-## edgarquery<br/>
+## edgarlatest10K<br/>
 ##<br/>
-usage: edgarquery [-h] [--cik CIK] [--ticker TICKER] [--cy CY] [--frame FRAME]<br/>
-[--units UNITS] [--fact FACT] [--directory DIRECTORY]<br/>
-[--file FILE] [--companyconcept] [--companyfacts]<br/>
-[--xbrlframes] [--companyfactsarchivezip] [--submissionszip]<br/>
-[--financialstatementandnotesdataset]<br/>
+usage: edgarlatest10K [-h] [--cik CIK] [--ticker TICKER] [--link]<br/>
+[--directory DIRECTORY] [--show]<br/>
 <br/>
-query SEC EDGAR site NOTE thæt EQEMAIL env variable is required and must<br/>
-contain a valid User-Agent such as your email address<br/>
+find the most recent 10-K for cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
---ticker TICKER       company stock ticker<br/>
---cy CY               calendar year e.g. CY2023, CY2023Q1, CY2023Q4I<br/>
---frame FRAME         reporting frame e.g us-gaap, ifrs-full, dei, srt<br/>
---units UNITS         USD or shares<br/>
---fact FACT           fact to collect e.g AccountsPayableCurrent, USD-per-<br/>
-shares<br/>
+--ticker TICKER       company ticker symbol<br/>
+--link                return the url for the latest 10-K<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
---file FILE           file in which to store the output argument allowed for<br/>
-each query type if --directory is not provided, it<br/>
-should be the full path<br/>
---companyconcept      returns all the XBRL disclosures from a single company<br/>
---cik or --ticker required --frame - default us-gaap --fact -<br/>
-default USD-per-shares<br/>
---companyfacts        aggregates one fact for each reporting entity that is<br/>
-last filed that most closely fits the calendrical<br/>
-period requested --cik <br/>
---xbrlframes          returns all the company concepts data for a CIK --cy<br/>
-required<br/>
---companyfactsarchivezip<br/>
-returns daily companyfacts index in a zip file<br/>
---submissionszip      returns daily index of submissions in a zip file<br/>
---financialstatementandnotesdataset<br/>
-returns zip file with financial statement and notes<br/>
-summaries --cy required<br/>
+--show                show the 10-K stored in directory to your browser<br/>
 <br/>
 <br/>
 ##<br/>
-## edgarlatest10K<br/>
+## edgarlatestsubmission<br/>
 ##<br/>
-usage: edgarlatest10K [-h] [--cik CIK] [--ticker TICKER] [--link]<br/>
-[--directory DIRECTORY]<br/>
+usage: edgarlatestsubmission [-h] [--cik CIK] [--ticker TICKER]<br/>
+[--submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}]<br/>
+[--link] [--directory DIRECTORY] [--show]<br/>
 <br/>
-find the most recent 10-K for cik<br/>
+find the most recent X-K for cik<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --cik CIK             10-digit Central Index Key<br/>
 --ticker TICKER       company ticker symbol<br/>
---link                return the url for the latest 10-K<br/>
+--submission {SC 13D,13F-HR,DEF 14A,8-K,10-K,10-Q}<br/>
+X-K submission type<br/>
+--link                return the url for the latest X-K<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
+--show                show the X-K stored in directory to your browser<br/>
 <br/>
 <br/>
 ##<br/>
 ## edgarlatestsubmissions<br/>
 ##<br/>
 usage: edgarlatestsubmissions [-h] [--cik CIK] [--ticker TICKER]<br/>
 [--directory DIRECTORY] [--file FILE]<br/>
@@ -203,14 +183,57 @@
 --ticker TICKER       company ticker symbol<br/>
 --directory DIRECTORY<br/>
 directory to store the output<br/>
 --file FILE           where to store the output<br/>
 <br/>
 <br/>
 ##<br/>
+## edgarquery<br/>
+##<br/>
+usage: edgarquery [-h] [--cik CIK] [--ticker TICKER] [--cy CY]<br/>
+[--frame FRAME] [--units UNITS] [--fact FACT]<br/>
+[--directory DIRECTORY] [--file FILE] [--companyconcept]<br/>
+[--companyfacts] [--xbrlframes]<br/>
+[--companyfactsarchivezip] [--submissionszip]<br/>
+[--financialstatementandnotesdataset]<br/>
+<br/>
+query SEC EDGAR site NOTE thæt EQEMAIL env variable is required and must<br/>
+contain a valid User-Agent such as your email address<br/>
+<br/>
+options:<br/>
+-h, --help            show this help message and exit<br/>
+--cik CIK             10-digit Central Index Key<br/>
+--ticker TICKER       company stock ticker<br/>
+--cy CY               calendar year e.g. CY2023, CY2023Q1, CY2023Q4I<br/>
+--frame FRAME         reporting frame e.g us-gaap, ifrs-full, dei, srt<br/>
+--units UNITS         USD or shares<br/>
+--fact FACT           fact to collect e.g AccountsPayableCurrent, USD-per-<br/>
+shares<br/>
+--directory DIRECTORY<br/>
+directory to store the output<br/>
+--file FILE           file in which to store the output argument allowed for<br/>
+each query type if --directory is not provided, it<br/>
+should be the full path<br/>
+--companyconcept      returns all the XBRL disclosures from a single company<br/>
+--cik required --frame - default us-gaap --fact -<br/>
+default USD-per-shares<br/>
+--companyfacts        aggregates one fact for each reporting entity that is<br/>
+last filed that most closely fits the calendrical<br/>
+period requested --cik required<br/>
+--xbrlframes          returns all the company concepts data for a CIK --cy<br/>
+required<br/>
+--companyfactsarchivezip<br/>
+returns daily companyfacts index in a zip file<br/>
+--submissionszip      returns daily index of submissions in a zip file<br/>
+--financialstatementandnotesdataset<br/>
+returns zip file with financial statement and notes<br/>
+summaries --cy required<br/>
+<br/>
+<br/>
+##<br/>
 ## edgarsubmissions<br/>
 ##<br/>
 usage: edgarsubmissions [-h] [--cik CIK] [--ticker TICKER] [--year YEAR]<br/>
 [--file FILE] [--directory DIRECTORY]<br/>
 <br/>
 find the most recent submissions for cik<br/>
 <br/>
@@ -223,16 +246,16 @@
 --directory DIRECTORY<br/>
 store the output in this directory<br/>
 <br/>
 <br/>
 ##<br/>
 ## edgarsubmissionsziptocsv<br/>
 ##<br/>
-usage: edgarsubmissionsziptocsv [-h] [--zipfile ZIPFILE] [--directory DIRECTORY]<br/>
-[--files FILES]<br/>
+usage: edgarsubmissionsziptocsv [-h] [--zipfile ZIPFILE]<br/>
+[--directory DIRECTORY] [--files FILES]<br/>
 <br/>
 Extract one or more json files from an SEC EDGAR submissions.zip file and<br/>
 convert to CSV<br/>
 <br/>
 options:<br/>
 -h, --help            show this help message and exit<br/>
 --zipfile ZIPFILE     submissions.zip file to process - required<br/>
```

