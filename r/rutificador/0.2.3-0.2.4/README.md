# Comparing `tmp/rutificador-0.2.3.tar.gz` & `tmp/rutificador-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rutificador-0.2.3.tar", max compression
+gzip compressed data, was "rutificador-0.2.4.tar", max compression
```

## Comparing `rutificador-0.2.3.tar` & `rutificador-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1112 2024-05-03 20:14:43.644288 rutificador-0.2.3/LICENSE
--rw-r--r--   0        0        0     4332 2024-05-03 20:14:43.644288 rutificador-0.2.3/README.md
--rw-r--r--   0        0        0     1100 2024-05-03 20:14:43.644288 rutificador-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      100 2024-05-03 20:14:43.644288 rutificador-0.2.3/rutificador/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-03 20:14:43.644288 rutificador-0.2.3/rutificador/main.py
--rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 rutificador-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-03 23:06:56.408919 rutificador-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4357 2024-05-03 23:06:56.408919 rutificador-0.2.4/README.md
+-rw-r--r--   0        0        0     1100 2024-05-03 23:06:56.408919 rutificador-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      101 2024-05-03 23:06:56.412919 rutificador-0.2.4/rutificador/__init__.py
+-rw-r--r--   0        0        0     9142 2024-05-03 23:06:56.412919 rutificador-0.2.4/rutificador/main.py
+-rw-r--r--   0        0        0     5297 1970-01-01 00:00:00.000000 rutificador-0.2.4/PKG-INFO
```

### Comparing `rutificador-0.2.3/LICENSE` & `rutificador-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rutificador-0.2.3/README.md` & `rutificador-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,18 +74,18 @@
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
 ruts_validos = Rut.validar_lista_ruts(ruts)
 print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
 # Salida:
-# RUTs válidos:
-# 12.345.678-5
-# 12.345.670-K
-# 98.765.432-1
+RUTs válidos:
+12.345.678-5
+12.345.670-K
+98.765.432-1
 
 # En formato csv
 ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
 csv_ruts = Rut.formatear_lista_ruts(ruts, formato='csv')
 print(csv_ruts)
 # Salida
 RUTs válidos:
@@ -115,15 +115,15 @@
     <rut>1234567-4</rut>
     <rut>18005183-k</rut>
 </root>
 ```
 
 ## Contribuciones
 
-Las contribuciones son bienvenidas. Para colaborar solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
+Las contribuciones son bienvenidas. Para colaborar puedes abrir un issue o si lo deseas puedes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
 
 ## Licencia
 
 Este proyecto está licenciado bajo la Licencia MIT.
 
 ## Créditos
```

### Comparing `rutificador-0.2.3/pyproject.toml` & `rutificador-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rutificador"
-version = "0.2.3"
+version = "0.2.4"
 description = "Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile."
 authors = ["Carlos Ortega González <carlosortega77@gmail.com>"]
 license = "MIT"
 homepage = "https://pypi.org/project/rutificador/"
 repository = "https://github.com/cortega26/Rutificador"
 keywords = ["RUT", "Chile", "validación", "formateo"]
 classifiers = [
```

### Comparing `rutificador-0.2.3/rutificador/main.py` & `rutificador-0.2.4/rutificador/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 import re
 
 FACTORES_DIGITO_VERIFICADOR: list[int] = [2, 3, 4, 5, 6, 7]
 MODULO_DIGITO_VERIFICADOR: int = 11
 RUT_REGEX: str = r"^(\d{1,8}(?:.\d{3})*)(-([0-9kK]))?$"
 
+
 class RutInvalidoError(Exception):
     """Lanzada cuando el RUT ingresado es inválido."""
 
+
 class RutBase:
     """Representa el número base de un RUT chileno."""
 
     def __init__(self, base: str):
         """
         Inicializa la instancia de RutBase.
 
@@ -45,14 +47,15 @@
             )
 
         return base_normalizada
 
     def __str__(self) -> str:
         return self.base
 
+
 class RutDigitoVerificador(RutBase):
     """Calcula y representa el dígito verificador de un RUT chileno."""
 
     def __init__(self, base: str):
         """
         Inicializa la instancia de RutDigitoVerificador.
 
@@ -77,14 +80,15 @@
             MODULO_DIGITO_VERIFICADOR - suma_parcial % MODULO_DIGITO_VERIFICADOR
         ) % MODULO_DIGITO_VERIFICADOR
         return str(digito_verificador) if digito_verificador < 10 else "k"
 
     def __str__(self) -> str:
         return self.digito_verificador
 
+
 class Rut:
     """
     Representa un RUT chileno.
 
     Atributos:
         rut_string (str): El RUT en formato string.
         base (RutBase): El número base del RUT.
@@ -92,15 +96,15 @@
 
     Métodos:
         formatear: Formatea el RUT según las opciones especificadas.
         validar_lista_ruts: Valida una lista de RUTs.
         formatear_lista_ruts: Formatea una lista de RUTs según las opciones especificadas.
     """
 
-    PATRON_RUT: re.Pattern = re.compile(RUT_REGEX)
+    PATRON_RUT = re.compile(RUT_REGEX)
 
     def __init__(self, rut: str):
         """
         Inicializa la instancia de Rut.
 
         Args:
             rut (str): El RUT en formato string.
@@ -124,17 +128,22 @@
 
     def _validar_digito_verificador(self) -> None:
         """
         Valida el dígito verificador del RUT.
         """
         match = Rut.PATRON_RUT.fullmatch(self.rut_string)
         digito_verificador_input = match.group(3).lower() if match.group(3) else None
-        digito_verificador_calculado = RutDigitoVerificador(self.base_string).digito_verificador
-
-        if digito_verificador_input and digito_verificador_input != digito_verificador_calculado:
+        digito_verificador_calculado = RutDigitoVerificador(
+            self.base_string
+        ).digito_verificador
+
+        if (
+            digito_verificador_input
+            and digito_verificador_input != digito_verificador_calculado
+        ):
             raise RutInvalidoError(
                 f"El dígito verificador '{digito_verificador_input}' no coincide con "
                 f"el dígito verificador calculado '{digito_verificador_calculado}'."
             )
 
     def __str__(self) -> str:
         return f"{self.base}-{self.digito_verificador}"
@@ -192,24 +201,24 @@
         invalidos: list[tuple[str, str]] = []
         for rut in ruts:
             try:
                 rut_valido: str = str(Rut(rut))
                 validos.append(rut_valido)
             except RutInvalidoError as e:
                 invalidos.append((rut, str(e)))
-        return {'validos': validos, 'invalidos': invalidos}
+        return {"validos": validos, "invalidos": invalidos}
 
     @staticmethod
     def _formatear_csv(ruts_formateados: list[str]) -> str:
         cadena_ruts: str = "\n".join(ruts_formateados)
         return f"rut\n{cadena_ruts}"
 
     @staticmethod
     def _formatear_xml(ruts_formateados: list[str]) -> str:
-        xml_lines:list[str] = ["<root>"]
+        xml_lines: list[str] = ["<root>"]
         for rut in ruts_formateados:
             xml_lines.append(f"    <rut>{rut}</rut>")
         xml_lines.append("</root>")
         return "\n".join(xml_lines)
 
     @staticmethod
     def _formatear_json(ruts_formateados: list[str]) -> str:
@@ -217,15 +226,15 @@
         return str(ruts_json)
 
     @staticmethod
     def formatear_lista_ruts(
         ruts: list[str],
         separador_miles: bool = False,
         mayusculas: bool = False,
-        formato = None,
+        formato=None,
     ) -> str:
         """
         Formatea una lista de RUTs según las opciones especificadas.
 
         Args:
             ruts (list[str]): Una lista de RUTs en formato string o numérico.
             separador_miles (bool, optional): Si se deben agregar separadores de miles (puntos).
@@ -238,28 +247,29 @@
         """
         formato_salida: dict[str, callable] = {
             "csv": Rut._formatear_csv,
             "xml": Rut._formatear_xml,
             "json": Rut._formatear_json,
         }
         ruts_validos_invalidos: dict[str, list[str]] = Rut.validar_lista_ruts(ruts)
-        ruts_validos: list[str] = ruts_validos_invalidos['validos']
-        ruts_invalidos: list[tuple[str, str]] = ruts_validos_invalidos['invalidos']
+        ruts_validos: list[str] = ruts_validos_invalidos["validos"]
+        ruts_invalidos: list[tuple[str, str]] = ruts_validos_invalidos["invalidos"]
 
-        resultado: str = ''
+        resultado: str = ""
         if ruts_validos:
-            ruts_validos_formateados: list[str] = [Rut(rut).formatear(separador_miles, mayusculas)
-                                                   for rut in ruts_validos]
-            resultado += 'RUTs válidos:\n'
-            if formato in ('csv', 'xml', 'json'):
+            ruts_validos_formateados: list[str] = [
+                Rut(rut).formatear(separador_miles, mayusculas) for rut in ruts_validos
+            ]
+            resultado += "RUTs válidos:\n"
+            if formato in ("csv", "xml", "json"):
                 resultado += formato_salida[formato](ruts_validos_formateados)
             else:
-                #resultado += '\n'.join(ruts_validos_formateados)
-                resultado += '\n'.join(ruts_validos_formateados)
-            resultado += '\n\n'
+                # resultado += '\n'.join(ruts_validos_formateados)
+                resultado += "\n".join(ruts_validos_formateados)
+            resultado += "\n\n"
 
         if ruts_invalidos:
-            resultado += 'RUTs inválidos:\n'
+            resultado += "RUTs inválidos:\n"
             for rut, error in ruts_invalidos:
-                resultado += f'{rut} - {error}\n'
+                resultado += f"{rut} - {error}\n"
 
         return resultado
```

### Comparing `rutificador-0.2.3/PKG-INFO` & `rutificador-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rutificador
-Version: 0.2.3
+Version: 0.2.4
 Summary: Esta librería proporciona una implementación en Python para validar y formatear el Rol Único Tributario (RUT) utilizado en Chile.
 Home-page: https://pypi.org/project/rutificador/
 License: MIT
 Keywords: RUT,Chile,validación,formateo
 Author: Carlos Ortega González
 Author-email: carlosortega77@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -96,18 +96,18 @@
 
 ```python
 # Sin formato
 ruts = ['12345678-5', '12345670-k', '98765432-1']
 ruts_validos = Rut.validar_lista_ruts(ruts)
 print(Rut.formatear_lista_ruts(ruts_validos, separador_miles=True, mayusculas=True))
 # Salida:
-# RUTs válidos:
-# 12.345.678-5
-# 12.345.670-K
-# 98.765.432-1
+RUTs válidos:
+12.345.678-5
+12.345.670-K
+98.765.432-1
 
 # En formato csv
 ruts = ['12.345.678', '9876543', '1.234.567-4', '18005183']
 csv_ruts = Rut.formatear_lista_ruts(ruts, formato='csv')
 print(csv_ruts)
 # Salida
 RUTs válidos:
@@ -137,15 +137,15 @@
     <rut>1234567-4</rut>
     <rut>18005183-k</rut>
 </root>
 ```
 
 ## Contribuciones
 
-Las contribuciones son bienvenidas. Para colaborar solo debes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
+Las contribuciones son bienvenidas. Para colaborar puedes abrir un issue o si lo deseas puedes hacer un fork del repositorio, crear una rama nueva, hacer los cambios que consideres pertinentes con su respectiva documentación, hacer el commit, el push y el pull request para migrar los cambios al 'master'. Finalmente, asegúrate de describir los cambios que realizaste y por qué crees son necesarios.
 
 ## Licencia
 
 Este proyecto está licenciado bajo la Licencia MIT.
 
 ## Créditos
```

