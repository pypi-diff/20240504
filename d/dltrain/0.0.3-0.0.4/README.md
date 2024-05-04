# Comparing `tmp/dltrain-0.0.3.tar.gz` & `tmp/dltrain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltrain-0.0.3.tar", last modified: Sun Apr  7 12:27:38 2024, max compression
+gzip compressed data, was "dltrain-0.0.4.tar", last modified: Sat May  4 14:02:03 2024, max compression
```

## Comparing `dltrain-0.0.3.tar` & `dltrain-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 12:27:38.743213 dltrain-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      813 2024-04-07 12:27:38.742213 dltrain-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-04-07 12:04:01.000000 dltrain-0.0.3/README.md
--rw-rw-rw-   0        0        0      625 2024-04-07 12:26:50.000000 dltrain-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 12:27:38.743213 dltrain-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-07 12:27:38.697214 dltrain-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 12:27:38.720212 dltrain-0.0.3/src/dltrain/
--rw-rw-rw-   0        0        0      219 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:27:38.740212 dltrain-0.0.3/src/dltrain/builder/
--rw-rw-rw-   0        0        0      132 2024-04-05 16:31:47.000000 dltrain-0.0.3/src/dltrain/builder/__init__.py
--rw-rw-rw-   0        0        0     5588 2024-04-07 10:16:53.000000 dltrain-0.0.3/src/dltrain/builder/builder.py
--rw-rw-rw-   0        0        0      878 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/builder/optimizer.py
--rw-rw-rw-   0        0        0      764 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/builder/scheduler.py
--rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/checkpoint.py
--rw-rw-rw-   0        0        0     5167 2024-04-07 11:47:19.000000 dltrain-0.0.3/src/dltrain/dataset.py
--rw-rw-rw-   0        0        0     1235 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/delineator.py
--rw-rw-rw-   0        0        0      933 2024-04-05 11:07:29.000000 dltrain-0.0.3/src/dltrain/error.py
--rw-rw-rw-   0        0        0     2136 2024-04-07 12:00:12.000000 dltrain-0.0.3/src/dltrain/evaluation.py
--rw-rw-rw-   0        0        0     1738 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/forward.py
--rw-rw-rw-   0        0        0     4489 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/models.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/options.py
--rw-rw-rw-   0        0        0    10040 2024-04-07 12:21:06.000000 dltrain-0.0.3/src/dltrain/train.py
--rw-rw-rw-   0        0        0     1145 2024-04-07 09:09:29.000000 dltrain-0.0.3/src/dltrain/transform.py
--rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.0.3/src/dltrain/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:27:38.741222 dltrain-0.0.3/src/dltrain.egg-info/
--rw-rw-rw-   0        0        0      813 2024-04-07 12:27:38.000000 dltrain-0.0.3/src/dltrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2024-04-07 12:27:38.000000 dltrain-0.0.3/src/dltrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 12:27:38.000000 dltrain-0.0.3/src/dltrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 12:27:38.000000 dltrain-0.0.3/src/dltrain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.826791 dltrain-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      813 2024-05-04 14:02:03.825799 dltrain-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-04-07 12:04:01.000000 dltrain-0.0.4/README.md
+-rw-rw-rw-   0        0        0      625 2024-04-08 10:01:12.000000 dltrain-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 14:02:03.826791 dltrain-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.783791 dltrain-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.801791 dltrain-0.0.4/src/dltrain/
+-rw-rw-rw-   0        0        0      219 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.823792 dltrain-0.0.4/src/dltrain/builder/
+-rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.0.4/src/dltrain/builder/__init__.py
+-rw-rw-rw-   0        0        0     1132 2024-05-04 11:16:47.000000 dltrain-0.0.4/src/dltrain/builder/base.py
+-rw-rw-rw-   0        0        0     3623 2024-05-04 13:52:21.000000 dltrain-0.0.4/src/dltrain/builder/builder.py
+-rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.0.4/src/dltrain/builder/core.py
+-rw-rw-rw-   0        0        0      613 2024-05-04 13:43:22.000000 dltrain-0.0.4/src/dltrain/builder/criterion.py
+-rw-rw-rw-   0        0        0     1377 2024-05-04 13:34:54.000000 dltrain-0.0.4/src/dltrain/builder/evaluation_handler.py
+-rw-rw-rw-   0        0        0      631 2024-05-04 13:34:54.000000 dltrain-0.0.4/src/dltrain/builder/model.py
+-rw-rw-rw-   0        0        0     1143 2024-05-04 13:53:40.000000 dltrain-0.0.4/src/dltrain/builder/optimizer.py
+-rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.0.4/src/dltrain/builder/scheduler.py
+-rw-rw-rw-   0        0        0      718 2024-05-04 13:34:54.000000 dltrain-0.0.4/src/dltrain/builder/transforms.py
+-rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/checkpoint.py
+-rw-rw-rw-   0        0        0     6069 2024-04-08 10:00:24.000000 dltrain-0.0.4/src/dltrain/dataset.py
+-rw-rw-rw-   0        0        0     1235 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/delineator.py
+-rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.0.4/src/dltrain/error.py
+-rw-rw-rw-   0        0        0     2644 2024-05-04 03:27:06.000000 dltrain-0.0.4/src/dltrain/evaluation.py
+-rw-rw-rw-   0        0        0     1738 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/forward.py
+-rw-rw-rw-   0        0        0     4489 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/models.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/options.py
+-rw-rw-rw-   0        0        0    11789 2024-05-04 03:27:06.000000 dltrain-0.0.4/src/dltrain/train.py
+-rw-rw-rw-   0        0        0     1145 2024-04-07 09:09:29.000000 dltrain-0.0.4/src/dltrain/transform.py
+-rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.0.4/src/dltrain/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:02:03.824792 dltrain-0.0.4/src/dltrain.egg-info/
+-rw-rw-rw-   0        0        0      813 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-04 14:02:03.000000 dltrain-0.0.4/src/dltrain.egg-info/top_level.txt
```

### Comparing `dltrain-0.0.3/LICENSE` & `dltrain-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/PKG-INFO` & `dltrain-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dltrain-0.0.3/pyproject.toml` & `dltrain-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dltrain"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="XiaosYu", email="lijingyu_ai@163.com" },
 ]
 description = "This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dltrain-0.0.3/src/dltrain/checkpoint.py` & `dltrain-0.0.4/src/dltrain/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/src/dltrain/dataset.py` & `dltrain-0.0.4/src/dltrain/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,36 @@
+import torch
 from torch.utils.data import Dataset, DataLoader
 from torch import Tensor, cat
 from abc import ABCMeta, abstractmethod
-
 from .error import check_length, try_convert, raise_error
 
+import os
+
 __all__ = [
     'DatasetWizard',
     'DLDataset',
     'VectorCategoricalDataset',
     'VectorRegressionDataset',
     'PyTorchNativeDataset',
     'ImageCategoricalDataset'
 ]
 
 
+def load_images(folder_name):
+    from PIL import Image
+    from torchvision.transforms.functional import to_tensor
+
+    images = []
+    for filename in os.listdir(folder_name):
+        image = Image.open(filename)
+        images.append(to_tensor(image))
+
+    return torch.Tensor(images)
+
 class DatasetWizard:
     @classmethod
     def use_mnist(cls, root, train, download=False):
         from torchvision.datasets import MNIST
         from torchvision.transforms import ToTensor
 
         dataset = MNIST(root, train=train, transform=ToTensor(), download=download)
@@ -164,7 +177,23 @@
         self.targets = targets
 
     def get_length(self):
         return len(self.features)
 
     def index_of(self, idx):
         return self.features[idx], self.targets[idx]
+
+
+class ImageMaskedDataset(DLDataset):
+    def __init__(self, source_image_folder, masked_image_folder):
+        source_images = load_images(source_image_folder)
+        masked_images = load_images(masked_image_folder)
+        self.source_images = source_images
+        self.masked_images = masked_images
+
+        check_length(len(source_images), len(masked_images), 'source images', 'masked images')
+
+    def index_of(self, idx):
+        return self.source_images[idx], self.masked_images[idx]
+
+    def get_length(self):
+        return len(self.source_images)
```

### Comparing `dltrain-0.0.3/src/dltrain/delineator.py` & `dltrain-0.0.4/src/dltrain/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/src/dltrain/error.py` & `dltrain-0.0.4/src/dltrain/error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 def try_convert(variable, convert_function, variable_name, target_type_name):
     try:
         variable = convert_function(variable)
         return variable
     except:
         raise_error(f"convert {variable_name} to {target_type_name}",
-                    f"Could not convert {variable_name} type({type(variable)}) to {target_type_name}")
+                    f"Could not convert {variable_name} type({type(variable)}) to {target_type_name}")
```

### Comparing `dltrain-0.0.3/src/dltrain/evaluation.py` & `dltrain-0.0.4/src/dltrain/evaluation.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,48 +23,65 @@
         self.predictions = prediction if self.predictions is None else torch.cat([self.predictions, prediction], dim=0)
 
     def reset(self):
         self.predictions = None
 
 
 class EvaluationHandler(metaclass=ABCMeta):
+    def __init__(self, drawable=False):
+        self.drawable = drawable
+
+    def __call__(self, *args, **kwargs):
+        return self.compute(*args, **kwargs)
+
     @abstractmethod
     def compute(self, epoch_predictions: Tensor, epoch_exacts: Tensor):
         pass
 
 
 class Accuracy(EvaluationHandler):
+    def __init__(self, drawable=False):
+        super().__init__(drawable)
+
     def compute(self, epoch_predictions, epoch_exacts):
         return int(torch.sum(epoch_predictions.argmax(dim=1) == epoch_exacts).item()) / epoch_exacts.shape[0]
 
 
 class ConfusionMatrix(EvaluationHandler):
-    def __init__(self):
+    def __init__(self, drawable=False):
+        super().__init__(drawable)
         from sklearn.metrics import confusion_matrix
         self.func = confusion_matrix
 
     def compute(self, epoch_predictions, epoch_exacts):
         matrix = self.func(epoch_exacts.cpu().detach().numpy(), epoch_predictions.argmax(dim=1).cpu().detach().numpy())
         return matrix
 
 
 class RootMeanSquareError(EvaluationHandler):
+    def __init__(self, drawable=False):
+        super().__init__(drawable)
+
     def compute(self, epoch_predictions: Tensor, epoch_exacts: Tensor):
         mse = torch.nn.functional.mse_loss(epoch_predictions, epoch_exacts)
         rmse = torch.sqrt(mse)
         return float(rmse)
 
 
 class MeanSquareError(EvaluationHandler):
+    def __init__(self, drawable=False):
+        super().__init__(drawable)
+
     def compute(self, epoch_predictions: Tensor, epoch_exacts: Tensor):
         mse = torch.nn.functional.mse_loss(epoch_predictions, epoch_exacts)
         return float(mse)
 
 
 class RSquare(EvaluationHandler):
-    def __init__(self):
+    def __init__(self, drawable=False):
+        super().__init__(drawable)
         from sklearn.metrics import r2_score
         self.func = r2_score
 
     def compute(self, epoch_predictions: Tensor, epoch_exacts: Tensor):
         r2 = self.func(epoch_exacts.cpu().detach().numpy(), epoch_predictions.cpu().detach().numpy())
         return float(r2)
```

### Comparing `dltrain-0.0.3/src/dltrain/forward.py` & `dltrain-0.0.4/src/dltrain/forward.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/src/dltrain/models.py` & `dltrain-0.0.4/src/dltrain/models.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/src/dltrain/options.py` & `dltrain-0.0.4/src/dltrain/options.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/src/dltrain/train.py` & `dltrain-0.0.4/src/dltrain/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
+
+import numpy as np
 import torch
 import pandas as pd
 
 from .utils import set_plt, LoggerContext
+from .error import try_convert
 
 from torch.utils.data import DataLoader
 
 from abc import ABCMeta, abstractmethod
 from tqdm import tqdm
 
 from .options import TrainOptions
@@ -157,26 +160,26 @@
 
                 if eval_loss < best_eval_loss:
                     torch.save(model.cpu(), f'{options.task_name}/weights/best.pt')
 
                 # 分别计算验证Handler
                 if train_evaluation_handlers is not None:
                     for key, handler in train_evaluation_handlers.items():
-                        val = handler.compute(train_evaluation.predictions, train_evaluation.exacts)
-                        if key in total_train_evaluation:
+                        val = handler(train_evaluation.predictions, train_evaluation.exacts)
+                        if key in total_train_evaluation and val is not None:
                             total_train_evaluation[key].append(val)
-                        else:
+                        elif val is not None:
                             total_train_evaluation[key] = [val]
 
                 if eval_evaluation_handlers is not None:
                     for key, handler in eval_evaluation_handlers.items():
-                        val = handler.compute(eval_evaluation.predictions, eval_evaluation.exacts)
-                        if key in total_eval_evaluation:
+                        val = handler(eval_evaluation.predictions, eval_evaluation.exacts)
+                        if key in total_eval_evaluation and val is not None:
                             total_eval_evaluation[key].append(val)
-                        else:
+                        elif val is not None:
                             total_eval_evaluation[key] = [val]
 
                 train_evaluation.reset()
                 eval_evaluation.reset()
 
                 end_time = datetime.now()
                 # Eval the Epoch Results
@@ -194,15 +197,15 @@
                     for key in eval_evaluation_handlers:
                         logger.info(f'Eval {key}: {total_eval_evaluation[key][-1]}')
 
                 if options.save_checkpoint:
                     # Save checkpoint
                     checkpoint = CheckPoint(
                         epoch,
-                        optimizer.state_dict(),
+                        optimizer.state_dict() if optimizer is not None else None,
                         scheduler.state_dict() if scheduler is not None else None,
                         total_train_loss,
                         total_eval_loss,
                         total_train_evaluation,
                         total_eval_evaluation,
                         options,
                         best_eval_loss
@@ -225,14 +228,48 @@
         loss_frame = pd.DataFrame({
             'Train Loss': total_train_loss,
             'Eval Loss': total_eval_loss
         })
         loss_frame.index.name = 'Epoch'
         loss_frame.to_csv(f'{options.task_name}/loss_result.csv', encoding='utf-8')
 
+        # 映射可计算列
+        for key in total_eval_evaluation:
+            data = total_eval_evaluation[key]
+            if isinstance(data, torch.Tensor):
+                total_eval_evaluation[key] = data.cpu().detach()
+
+        for key in total_train_evaluation:
+            data = total_train_evaluation[key]
+            if isinstance(data, torch.Tensor):
+                total_eval_evaluation[key] = data.cpu().detach()
+
+        # 判断验证列是否可绘制
+        for (key, value) in total_train_evaluation.items():
+            drawable = train_evaluation_handlers[key].drawable
+            if drawable:
+                value = try_convert(value, np.array, f'{key} train evaluation', 'numpy.array')
+                if len(value.shape) == 2 or len(value.shape) == 1:
+                    value = value.reshape(-1)
+                    plt.figure(dpi=300)
+                    plt.plot(value, label=key)
+                    plt.legend()
+                    plt.savefig(f'{options.task_name}/{key}-train.png')
+
+        for (key, value) in total_eval_evaluation.items():
+            drawable = eval_evaluation_handlers[key].drawable
+            if drawable:
+                value = try_convert(value, np.array, f'{key} eval evaluation', 'numpy.array')
+                if len(value.shape) == 2 or len(value.shape) == 1:
+                    value = value.reshape(-1)
+                    plt.figure(dpi=300)
+                    plt.plot(value, label=key)
+                    plt.legend()
+                    plt.savefig(f'{options.task_name}/{key}-eval.png')
+
         if train_evaluation_handlers is not None:
             train_evaluation_frame = pd.DataFrame(
                 {
                     **total_train_evaluation
                 }
             )
             train_evaluation_frame.index.name = 'Epoch'
@@ -243,8 +280,8 @@
                 {
                     **total_eval_evaluation
                 }
             )
             eval_evaluation_frame.index.name = 'Epoch'
             eval_evaluation_frame.to_csv(f'{options.task_name}/eval_evaluation_result.csv', encoding='utf-8')
 
-        logger.save(f'{options.task_name}/log.txt')
+        logger.save(f'{options.task_name}/log.txt')
```

### Comparing `dltrain-0.0.3/src/dltrain/transform.py` & `dltrain-0.0.4/src/dltrain/transform.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/src/dltrain/utils.py` & `dltrain-0.0.4/src/dltrain/utils.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.3/src/dltrain.egg-info/PKG-INFO` & `dltrain-0.0.4/src/dltrain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dltrain-0.0.3/src/dltrain.egg-info/SOURCES.txt` & `dltrain-0.0.4/src/dltrain.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -14,10 +14,16 @@
 src/dltrain/transform.py
 src/dltrain/utils.py
 src/dltrain.egg-info/PKG-INFO
 src/dltrain.egg-info/SOURCES.txt
 src/dltrain.egg-info/dependency_links.txt
 src/dltrain.egg-info/top_level.txt
 src/dltrain/builder/__init__.py
+src/dltrain/builder/base.py
 src/dltrain/builder/builder.py
+src/dltrain/builder/core.py
+src/dltrain/builder/criterion.py
+src/dltrain/builder/evaluation_handler.py
+src/dltrain/builder/model.py
 src/dltrain/builder/optimizer.py
-src/dltrain/builder/scheduler.py
+src/dltrain/builder/scheduler.py
+src/dltrain/builder/transforms.py
```

