# Comparing `tmp/geoparser-0.1.4.tar.gz` & `tmp/geoparser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoparser-0.1.4.tar", last modified: Sat Apr 27 17:11:00 2024, max compression
+gzip compressed data, was "geoparser-0.1.5.tar", last modified: Sat May  4 17:19:45 2024, max compression
```

## Comparing `geoparser-0.1.4.tar` & `geoparser-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 17:11:00.453529 geoparser-0.1.4/
--rw-rw-rw-   0        0        0     1083 2024-04-27 16:24:43.000000 geoparser-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     4408 2024-04-27 17:11:00.453529 geoparser-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4006 2024-04-27 17:04:25.000000 geoparser-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 17:11:00.436530 geoparser-0.1.4/geoparser/
--rw-rw-rw-   0        0        0       34 2024-04-27 16:24:43.000000 geoparser-0.1.4/geoparser/__init__.py
--rw-rw-rw-   0        0        0      232 2024-04-27 16:24:43.000000 geoparser-0.1.4/geoparser/__main__.py
--rw-rw-rw-   0        0        0     3977 2024-04-27 16:24:43.000000 geoparser-0.1.4/geoparser/downloader.py
--rw-rw-rw-   0        0        0     1525 2024-04-27 16:24:43.000000 geoparser-0.1.4/geoparser/entities.py
--rw-rw-rw-   0        0        0     5583 2024-04-27 16:24:43.000000 geoparser-0.1.4/geoparser/gazetteer.py
--rw-rw-rw-   0        0        0     8415 2024-04-27 16:24:43.000000 geoparser-0.1.4/geoparser/geoparser.py
-drwxrwxrwx   0        0        0        0 2024-04-27 17:11:00.452531 geoparser-0.1.4/geoparser.egg-info/
--rw-rw-rw-   0        0        0     4408 2024-04-27 17:11:00.000000 geoparser-0.1.4/geoparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-04-27 17:11:00.000000 geoparser-0.1.4/geoparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 17:11:00.000000 geoparser-0.1.4/geoparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-27 17:11:00.000000 geoparser-0.1.4/geoparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 17:11:00.000000 geoparser-0.1.4/geoparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 17:11:00.453529 geoparser-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      763 2024-04-27 17:09:29.000000 geoparser-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:19:45.709174 geoparser-0.1.5/
+-rw-rw-rw-   0        0        0     1083 2024-05-04 16:50:30.000000 geoparser-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     5547 2024-05-04 17:19:45.708176 geoparser-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5145 2024-05-04 16:50:30.000000 geoparser-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 17:19:45.691173 geoparser-0.1.5/geoparser/
+-rw-rw-rw-   0        0        0       34 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/__init__.py
+-rw-rw-rw-   0        0        0      890 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/__main__.py
+-rw-rw-rw-   0        0        0     6101 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/database.py
+-rw-rw-rw-   0        0        0     2663 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/downloader.py
+-rw-rw-rw-   0        0        0     1525 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/entities.py
+-rw-rw-rw-   0        0        0    11661 2024-05-04 16:50:30.000000 geoparser-0.1.5/geoparser/geoparser.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:19:45.707174 geoparser-0.1.5/geoparser.egg-info/
+-rw-rw-rw-   0        0        0     5547 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 17:19:45.000000 geoparser-0.1.5/geoparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 17:19:45.709174 geoparser-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-05-04 16:50:30.000000 geoparser-0.1.5/setup.py
```

### Comparing `geoparser-0.1.4/LICENSE` & `geoparser-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.4/PKG-INFO` & `geoparser-0.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,98 @@
-Metadata-Version: 2.1
-Name: geoparser
-Version: 0.1.4
-Summary: A geoparsing library for English texts
-Author: Diego Gomes
-Author-email: diego.gomes@uzh.ch
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Geoparser
 
-Geoparser is a Python library for geoparsing English texts. It leverages spaCy for toponym recognition and tine-tuned SentenceTransformer models for toponym resolution.
+Geoparser is a Python library for geoparsing English texts. It leverages spaCy for toponym recognition and fine-tuned SentenceTransformer models for toponym resolution.
 
 ## Installation
 
 Install Geoparser using pip:
 
 ```bash
 pip install geoparser
 ```
 
+## Dependencies
+
+Geoparser depends on the following Python libraries:
+
+- **[appdirs](https://github.com/ActiveState/appdirs)**
+- **[numpy](https://numpy.org/)**
+- **[pandas](https://pandas.pydata.org/)**
+- **[requests](https://requests.readthedocs.io/en/latest/)**
+- **[sentence_transformers](https://www.sbert.net/)**
+- **[spacy](https://spacy.io/)**
+- **[torch](https://pytorch.org/)**
+- **[tqdm](https://tqdm.github.io/)**
+
+These dependencies are automatically installed when building Geoparser with pip.
+
 ## Download Required Data
 
-After installation, you need to download the necessary data files for Geoparser to function properly:
+After installation, you need to execute the following command to download the necessary files for Geoparser to function:
 
 ```bash
 python -m geoparser download
 ```
 
-This command will download the following resources:
+This command will download the following resources and setup a SQLite database for the GeoNames data:
 
 - **spaCy Models**: Two models are downloaded:
   - `en_core_web_sm`: A less accurate but faster model.
   - `en_core_web_trf`: A more accurate but slower model.
 - **GeoNames Data**: The following files are downloaded from GeoNames:
   - [All Countries](http://download.geonames.org/export/dump/allCountries.zip)
+  - [Alternate Names](https://download.geonames.org/export/dump/alternateNames.zip)
   - [Admin1 Codes](http://download.geonames.org/export/dump/admin1CodesASCII.txt)
   - [Admin2 Codes](http://download.geonames.org/export/dump/admin2Codes.txt)
   - [Country Info](http://download.geonames.org/export/dump/countryInfo.txt)
   - [Feature Codes](http://download.geonames.org/export/dump/featureCodes_en.txt)
 
-These files are stored in the user-specific data directory:
+These files are temporarily stored in your system's user-specific data directory during the database setup. Once the database has been populated with the data, the original files are automatically deleted to free up space. The database is then stored in this location:
 
-- **Windows**: `C:\Users\<Username>\AppData\Local\geoparser\`
-- **macOS**: `~/Library/Application Support/geoparser/`
-- **Linux**: `~/.local/share/geoparser/`
+- **Windows**: `C:\Users\<Username>\AppData\Local\geoparser\geonames.db`
+- **macOS**: `~/Library/Application Support/geoparser/geonames.db`
+- **Linux**: `~/.local/share/geoparser/geonames.db`
 
-Please ensure you have adequate disk space available, as the total size of these files is approximately 2.3 GB.
+Please ensure you have enough disk space available. The final size of the downloaded GeoNames data will be approximately 3.2 GB, increasing temporarily to 5.5 GB during the download and setup process.
 
 ## Usage
 
 ### Instantiating the Geoparser
 
-To use Geoparser, you need to instantiate an object of the `Geoparser` class. You can specify which spaCy and transformer model to use, optimizing either for accuracy or speed. By default, the library uses accuracy-optimized models:
+To use Geoparser, you need to instantiate an object of the `Geoparser` class. You can specify which spaCy and transformer model to use, optimising either for accuracy or speed. By default, the library uses accuracy-optimised models:
 
 ```python
 from geoparser import Geoparser
 
 geo = Geoparser()
 ```
 
+Default configuration:
+
+```python
+geo = Geoparser(spacy_model='en_core_web_trf', transformer_model='dguzh/geo-all-distilroberta-v1')
+```
+
 For faster performance, you can opt for the smaller models:
 
 ```python
 geo = Geoparser(spacy_model='en_core_web_sm', transformer_model='dguzh/geo-all-MiniLM-L6-v2')
 ```
 
-You can mix and match these models depending on your specific needs. Note that the transformer models `dguzh/geo-all-distilroberta-v1` and `dguzh/geo-all-MiniLM-L6-v2` are preliminary versions. Future updates aim to refine these models to improve the accuracy of toponym disambiguation.
+You can mix and match these models depending on your specific needs. Note that the SentenceTransformer models `dguzh/geo-all-distilroberta-v1` and `dguzh/geo-all-MiniLM-L6-v2` are preliminary versions. Future updates aim to refine these models to improve the accuracy of toponym disambiguation.
 
 ### Parsing Texts
 
-Geoparser is optimized for parsing large collections of texts at once. Pass a list of strings to the `parse` method:
+Geoparser is optimised for parsing large collections of texts at once. Pass a list of strings to the `parse` method:
 
 ```python
 docs = geo.parse(["Sample text 1", "Sample text 2", "Sample text 3"])
 ```
 
-The `parse` method returns a list of `Document` objects, where each `Document` contains a list of `Toponym` objects. Each `Toponym` that is successfully geocoded will have a corresponding `Location` object with detailed geographical data:
-
-### Location Attributes
-
-Each `Location` object has the following attributes:
+The `parse` method returns a list of `Document` objects, where each `Document` contains a list of `Toponym` objects. Each `Toponym` that is successfully geocoded will have a corresponding `Location` object with the following attributes:
 
 - `geonameid`: The unique identifier for the place in the GeoNames database.
 - `name`: The name of the geographical location.
 - `admin2_geonameid`: The GeoNames identifier for the second-level administrative division.
 - `admin2_name`: The name of the second-level administrative division.
 - `admin1_geonameid`: The GeoNames identifier for the first-level administrative division.
 - `admin1_name`: The name of the first-level administrative division.
@@ -97,18 +102,23 @@
 - `latitude`: The latitude of the location.
 - `longitude`: The longitude of the location.
 - `elevation`: The elevation of the location in meters.
 - `population`: The population of the location.
 
 ## Example
 
-Here's an example showing how the library might be used:
+Here's an example illustrating how the library might be used:
 
 ```python
+from geoparser import Geoparser
+
+geo = Geoparser()
+
 text = "Zurich is a city rich in history."
+
 docs = geo.parse([text])
 
 for doc in docs:
     for toponym in doc.toponyms:
         if toponym.location:
             print(toponym, "->", toponym.location)
 ```
```

### Comparing `geoparser-0.1.4/geoparser/entities.py` & `geoparser-0.1.5/geoparser/entities.py`

 * *Files identical despite different names*

### Comparing `geoparser-0.1.4/geoparser.egg-info/PKG-INFO` & `geoparser-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,111 @@
 Metadata-Version: 2.1
 Name: geoparser
-Version: 0.1.4
+Version: 0.1.5
 Summary: A geoparsing library for English texts
 Author: Diego Gomes
 Author-email: diego.gomes@uzh.ch
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Geoparser
 
-Geoparser is a Python library for geoparsing English texts. It leverages spaCy for toponym recognition and tine-tuned SentenceTransformer models for toponym resolution.
+Geoparser is a Python library for geoparsing English texts. It leverages spaCy for toponym recognition and fine-tuned SentenceTransformer models for toponym resolution.
 
 ## Installation
 
 Install Geoparser using pip:
 
 ```bash
 pip install geoparser
 ```
 
+## Dependencies
+
+Geoparser depends on the following Python libraries:
+
+- **[appdirs](https://github.com/ActiveState/appdirs)**
+- **[numpy](https://numpy.org/)**
+- **[pandas](https://pandas.pydata.org/)**
+- **[requests](https://requests.readthedocs.io/en/latest/)**
+- **[sentence_transformers](https://www.sbert.net/)**
+- **[spacy](https://spacy.io/)**
+- **[torch](https://pytorch.org/)**
+- **[tqdm](https://tqdm.github.io/)**
+
+These dependencies are automatically installed when building Geoparser with pip.
+
 ## Download Required Data
 
-After installation, you need to download the necessary data files for Geoparser to function properly:
+After installation, you need to execute the following command to download the necessary files for Geoparser to function:
 
 ```bash
 python -m geoparser download
 ```
 
-This command will download the following resources:
+This command will download the following resources and setup a SQLite database for the GeoNames data:
 
 - **spaCy Models**: Two models are downloaded:
   - `en_core_web_sm`: A less accurate but faster model.
   - `en_core_web_trf`: A more accurate but slower model.
 - **GeoNames Data**: The following files are downloaded from GeoNames:
   - [All Countries](http://download.geonames.org/export/dump/allCountries.zip)
+  - [Alternate Names](https://download.geonames.org/export/dump/alternateNames.zip)
   - [Admin1 Codes](http://download.geonames.org/export/dump/admin1CodesASCII.txt)
   - [Admin2 Codes](http://download.geonames.org/export/dump/admin2Codes.txt)
   - [Country Info](http://download.geonames.org/export/dump/countryInfo.txt)
   - [Feature Codes](http://download.geonames.org/export/dump/featureCodes_en.txt)
 
-These files are stored in the user-specific data directory:
+These files are temporarily stored in your system's user-specific data directory during the database setup. Once the database has been populated with the data, the original files are automatically deleted to free up space. The database is then stored in this location:
 
-- **Windows**: `C:\Users\<Username>\AppData\Local\geoparser\`
-- **macOS**: `~/Library/Application Support/geoparser/`
-- **Linux**: `~/.local/share/geoparser/`
+- **Windows**: `C:\Users\<Username>\AppData\Local\geoparser\geonames.db`
+- **macOS**: `~/Library/Application Support/geoparser/geonames.db`
+- **Linux**: `~/.local/share/geoparser/geonames.db`
 
-Please ensure you have adequate disk space available, as the total size of these files is approximately 2.3 GB.
+Please ensure you have enough disk space available. The final size of the downloaded GeoNames data will be approximately 3.2 GB, increasing temporarily to 5.5 GB during the download and setup process.
 
 ## Usage
 
 ### Instantiating the Geoparser
 
-To use Geoparser, you need to instantiate an object of the `Geoparser` class. You can specify which spaCy and transformer model to use, optimizing either for accuracy or speed. By default, the library uses accuracy-optimized models:
+To use Geoparser, you need to instantiate an object of the `Geoparser` class. You can specify which spaCy and transformer model to use, optimising either for accuracy or speed. By default, the library uses accuracy-optimised models:
 
 ```python
 from geoparser import Geoparser
 
 geo = Geoparser()
 ```
 
+Default configuration:
+
+```python
+geo = Geoparser(spacy_model='en_core_web_trf', transformer_model='dguzh/geo-all-distilroberta-v1')
+```
+
 For faster performance, you can opt for the smaller models:
 
 ```python
 geo = Geoparser(spacy_model='en_core_web_sm', transformer_model='dguzh/geo-all-MiniLM-L6-v2')
 ```
 
-You can mix and match these models depending on your specific needs. Note that the transformer models `dguzh/geo-all-distilroberta-v1` and `dguzh/geo-all-MiniLM-L6-v2` are preliminary versions. Future updates aim to refine these models to improve the accuracy of toponym disambiguation.
+You can mix and match these models depending on your specific needs. Note that the SentenceTransformer models `dguzh/geo-all-distilroberta-v1` and `dguzh/geo-all-MiniLM-L6-v2` are preliminary versions. Future updates aim to refine these models to improve the accuracy of toponym disambiguation.
 
 ### Parsing Texts
 
-Geoparser is optimized for parsing large collections of texts at once. Pass a list of strings to the `parse` method:
+Geoparser is optimised for parsing large collections of texts at once. Pass a list of strings to the `parse` method:
 
 ```python
 docs = geo.parse(["Sample text 1", "Sample text 2", "Sample text 3"])
 ```
 
-The `parse` method returns a list of `Document` objects, where each `Document` contains a list of `Toponym` objects. Each `Toponym` that is successfully geocoded will have a corresponding `Location` object with detailed geographical data:
-
-### Location Attributes
-
-Each `Location` object has the following attributes:
+The `parse` method returns a list of `Document` objects, where each `Document` contains a list of `Toponym` objects. Each `Toponym` that is successfully geocoded will have a corresponding `Location` object with the following attributes:
 
 - `geonameid`: The unique identifier for the place in the GeoNames database.
 - `name`: The name of the geographical location.
 - `admin2_geonameid`: The GeoNames identifier for the second-level administrative division.
 - `admin2_name`: The name of the second-level administrative division.
 - `admin1_geonameid`: The GeoNames identifier for the first-level administrative division.
 - `admin1_name`: The name of the first-level administrative division.
@@ -97,18 +115,23 @@
 - `latitude`: The latitude of the location.
 - `longitude`: The longitude of the location.
 - `elevation`: The elevation of the location in meters.
 - `population`: The population of the location.
 
 ## Example
 
-Here's an example showing how the library might be used:
+Here's an example illustrating how the library might be used:
 
 ```python
+from geoparser import Geoparser
+
+geo = Geoparser()
+
 text = "Zurich is a city rich in history."
+
 docs = geo.parse([text])
 
 for doc in docs:
     for toponym in doc.toponyms:
         if toponym.location:
             print(toponym, "->", toponym.location)
 ```
```

### Comparing `geoparser-0.1.4/setup.py` & `geoparser-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='geoparser',
-    version='0.1.4',
+    version='0.1.5',
     author='Diego Gomes',
     author_email='diego.gomes@uzh.ch',
     packages=find_packages(),
     description='A geoparsing library for English texts',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

