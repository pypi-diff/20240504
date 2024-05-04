# Comparing `tmp/sumapi-0.3.8.tar.gz` & `tmp/sumapi-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sumapi-0.3.8.tar", last modified: Tue Jan 18 19:33:09 2022, max compression
+gzip compressed data, was "sumapi-0.3.9.tar", last modified: Sat May  4 21:36:18 2024, max compression
```

## Comparing `sumapi-0.3.8.tar` & `sumapi-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-01-18 19:33:09.954742 sumapi-0.3.8/
--rw-rw-rw-   0        0        0     1085 2020-11-20 12:44:36.000000 sumapi-0.3.8/LICENSE
--rw-rw-rw-   0        0        0    12597 2022-01-18 19:33:09.954742 sumapi-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    12117 2022-01-18 18:21:31.000000 sumapi-0.3.8/README.md
--rw-rw-rw-   0        0        0       86 2022-01-18 19:33:09.959961 sumapi-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      728 2022-01-18 19:32:31.000000 sumapi-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-18 19:33:09.933009 sumapi-0.3.8/sumapi/
--rw-rw-rw-   0        0        0        0 2020-11-24 16:52:24.000000 sumapi-0.3.8/sumapi/__init__.py
--rw-rw-rw-   0        0        0    38680 2022-01-18 18:21:46.000000 sumapi-0.3.8/sumapi/api.py
--rw-rw-rw-   0        0        0      560 2021-08-25 11:01:32.000000 sumapi-0.3.8/sumapi/config.py
-drwxrwxrwx   0        0        0        0 2022-01-18 19:33:09.953742 sumapi-0.3.8/sumapi.egg-info/
--rw-rw-rw-   0        0        0    12597 2022-01-18 19:33:09.000000 sumapi-0.3.8/sumapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2022-01-18 19:33:09.000000 sumapi-0.3.8/sumapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-18 19:33:09.000000 sumapi-0.3.8/sumapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-01-18 19:33:09.000000 sumapi-0.3.8/sumapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-01-18 19:33:09.000000 sumapi-0.3.8/sumapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 21:36:18.282915 sumapi-0.3.9/
+-rw-rw-rw-   0        0        0      153 2024-05-04 21:30:30.000000 sumapi-0.3.9/.gitignore
+-rw-rw-rw-   0        0        0     1085 2024-05-04 21:30:30.000000 sumapi-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0    12843 2024-05-04 21:36:18.283915 sumapi-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12363 2024-05-04 21:35:20.000000 sumapi-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 21:36:18.253680 sumapi-0.3.9/docs/
+-rw-rw-rw-   0        0        0    22215 2024-05-04 21:30:30.000000 sumapi-0.3.9/docs/sumapi_logo.png
+-rw-rw-rw-   0        0        0       32 2024-05-04 21:30:30.000000 sumapi-0.3.9/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-05-04 21:36:18.284916 sumapi-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-05-04 21:36:13.000000 sumapi-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:36:18.256680 sumapi-0.3.9/sumapi/
+drwxrwxrwx   0        0        0        0 2024-05-04 21:36:18.278864 sumapi-0.3.9/sumapi/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    38187 2024-05-04 21:30:30.000000 sumapi-0.3.9/sumapi/.ipynb_checkpoints/api-checkpoint.py
+-rw-rw-rw-   0        0        0      560 2024-05-04 21:30:30.000000 sumapi-0.3.9/sumapi/.ipynb_checkpoints/config-checkpoint.py
+-rw-rw-rw-   0        0        0        0 2024-05-04 21:30:30.000000 sumapi-0.3.9/sumapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:36:18.281914 sumapi-0.3.9/sumapi/__pycache__/
+-rw-rw-rw-   0        0        0    19762 2024-05-04 21:30:30.000000 sumapi-0.3.9/sumapi/__pycache__/api.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1518 2024-05-04 21:30:30.000000 sumapi-0.3.9/sumapi/__pycache__/auth.cpython-37.pyc
+-rw-rw-rw-   0        0        0      530 2024-05-04 21:30:30.000000 sumapi-0.3.9/sumapi/__pycache__/config.cpython-37.pyc
+-rw-rw-rw-   0        0        0    40464 2024-05-04 21:33:25.000000 sumapi-0.3.9/sumapi/api.py
+-rw-rw-rw-   0        0        0      641 2024-05-04 21:35:28.000000 sumapi-0.3.9/sumapi/config.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:36:18.276863 sumapi-0.3.9/sumapi.egg-info/
+-rw-rw-rw-   0        0        0    12843 2024-05-04 21:36:17.000000 sumapi-0.3.9/sumapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-04 21:36:18.000000 sumapi-0.3.9/sumapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 21:36:17.000000 sumapi-0.3.9/sumapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-04 21:36:17.000000 sumapi-0.3.9/sumapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 21:36:17.000000 sumapi-0.3.9/sumapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 21:36:18.281914 sumapi-0.3.9/tests/
+-rw-rw-rw-   0        0        0     5147 2024-05-04 21:30:30.000000 sumapi-0.3.9/tests/unit_test.py
```

### Comparing `sumapi-0.3.8/LICENSE` & `sumapi-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sumapi-0.3.8/PKG-INFO` & `sumapi-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumapi
-Version: 0.3.8
+Version: 0.3.9
 Summary: API Library for SumAPI with Python
 Home-page: https://github.com/summarify/sumapi
 Author: Summarify
 Author-email: info@summarify.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -204,14 +204,24 @@
 
 context = """ABASIYANIK, Sait Faik. Hikayeci (Adapazarı 23 Kasım 1906-İstanbul 11 Mayıs 1954). İlk öğrenimine Adapazarı’nda Rehber-i Terakki Mektebi’nde başladı. İki yıl kadar Adapazarı İdadisi’nde okudu. İstanbul Erkek Lisesi’nde devam ettiği orta öğrenimini Bursa Lisesi’nde tamamladı (1928). İstanbul Edebiyat Fakültesi’ne iki yıl devam ettikten sonra babasının isteği üzerine iktisat öğrenimi için İsviçre’ye gitti. Kısa süre sonra iktisat öğrenimini bırakarak Lozan’dan Grenoble’a geçti. Üç yıl başıboş bir edebiyat öğrenimi gördükten sonra babası tarafından geri çağrıldı (1933). Bir müddet Halıcıoğlu Ermeni Yetim Mektebi'nde Türkçe grup dersleri öğretmenliği yaptı. Ticarete atıldıysa da tutunamadı. Bir ay Haber gazetesinde adliye muhabirliği yaptı (1942). Babasının ölümü üzerine aileden kalan emlakin geliri ile avare bir hayata başladı. Evlenemedi. Yazları Burgaz adasındaki köşklerinde, kışları Şişli’deki apartmanlarında annesi ile beraber geçen bu fazla içkili bohem hayatı ömrünün sonuna kadar sürdü."""
 
 api.question_answering(context=context, question="Sait Faik nerede doğdu?")
 # {'body': 'Sait Faik nerede doğdu?', 'evaluation': {'score': 0.9611985087394714, 'answer': 'Adapazarı'}}
 ```
 
+**Next Character Prediction**
+
+```python
+from sumapi.api import SumAPI
+
+api = SumAPI(username='<your_username>', password='<your_password')
+
+api.next_character_prediction('Mustafa Kemal Atatürk', domain='general', max_length=100)
+```
+
 **Multi Argument**
 
 ```python
 from sumapi.api import SumAPI
 import pandas as pd
 
 api = SumAPI(username='<your_username>', password='<your_password')
```

### Comparing `sumapi-0.3.8/README.md` & `sumapi-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,24 @@
 
 context = """ABASIYANIK, Sait Faik. Hikayeci (Adapazarı 23 Kasım 1906-İstanbul 11 Mayıs 1954). İlk öğrenimine Adapazarı’nda Rehber-i Terakki Mektebi’nde başladı. İki yıl kadar Adapazarı İdadisi’nde okudu. İstanbul Erkek Lisesi’nde devam ettiği orta öğrenimini Bursa Lisesi’nde tamamladı (1928). İstanbul Edebiyat Fakültesi’ne iki yıl devam ettikten sonra babasının isteği üzerine iktisat öğrenimi için İsviçre’ye gitti. Kısa süre sonra iktisat öğrenimini bırakarak Lozan’dan Grenoble’a geçti. Üç yıl başıboş bir edebiyat öğrenimi gördükten sonra babası tarafından geri çağrıldı (1933). Bir müddet Halıcıoğlu Ermeni Yetim Mektebi'nde Türkçe grup dersleri öğretmenliği yaptı. Ticarete atıldıysa da tutunamadı. Bir ay Haber gazetesinde adliye muhabirliği yaptı (1942). Babasının ölümü üzerine aileden kalan emlakin geliri ile avare bir hayata başladı. Evlenemedi. Yazları Burgaz adasındaki köşklerinde, kışları Şişli’deki apartmanlarında annesi ile beraber geçen bu fazla içkili bohem hayatı ömrünün sonuna kadar sürdü."""
 
 api.question_answering(context=context, question="Sait Faik nerede doğdu?")
 # {'body': 'Sait Faik nerede doğdu?', 'evaluation': {'score': 0.9611985087394714, 'answer': 'Adapazarı'}}
 ```
 
+**Next Character Prediction**
+
+```python
+from sumapi.api import SumAPI
+
+api = SumAPI(username='<your_username>', password='<your_password')
+
+api.next_character_prediction('Mustafa Kemal Atatürk', domain='general', max_length=100)
+```
+
 **Multi Argument**
 
 ```python
 from sumapi.api import SumAPI
 import pandas as pd
 
 api = SumAPI(username='<your_username>', password='<your_password')
```

### Comparing `sumapi-0.3.8/setup.py` & `sumapi-0.3.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sumapi",
-    version="0.3.8",
+    version="0.3.9",
     author="Summarify",
     author_email="info@summarify.io",
     description="API Library for SumAPI with Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/summarify/sumapi",
     packages=setuptools.find_packages(),
```

### Comparing `sumapi-0.3.8/sumapi/api.py` & `sumapi-0.3.9/sumapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                     'accept': 'application/json',
                     'Authorization': f"Bearer {self._get_token()['access_token']}",
                     'Content-Type': 'application/json'}
                 return True
         else:
             return False
 
-    def prepare_data(self, body=None, domain=None, categories=None, context=None, question=None, percentage=None, word_count=None):
+    def prepare_data(self, body=None, domain=None, categories=None, context=None, question=None, percentage=None, word_count=None, max_length=None):
         """
             Function to create json for queries.
         """
         if percentage != None or word_count != None:
             data = {
                 'body': body,
                 'percentage': percentage,
@@ -106,14 +106,20 @@
                 'question': question
             }
         elif domain != None:
             data = {
                 'body': body,
                 'domain': domain
             }
+        elif max_length != None:
+            data = {
+                'body': body,
+                'domain': domain,
+                'max_length': max_length
+            }
 
         return data
 
     def sentiment_analysis(self, text, domain='general'):
         """
             It makes sentiment analysis prediction for the sentences / samples you send.
 
@@ -498,14 +504,56 @@
                 return response_json
         except JSONDecodeError:
             return response.content
         except ConnectionError:
             raise ConnectionError("Error with Connection, Check your Internet Connection or visit api.summarify.io/status for SumAPI Status")
         return response_json
 
+    def next_character_prediction(self, text, domain='sumgpt-small', max_length=100):
+        """
+            It makes next character prediction for your text.
+
+            Parameters
+            ----------
+            text : str
+                Your sample text.
+            domain: str
+                Model Domain ['sumgpt-small']
+            max_length: int
+                Parameter specifies the maximum number of tokens the text generator will produce, limiting the length of the generated text.
+
+            Returns
+            -------
+            dict:
+                body: str
+                    Your sample text.
+                evaluation: dict
+                    evaluation: str
+                        Predicted text
+
+            Examples
+            --------
+            from sumapi.api import SumAPI
+
+            api = SumAPI(username='<your_username>', password='<your_password>')
+
+            api.next_character_prediction('Mustafa Kemal Atatürk', domain='general', max_length=100)
+        """
+        data = self.prepare_data(body=text, domain=domain, max_length=max_length)
+
+        try:
+            response = requests.post(URL['nextCharacterPredictionURL'], headers=self.headers, json=data)
+            response_json = response.json()
+            
+        except JSONDecodeError:
+            return response.content
+        except ConnectionError:
+            raise ConnectionError("Error with Connection, Check your Internet Connection or visit api.summarify.io/status for SumAPI Status")
+        return response_json
+
     def multi_request(self, data, packet_size=250):
         """
             It allows you to make multiple queries to different products at the same time. We recommend this for large datasets.
 
             Parameters
             ----------
             data : pandas.dataframe
```

### Comparing `sumapi-0.3.8/sumapi/config.py` & `sumapi-0.3.9/sumapi/.ipynb_checkpoints/config-checkpoint.py`

 * *Files identical despite different names*

### Comparing `sumapi-0.3.8/sumapi.egg-info/PKG-INFO` & `sumapi-0.3.9/sumapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumapi
-Version: 0.3.8
+Version: 0.3.9
 Summary: API Library for SumAPI with Python
 Home-page: https://github.com/summarify/sumapi
 Author: Summarify
 Author-email: info@summarify.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -204,14 +204,24 @@
 
 context = """ABASIYANIK, Sait Faik. Hikayeci (Adapazarı 23 Kasım 1906-İstanbul 11 Mayıs 1954). İlk öğrenimine Adapazarı’nda Rehber-i Terakki Mektebi’nde başladı. İki yıl kadar Adapazarı İdadisi’nde okudu. İstanbul Erkek Lisesi’nde devam ettiği orta öğrenimini Bursa Lisesi’nde tamamladı (1928). İstanbul Edebiyat Fakültesi’ne iki yıl devam ettikten sonra babasının isteği üzerine iktisat öğrenimi için İsviçre’ye gitti. Kısa süre sonra iktisat öğrenimini bırakarak Lozan’dan Grenoble’a geçti. Üç yıl başıboş bir edebiyat öğrenimi gördükten sonra babası tarafından geri çağrıldı (1933). Bir müddet Halıcıoğlu Ermeni Yetim Mektebi'nde Türkçe grup dersleri öğretmenliği yaptı. Ticarete atıldıysa da tutunamadı. Bir ay Haber gazetesinde adliye muhabirliği yaptı (1942). Babasının ölümü üzerine aileden kalan emlakin geliri ile avare bir hayata başladı. Evlenemedi. Yazları Burgaz adasındaki köşklerinde, kışları Şişli’deki apartmanlarında annesi ile beraber geçen bu fazla içkili bohem hayatı ömrünün sonuna kadar sürdü."""
 
 api.question_answering(context=context, question="Sait Faik nerede doğdu?")
 # {'body': 'Sait Faik nerede doğdu?', 'evaluation': {'score': 0.9611985087394714, 'answer': 'Adapazarı'}}
 ```
 
+**Next Character Prediction**
+
+```python
+from sumapi.api import SumAPI
+
+api = SumAPI(username='<your_username>', password='<your_password')
+
+api.next_character_prediction('Mustafa Kemal Atatürk', domain='general', max_length=100)
+```
+
 **Multi Argument**
 
 ```python
 from sumapi.api import SumAPI
 import pandas as pd
 
 api = SumAPI(username='<your_username>', password='<your_password')
```

