# Comparing `tmp/exper-0.1.4.tar.gz` & `tmp/exper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exper-0.1.4.tar", last modified: Wed Jan  3 05:36:37 2024, max compression
+gzip compressed data, was "exper-0.2.0.tar", last modified: Sat May  4 18:52:02 2024, max compression
```

## Comparing `exper-0.1.4.tar` & `exper-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 mrzz       (501) staff       (20)        0 2024-01-03 05:36:37.974542 exper-0.1.4/
--rw-r--r--   0 mrzz       (501) staff       (20)       15 2023-11-15 13:22:38.000000 exper-0.1.4/MANIFEST.in
--rw-r--r--   0 mrzz       (501) staff       (20)     1463 2024-01-03 05:36:37.974410 exper-0.1.4/PKG-INFO
--rw-r--r--   0 mrzz       (501) staff       (20)     1261 2024-01-03 05:32:27.000000 exper-0.1.4/README.md
-drwxr-xr-x   0 mrzz       (501) staff       (20)        0 2024-01-03 05:36:37.973462 exper-0.1.4/exper/
--rw-r--r--   0 mrzz       (501) staff       (20)      110 2023-11-15 13:22:38.000000 exper-0.1.4/exper/__init__.py
--rw-r--r--   0 mrzz       (501) staff       (20)     8430 2023-11-15 13:22:38.000000 exper-0.1.4/exper/comms.py
--rw-r--r--   0 mrzz       (501) staff       (20)     7860 2023-11-15 13:22:38.000000 exper-0.1.4/exper/core.py
--rw-r--r--   0 mrzz       (501) staff       (20)     2029 2023-11-15 13:22:38.000000 exper-0.1.4/exper/cuda_utils.py
--rw-r--r--   0 mrzz       (501) staff       (20)     9543 2024-01-03 05:31:36.000000 exper-0.1.4/exper/engine.py
--rw-r--r--   0 mrzz       (501) staff       (20)     1650 2023-11-15 13:22:38.000000 exper-0.1.4/exper/loss_utils.py
--rw-r--r--   0 mrzz       (501) staff       (20)     1044 2023-11-15 13:22:38.000000 exper-0.1.4/exper/pretty.py
-drwxr-xr-x   0 mrzz       (501) staff       (20)        0 2024-01-03 05:36:37.974225 exper-0.1.4/exper.egg-info/
--rw-r--r--   0 mrzz       (501) staff       (20)     1463 2024-01-03 05:36:37.000000 exper-0.1.4/exper.egg-info/PKG-INFO
--rw-r--r--   0 mrzz       (501) staff       (20)      293 2024-01-03 05:36:37.000000 exper-0.1.4/exper.egg-info/SOURCES.txt
--rw-r--r--   0 mrzz       (501) staff       (20)        1 2024-01-03 05:36:37.000000 exper-0.1.4/exper.egg-info/dependency_links.txt
--rw-r--r--   0 mrzz       (501) staff       (20)       22 2024-01-03 05:36:37.000000 exper-0.1.4/exper.egg-info/requires.txt
--rw-r--r--   0 mrzz       (501) staff       (20)        6 2024-01-03 05:36:37.000000 exper-0.1.4/exper.egg-info/top_level.txt
--rw-r--r--   0 mrzz       (501) staff       (20)       38 2024-01-03 05:36:37.974587 exper-0.1.4/setup.cfg
--rw-r--r--   0 mrzz       (501) staff       (20)      524 2024-01-03 05:32:18.000000 exper-0.1.4/setup.py
+drwxr-xr-x   0 mrzz       (501) staff       (20)        0 2024-05-04 18:52:02.296353 exper-0.2.0/
+-rw-r--r--   0 mrzz       (501) staff       (20)       15 2024-05-04 18:18:39.000000 exper-0.2.0/MANIFEST.in
+-rw-r--r--   0 mrzz       (501) staff       (20)     1515 2024-05-04 18:52:02.295605 exper-0.2.0/PKG-INFO
+-rw-r--r--   0 mrzz       (501) staff       (20)     1261 2024-05-04 18:18:39.000000 exper-0.2.0/README.md
+drwxr-xr-x   0 mrzz       (501) staff       (20)        0 2024-05-04 18:52:02.292042 exper-0.2.0/exper/
+-rw-r--r--   0 mrzz       (501) staff       (20)      245 2024-05-04 18:12:58.000000 exper-0.2.0/exper/__init__.py
+-rw-r--r--   0 mrzz       (501) staff       (20)     8630 2024-05-04 18:12:58.000000 exper-0.2.0/exper/comms.py
+-rw-r--r--   0 mrzz       (501) staff       (20)     6156 2024-05-04 18:12:58.000000 exper-0.2.0/exper/core.py
+-rw-r--r--   0 mrzz       (501) staff       (20)     2495 2024-05-04 16:41:41.000000 exper-0.2.0/exper/cuda_utils.py
+-rw-r--r--   0 mrzz       (501) staff       (20)    11431 2024-05-04 18:12:58.000000 exper-0.2.0/exper/engine.py
+-rw-r--r--   0 mrzz       (501) staff       (20)     1640 2024-05-04 14:13:07.000000 exper-0.2.0/exper/loss_utils.py
+-rw-r--r--   0 mrzz       (501) staff       (20)     1109 2024-05-04 18:12:58.000000 exper-0.2.0/exper/pretty.py
+-rw-r--r--   0 mrzz       (501) staff       (20)     1385 2024-05-04 18:12:58.000000 exper-0.2.0/exper/tasks.py
+drwxr-xr-x   0 mrzz       (501) staff       (20)        0 2024-05-04 18:52:02.295128 exper-0.2.0/exper.egg-info/
+-rw-r--r--   0 mrzz       (501) staff       (20)     1515 2024-05-04 18:52:02.000000 exper-0.2.0/exper.egg-info/PKG-INFO
+-rw-r--r--   0 mrzz       (501) staff       (20)      323 2024-05-04 18:52:02.000000 exper-0.2.0/exper.egg-info/SOURCES.txt
+-rw-r--r--   0 mrzz       (501) staff       (20)        1 2024-05-04 18:52:02.000000 exper-0.2.0/exper.egg-info/dependency_links.txt
+-rw-r--r--   0 mrzz       (501) staff       (20)       22 2024-05-04 18:52:02.000000 exper-0.2.0/exper.egg-info/requires.txt
+-rw-r--r--   0 mrzz       (501) staff       (20)        6 2024-05-04 18:52:02.000000 exper-0.2.0/exper.egg-info/top_level.txt
+-rw-r--r--   0 mrzz       (501) staff       (20)      688 2024-05-04 18:28:35.000000 exper-0.2.0/pyproject.toml
+-rw-r--r--   0 mrzz       (501) staff       (20)       38 2024-05-04 18:52:02.296516 exper-0.2.0/setup.cfg
+-rw-r--r--   0 mrzz       (501) staff       (20)      524 2024-05-04 18:28:35.000000 exper-0.2.0/setup.py
```

### Comparing `exper-0.1.4/PKG-INFO` & `exper-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: exper
-Version: 0.1.4
+Version: 0.2.0
 Summary: This is a python package for running deep learning experiments. Users can rapidly run their experiments by importing this module.
 Author: Mrzz
+Requires-Dist: torch
+Requires-Dist: torch_geometric
 
 # exper
 
 `exper` is a very lightweight Python package designed for personal use to speed up the execution of PyTorch-based deep learning experiments. This framework is specifically crafted to support Distributed Data Parallel (DDP) training, mix precision training and provides a convenient mechanism for saving experiment logs.
 
 ## Features:
```

### Comparing `exper-0.1.4/README.md` & `exper-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `exper-0.1.4/exper/comms.py` & `exper-0.2.0/exper/comms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-import os
 import multiprocessing
+import os
 from collections import defaultdict
 
 import torch
 from torch import distributed as dist
+from torch.distributed.distributed_c10d import Work
 
 
 cpu_group = None
 gpu_group = None
 
 
-def get_rank():
+def get_rank() -> int:
     """
     Get the rank of this process in distributed processes.
 
     Return 0 for single process case.
     """
     if dist.is_initialized():
         return dist.get_rank()
     if "RANK" in os.environ:
         return int(os.environ["RANK"])
     return 0
 
 
-def get_world_size():
+def get_world_size() -> int:
     """
     Get the total number of distributed processes.
 
     Return 1 for single process case.
     """
     if dist.is_initialized():
         return dist.get_world_size()
     if "WORLD_SIZE" in os.environ:
         return int(os.environ["WORLD_SIZE"])
     return 1
 
 
-def get_group(device):
+def get_group(device: torch.device):
     """
     Get the process group corresponding to the given device.
 
     Parameters:
         device (torch.device): query device
     """
     group = cpu_group if device.type == "cpu" else gpu_group
     if group is None:
-        raise ValueError("%s group is not initialized. Use comm.init_process_group() to initialize it"
-                         % device.type.upper())
+        raise ValueError(
+            "%s group is not initialized. Use comm.init_process_group() to initialize it"
+            % device.type.upper()
+        )
     return group
 
 
-def init_process_group(backend, init_method=None, **kwargs):
+def init_process_group(backend: str, init_method: str | None, **kwargs) -> None:
     """
     Initialize CPU and/or GPU process groups.
 
     Parameters:
         backend (str): Communication backend. Use ``nccl`` for GPUs and ``gloo`` for CPUs.
         init_method (str, optional): URL specifying how to initialize the process group
     """
@@ -65,32 +68,33 @@
     gpu_group = dist.group.WORLD
     # if backend == "nccl":
     #     cpu_group = dist.new_group(backend="gloo")
     # else:
     cpu_group = gpu_group
 
 
-def get_cpu_count():
+def get_cpu_count() -> int:
     """
     Get the number of CPUs on this node.
     """
     return multiprocessing.cpu_count()
 
 
-def synchronize():
+def synchronize() -> None | Work | bool:
     """
     Synchronize among all distributed processes.
     """
     if get_world_size() > 1:
         dist.barrier()
 
 
-def _recursive_read(obj):
+def _recursive_read(obj) -> tuple[defaultdict, defaultdict]:
     values = defaultdict(list)
     sizes = defaultdict(list)
+
     if isinstance(obj, torch.Tensor):
         values[obj.dtype] += [obj.flatten()]
         sizes[obj.dtype] += [torch.tensor([obj.numel()], device=obj.device)]
     elif isinstance(obj, dict):
         for v in obj.values():
             child_values, child_sizes = _recursive_read(v)
             for k, v in child_values.items():
@@ -133,15 +137,15 @@
             new_v, values = _recursive_write(v, values, sizes)
             new_obj.append(new_v)
     else:
         raise ValueError("Unknown type `%s`" % type(obj))
     return new_obj, values
 
 
-def reduce(obj, op="sum", dst=None):
+def reduce(obj: object, op="sum", dst: int | None = None):
     """
     Reduce any nested container of tensors.
 
     Parameters:
         obj (Object): any container object. Can be nested list, tuple or dict.
         op (str, optional): element-wise reduction operator.
             Available operators are ``sum``, ``mean``, ``min``, ``max``, ``product``.
@@ -240,30 +244,30 @@
     """
     values, sizes = _recursive_read(obj)
     sizes = {k: torch.cat(v) for k, v in sizes.items()}
 
     sizes = stack(sizes)
     cated = {}
     for k, value in values.items():
-        size = sizes[k].t().flatten() # sizes[k]: (num_worker, num_obj)
+        size = sizes[k].t().flatten()  # sizes[k]: (num_worker, num_obj)
         dtype = value[0].dtype
         # NCCL can't solve bool. Cast them to byte
         if dtype == torch.bool:
             dtype = torch.uint8
         s = torch.zeros(size.sum(), dtype=dtype, device=value[0].device)
         obj_id = get_rank()
         world_size = get_world_size()
         offset = size[:obj_id].sum()
         for v in value:
             assert offset + v.numel() <= len(s)
-            s[offset: offset + v.numel()] = v
-            offset += size[obj_id: obj_id + world_size].sum()
+            s[offset : offset + v.numel()] = v
+            offset += size[obj_id : obj_id + world_size].sum()
             obj_id += world_size
         group = get_group(s.device)
         if dst is None:
             dist.all_reduce(s, op=dist.ReduceOp.SUM, group=group)
         else:
             dist.reduce(s, op=dist.ReduceOp.SUM, dst=dst, group=group)
         cated[k] = s.type(value[0].dtype)
     sizes = {k: v.sum(dim=0) for k, v in sizes.items()}
 
-    return _recursive_write(obj, cated, sizes)[0]
+    return _recursive_write(obj, cated, sizes)[0]
```

### Comparing `exper-0.1.4/exper/core.py` & `exper-0.2.0/exper/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-import pprint
 import logging
-import warnings
-import exper.pretty as pretty
+import pprint
+import time
+from abc import ABC, abstractmethod
 from collections import defaultdict
-import torch
+
 import numpy as np
-import time
+import torch
+
+import exper.pretty as pretty
+
 
 logger = logging.getLogger(__name__)
 
 
-class LoggerBase(object):
+class LoggerBase(ABC):
     """
     Base class for loggers.
 
     Any custom logger should be derived from this class.
     """
 
-    def log(self, record, step_id, category="train/batch"):
+    @abstractmethod
+    def log(self, record: dict, step_id: int, category: str = "train/batch") -> None:
         """
         Log a record.
 
         Parameters:
             record (dict): dict of any metric
             step_id (int): index of this log step
             category (str, optional): log category.
                 Available types are ``train/batch``, ``train/epoch``, ``valid/epoch`` and ``test/epoch``.
         """
         raise NotImplementedError
 
-    def log_config(self, config):
+    @abstractmethod
+    def log_config(self, config: dict) -> None:
         """
         Log a hyperparameter config.
 
         Parameters:
             config (dict): hyperparameter config
         """
         raise NotImplementedError
@@ -53,137 +58,93 @@
         format = logging.Formatter("%(asctime)-10s %(message)s", "%H:%M:%S")
         handler = logging.FileHandler("log.txt")
         handler.setFormatter(format)
         logger = logging.getLogger("")
         logger.addHandler(handler)
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.logger = logging.getLogger(__name__)
 
-    def log(self, record, step_id, category="train/batch"):
+    def log(self, record: dict, step_id: int, category: str = "train/batch") -> None:
         if category.endswith("batch"):
             self.logger.warning(pretty.separator)
         elif category.endswith("epoch"):
             self.logger.warning(pretty.line)
         if category == "train/epoch":
             for k in sorted(record.keys()):
                 self.logger.warning("average %s: %g" % (k, record[k]))
         else:
             for k in sorted(record.keys()):
                 self.logger.warning("%s: %g" % (k, record[k]))
 
-    def log_config(self, config):
+    def log_config(self, config: dict) -> None:
         self.logger.warning(pprint.pformat(config))
 
 
-class WandbLogger(LoggingLogger):
-    """
-    Log outputs with `Weights and Biases`_ and track the experiment progress.
-
-    Note this class also output logs with the builtin logging module.
-
-    See `wandb.init`_ for more details.
-
-    .. _Weights and Biases:
-        https://docs.wandb.ai
-
-    .. _wandb.init:
-        https://docs.wandb.ai/ref/python/init
-
-    Parameters:
-        project (str, optional): name of the project
-        name (str, optional): name of this run
-        dir (str, optional): path to store meta data. Default is `./wandb`.
-        kwargs: keyword arguments for `wandb.init`_
-    """
-
-    def __init__(self, project=None, name=None, dir=None, **kwargs):
-        super(WandbLogger, self).__init__()
-        try:
-            import wandb
-        except ModuleNotFoundError:
-            raise ModuleNotFoundError("Wandb is not found. Please install it with `pip install wandb`")
-
-        if wandb.run is not None:
-            warnings.warn(
-                "There is a wandb run already in progress and newly created instances of `WandbLogger` will reuse"
-                " this run. If this is not desired, call `wandb.finish()` or `WandbLogger.finish()` before instantiating `WandbLogger`."
-            )
-            self.run = wandb.run
-        else:
-            self.run = wandb.init(project=project, name=name, dir=dir, **kwargs)
-
-        self.run.define_metric("train/batch/*", step_metric="batch", summary="none")
-        for split in ["train", "valid", "test"]:
-            self.run.define_metric("%s/epoch/*" % split, step_metric="epoch")
-
-    def log(self, record, step_id, category="train/batch"):
-        super(WandbLogger, self).log(record, step_id, category)
-        record = {"%s/%s" % (category, k): v for k, v in record.items()}
-        step_name = category.split("/")[-1]
-        record[step_name] = step_id
-        self.run.log(record)
-
-    def log_config(self, confg_dict):
-        super(WandbLogger, self).log_config(confg_dict)
-        self.run.config.update(confg_dict)
-
-
 class Meter(object):
     """
     Meter for recording metrics and training progress.
 
     Parameters:
-        log_interval (int, optional): log every n updates
-        silent (int, optional): surpress all outputs or not
-        logger (core.LoggerBase, optional): log handler
+        log_interval (int): log every n updates
+        silent (int): surpress all outputs or not
+        logger (core.LoggerBase): log handler
     """
 
-    def __init__(self, log_interval=100, silent=False, logger=None):
+    def __init__(
+        self,
+        logger: LoggerBase,
+        log_interval: int = 100,
+        silent: bool = False,
+    ) -> None:
+        
         self.records = defaultdict(list)
         self.log_interval = log_interval
         self.epoch2batch = [0]
         self.time = [time.time()]
         self.epoch_id = 0
         self.batch_id = 0
         self.silent = silent
         self.logger = logger
 
-    def log(self, record, category="train/batch"):
+    def log(self, record: dict, category: str ="train/batch") -> None:
         """
         Log a record.
 
         Parameters:
             record (dict): dict of any metric
             category (str, optional): log category.
                 Available types are ``train/batch``, ``train/epoch``, ``valid/epoch`` and ``test/epoch``.
         """
         if self.silent:
             return
 
+        step_id: int = -1
+
         if category.endswith("batch"):
             step_id = self.batch_id
         elif category.endswith("epoch"):
             step_id = self.epoch_id
+
         self.logger.log(record, step_id=step_id, category=category)
 
-    def log_config(self, config):
+    def log_config(self, config: dict):
         """
         Log a hyperparameter config.
 
         Parameters:
             config (dict): hyperparameter config
         """
         if self.silent:
             return
 
         self.logger.log_config(config)
 
-    def update(self, record):
+    def update(self, record: dict):
         """
         Update the meter with a record.
 
         Parameters:
             record (dict): dict of any metric
         """
         if self.batch_id % self.log_interval == 0:
@@ -198,33 +159,40 @@
     def step(self):
         """
         Step an epoch for this meter.
 
         Instead of manually invoking :meth:`step()`, it is suggested to use the following line
 
             >>> for epoch in meter(num_epoch):
-            >>>     # do something
+            >>> # do something
         """
         self.epoch_id += 1
         self.epoch2batch.append(self.batch_id)
         self.time.append(time.time())
         index = slice(self.epoch2batch[-2], self.epoch2batch[-1])
         duration = self.time[-1] - self.time[-2]
         speed = (self.epoch2batch[-1] - self.epoch2batch[-2]) / duration
         if self.silent:
             return
 
         logger.warning("duration: %s" % pretty.time(duration))
         logger.warning("speed: %.2f batch / sec" % speed)
 
-        eta = (self.time[-1] - self.time[self.start_epoch]) \
-              / (self.epoch_id - self.start_epoch) * (self.end_epoch - self.epoch_id)
+        eta = (
+            (self.time[-1] - self.time[self.start_epoch])
+            / (self.epoch_id - self.start_epoch)
+            * (self.end_epoch - self.epoch_id)
+        )
+
         logger.warning("ETA: %s" % pretty.time(eta))
         if torch.cuda.is_available():
-            logger.warning("max GPU memory: %.1f MiB" % (torch.cuda.max_memory_allocated() / 1e6))
+            logger.warning(
+                "max GPU memory: %.1f MiB" % (torch.cuda.max_memory_allocated() / 1e6)
+            )
+
             torch.cuda.reset_peak_memory_stats()
 
         record = {}
         for k, v in self.records.items():
             record[k] = np.mean(v[index])
         self.log(record, category="train/epoch")
 
@@ -237,8 +205,7 @@
                 logger.warning(pretty.separator)
                 logger.warning("Epoch %d begin" % epoch)
             yield epoch
             if not self.silent:
                 logger.warning(pretty.separator)
                 logger.warning("Epoch %d end" % epoch)
             self.step()
-
```

### Comparing `exper-0.1.4/exper/engine.py` & `exper-0.2.0/exper/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,29 @@
+import logging
 import os
 import sys
-import logging
+from typing import Any, List
 
 import torch
-from torch import nn
 from torch import distributed as dist
+from torch import nn
 from torch.cuda import amp as amp
-
-from torch.optim.optimizer import Optimizer
 from torch.optim.lr_scheduler import LRScheduler
+from torch.optim.optimizer import Optimizer
 from torch.utils import data as torch_data
 from torch.utils.data import Dataset
+from torch.utils.data.dataloader import DataLoader
+from torch_geometric.data import Dataset as PyGDataset
+from torch_geometric.loader import DataLoader as PyGDataLoader
 
-from torch_geometric.loader import DataLoader
+import exper.comms as comms
 import exper.core as core
 import exper.cuda_utils as utils
-import exper.comms as comms
 import exper.pretty as pretty
-from exper.loss_utils import loss_function_resolver
-
-from typing import (
-    List,
-    Optional,
-    Union,
-)
+from exper.tasks import Task
 
 
 module = sys.modules[__name__]
 logger_outside = logging.getLogger(__name__)
 
 
 class Engine:
@@ -46,158 +42,221 @@
         logger (str or core.LoggerBase, optional): logger type or logger instance.
             Available types are ``logging`` and ``wandb``.
         half_precision(bool, optional): use the half precision mode
 
     """
 
     def __init__(  # noqa
-      self, task: nn.Module,
-      train_set: Dataset,
-      valid_set: Dataset,
-      test_set: Dataset,
-      optimizer: Optimizer,
-      scheduler: LRScheduler = None,
-      gpus: Union[List[int], None] = None,
-      batch_size: int = 1,
-      num_worker: int = 0,
-      log_interval: int = 100,
-      half_precision: bool = False,
-      **kwargs,
+        self,
+        task: Task,
+        train_set: Dataset | PyGDataset,
+        valid_set: Dataset | PyGDataset,
+        test_set: Dataset | PyGDataset,
+        optimizer: Optimizer,
+        scheduler: LRScheduler | None = None,
+        gpus: List[int] | None = None,
+        batch_size: int = 1,
+        num_worker: int = 0,
+        log_interval: int = 100,
+        half_precision: bool = False,
+        *args: Any,
+        **kwargs: Any,
     ):
-
         self.rank = comms.get_rank()
         self.world_size = comms.get_world_size()
         self.gpus = gpus
         self.batch_size = batch_size
         self.num_worker = num_worker
         self.half_precision = half_precision
-        self.follow_batch = kwargs.get("follow_batch", None)
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+        if not hasattr(self, "follow_batch"):
+            self.follow_batch = None
 
         if gpus is None:
             self.device = torch.device("cpu")
         else:
             if len(gpus) != self.world_size:
                 error_msg = "World size is %d but found %d GPUs in the argument"
                 if self.world_size == 1:
-                    error_msg += ". Did you launch with `python -m torch.distributed.launch`?"
+                    error_msg += (
+                        ". Did you launch with `python -m torch.distributed.launch`?"
+                    )
                 raise ValueError(error_msg % (self.world_size, len(gpus)))
             self.device = torch.device(gpus[self.rank % len(gpus)])
 
         if self.world_size > 1 and not dist.is_initialized():
             if self.rank == 0:
                 module.logger_outside.info("Initializing distributed process group")
             backend = "gloo" if gpus is None else "nccl"
             comms.init_process_group(backend, init_method="env://")
 
         if self.world_size > 1:
-            task = nn.SyncBatchNorm.convert_sync_batchnorm(task)
+            task = nn.SyncBatchNorm.convert_sync_batchnorm(task)  # type: ignore
         if self.device.type == "cuda":
             task = task.cuda(self.device)
 
         # `task` is a self-designed model to perform your experiments
-        self.model: nn.Module = task
+        self.model = task
 
         # Here are datasets you will use during the experiments
         self.train_set = train_set
         self.valid_set = valid_set
         self.test_set = test_set
 
+        # determine the dataset type
+        self.dataset_type = train_set.__module__.split(".")[0]
+
         # This is the optimizer and scheduler to help the model optimize and converge
         self.optimizer = optimizer
         self.scheduler = scheduler
 
         if self.half_precision:
             self.scaler = amp.GradScaler(enabled=True)
 
         # Here are functions to record experiments
         self.log = core.LoggingLogger()
-        self.meter = core.Meter(log_interval=log_interval, silent=self.rank > 0, logger=self.log)
-        module.logger_outside.warning("Mix Precision Training Enabled: {}".format(self.half_precision))
+        self.meter = core.Meter(
+            log_interval=log_interval, silent=self.rank > 0, logger=self.log
+        )
+
+        module.logger_outside.warning(
+            "Mix Precision Training Enabled: {}".format(self.half_precision)
+        )
 
-    def train(self, num_epoch=1):
+    def train(self, num_epoch: int = 1):
         """
         Parameters:
             num_epoch (int, optional): number of epochs
         """
-        sampler = torch_data.DistributedSampler(self.train_set, self.world_size, self.rank)
-        dataloader = DataLoader(self.train_set, self.batch_size, sampler=sampler,
-                                num_workers=self.num_worker, follow_batch=self.follow_batch)
+        sampler = torch_data.DistributedSampler(
+            self.train_set, self.world_size, self.rank
+        )
+
+        if self.dataset_type == "torch":
+            dataloader = DataLoader(
+                self.train_set,
+                self.batch_size,
+                sampler=sampler,
+                num_workers=self.num_worker,
+            )
+
+        else:
+            assert isinstance(self.train_set, PyGDataset)
+            dataloader = PyGDataLoader(
+                self.train_set,
+                self.batch_size,
+                sampler=sampler,
+                num_workers=self.num_worker,
+                follow_batch=self.follow_batch,
+            )
+
         model = self.model
 
+        # TODO: here we use the DDP to wrapper the model
+        # self.model -> the original model
+        # model -> the wrappered model
+
         if self.world_size > 1:
             if self.device.type == "cuda":
-                model = nn.parallel.DistributedDataParallel(model, device_ids=[self.device], find_unused_parameters=True)
+                model = nn.parallel.DistributedDataParallel(
+                    model, device_ids=[self.device], find_unused_parameters=True
+                )
             else:
-                model = nn.parallel.DistributedDataParallel(model, find_unused_parameters=True)
+                model = nn.parallel.DistributedDataParallel(
+                    model, find_unused_parameters=True
+                )
 
         model.train()
 
         for epoch in self.meter(num_epoch):
             sampler.set_epoch(epoch)
             losses = []
 
             for i, batch in enumerate(dataloader):
                 if self.device.type == "cuda":
                     batch = utils.cuda(batch, device=self.device)
 
-                # DDP warp the original model so use the `self.model` to get label
-                target = self.model.target(batch)
+                # TODO: cause DDP warp the original model
+                # so use the `self.model` to get label
+                # target = self.model.target(batch)
 
                 with torch.cuda.amp.autocast(enabled=self.half_precision):
                     # TODO: be sure to use `model` (not `self.model`)
                     loss, pred = model(batch)
 
+                # TODO: this is the mix precision training strategy
                 if self.half_precision:
                     self.scaler.scale(loss).backward()
                     torch.nn.utils.clip_grad_norm_(model.parameters(), 10)
                     self.scaler.step(self.optimizer)
                     self.scaler.update()
 
                 else:
                     loss.backward()
                     torch.nn.utils.clip_grad_norm_(model.parameters(), 10)
                     self.optimizer.step()
 
                 self.optimizer.zero_grad()
                 # TODO: Here we can add self-designed loss to update the model
                 # TODO: key: loss name (support multiple loss record)
-                cur_loss = {self.model.loss_name: loss}
-                losses.append(cur_loss)
+                # TODO: You have to implement the loss_name attribute in the self.model
+                cur_batch_loss_info = self.model.loss_info()
+                losses.append(cur_batch_loss_info)
 
                 # Here is the DDP loss, we need to get the loss from all clusters
-                cur_loss = utils.stack(losses, dim=0)
-                cur_loss = utils.mean(cur_loss, dim=0)
+                n_loss = utils.stack(losses, dim=0)
+                n_loss = utils.mean(n_loss, dim=0)
 
                 if self.world_size > 1:
-                    cur_loss = comms.reduce(cur_loss, op="mean")
-                self.meter.update(cur_loss)
+                    n_loss = comms.reduce(n_loss, op="mean")
+                assert isinstance(n_loss, dict)
+                self.meter.update(n_loss)
 
                 # clear the loss history
                 losses = []
 
             if self.scheduler:
                 self.scheduler.step()
 
     @torch.no_grad()
-    def evaluate(self, split, log=True):
+    def evaluate(self, split: str = "train", log: bool = True):
         """
         Parameters:
             split (str): split to evaluate. Can be ``train``, ``valid`` or ``test``.
             log (bool, optional): log metrics or not
         Returns:
             dict: metrics
         """
         if self.rank == 0:
             self.log.logger.warning(pretty.separator)
             self.log.logger.warning("Evaluate on %s" % split)
+
         test_set = getattr(self, "%s_set" % split)
 
         sampler = torch_data.DistributedSampler(test_set, self.world_size, self.rank)
-        dataloader = DataLoader(test_set, self.batch_size, sampler=sampler,
-                                num_workers=self.num_worker, follow_batch=self.follow_batch)
+
+        if self.dataset_type == "torch":
+            dataloader = DataLoader(
+                self.test_set,
+                self.batch_size,
+                sampler=sampler,
+                num_workers=self.num_worker,
+            )
+
+        else:
+            assert isinstance(self.test_set, PyGDataset)
+            dataloader = PyGDataLoader(
+                self.test_set,
+                self.batch_size,
+                sampler=sampler,
+                num_workers=self.num_worker,
+                follow_batch=self.follow_batch,
+            )
 
         model = self.model
         model.eval()
 
         preds = []
         targets = []
         for i, batch in enumerate(dataloader):
@@ -214,14 +273,16 @@
         target = utils.cat(targets)
 
         if self.world_size > 1:
             pred = comms.cat(pred)
             target = comms.cat(target)
 
         metric = model.evaluate(pred, target)
+
+        # TODO: we only keep the main thread log record
         if log and self.rank == 0:
             self.meter.log(metric, category="%s/epoch" % split)
         return metric
 
     def load(self, checkpoint, load_optimizer=True):
         """
         Load a checkpoint from file.
@@ -233,14 +294,15 @@
         if comms.get_rank() == 0:
             self.log.logger.warning("Load checkpoint from %s" % checkpoint)
 
         checkpoint = os.path.expanduser(checkpoint)
         state = torch.load(checkpoint, map_location=self.device)
 
         self.model.load_state_dict(state["model"])
+        self.meter.epoch_id = state["epoch_id"]
 
         if load_optimizer:
             self.optimizer.load_state_dict(state["optimizer"])
             for state in self.optimizer.state.values():
                 for k, v in state.items():
                     if isinstance(v, torch.Tensor):
                         state[k] = v.to(self.device)
@@ -256,15 +318,16 @@
         """
         if comms.get_rank() == 0:
             self.log.logger.warning("Save checkpoint to %s" % checkpoint)
         checkpoint = os.path.expanduser(checkpoint)
         if self.rank == 0:
             state = {
                 "model": self.model.state_dict(),
-                "optimizer": self.optimizer.state_dict()
+                "optimizer": self.optimizer.state_dict(),
+                "epoch_id": self.meter.epoch_id,
             }
             torch.save(state, checkpoint)
         comms.synchronize()
 
     @property
     def epoch(self):
         """Current epoch."""
```

### Comparing `exper-0.1.4/exper/pretty.py` & `exper-0.2.0/exper/pretty.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from typing import Sequence
+
+
 separator = ">" * 30
 line = "-" * 30
 
-def time(seconds):
+
+def time(seconds: float) -> str:
     """
     Format time as a string.
 
     Parameters:
         seconds (float): time in seconds
     """
     sec_per_min = 60
@@ -18,19 +22,21 @@
         return "%.2f hours" % (seconds / sec_per_hour)
     elif seconds > sec_per_min:
         return "%.2f mins" % (seconds / sec_per_min)
     else:
         return "%.2f secs" % seconds
 
 
-def long_array(array, truncation=10, display=3):
+def long_array[T](array: Sequence[T], truncation: int = 10, display: int = 3) -> str:
     """
     Format an array as a string.
 
     Parameters:
         array (array_like): array-like data
-        truncation (int, optional): truncate array if its length exceeds this threshold
-        display (int, optional): number of elements to display at the beginning and the end in truncated mode
+        truncation (int): truncate array if its length exceeds this threshold
+        display (int): number of elements to display at the beginning and the end in truncated mode
     """
     if len(array) <= truncation:
         return "%s" % array
-    return "%s, ..., %s" % (str(array[:display])[:-1], str(array[-display:])[1:])
+    return "%s, ..., %s" % (str(array[:display])[:-1], str(array[-display:])[1:])
+
+
```

### Comparing `exper-0.1.4/exper.egg-info/PKG-INFO` & `exper-0.2.0/exper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: exper
-Version: 0.1.4
+Version: 0.2.0
 Summary: This is a python package for running deep learning experiments. Users can rapidly run their experiments by importing this module.
 Author: Mrzz
+Requires-Dist: torch
+Requires-Dist: torch_geometric
 
 # exper
 
 `exper` is a very lightweight Python package designed for personal use to speed up the execution of PyTorch-based deep learning experiments. This framework is specifically crafted to support Distributed Data Parallel (DDP) training, mix precision training and provides a convenient mechanism for saving experiment logs.
 
 ## Features:
```

### Comparing `exper-0.1.4/setup.py` & `exper-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name='exper',
-    version='0.1.4',
+    version='0.2.0',
     author="Mrzz",
     description="This is a python package for running deep learning experiments. "
                 "Users can rapidly run their experiments by importing this module.",
     packages=find_packages(),
     long_description=long_description,
     install_requires=["torch", "torch_geometric"],
     include_package_data=True
```

