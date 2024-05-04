# Comparing `tmp/pt_pump_up-0.0.8.tar.gz` & `tmp/pt_pump_up-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_pump_up-0.0.8.tar", last modified: Wed Mar 20 12:24:53 2024, max compression
+gzip compressed data, was "pt_pump_up-0.0.9.tar", last modified: Wed Mar 20 15:26:44 2024, max compression
```

## Comparing `pt_pump_up-0.0.8.tar` & `pt_pump_up-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 12:24:53.139766 pt_pump_up-0.0.8/
--rw-rw-rw-   0        0        0      643 2024-03-20 12:24:53.132509 pt_pump_up-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-09 12:28:59.000000 pt_pump_up-0.0.8/README.md
--rw-rw-rw-   0        0        0      899 2024-03-20 12:24:33.000000 pt_pump_up-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-20 12:24:53.142758 pt_pump_up-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-20 12:24:52.751944 pt_pump_up-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-20 12:24:52.878944 pt_pump_up-0.0.8/src/pt_pump_up/
--rw-rw-rw-   0        0        0     3500 2024-03-13 15:20:03.000000 pt_pump_up-0.0.8/src/pt_pump_up/PT_Pump_Up.py
--rw-rw-rw-   0        0        0       40 2024-03-09 12:46:21.000000 pt_pump_up-0.0.8/src/pt_pump_up/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 12:24:53.023763 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/
--rw-rw-rw-   0        0        0     2792 2024-03-20 11:55:51.000000 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/TrainerFactory.py
--rw-rw-rw-   0        0        0       44 2024-03-20 11:56:00.000000 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 12:24:53.085498 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/
--rw-rw-rw-   0        0        0      941 2024-03-20 12:23:29.000000 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/TextClassificationStrategy.py
--rw-rw-rw-   0        0        0     3091 2024-03-20 12:23:33.000000 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/TokenClassificationStrategy.py
--rw-rw-rw-   0        0        0     1557 2024-03-20 11:41:36.000000 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/TrainingStrategy.py
--rw-rw-rw-   0        0        0      184 2024-03-20 10:41:39.000000 pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/__init__.py
--rw-rw-rw-   0        0        0      880 2024-03-13 17:06:15.000000 pt_pump_up-0.0.8/src/pt_pump_up/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-20 12:24:53.113458 pt_pump_up-0.0.8/src/pt_pump_up.egg-info/
--rw-rw-rw-   0        0        0      643 2024-03-20 12:24:52.000000 pt_pump_up-0.0.8/src/pt_pump_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      689 2024-03-20 12:24:52.000000 pt_pump_up-0.0.8/src/pt_pump_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 12:24:52.000000 pt_pump_up-0.0.8/src/pt_pump_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-03-20 12:24:52.000000 pt_pump_up-0.0.8/src/pt_pump_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-20 12:24:52.000000 pt_pump_up-0.0.8/src/pt_pump_up.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-20 12:24:53.088543 pt_pump_up-0.0.8/tests/
--rw-rw-rw-   0        0        0     1357 2024-03-13 16:54:00.000000 pt_pump_up-0.0.8/tests/test_pt_pump_up.py
+drwxrwxrwx   0        0        0        0 2024-03-20 15:26:44.757686 pt_pump_up-0.0.9/
+-rw-rw-rw-   0        0        0      643 2024-03-20 15:26:44.754260 pt_pump_up-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-09 12:28:59.000000 pt_pump_up-0.0.9/README.md
+-rw-rw-rw-   0        0        0      899 2024-03-20 15:26:36.000000 pt_pump_up-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-20 15:26:44.758657 pt_pump_up-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-20 15:26:44.569888 pt_pump_up-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-03-20 15:26:44.607868 pt_pump_up-0.0.9/src/pt_pump_up/
+-rw-rw-rw-   0        0        0     3500 2024-03-13 15:20:03.000000 pt_pump_up-0.0.9/src/pt_pump_up/PT_Pump_Up.py
+-rw-rw-rw-   0        0        0       40 2024-03-09 12:46:21.000000 pt_pump_up-0.0.9/src/pt_pump_up/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-20 15:26:44.686935 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/
+-rw-rw-rw-   0        0        0     2995 2024-03-20 15:24:07.000000 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/TrainerFactory.py
+-rw-rw-rw-   0        0        0       44 2024-03-20 11:56:00.000000 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-20 15:26:44.723959 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/
+-rw-rw-rw-   0        0        0      979 2024-03-20 15:19:17.000000 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/TextClassificationStrategy.py
+-rw-rw-rw-   0        0        0     3076 2024-03-20 15:18:53.000000 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/TokenClassificationStrategy.py
+-rw-rw-rw-   0        0        0     2254 2024-03-20 15:18:44.000000 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/TrainingStrategy.py
+-rw-rw-rw-   0        0        0      184 2024-03-20 10:41:39.000000 pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/__init__.py
+-rw-rw-rw-   0        0        0      880 2024-03-13 17:06:15.000000 pt_pump_up-0.0.9/src/pt_pump_up/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-20 15:26:44.744355 pt_pump_up-0.0.9/src/pt_pump_up.egg-info/
+-rw-rw-rw-   0        0        0      643 2024-03-20 15:26:44.000000 pt_pump_up-0.0.9/src/pt_pump_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2024-03-20 15:26:44.000000 pt_pump_up-0.0.9/src/pt_pump_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-20 15:26:44.000000 pt_pump_up-0.0.9/src/pt_pump_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-03-20 15:26:44.000000 pt_pump_up-0.0.9/src/pt_pump_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-20 15:26:44.000000 pt_pump_up-0.0.9/src/pt_pump_up.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-20 15:26:44.737116 pt_pump_up-0.0.9/tests/
+-rw-rw-rw-   0        0        0     1357 2024-03-13 16:54:00.000000 pt_pump_up-0.0.9/tests/test_pt_pump_up.py
```

### Comparing `pt_pump_up-0.0.8/PKG-INFO` & `pt_pump_up-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt_pump_up
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hub for Portuguese NLP resources
 Author-email: Rúben Almeida <ruben.f.almeida@inesctec.pt>, Alípio Jorge <alipio.jorge@inesctec.pt>, Ricardo Campos <ricardo.campos@inesctec.pt>, Sérgio Nunes <sergio.nunes@inesctec.pt>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: datasets>=2.17.1
 Requires-Dist: pytest>=8.0.2
 Requires-Dist: transformers>=4.38.2
```

### Comparing `pt_pump_up-0.0.8/pyproject.toml` & `pt_pump_up-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pt_pump_up"
-version = "0.0.8"
+version = "0.0.9"
 description = "Hub for Portuguese NLP resources"
 readme = "README.md"
 authors = [
     {name = "Rúben Almeida", email = "ruben.f.almeida@inesctec.pt"},
     {name = "Alípio Jorge", email = "alipio.jorge@inesctec.pt"},
     {name = "Ricardo Campos", email = "ricardo.campos@inesctec.pt"},
     {name = "Sérgio Nunes", email = "sergio.nunes@inesctec.pt"},
```

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up/PT_Pump_Up.py` & `pt_pump_up-0.0.9/src/pt_pump_up/PT_Pump_Up.py`

 * *Files identical despite different names*

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/TrainerFactory.py` & `pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/TrainerFactory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
-from transformers import Trainer
-from transformers import TrainingArguments
+from transformers import Trainer, TrainingArguments, EarlyStoppingCallback
 from pt_pump_up import PTPumpUpClient
 from pt_pump_up.benchmarking.training_strategies import TokenClassificationStrategy, TextClassificationStrategy
 
 
 class TrainerFactory:
     @staticmethod
-    def create(nlp_task: str, repository_name: str, model_name: str, lr: float, batch_size: int, max_epochs: int, train_dataset, eval_dataset=None):
+    def create(nlp_task: str, repository_name: str, model_name: str, lr: float, max_epochs: int, train_dataset, eval_dataset=None):
         strategy = None
         nlp_tasks = PTPumpUpClient().all_nlp_tasks()
 
         nlp_task = nlp_tasks[nlp_tasks['short_name'] == nlp_task].to_dict('records')[
             0]
 
         if nlp_task is None:
             raise Exception("NLP Task not found")
 
         if nlp_task['standard_format'] == 'Token Classification':
             strategy = TokenClassificationStrategy(
                 model_name, nlp_task['short_name'].lower(), train_dataset.features[f"{nlp_task['short_name'].lower()}_tags"].feature.names)
 
         elif nlp_task['standard_format'] == 'Text Classification':
-            strategy = TextClassificationStrategy()
+            strategy = TextClassificationStrategy(
+                model_name, train_dataset.features['label'].feature.names)
 
         elif nlp_task['standard_format'] == 'Question Answering':
             raise Exception("Not implemented")
         elif nlp_task['standard_format'] == 'Summarization':
             raise Exception("Not implemented")
         elif nlp_task['standard_format'] == 'Translation':
             raise Exception("Not implemented")
@@ -38,19 +38,21 @@
             raise Exception("Strategy not found for NLP Task")
 
         args = TrainingArguments(
             output_dir=os.path.join(os.getcwd(), 'output'),
             evaluation_strategy="epoch",
             learning_rate=lr,
             save_strategy="epoch",
-            per_device_train_batch_size=batch_size,
-            per_device_eval_batch_size=batch_size,
+            auto_find_batch_size=True,
             num_train_epochs=max_epochs,
             load_best_model_at_end=True,
+            metric_for_best_model=strategy.metric_for_best_model,
             hub_model_id=repository_name,
+            label_names=strategy.label_names,
+            bf16=True,
             push_to_hub=True,
         )
 
         # PreProcessing Data
         train_dataset = train_dataset.map(strategy.prepare_data, batched=True)
         eval_dataset = eval_dataset.map(
             strategy.prepare_data, batched=True) if eval_dataset else None
@@ -60,8 +62,9 @@
             model=strategy.model,
             args=args,
             compute_metrics=strategy.compute_metrics,
             train_dataset=train_dataset,
             eval_dataset=eval_dataset,
             data_collator=strategy.collator,
             tokenizer=strategy.tokenizer,
+            callbacks=[EarlyStoppingCallback(early_stopping_patience=3)]
         )
```

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/TextClassificationStrategy.py` & `pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/TextClassificationStrategy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import evaluate
 from pt_pump_up.benchmarking.training_strategies import TrainingStrategy
 from transformers import AutoModelForSequenceClassification, DataCollatorWithPadding
 import numpy as np
 
 
 class TextClassificationStrategy(TrainingStrategy):
-    def __init__(self, model_name) -> None:
-        super().__init__(model_name)
+    def __init__(self, model_name, label_names) -> None:
+        super().__init__(model_name, label_names, "accuracy")
         self.model = AutoModelForSequenceClassification.from_pretrained(
             model_name)
         self.collator = DataCollatorWithPadding(tokenizer=self.tokenizer)
         self.metric = evaluate.load("accuracy")
 
     def prepare_data(self, examples):
         return self.tokenizer(examples["text"], truncation=True, max_length=self.model.config.max_position_embeddings)
```

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/TokenClassificationStrategy.py` & `pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/TokenClassificationStrategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import evaluate
 from transformers import DataCollatorForTokenClassification, AutoModelForTokenClassification
 from pt_pump_up.benchmarking.training_strategies import TrainingStrategy
 import numpy as np
 
 
 class TokenClassificationStrategy(TrainingStrategy):
-    def __init__(self, model_name, task, label_list, label_all_tokens: bool = False) -> None:
-        super().__init__(model_name)
+    def __init__(self, model_name, task, label_names, label_all_tokens: bool = False) -> None:
+        super().__init__(model_name, label_names, "f1")
 
         self.model = AutoModelForTokenClassification.from_pretrained(
-            model_name, num_labels=len(label_list))
+            model_name, num_labels=len(label_names))
 
         self.collator = DataCollatorForTokenClassification(
             tokenizer=self.tokenizer)
         self.metric = evaluate.load("seqeval")
         self.task = task
         self.label_all_tokens = label_all_tokens
-        self.label_list = label_list
 
     def prepare_data(self, examples):
         tokenized_inputs = self.tokenizer(
             examples["tokens"], truncation=True, is_split_into_words=True, max_length=self.model.config.max_position_embeddings)
 
         labels = []
         for i, label in enumerate(examples[f"{self.task}_tags"]):
@@ -50,20 +49,20 @@
 
     def compute_metrics(self, eval_pred):
         predictions, labels = eval_pred
         predictions = np.argmax(predictions, axis=2)
 
         # Remove ignored index (special tokens)
         true_predictions = [
-            [self.label_list[p]
+            [self.label_names[p]
                 for (p, l) in zip(prediction, label) if l != -100]
             for prediction, label in zip(predictions, labels)
         ]
         true_labels = [
-            [self.label_list[l]
+            [self.label_names[l]
                 for (p, l) in zip(prediction, label) if l != -100]
             for prediction, label in zip(predictions, labels)
         ]
 
         results = self.metric.compute(
             predictions=true_predictions, references=true_labels)
         return {
```

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up/benchmarking/training_strategies/TrainingStrategy.py` & `pt_pump_up-0.0.9/src/pt_pump_up/benchmarking/training_strategies/TrainingStrategy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from abc import ABC, abstractmethod
 from transformers import AutoTokenizer
 
 
 class TrainingStrategy(ABC):
-    def __init__(self, model_name) -> None:
+    def __init__(self, model_name, label_names, metric_for_best_model) -> None:
         self._model_name = model_name
         self._collator = None
         self._metric = None
         self._model = None
         self._tokenizer = AutoTokenizer.from_pretrained(model_name)
+        self._label_names = label_names
+        self._metric_for_best_model = metric_for_best_model
 
     @abstractmethod
     def prepare_data(self, examples):
         raise NotImplementedError
 
     @abstractmethod
     def compute_metrics(self, eval_pred):
@@ -58,7 +60,26 @@
             raise Exception("Model not set")
 
         return self._model
 
     @model.setter
     def model(self, model):
         self._model = model
+
+    @property
+    def label_names(self):
+        return self._label_names
+
+    @label_names.setter
+    def label_names(self, label_names):
+        self._label_names = label_names
+
+    @property
+    def metric_for_best_model(self):
+        if self._metric_for_best_model is None:
+            raise Exception("Metric for best model not set")
+
+        return self._metric_for_best_model
+
+    @metric_for_best_model.setter
+    def metric_for_best_model(self, metric_for_best_model):
+        self._metric_for_best_model = metric_for_best_model
```

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up/utils.py` & `pt_pump_up-0.0.9/src/pt_pump_up/utils.py`

 * *Files identical despite different names*

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up.egg-info/PKG-INFO` & `pt_pump_up-0.0.9/src/pt_pump_up.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt_pump_up
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hub for Portuguese NLP resources
 Author-email: Rúben Almeida <ruben.f.almeida@inesctec.pt>, Alípio Jorge <alipio.jorge@inesctec.pt>, Ricardo Campos <ricardo.campos@inesctec.pt>, Sérgio Nunes <sergio.nunes@inesctec.pt>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: datasets>=2.17.1
 Requires-Dist: pytest>=8.0.2
 Requires-Dist: transformers>=4.38.2
```

### Comparing `pt_pump_up-0.0.8/src/pt_pump_up.egg-info/SOURCES.txt` & `pt_pump_up-0.0.9/src/pt_pump_up.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pt_pump_up-0.0.8/tests/test_pt_pump_up.py` & `pt_pump_up-0.0.9/tests/test_pt_pump_up.py`

 * *Files identical despite different names*

