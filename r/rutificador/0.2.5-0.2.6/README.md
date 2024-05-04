# Comparing `tmp/rutificador-0.2.5.tar.gz` & `tmp/rutificador-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.2.5.tar", max compression
+gzip compressed data, was "rutificador-0.2.6.tar", max compression
```

## Comparing `rutificador-0.2.5.tar` & `rutificador-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-04 17:16:37.739913 rutificador-0.2.5/LICENSE
--rw-r--r--   0        0        0     4357 2024-05-04 17:16:37.739913 rutificador-0.2.5/README.md
--rw-r--r--   0        0        0     1100 2024-05-04 17:16:37.739913 rutificador-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      101 2024-05-04 17:16:37.739913 rutificador-0.2.5/rutificador/__init__.py
--rw-r--r--   0        0        0     9142 2024-05-04 17:16:37.739913 rutificador-0.2.5/rutificador/main.py
--rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 rutificador-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-04 18:23:21.877266 rutificador-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4452 2024-05-04 18:23:21.877266 rutificador-0.2.6/README.md
+-rw-r--r--   0        0        0     1100 2024-05-04 18:23:21.877266 rutificador-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      101 2024-05-04 18:23:21.877266 rutificador-0.2.6/rutificador/__init__.py
+-rw-r--r--   0        0        0     9142 2024-05-04 18:23:21.877266 rutificador-0.2.6/rutificador/main.py
+-rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 rutificador-0.2.6/PKG-INFO
```

### Comparing `rutificador-0.2.5/LICENSE` & `rutificador-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.5/README.md` & `rutificador-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -113,17 +113,21 @@
     <rut>12345678-5</rut>
     <rut>9876543-3</rut>
     <rut>1234567-4</rut>
     <rut>18005183-k</rut>
 </root>
 ```
 
+## Problemas o Requerimientos
+
+¿Te gustaría reportar algún error, solicitar alguna modificación o característica adicional en esta librería? Solo debes abrir un 'issue' y describir tu petición de la forma más precisa y clara posible.
+
 ## Contribuciones
 
-Las contribuciones son bienvenidas. Para colaborar puedes abrir un issue o si lo deseas puedes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
+Las contribuciones son bienvenidas. Solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, y finalmente el push y el pull request para migrar los cambios al 'master'.
 
 ## Licencia
 
 Este proyecto está licenciado bajo la Licencia MIT.
 
 ## Créditos
```

### Comparing `rutificador-0.2.5/pyproject.toml` & `rutificador-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.2.5"
+version = "0.2.6"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://pypi.org/project/rutificador/"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.2.5/rutificador/main.py` & `rutificador-0.2.6/rutificador/main.py`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.5/PKG-INFO` & `rutificador-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.2.5
+Version: 0.2.6
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://pypi.org/project/rutificador/
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -135,17 +135,21 @@
     <rut>12345678-5</rut>
     <rut>9876543-3</rut>
     <rut>1234567-4</rut>
     <rut>18005183-k</rut>
 </root>
 ```
 
+## Problemas o Requerimientos
+
+¿Te gustaría reportar algún error, solicitar alguna modificación o característica adicional en esta librería? Solo debes abrir un 'issue' y describir tu petición de la forma más precisa y clara posible.
+
 ## Contribuciones
 
-Las contribuciones son bienvenidas. Para colaborar puedes abrir un issue o si lo deseas puedes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
+Las contribuciones son bienvenidas. Solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, y finalmente el push y el pull request para migrar los cambios al 'master'.
 
 ## Licencia
 
 Este proyecto está licenciado bajo la Licencia MIT.
 
 ## Créditos
```

