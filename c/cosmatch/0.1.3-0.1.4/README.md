# Comparing `tmp/cosmatch-0.1.3.tar.gz` & `tmp/cosmatch-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmatch-0.1.3.tar", max compression
+gzip compressed data, was "cosmatch-0.1.4.tar", max compression
```

## Comparing `cosmatch-0.1.3.tar` & `cosmatch-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,45 @@
--rw-r--r--   0        0        0     6016 2024-03-22 10:51:29.836744 cosmatch-0.1.3/Readme.md
--rw-r--r--   0        0        0      381 2024-03-22 10:51:29.836744 cosmatch-0.1.3/cosmatch/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 10:51:29.866744 cosmatch-0.1.3/cosmatch/classification/__init__.py
--rw-r--r--   0        0        0     1379 2024-03-22 10:51:29.836744 cosmatch-0.1.3/cosmatch/classification/classification.py
--rw-r--r--   0        0        0      187 2024-03-22 10:51:29.836744 cosmatch-0.1.3/cosmatch/fake/__init__.py
--rw-r--r--   0        0        0    12576 2024-03-22 10:51:29.836744 cosmatch-0.1.3/cosmatch/fake/catalog_generator.py
--rw-r--r--   0        0        0      592 2024-03-22 10:51:29.836744 cosmatch-0.1.3/cosmatch/load/__init__.py
--rw-r--r--   0        0        0    11448 2024-03-22 10:51:29.836744 cosmatch-0.1.3/cosmatch/load/data_loader.py
--rw-r--r--   0        0        0       94 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/__init__.py
--rw-r--r--   0        0        0     5550 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/connection.py
--rw-r--r--   0        0        0    53019 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/data_handler.py
--rw-r--r--   0        0        0    11061 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/metrics.py
--rw-r--r--   0        0        0      371 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/models/__init__.py
--rw-r--r--   0        0        0     4087 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/models/base.py
--rw-r--r--   0        0        0      240 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/models/custom/__init__.py
--rw-r--r--   0        0        0     2884 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/models/custom/custom.py
--rw-r--r--   0        0        0     7659 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/models/custom/optimization.py
--rw-r--r--   0        0        0      686 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/models/custom/predict_models.py
--rw-r--r--   0        0        0     3197 2024-03-22 10:51:29.837744 cosmatch-0.1.3/cosmatch/match/models/custom/prob_transformer.py
--rw-r--r--   0        0        0    13400 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/match/models/ml_models.py
--rw-r--r--   0        0        0    12220 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/match/models/nway_models.py
--rw-r--r--   0        0        0    29596 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/match/nway.py
--rw-r--r--   0        0        0     5044 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/match/pipeline.py
--rw-r--r--   0        0        0     1560 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/match/pretrained/hyperparams.pickle
--rw-r--r--   0        0        0       24 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/search/__init__.py
--rw-r--r--   0        0        0    26653 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/search/find_hmxb.py
--rw-r--r--   0        0        0     1182 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/settings.py
--rw-r--r--   0        0        0    32583 2024-03-22 10:51:29.838744 cosmatch-0.1.3/cosmatch/transforms.py
--rw-r--r--   0        0        0      884 2024-03-22 10:51:29.839744 cosmatch-0.1.3/cosmatch/utils/__init__.py
--rw-r--r--   0        0        0     7052 2024-03-22 10:51:29.839744 cosmatch-0.1.3/cosmatch/utils/astrometry.py
--rw-r--r--   0        0        0     5110 2024-03-22 10:51:29.839744 cosmatch-0.1.3/cosmatch/utils/columns_handler.py
--rw-r--r--   0        0        0     5104 2024-03-22 10:51:29.839744 cosmatch-0.1.3/cosmatch/utils/io.py
--rw-r--r--   0        0        0     1417 2024-03-22 10:51:29.840744 cosmatch-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7646 1970-01-01 00:00:00.000000 cosmatch-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-05-04 13:29:30.094414 cosmatch-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6016 2024-05-04 13:29:30.094414 cosmatch-0.1.4/Readme.md
+-rw-r--r--   0        0        0      495 2024-05-04 13:29:30.094414 cosmatch-0.1.4/cosmatch/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-04 13:29:30.094414 cosmatch-0.1.4/cosmatch/classification/__init__.py
+-rw-r--r--   0        0        0     3736 2024-05-04 13:29:30.094414 cosmatch-0.1.4/cosmatch/classification/classification.py
+-rw-r--r--   0        0        0      187 2024-05-04 13:29:30.094414 cosmatch-0.1.4/cosmatch/fake/__init__.py
+-rw-r--r--   0        0        0    12576 2024-05-04 13:29:30.094414 cosmatch-0.1.4/cosmatch/fake/catalog_generator.py
+-rw-r--r--   0        0        0     1423 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/load/__init__.py
+-rw-r--r--   0        0        0     2779 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/load/disk_loader.py
+-rw-r--r--   0        0        0    27581 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/load/neighbours_loader.py
+-rw-r--r--   0        0        0      752 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/load/utils.py
+-rw-r--r--   0        0        0      249 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/match/__init__.py
+-rw-r--r--   0        0        0    16125 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/match/connection.py
+-rw-r--r--   0        0        0    53070 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/match/data_handler.py
+-rw-r--r--   0        0        0    11061 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/match/metrics.py
+-rw-r--r--   0        0        0      371 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/match/models/__init__.py
+-rw-r--r--   0        0        0     4440 2024-05-04 13:29:30.095414 cosmatch-0.1.4/cosmatch/match/models/base.py
+-rw-r--r--   0        0        0      240 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/models/custom/__init__.py
+-rw-r--r--   0        0        0     2884 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/models/custom/custom.py
+-rw-r--r--   0        0        0     7659 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/models/custom/optimization.py
+-rw-r--r--   0        0        0      686 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/models/custom/predict_models.py
+-rw-r--r--   0        0        0     3197 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/models/custom/prob_transformer.py
+-rw-r--r--   0        0        0    13677 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/models/ml_models.py
+-rw-r--r--   0        0        0    12405 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/models/nway_models.py
+-rw-r--r--   0        0        0    29596 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/nway.py
+-rw-r--r--   0        0        0     5057 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/pipeline.py
+-rw-r--r--   0        0        0     1560 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/pretrained/hyperparams.pickle
+-rw-r--r--   0        0        0     6602 2024-05-04 13:29:30.096414 cosmatch-0.1.4/cosmatch/match/union.py
+-rw-r--r--   0        0        0      490 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5154 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/preprocessing/duplicates.py
+-rw-r--r--   0        0        0     1410 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/preprocessing/gaps.py
+-rw-r--r--   0        0        0       24 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/search/__init__.py
+-rw-r--r--   0        0        0     6668 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/search/autoencoder.py
+-rw-r--r--   0        0        0    24808 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/search/find_hmxb.py
+-rw-r--r--   0        0        0     2304 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/search/io.py
+-rw-r--r--   0        0        0     7208 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/search/read_catalogues.py
+-rw-r--r--   0        0        0     6745 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/search/utils.py
+-rw-r--r--   0        0        0     1182 2024-05-04 13:29:30.097414 cosmatch-0.1.4/cosmatch/settings.py
+-rw-r--r--   0        0        0    33737 2024-05-04 13:29:30.098414 cosmatch-0.1.4/cosmatch/transforms.py
+-rw-r--r--   0        0        0     1394 2024-05-04 13:29:30.098414 cosmatch-0.1.4/cosmatch/utils/__init__.py
+-rw-r--r--   0        0        0     7056 2024-05-04 13:29:30.098414 cosmatch-0.1.4/cosmatch/utils/astrometry.py
+-rw-r--r--   0        0        0     7034 2024-05-04 13:29:30.098414 cosmatch-0.1.4/cosmatch/utils/columns_handler.py
+-rw-r--r--   0        0        0     5104 2024-05-04 13:29:30.098414 cosmatch-0.1.4/cosmatch/utils/io.py
+-rw-r--r--   0        0        0     1417 2024-05-04 13:29:30.099414 cosmatch-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7646 1970-01-01 00:00:00.000000 cosmatch-0.1.4/PKG-INFO
```

### Comparing `cosmatch-0.1.3/Readme.md` & `cosmatch-0.1.4/Readme.md`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/fake/catalog_generator.py` & `cosmatch-0.1.4/cosmatch/fake/catalog_generator.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/match/data_handler.py` & `cosmatch-0.1.4/cosmatch/match/data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,14 +655,15 @@
     data = join_table.join(frame.rename(columns=rename_frame).set_index(frame.attrs['id']), on='id_frame', how='left')
     data = data.join(target.rename(columns=rename_target).set_index(target.attrs['id']), on='id_target', how='left')
     data.rename(columns={'id_frame': frame.attrs['id'], 'id_target': target.attrs['id'],
                          'ra_frame': frame.attrs['ra'], 'dec_frame': frame.attrs['dec'],
                          'ra_target': target.attrs['ra'], 'dec_target': target.attrs['dec']}, inplace=True)
     
     unite_attrs_from_frame_and_target(data, frame, target)
+    data.attrs['poserr'] = target.attrs['poserr']
 
     return data
 
 
 def _prepare_proper_copies(df: pd.DataFrame, columns: list[str] = ['id', 'ra', 'dec']) -> pd.DataFrame:
     """Подгатавливает копии для построения основы будущего совмещенного каталога, к которому потом будут присоединены оставшиеся колонки."""
     check_attrs_structure(df, columns)
```

### Comparing `cosmatch-0.1.3/cosmatch/match/metrics.py` & `cosmatch-0.1.4/cosmatch/match/metrics.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/match/models/base.py` & `cosmatch-0.1.4/cosmatch/match/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,41 @@
 
 from typing import Union, Any
 
 
 class Model:
     """Абстрактная модель для решения задачи отождествления."""
 
-    @abstractmethod
     def __init__(self) -> None:
         """Абстрактный метод для переопределения в наследуемых классах."""
-        pass
+        self.fitted = False
 
     @abstractmethod
     def predict_proba(self, df: pd.DataFrame) -> pd.DataFrame:
         """Предсказание вероятностей."""
         pass
 
+    def _predict_proba_help(self, df: pd.DataFrame) -> None:
+        if not self.fitted and self.fit_required:
+            raise ValueError('Model is not fitted')
+
     def __str__(self) -> str:
         """String representation."""
         return self.__class__.__name__  # type: ignore
 
     def __name__(self) -> str:
         """Name."""
         return 'model'
 
     def fit(self, X: pd.DataFrame, y: np.ndarray) -> 'Model':
         """Обучение модели."""
-        return NotImplemented
+        pass
+    
+    def _fit_help(self, X: pd.DataFrame, y: np.ndarray) -> None:
+        self.fitted=True
 
     def get_predicted(self, X: pd.DataFrame) -> pd.DataFrame:
         """Сделать предсказания модели с 3 вероятностями: p_i, P_i, P_0 и флагом наиболее вероятного отождествления."""
         X = X.copy()
         mark = self.predict_proba(X)
         return ProbTransformer.transform(X, mark)
 
@@ -56,14 +62,16 @@
 
 
 class NearestNeighbour(Model):
     """Модель поиска ближайшего соседа. Строит вероятнсти TODO."""
 
     def __init__(self, frequency_between: tuple[int, int] = (10, 15)) -> None:
         """Инициализация модели."""
+        self.fit_required = False
+        self.fitted = False
         self.frequency_between = frequency_between
 
     def _join_neighbours(self, data: pd.DataFrame, query: str) -> pd.DataFrame:
         """Строит датасет с колонкой равной количеству соседей в радиусе."""
         neighbours = data.query(query)[data.attrs['id_frame']].value_counts().reset_index()
         neighbours.columns = [data.attrs['id_frame'], 'neighbours']
         return data.join(neighbours.set_index(data.attrs['id_frame']), 
@@ -81,11 +89,12 @@
         Выполняет метод predict_proba для внутренней модели.
 
         Args:
             X: Таблица с парами рентген-оптика.
         Returns:
             Возвращает вероятности принадлежности пары к первому классу.
         """
+        self._predict_proba_help(X)
         area = (self.frequency_between[1] ** 2 - self.frequency_between[0] ** 2) * np.pi
         freq = self._join_neighbours(X, f'distance<={self.frequency_between[1]}') - self._join_neighbours(X, f'distance<={self.frequency_between[0]}')
-        res = self._calc_p_match(1, X['distance'], X['poserr'], freq / area)
+        res = self._calc_p_match(1, X['distance'], X[X.attrs['poserr']], freq / area)
         return res
```

### Comparing `cosmatch-0.1.3/cosmatch/match/models/custom/custom.py` & `cosmatch-0.1.4/cosmatch/match/models/custom/custom.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/match/models/custom/optimization.py` & `cosmatch-0.1.4/cosmatch/match/models/custom/optimization.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/match/models/custom/predict_models.py` & `cosmatch-0.1.4/cosmatch/match/models/custom/predict_models.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/match/models/custom/prob_transformer.py` & `cosmatch-0.1.4/cosmatch/match/models/custom/prob_transformer.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/match/models/ml_models.py` & `cosmatch-0.1.4/cosmatch/match/models/ml_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 
     * P_0 - вероятность источника быть бездомным. То есть все найденные пары с этим источником неверные отождествления.
 
     """
 
     def __init__(self) -> None:
         """Инициализация модели."""
+        self.fit_required = True
+        self.fitted = False
         self.model = None
 
     @abstractmethod
     def _params_space(self) -> Union[Tuple[dict, dict], None]:
         """
         Абстрактный метод для переопределения в наследуемых классах.
 
@@ -162,34 +164,38 @@
         """
         Обучить модель на помеченном наборе данных.
 
         Args:
             X: Таблица пар рентген-оптика с признаками и id источников.
             y: Массив меток классов.
         """
+        self._fit_help(X, y)
         self.model.fit(self._drop_id(X), y)
         return self
 
     def predict_proba(self, X: pd.DataFrame) -> np.ndarray:
         """
         Выполняет метод predict_proba для внутренней модели.
 
         Args:
             X: Таблица с парами рентген-оптика.
         Returns:
             Возвращает вероятности принадлежности пары к первому классу.
         """
+        self._predict_proba_help(X)
         return self.model.predict_proba(self._drop_id(X))[:, 1]
 
 
 class Catboost(ModelML):
     """Градиентный бустинг."""
 
     def __init__(self, gpu: bool = False) -> None:
         """Инициализация модели."""
+        self.fit_required = True
+        self.fitted = False
         self.gpu = gpu
         self.model = boost.CatBoostClassifier()
         self.load_default_params()
 
     def set_params(self, params: dict[str, float]) -> 'Catboost':
         """Устанавливает параметры модели."""
         params_ = {'iterations': 250}
@@ -203,14 +209,15 @@
             self.load_params('default_cpu')  # REDO
         else:
             self.load_params()
         return self
 
     def fit(self, X: pd.DataFrame, y: np.ndarray) -> 'Catboost':
         """Обучение модели."""
+        self._fit_help(X, y)
         X_train, X_test, y_train, y_test = train_test_split(self._drop_id(X),
                                                             y, test_size=0.2, random_state=42)
         params = self.model.get_params()
         self.model = boost.CatBoostClassifier().set_params(**params)
         self.model.set_params(**{'use_best_model': True, 'eval_metric': 'F1'})
         self.model.fit(X_train, y_train, eval_set=(X_test, y_test),
                        use_best_model=True, early_stopping_rounds=50, logging_level='Silent')
@@ -250,14 +257,16 @@
 
 
 class RandomForest(ModelML):
     """Случайный лес."""
 
     def __init__(self) -> None:
         """Инициализация модели."""
+        self.fit_required = True
+        self.fitted = False
         self.model = RandomForestClassifier()
         self.load_default_params()
 
     def _params_space(self) -> Tuple[dict[str, Any], dict[str, Any]]:
         """
         Возвращает пространство для перебора гиперпараметров с помощью бибилиотеки hyperopt.
```

### Comparing `cosmatch-0.1.3/cosmatch/match/models/nway_models.py` & `cosmatch-0.1.4/cosmatch/match/models/nway_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 
 class NWAY(Model):
     """Модель NWAY для поиска отождествлений без использования приора."""
 
     def __init__(self, distance: float = 15, opt_err: float = 0.1, prior_completeness: float = 0.9) -> None:
         """Инициализация модели."""
+        self.fit_required = False
+        self.fitted = False
         if not os.path.exists('nway_data'):
             os.mkdir('nway_data')
         self._distance = distance
         self._opt_err = opt_err
         self._prior_completeness = prior_completeness
 
     def _save_fits(self, df: pd.DataFrame, name: str, area: float) -> None:
@@ -135,14 +137,16 @@
 
 
 class NWAYauto(NWAY):
     """Модель NWAY для поиска отождествлений с использованием автоматически генерируемого приора."""
 
     def __init__(self, distance: float = 15, opt_err: float = 0.1, prior_completeness: float = 0.9, prior_radius: float = 3.5) -> None:
         """Инициализация модели."""
+        self.fit_required = False
+        self.fitted = False
         super().__init__(distance, opt_err, prior_completeness)
         self.prior_radius = prior_radius
 
     def get_predicted(self, df: Union[pd.DataFrame, None] = None, opt: Union[pd.DataFrame, None] = None,
                       xray: Union[pd.DataFrame, None] = None) -> pd.DataFrame:
         """Сделать предсказания модели с 3 вероятностями: p_i, P_i, P_0."""
         if df is None and opt is None and xray is None:
@@ -177,14 +181,16 @@
 
 
 class NWAYml(NWAY):
 
     def __init__(self, distance: float = 15, opt_err: float = 0.1, prior_completeness: float = 0.9,
                  ml_model: ModelML = Catboost(), bins: int = 20) -> None:
         """Инициализация модели."""
+        self.fit_required = True
+        self.fitted = False
         super().__init__(distance, opt_err, prior_completeness)
         self.ml_model = ml_model
         self.bins = bins
 
     def save_prior(self, y: np.ndarray, pred: pd.DataFrame) -> None:
         """Сохранить приор, для использования его в модели."""
         arr = np.stack((y, pred)).T
```

### Comparing `cosmatch-0.1.3/cosmatch/match/nway.py` & `cosmatch-0.1.4/cosmatch/match/nway.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/match/pipeline.py` & `cosmatch-0.1.4/cosmatch/match/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,10 +110,10 @@
         # df = self.transform(df, name_pattern)
         # Это надо оптимизировать
         if self.fitted_columns is None:
             predict = self.model.get_predicted(df)
         else:
             predict = self.model.get_predicted(df[self.fitted_columns])  # type: ignore
         if not keep_features:
-            return predict[df.attrs['ids'] + df.attrs['coords'] + ['poserr', 'distance',
-                            'p_i', 'P_i', 'P_0', 'flag_best']]
+            return predict[df.attrs['ids'] + df.attrs['coords'] + [df.attrs['poserr']] +
+                            ['distance', 'p_i', 'P_i', 'P_0', 'flag_best']]
         return predict
```

### Comparing `cosmatch-0.1.3/cosmatch/match/pretrained/hyperparams.pickle` & `cosmatch-0.1.4/cosmatch/match/pretrained/hyperparams.pickle`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/search/find_hmxb.py` & `cosmatch-0.1.4/cosmatch/search/find_hmxb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,73 @@
-import torch
-import pytorch_lightning as L
-from torch.utils.data import Dataset
-from torchvision import datasets
-import torch.optim as optim
-import torch.nn as nn
+
+
 from sklearn.manifold import TSNE
 from sklearn.preprocessing import StandardScaler
 from sklearn.metrics import roc_auc_score
 from matplotlib import pyplot as plt
 from typing import Union, Callable, Tuple, Any
 import pandas as pd
 import numpy as np
 from collections import Counter
 
 from ..utils import add_postfix_to_main_columns, correlate
 from ..match.connection import mark_object_in_catalog
 
 
+def make_data():
+    data = pd.read_pickle('DS/find_hmxb/initial_data_mass.pickle')
+    data = data.query('id_xmm!=-1 and abs(b_deg)<20')
+
+    wise = pd.read_csv('DS/tmp/all_cat.csv')[['main_id', 'ra', 'dec','W1mag', 'W2mag', 'W3mag', 'W4mag', 'main_type']]
+    wise.columns = ['id_wise', 'ra_wise', 'dec_wise', 'W1mag', 'W2mag', 'W3mag', 'W4mag', 'otype']
+
+    wise = pd.read_csv('DS/tmp/all_cat.csv')[['main_id', 'ra', 'dec','W1mag', 'W2mag', 'W3mag', 'W4mag', 'main_type']]
+    wise.columns = ['id_wise', 'ra_wise', 'dec_wise', 'W1mag', 'W2mag', 'W3mag', 'W4mag', 'otype']
+
+    for i in wise.columns:
+        data[i] = wise[i].values
+
+    if True:
+        data['otype'] = data['otype'].replace({'CV*': 'CV', 
+                                            'G': 'Galaxy', 
+                                            'QSO': 'Quasar',
+                                            
+                                            'BLL': 'Quasar',
+                                            "Sy1": 'Galaxy',
+                                            'Sy2': 'Galaxy', 
+                                            'GiC': 'Galaxy',
+                                            'GiG': 'Galaxy',
+                                            'AGN': 'Galaxy',
+                                            'rG': 'Galaxy'
+                                            })
+
+    data.attrs['ids'].append('id_wise')
+    data.attrs['coord'].append('dec_wise')
+    data.attrs['coord'].append('ra_wise')
+    data.attrs['names'].append('wise')
+
+    data['w1-w2'] = data['W1mag'] - data['W2mag']
+    data['new_parallax'] = data['parallax'].values/ data['parallax_error'].values
+
+    del data['parallax'], data['parallax_error']
+
+    return data
+
+
+
 def tsne(data: pd.DataFrame, ignored: list, verbose: bool = False, random_state: int = 42,
          perplexity: int = 400, scalar: bool = True, n_components: int = 2) -> pd.DataFrame:
 
     model = TSNE(n_components=n_components, learning_rate='auto', init='random', perplexity=perplexity,
                  random_state=random_state, verbose=verbose)
 
     data = data.drop(columns=ignored)
 
     for i in data.columns:
-        data[i] = data[i].fillna(data.loc[data[i].notna(), i].mean())
+        data[i] = data[i].fillna(data.loc[data[i].notna(), i].quantile(0.95))
         if data[i].isna().sum() > 0:
             del data[i]
 
     if scalar:
         data = StandardScaler().fit_transform(data)
     X_tr = model.fit_transform(data)
     return X_tr
@@ -39,53 +76,121 @@
 def plot_hmxb(compressed: np.ndarray, train: pd.DataFrame, ax: Union[plt.Axes, None] = None, name: str = '') -> None:  # *(train.g_mag<12)
 
     if ax is None:
         fig, ax = plt.subplots()
     compressed_false = compressed[train.type=='None']
     ax.scatter(compressed_false[:, 0], compressed_false[:, 1], s=0.1, c='g', label='Unknown')
 
-    color = {'CV': 'orange', 'Quasar': 'black', 'Star': 'purple','LMXB': 'b',  'HMXB': 'r', }
+    color = {
+        #'CV': 'orange', 'Quasar': 'black', 'Star': 'purple',
+        'LMXB': 'b',  
+        'HMXB': 'r', }
 
     for key, val in color.items():
         x = compressed[train.type.values == key]
         ax.scatter(x[:, 0], x[:, 1], s=6, c=val, label=key)
 
     plt.legend()
 
 
     if name:
         ax.set_title(name)
 
-def plot_hmxb(compressed: np.ndarray, train: pd.DataFrame, ax: Union[plt.Axes, None] = None, name: str = '',) -> None:  # *(train.g_mag<12)
+def plot_hmxb(compressed: np.ndarray, train: pd.DataFrame, ax: Union[plt.Axes, None] = None, name: str = '',scaler: int=1) -> None:  # *(train.g_mag<12)
 
     if ax is None:
         fig, ax = plt.subplots()
-    compressed_false = compressed[train.otype.isna()]
-    ax.scatter(compressed_false[:, 0], compressed_false[:, 1], s=0.1, c='g', label='Unknown')
+    compressed_false = compressed[train['otype'].isna()]
+    ax.scatter(compressed_false[:, 0], compressed_false[:, 1], s=0.05, c='g', label='Unknown')
 
     if 'otype' in train.columns:
-        color = {'Quasar': 'black', 'CV':'orange', 'Galaxy': 'purple', 'EB*': 'y'}
+        color = {
+        #'Star': 'purple', 
+        #'XRAY': 'orange', 'YSO': 'black',
+        #'LMXB': 'b',  
+        'HMXB': 'r', 
+        #'HMXB_CAND': 'b'
+        }
         for key, val in color.items():
-            x = compressed[train.otype.values == key]
-            ax.scatter(x[:, 0], x[:, 1], s=6, c=val)
+            if key=='HMXB' or key=='HMXB_CAND':
+                x = compressed[(train['otype'].values == key)| (train['type']==key)]
+                ax.scatter(x[:, 0], x[:, 1], s=15*scaler, c=val, label=key)
+                continue
+            #print(key)
+            x = compressed[(train.otype.values == key)| (train['type']==key)]
+            #print(x.shape)
+            ax.scatter(x[:, 0], x[:, 1], s=3*scaler, c=val, label=key)
+
+    #plt.legend(fontsize='x-small', bbox_to_anchor=(1.1, 1.1))
+    ax.set_xticks([])
+    ax.set_yticks([])
+    if name:
+        ax.set_title(name + f' | HMXB:{train["type"].value_counts()["HMXB"]}, TOTAL:{train.shape[0]}')
 
-    color = {'CV': 'orange', 'Quasar': 'black', 'Galaxy': 'purple','LMXB': 'b',  'HMXB': 'r', }
+def plot_hmxb_classes(compressed: np.ndarray, train: pd.DataFrame, ax: Union[plt.Axes, None] = None, name: str = '',scaler: int=1) -> None:  # *(train.g_mag<12)
 
-    for key, val in color.items():
-        x = compressed[train.type.values == key]
-        ax.scatter(x[:, 0], x[:, 1], s=6, c=val, label=key)
+    if ax is None:
+        fig, ax = plt.subplots()
+    compressed_false = compressed[train.otype.isna()]
+    ax.scatter(compressed_false[:, 0], compressed_false[:, 1], s=0.001, c='b', label='Unknown')
 
+    colors = ['red', 'blue', 'green', 'purple', 'yellow', 'pink']
+    replace = {0:'red', 1:'blue', 2:'green', 3:'purple', 4:'yellow', 5:'pink'}
+    compressed_hmxb = compressed[train['type']=='HMXB']
+    ax.scatter(compressed_hmxb[:, 0], compressed_hmxb[:, 1], s=15*scaler, 
+                c=train[train['type']=='HMXB']['last_claster'].replace(replace), label='HMXB')
+
+    plt.legend(fontsize='x-small', bbox_to_anchor=(1.1, 1.1))
+    ax.set_xticks([])
+    ax.set_yticks([])
+    if name:
+        ax.set_title(name, fontsize='x-small')
 
+def plot_hmxb_partial(compressed: np.ndarray, train: pd.DataFrame, ax: Union[plt.Axes, None] = None, name: str = '', classes: list = []) -> None:
 
-    plt.legend()
+    if ax is None:
+        fig, ax = plt.subplots()
+    compressed_false = compressed[train.type=='None']
+    ax.scatter(compressed_false[:, 0], compressed_false[:, 1], s=0.001, c='b', label='Unknown')
+
+    colors = ['black', 'orange', 'purple', 'g', 'magenta', 'pink', 'yellow' ]
+
+    for num, color in enumerate(classes):
+        x = compressed[(train.otype.values == classes[num])|(train.type.values == classes[num])]
+        ax.scatter(x[:, 0], x[:, 1], s=20, c=colors[num], label=classes[num])
+
+    ax.legend(loc='upper right',fontsize='small')
 
 
     if name:
         ax.set_title(name)
 
+def plot_mag_shift(real_data, nn_data, ind=639, ax=None):
+    import seaborn as sns
+    maggas = ['g_mag', 'bp_mag', 'rp_mag', 'Jmag', 'Hmag', 'Kmag', 'rmag', 'imag', 'Hamag', 'mag_flux_1', 'mag_flux_2', 'mag_flux_3']
+    stat = []
+    for i in maggas:
+        stat.append([real_data.iloc[ind][i], nn_data.iloc[ind][i], real_data[i].quantile(0.1), real_data[i].quantile(0.9)])
+
+    stat = np.array(stat)
+
+    maggas = ['g_mag', 'bp_mag', 'rp_mag', 'Jmag', 'Hmag', 'Kmag', 'rmag', 'imag', 'Hamag', 'Xmag_02-05', 'Xmag_05-1', 'Xmag_1-2']
+
+    if ax is None:
+        fig, ax = plt.subplots()
+
+    ax.plot(maggas, stat[:,0], 'g-', label='real')
+    ax.plot(maggas, stat[:,1], 'b-', label='nn')
+
+    # Add boxplot to each point
+    for x, (x_val, y_val) in enumerate(zip(maggas, stat)):
+        sns.boxplot(x=[x_val, x_val], y=[stat[x, 2], stat[x, 3]], ax=ax, width=0.1, color='red')
+
+    ax.tick_params(axis='x', labelrotation=90)
+
 
 # ----------------------------------------------------------------------------------------------- #
 #                                         Gat rank                                                #
 # ----------------------------------------------------------------------------------------------- #
 
 
 def dist_to_n_nearest_(n_coords: np.ndarray, m_coords: np.ndarray, count_nearest: int = 5, how: str = 'mean') -> np.ndarray:
@@ -153,27 +258,28 @@
 
 
 def roc_auc_rank(sorted_data: pd.DataFrame, mark: np.ndarray) -> float:
     return roc_auc_score(mark, -sorted_data.index)
 
 
 def evaluate_compression(compress: np.ndarray, data: pd.DataFrame, samples: int = 10, sample_size: int = 20,
-                         metric: str = 'mean', n_nearest: int = 10,
+                         metric: str = 'mean', n_nearest: int = 5,
                          score_fn: Callable = lambda x, y: number_top_n(x, y, n=10)) -> float:
     scores = []
     for i in range(samples):
-        data_ = data[['id_gaia', 'is_hmxb']].copy()
+        data_ = data[['id_gaia', 'type', 'otype']].copy()
+        #data_.loc[data_['otype']=='HMXB', 'type'] = 'HMXB'
         data_['id_gaia'] = data_['id_gaia'].astype(np.int64)
-        id_hmxb = data_.query('is_hmxb==1')['id_gaia'].sample(sample_size).values
+        id_hmxb = data_.query('type=="HMXB"')['id_gaia'].sample(sample_size).values
 
-        data_['metric'] = dist_to_n_nearest(compress[data_.is_hmxb.astype(bool) * (~data_.id_gaia.isin(id_hmxb))],
+        data_['metric'] = dist_to_n_nearest(compress[(data_['type']=='HMXB') * (~data_.id_gaia.isin(id_hmxb))],
                                             compress, n_nearest, metric)
         data_.sort_values('metric', inplace=True)
-        data_ = data_[(data_['is_hmxb'] != 1) | (data_['id_gaia'].isin(id_hmxb))].reset_index(drop=True)
-        score = score_fn(data_, data_.id_gaia.isin(id_hmxb))
+        data_ = data_[(data_['type'] != 'HMXB') | (data_['id_gaia'].isin(id_hmxb))].reset_index(drop=True)
+        score = score_fn(data_, data_['id_gaia'].isin(id_hmxb))
         scores.append(score)
     return np.array(scores).mean()
 
 
 # ----------------------------------------------------------------------------------------------- #
 #                                  подготовка кандидатов                                          #
 # ----------------------------------------------------------------------------------------------- #
@@ -223,250 +329,84 @@
                              'score', 'was_last_top50', 'is_lmxb', 'to_copy', 'url_xray', 'url_gaia']]
 
     candidates['id_gaia'] = candidates['id_gaia'].astype(str)
     candidates['id_xmm'] = candidates['id_xmm'].astype(str)
     candidates['id_ps'] = candidates['id_ps'].astype(str)
     return candidates
 
-# ----------------------------------------------------------------------------------------------- #
-#                                          Нейронки                                               #
-# ----------------------------------------------------------------------------------------------- #
-
-
-class DeepAutoencoder(nn.Module):
-    def __init__(self, shape_0: int) -> None:
-        input_dim = shape_0
-        hidden_dim1 = 20
-        hidden_dim2 = 10
-        latent_dim = 2
-        super(DeepAutoencoder, self).__init__()
-        self.encoder = nn.Sequential(
-            nn.Linear(input_dim, hidden_dim1),
-            nn.ReLU(),
-            nn.Linear(hidden_dim1, hidden_dim2),
-            nn.ReLU(),
-            nn.Linear(hidden_dim2, latent_dim)
-        )
-        self.decoder = nn.Sequential(
-            nn.Linear(latent_dim, hidden_dim2),
-            nn.ReLU(),
-            nn.Linear(hidden_dim2, hidden_dim1),
-            nn.ReLU(),
-            nn.Linear(hidden_dim1, input_dim),
-            nn.Sigmoid()
-        )
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        x = self.encoder(x)
-        x = self.decoder(x)
-        return x
-
-
-class MyEncoder(nn.Module):
-
-    def __init__(self, shapes: list, relu: bool = True, dropout: Union[float, None] = None) -> None:
-        super().__init__()
-        list_of_layers = []
-        for i in range(len(shapes) - 2):
-            list_of_layers.append(nn.Linear(shapes[i], shapes[i + 1]))
-            if relu:
-                list_of_layers.append(nn.ReLU())
-            if dropout is not None:
-                list_of_layers.append(nn.Dropout(p=dropout))
-        list_of_layers.append(nn.Linear(shapes[-2], shapes[-1]))
-
-        self.layers = nn.Sequential(*list_of_layers)
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self.layers(x)
-
-
-class MyDecoder(nn.Module):
-
-    def __init__(self, shapes: list, relu: bool = True, dropout: Union[float, None] = None) -> None:
-        super().__init__()
-        list_of_layers = []
-        for i in range(len(shapes) - 2):
-            list_of_layers.append(nn.Linear(shapes[-i - 1], shapes[-i - 2]))
-            if relu:
-                list_of_layers.append(nn.ReLU())
-            if dropout is not None:
-                list_of_layers.append(nn.Dropout(p=dropout))
-        list_of_layers.append(nn.Linear(shapes[1], shapes[0]))
-        self.layers = nn.Sequential(*list_of_layers)
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self.layers(x)
-
-
-class MyAutoencoder(L.LightningModule):
-
-    def __init__(self, shapes: list, relu: bool = True, dropout_en: Union[float, None] = None,
-                 dropout_de: Union[float, None] = None) -> None:
-        super().__init__()
-        self.encoder = MyEncoder(shapes, relu, dropout_en)
-        self.decoder = MyDecoder(shapes, relu, dropout_de)
-
-        self.val_outputs: list = []
-        self.train_outputs: list = []
-        self.train_loss: list = []
-        self.val_loss: list = []
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        x = self.encoder(x)
-        x = self.decoder(x)
-        return x
-
-    def calc_loss(self, x: torch.Tensor, x_hat: torch.Tensor) -> torch.Tensor:
-        loss = nn.functional.mse_loss(x_hat, x)
-        return loss
-
-    def training_step(self, batch: Tuple[torch.Tensor, torch.Tensor], batch_idx: int) -> dict[str, torch.Tensor]:
-        x, y = batch
-        x = x.view(x.size(0), -1)
-        y = y.view(y.size(0), -1)
-        x_hat = self.forward(x)
-        loss = self.calc_loss(x_hat, y)
-        self.log("train_loss", loss, on_step=False, on_epoch=True, prog_bar=True, logger=False)
-        self.train_outputs.append({'loss': loss})
-        return {'loss': loss}
-
-    def validation_step(self, batch: Tuple[torch.Tensor, torch.Tensor], batch_idx: int) -> dict[str, torch.Tensor]:
-        with torch.no_grad():
-            x, y = batch
-            x = x.view(x.size(0), -1)
-            x_hat = self.forward(x)
-            loss = self.calc_loss(x_hat, y)
-        self.log("val_loss", loss, prog_bar=True)
-        self.val_outputs.append({'loss': loss})
-        return {'loss': loss}
-
-    def configure_optimizers_(self) -> Tuple[list[torch.optim.Optimizer], list[dict[str, Any]]]:
-        optimizer = torch.optim.Adam(self.parameters(), lr=1e-3, weight_decay=5e-4)
-
-        lr_scheduler = {
-            'scheduler': torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, mode='min', factor=0.5, patience=10, min_lr=1e-6, verbose=True),
-            'monitor': 'val_loss',
-        }
-
-        return [optimizer], [lr_scheduler]
-
-    def configure_optimizers(self) -> Tuple[list[torch.optim.Optimizer], list[dict[str, Any]]]:
-        optimizer = torch.optim.Adam(self.parameters(), lr=1e-3, weight_decay=5e-4)
-
-        # Define a custom lambda function for the sawtooth learning rate
-        def lr_lambda(epoch: int) -> float:
-            # Define the sawtooth shape for the learning rate
-            cycle = 10  # Number of iterations in a cycle
-            return 0.5 * (1 - abs(epoch % cycle - cycle // 2) / (cycle // 2))
-
-        lr_scheduler = {
-            'scheduler': torch.optim.lr_scheduler.LambdaLR(optimizer, lr_lambda),
-            'interval': 'epoch',
-        }
-
-        return [optimizer], [lr_scheduler]
-
-    def on_validation_epoch_end(self) -> None:
-        # здесь вы можете использовать self.train_outputs для доступа к выводам обучения
-        avg_loss = torch.stack([x['loss'] for x in self.val_outputs]).mean()
-        print(f"| Val Loss: {avg_loss:.3f}")
-        self.log('val_loss', avg_loss, prog_bar=True, on_epoch=True, on_step=False)
-        self.val_outputs = []
-        self.val_loss.append(avg_loss)
-
-    def on_train_epoch_end(self) -> None:
-        # здесь вы можете использовать self.train_outputs для доступа к выводам обучения
-        avg_loss = torch.stack([x['loss'] for x in self.train_outputs]).mean()
-        print(f"| Train Loss: {avg_loss:.3f}")
-        self.log('train_loss', avg_loss, prog_bar=True, on_epoch=True, on_step=False)
-        self.train_outputs = []
-        self.train_loss.append(avg_loss)
-
-
-class MyDataset(Dataset):
-    def __init__(self, dataset: np.ndarray) -> None:
-        self.dataset = dataset
-        self.dataset = torch.tensor(self.dataset, dtype=torch.float)
-
-    def __len__(self) -> int:
-        return len(self.dataset)
-
-    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
-        return self.dataset[idx], self.dataset[idx]
     
 # ----------------------------------------------------------------------------------------------- #
 #                                          Добавить классы                                        #
 # ----------------------------------------------------------------------------------------------- #
 
 
 def make_star1():
     star_1 = pd.read_pickle('DS/find_hmxb/mark_in_catalog/star_1.pkl')
     star_1 = star_1[['recno', '_RA', '_DE']].rename(columns={'recno':'id', '_RA': 'ra', '_DE':'dec'})
-    add_postfix_to_id_ra_dec_col(star_1, 'star1')
+    add_postfix_to_main_columns(star_1, 'star1')
     star_1.attrs['name'] = 'star1'
     star_1.attrs['id'] = 'id_star1'
     star_1.attrs['ra'] = 'ra_star1'
     star_1.attrs['dec'] = 'dec_star1'
 
     return star_1
 
 def make_star2():
     star_2 = pd.read_pickle('DS/find_hmxb/mark_in_catalog/star_2.pkl')
     star_2 = star_2[['recno', 'RAJ2000', 'DEJ2000']].rename(columns={'recno':'id', 'RAJ2000': 'ra', 'DEJ2000':'dec'}).loc[1:]
-    add_postfix_to_id_ra_dec_col(star_2, 'star2')
+    add_postfix_to_main_columns(star_2, 'star2')
     star_2.attrs['name'] = 'star2'
     star_2.attrs['id'] = 'id_star2'
     star_2.attrs['ra'] = 'ra_star2'
     star_2.attrs['dec'] = 'dec_star2'
 
     star_2['ra_star2'] = star_2['ra_star2'].map(lambda x: float(x.split(' ')[0])*15 + float(x.split(' ')[1])*0.25 + float(x.split(' ')[2])*(0.25 / 60))
     star_2['dec_star2'] = star_2['dec_star2'].map(lambda x: float(x.split(' ')[0]) + float(x.split(' ')[1])*(1/60) + float(x.split(' ')[2])*(1/3600))
     return star_2
 
 def make_quas():
     quas = pd.read_pickle('DS/find_hmxb/mark_in_catalog/mil_quasar.pkl')
     quas = quas[['recno', 'RAJ2000', 'DEJ2000']].rename(columns={'recno':'id', 'RAJ2000': 'ra', 'DEJ2000':'dec'}).copy()
-    add_postfix_to_id_ra_dec_col(quas, 'quas')
+    add_postfix_to_main_columns(quas, 'quas')
     quas.attrs['name'] = 'quas'
     quas.attrs['id'] = 'id_quas'
     quas.attrs['ra'] = 'ra_quas'
     quas.attrs['dec'] = 'dec_quas'
 
     return quas
 
 def make_cv_cat1():
     cv_cat1 = pd.read_pickle('DS/find_hmxb/mark_in_catalog/cv_cat1.pkl')
     cv_cat1 = cv_cat1[['recno', 'RAJ2000', 'DEJ2000']].rename(columns={'recno':'id', 'RAJ2000': 'ra', 'DEJ2000':'dec'}).copy()
-    add_postfix_to_id_ra_dec_col(cv_cat1, 'cv1')
+    add_postfix_to_main_columns(cv_cat1, 'cv1')
     cv_cat1.attrs['name'] = 'cv1'
     cv_cat1.attrs['id'] = 'id_cv1'
     cv_cat1.attrs['ra'] = 'ra_cv1'
     cv_cat1.attrs['dec'] = 'dec_cv1'
 
     cv_cat1['ra_cv1'] = cv_cat1['ra_cv1'].map(lambda x: float(x.split(' ')[0])*15 + float(x.split(' ')[1])*0.25 + float(x.split(' ')[2])*(0.25 / 60))
     cv_cat1['dec_cv1'] = cv_cat1['dec_cv1'].map(lambda x: float(x.split(' ')[0]) + float(x.split(' ')[1])*(1/60) + float(x.split(' ')[2])*(1/3600))
     return cv_cat1
 
 def make_cv_cat2():
     cv_cat2 = pd.read_pickle('DS/find_hmxb/mark_in_catalog/cv_cat2.pkl')
     cv_cat2 = cv_cat2[['recno', 'RAJ2000', 'DEJ2000']].rename(columns={'recno':'id', 'RAJ2000': 'ra', 'DEJ2000':'dec'}).copy()
-    add_postfix_to_id_ra_dec_col(cv_cat2, 'cv2')
+    add_postfix_to_main_columns(cv_cat2, 'cv2')
     cv_cat2.attrs['name'] = 'cv2'
     cv_cat2.attrs['id'] = 'id_cv2'
     cv_cat2.attrs['ra'] = 'ra_cv2'
     cv_cat2.attrs['dec'] = 'dec_cv2'
 
     cv_cat2['ra_cv2'] = cv_cat2['ra_cv2'].map(lambda x: float(x.split(' ')[0])*15 + float(x.split(' ')[1])*0.25 + float(x.split(' ')[2])*(0.25 / 60))
     cv_cat2['dec_cv2'] = cv_cat2['dec_cv2'].map(lambda x: float(x.split(' ')[0]) + float(x.split(' ')[1])*(1/60) + float(x.split(' ')[2])*(1/3600))
     return cv_cat2
 
 def make_lis():
     desi_lis = pd.read_pickle('DS/LS/LS_class.pickle')
-    add_postfix_to_id_ra_dec_col(desi_lis, 'lis')
+    add_postfix_to_main_columns(desi_lis, 'lis')
     desi_lis.attrs['name'] = 'lis'
     desi_lis.attrs['id'] = 'id_lis'
     desi_lis.attrs['ra'] = 'ra_lis'
     desi_lis.attrs['dec'] = 'dec_lis'
 
     return desi_lis
 
@@ -514,27 +454,31 @@
     return df_main
 
 
 # ----------------------------------------------------------------------------------------------- #
 #                                          Clastering                                             #
 # ----------------------------------------------------------------------------------------------- #
 
-
-def prepare_classes(compressed, data, model, ax=None, name=''):
+def plot_classes(compressed, data,  classes, ax=None, name=''):
     if ax is None:
         fig, ax = plt.subplots()
     X = compressed[data.type=='HMXB']
-    classes = model.fit_predict(X)
-    while classes[0]!=0 or classes[6]!=2 or classes[8]!=3:
-        classes = model.fit_predict(X)
     color = ['red', 'blue', 'green', 'purple', 'yellow', 'pink']
     ax.scatter(compressed[:,0], compressed[:,1], s=0.001)
-    ax.scatter(X[:,0], X[:,1], color=[color[i] for i in classes])
-    classes = np.array([i if i!=-1 else np.max(classes)+1 for i in classes])
+    ax.scatter(X[:,0], X[:,1], color=[color[i] for i in classes], s=100)
     ax.set_title(name)
+
+def prepare_classes(compressed, data, model, ax=None, name='', plot=True):
+    X = compressed[data.type=='HMXB']
+    classes = model.fit_predict(X)
+    #while classes[0]!=0 or classes[6]!=2 or classes[8]!=3:
+    #    classes = model.fit_predict(X)
+    classes = np.array([i if i!=-1 else np.max(classes)+1 for i in classes])
+    if plot:
+        plot_classes(compressed, data, classes, ax, name)
     return classes
 
 def plot_class_distribution(classes, data, hmxb, ax=None, n_classes=5, name=''):
     if ax is None:
         fig, ax = plt.subplots()
 
     class_to_id_gaia = lambda x: data.query('type=="HMXB"').loc[classes==x].id_gaia
@@ -560,15 +504,15 @@
         ax.bar(sorted_categories, values, bottom=bottom, color=color[i])
         bottom += np.array(values)
     ax.set_title(name)
 
     
 def plot_class_distribution_separately(classes, data, hmxb, n_classes=5, names=['','','','',''], axes=None):
     if axes is None:
-        fig, axes = plt.subplots(1, 5, figsize=(20, 4))
+        fig, axes = plt.subplots(1, n_classes, figsize=(20, 4))
 
     class_to_id_gaia = lambda x: data.query('type=="HMXB"').loc[classes==x].id_gaia
 
     category_counts_all = Counter()
     for i in range(n_classes):
         id_gaia = class_to_id_gaia(i)
         hmxb_classes = ','.join(map(str, list(hmxb.query("id_gaia in @id_gaia").Xray_Type.values))).split(',')
@@ -588,23 +532,24 @@
         values = [category_counts.get(cat, 0) for cat in sorted_categories]
 
         ax.bar(sorted_categories, values, bottom=bottom, color=color[i])
         ax.set_title(f'Class {i}')
         ax.set_xlabel('HMXB Type')
         ax.set_ylabel('Count')
         ax.set_xticklabels(list(sorted_categories), rotation=90)
+        print(i)
         ax.set_title(names[i])
 
 
 def calc_centers(classes, compressed, data):
     coords = compressed[data['type']=='HMXB']
     centers = {}
     for class_ in set(classes):
         centers[class_] = np.mean(coords[classes==class_], axis=0)
     return centers
 
 def plot_centers(centers, ax=None, name=''):
     if ax is None:
         fig, ax = plt.subplots()
     for i in centers:
-        ax.scatter(centers[i][0], centers[i][1], color='black', s=30)
+        ax.scatter(centers[i][0], centers[i][1], color='black', s=150)
     ax.set_title(name)
```

### Comparing `cosmatch-0.1.3/cosmatch/settings.py` & `cosmatch-0.1.4/cosmatch/settings.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/cosmatch/transforms.py` & `cosmatch-0.1.4/cosmatch/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,18 @@
     def about(self) -> str:
         """
         Return a string that describes the transformation of the columns in the DataFrame.
 
         Returns:
             str: A string containing the required columns and the resulting columns after the transformation.
         """
+        needed_columns = '\n'.join(list(self.get_columns().keys()))
+        print(needed_columns)
         s = f"""Преобразование требует следующих колонок:
-            {self.get_columns()}
+            {needed_columns}
             В результате получатся такие колонки:
             {self.out_columns}"""
         return s
 
 
 class MultiTransform:
     """Класс для применения сразу нескольких преобразований."""
@@ -177,31 +179,31 @@
         columns = {}
         for transform in self.transforms:
             columns.update(transform.get_columns())
         return columns
 
     def about(self) -> str:
         """Описывает, какие колонки нужны будут для проведения преобразования и какие колонки получатся."""
-        s = f"""Преобразование требует следующих колонок:
-            {self.get_columns()}
+        needed_columns = '\n\t'+'\n\t'.join(f"{key}: {val}" for key, val in self.get_columns().items())
+        s = f"""Преобразование требует следующих колонок:{needed_columns}
             В результате Получатся такие колонки:
             {self.out_columns}"""
         return s
 
 
 class CoordinatesGalacticTransform(Transform):
     """Преобразует координаты, переводя их из экваториальных в галактические."""
 
     def __init__(self, 
                  coords_equatorial: tuple[str, str],
                  add_b_deg: bool = True, add_l_deg: bool = True,) -> None:
         """Init."""
         self.coords = coords_equatorial
         self.in_columns = {self.coords[0]: 'Ra degree of object',
-                           self.coords[0]: 'Dec degree of object'}
+                           self.coords[1]: 'Dec degree of object'}
         self.add_b_deg = add_b_deg
         self.add_l_deg = add_l_deg
         self.out_columns = []
 
         if self.add_b_deg:
             self.out_columns.append('b_deg')
         if self.add_l_deg:
@@ -460,14 +462,15 @@
             CoordinatesGalacticTransform(coords_equatorial=coorinates_equatorial,
                                            add_b_deg=add_b_deg, add_l_deg=add_l_deg),
             OtherAstrometryTransform(add_r98=add_r98, add_distance_in_error=add_distance_in_error),
             NeighboursTransform(to_r98=add_neighbours_to_r98, to_distance=add_neighbours_to_distance),
         ]
         if add_astro_factor:
             self.transforms.append(AstroFactorTransform(frequency_between=add_astro_factor_frequency_between))
+        self.out_columns = []
 
 
 class IgnoreTransform(Transform):
     """Класс для удаления заданных полей данных."""
 
     def __init__(self, ignored_features: list[str] = []) -> None:
         """
@@ -686,7 +689,25 @@
                                               add_astro_factor_frequency_between=(self.max_distance, 
                                                                                   max(self.max_distance-5, self.max_distance/2),)),
                       FluxesTransform(list(zip(self.fluxes, self.fluxes_err)), column_prefix='mag'),
                       ColorTransform(magnitudes=self.mag)]
         if self.ignore_fluxes:
             transforms += [IgnoreTransform(self.fluxes + self.fluxes_err)]
         return MultiTransform(transforms)
+    
+
+class AttrsAutoTransform:
+    """Auto transform with information from attrs."""
+    def __init__(self, max_distance: int) -> None:
+        self.max_distance = max_distance
+
+    def get_transforms(self, df: pd.DataFrame) -> MultiTransform:
+        distances = np.array([5, 10, 15, 20, 30])
+        distances = list(distances[distances <= self.max_distance])
+        distances.append(self.max_distance)
+        distances = list(set(distances))
+        transforms = [FullAstrometryTransform(coorinates_equatorial=(df.attrs['ra_frame'], df.attrs['dec_frame']),
+                 add_b_deg=True, add_l_deg=True, add_distance_in_error=True, add_r98=True,
+                 add_neighbours_to_r98=True, add_neighbours_to_distance=distances, add_astro_factor=True, 
+                 add_astro_factor_frequency_between=(self.max_distance, max(self.max_distance-5, self.max_distance/2))),
+                 ]
+        return MultiTransform(transforms)
```

### Comparing `cosmatch-0.1.3/cosmatch/utils/astrometry.py` & `cosmatch-0.1.4/cosmatch/utils/astrometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
     if frame_cord is None:
         frame_cord = [frame.attrs['ra'], frame.attrs['dec']] # type: ignore
     if target_cord is None:
         target_cord = [target.attrs['ra'], target.attrs['dec']] # type: ignore
 
     if lsuffix is None:
-        if frame.attrs['name']:
+        if 'name' in frame.attrs:
             lsuffix = '_' + frame.attrs['name']
         else:
             lsuffix = '_frame'
     if rsuffix is None:
-        if target.attrs['name']:
+        if 'name' in target.attrs:
             rsuffix = '_' + target.attrs['name']
         else:
             rsuffix = '_target'
 
     c1 = SkyCoord(ra=frame[frame_cord[0]].values * degree, # type: ignore
                   dec=frame[frame_cord[1]].values * degree) # type: ignore
     c2 = SkyCoord(ra=target[target_cord[0]].values * degree, # type: ignore
```

### Comparing `cosmatch-0.1.3/cosmatch/utils/columns_handler.py` & `cosmatch-0.1.4/cosmatch/utils/columns_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 import pandas as pd
 
 from typing import List, Union
 
 
+def merge_save_attrs(data, *args, **kwargs):
+    attrs = data.attrs
+    data = pd.merge(data, *args, **kwargs)
+    data.attrs = attrs
+    return data
+
+def add_postfix_to_columns(df: pd.DataFrame, postfix: Union[str, None], columns: List[str], add_to_attrs: bool = False) -> None:
+    for col in columns:
+        if postfix:
+            df.rename(columns={col: col + '_' + postfix}, inplace=True)
+            if add_to_attrs:
+                df.attrs[col] =  col + '_' + postfix
+        else:
+            if add_to_attrs:
+                df.attrs[col] = col
+
 def add_postfix_to_main_columns(df: pd.DataFrame, postfix: Union[str, None], add_to_attrs: bool = True) -> None:
     """
     Добавляет к имени колонок id, ra, dec постфикс postfix. Также позволяет добавить атрибуты ['name', 'id', 'ra', 'dec'].
     
     Args:
         df: DataFrame, к которому добавляются постфиксы. Columns = ['id', 'ra', 'dec']
         postfix: Постфикс для добавляемых колонок. Может быть None,\
@@ -35,28 +51,45 @@
         ...                       'dec': [1, 2, 3, 4, 5]})
         >>> add_postfix_to_main_columns(frame, postfix=None, add_to_attrs=True)
         >>> frame.columns
         Index(['id', 'ra', 'dec'], dtype='object')
         >>> frame.attrs
         {'name': '', 'id': 'id', 'ra': 'ra', 'dec': 'dec'} 
     """
-    if postfix:
-        df.rename(columns={'id': f'id_{postfix}', 'ra': f'ra_{postfix}',
-                        'dec': f'dec_{postfix}'}, inplace=True)
-        if add_to_attrs:
-            df.attrs['name'] = postfix
-            df.attrs['id'] = f'id_{postfix}'
-            df.attrs['ra'] = f'ra_{postfix}'
-            df.attrs['dec'] = f'dec_{postfix}'
-    else:
-        if add_to_attrs:
-            df.attrs['name'] = ''
-            df.attrs['id'] = 'id'
-            df.attrs['ra'] = 'ra'
-            df.attrs['dec'] = 'dec'
+    add_postfix_to_columns(df, postfix, ['id', 'ra', 'dec'], add_to_attrs)
+    if add_to_attrs:
+        df.attrs['name'] = '' if not postfix else postfix
+
+def add_postfix_to_all_columns_except(df: pd.DataFrame, postfix: Union[str, None], except_columns: List[str]) -> None:
+    for col in df.columns:
+        if col not in except_columns:
+            df.rename(columns={col: col + '_' + postfix}, inplace=True)
+    
+    for attr in ['id', 'ra', 'dec', 'poserr']:
+        if df.attrs[attr] not in except_columns:
+            df.attrs[attr] = df.attrs[attr] + '_' + postfix
+    
+    for attr in ['mags']:
+        new_objs = []
+        for obj in df.attrs[attr]:
+            if obj not in except_columns:
+                new_objs.append(obj + '_' + postfix)
+            else:
+                new_objs.append(obj)
+        df.attrs[attr] = new_objs
+
+def add_magnitudes_to_attrs(df: pd.DataFrame, mags: List[str], postfix: Union[str, None]) -> None:
+    #if postfix:
+    #    df.rename(columns={mag: mag + '_' + postfix for mag in mags}, inplace=True)
+    #    mags = [mag + '_' + postfix for mag in mags]
+    df.attrs['mags'] = mags
+
+
+def check_available_attrs(df: pd.DataFrame) -> List[str]:
+    return NotImplemented
 
 def unite_attrs_from_frame_and_target(df: pd.DataFrame, frame: pd.DataFrame, target: pd.DataFrame) -> None:
     check_attrs_structure(frame, ['name', 'id', 'ra', 'dec'])
     check_attrs_structure(target, ['name', 'id', 'ra', 'dec'])
     df.attrs['ids'] = [frame.attrs['id'], target.attrs['id']]
     df.attrs['coords'] = [frame.attrs['ra'], frame.attrs['dec'], target.attrs['ra'], target.attrs['dec']]
 
@@ -76,14 +109,25 @@
         if key not in df.attrs:
             raise ValueError(f'{key} not in attrs. To use correlation module you should add {key} in attrs.')
         
 def get_attrs_columns(df: pd.DataFrame, keys: list[str]=['id', 'ra', 'dec']) -> list[str]:
     """Возвращает список атрибутов в df."""
     return [df.attrs[key] for key in keys]
 
+def move_columns_ahead(df: pd.DataFrame, columns: List[str]) -> None:
+    """Перемещает колонки в начало датафрейма."""
+    first_columns = columns
+    other_columns = list(set(df.columns) - set(first_columns))
+    df = df[first_columns + other_columns]
+    return df
+
+def move_main_columns_ahead(df: pd.DataFrame, additional_columns: List[str] = []) -> None:
+    """Перемещает основные колонки в начало датафрейма."""
+    first_columns = [df.attrs['id'], df.attrs['ra'], df.attrs['dec']] + additional_columns
+    return move_columns_ahead(df, first_columns)
 
 # Legacy
 def find_all_id_cols(df: pd.DataFrame) -> List[str]:
     """Возвращает все колонки, которые начинаются на id."""
     return list(filter(lambda x: 'id_' in x, df.columns))
 
 # Legacy
```

### Comparing `cosmatch-0.1.3/cosmatch/utils/io.py` & `cosmatch-0.1.4/cosmatch/utils/io.py`

 * *Files identical despite different names*

### Comparing `cosmatch-0.1.3/pyproject.toml` & `cosmatch-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cosmatch"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Sbdjaro <kir.tearo@yandex.ru>"]
 readme = "Readme.md"
 packages = [{ include = "cosmatch", from = "." },]
 
 
 [tool.poetry.dependencies]
```

### Comparing `cosmatch-0.1.3/PKG-INFO` & `cosmatch-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmatch
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Sbdjaro
 Author-email: kir.tearo@yandex.ru
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

