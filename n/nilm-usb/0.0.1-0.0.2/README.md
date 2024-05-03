# Comparing `tmp/nilm_usb-0.0.1.tar.gz` & `tmp/nilm_usb-0.0.2.tar.gz`

## Comparing `nilm_usb-0.0.1.tar` & `nilm_usb-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 nilm_usb-0.0.1/src/nilm_usb/NILM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nilm_usb-0.0.1/src/nilm_usb/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nilm_usb-0.0.1/LICENSE
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 nilm_usb-0.0.1/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nilm_usb-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 nilm_usb-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 nilm_usb-0.0.2/src/nilm_usb/NILM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nilm_usb-0.0.2/src/nilm_usb/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nilm_usb-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 nilm_usb-0.0.2/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 nilm_usb-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 nilm_usb-0.0.2/PKG-INFO
```

### Comparing `nilm_usb-0.0.1/src/nilm_usb/NILM.py` & `nilm_usb-0.0.2/src/nilm_usb/NILM.py`

 * *Files identical despite different names*

### Comparing `nilm_usb-0.0.1/LICENSE` & `nilm_usb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nilm_usb-0.0.1/README.md` & `nilm_usb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nilm_usb-0.0.1/pyproject.toml` & `nilm_usb-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "nilm_usb"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="UFOTECH", email="gerencia@ufotech.co" },
   { name="Silvia Moreno", email="silvia.moreno@unisimon.edu.co" },
 ]
 description = "A NILM images classifier"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "keras==3.2.0",
-    "opencv-python>4.9",
-    "scikit-learn>1.4",
-    "scipy>1.13",
-    "tensorflow>2.16",
+    "opencv-python>=4.9",
+    "scikit-learn>=1.4",
+    "scipy>=1.13",
+    "tensorflow>=2.16",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `nilm_usb-0.0.1/PKG-INFO` & `nilm_usb-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: nilm_usb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A NILM images classifier
 Project-URL: Homepage, https://github.com/ufotechco/nilm_usb
 Author-email: UFOTECH <gerencia@ufotech.co>, Silvia Moreno <silvia.moreno@unisimon.edu.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: keras==3.2.0
-Requires-Dist: opencv-python>4.9
-Requires-Dist: scikit-learn>1.4
-Requires-Dist: scipy>1.13
-Requires-Dist: tensorflow>2.16
+Requires-Dist: opencv-python>=4.9
+Requires-Dist: scikit-learn>=1.4
+Requires-Dist: scipy>=1.13
+Requires-Dist: tensorflow>=2.16
 Description-Content-Type: text/markdown
 
 # NILM: Clasificador de Imágenes Utilizando Redes Neuronales Convolucionales
 
 Este proyecto consiste en una clase de Python llamada NILM (Neural Network Image Classifier) diseñada para realizar predicciones sobre imágenes utilizando un modelo de red neuronal convolucional pre-entrenado. El propósito principal de esta clase es predecir y clasificar imágenes en una de las cuatro clases distintas.
 
 ## Uso
```

