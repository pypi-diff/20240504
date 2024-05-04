# Comparing `tmp/pepperpepper-0.0.6.8.tar.gz` & `tmp/pepperpepper-0.0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.8.tar", last modified: Fri May  3 08:07:13 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.9.tar", last modified: Fri May  3 11:02:58 2024, max compression
```

## Comparing `pepperpepper-0.0.6.8.tar` & `pepperpepper-0.0.6.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/
--rw-rw-rw-   0        0        0      433 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.242176 pepperpepper-0.0.6.8/PepperPepper/
--rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.8/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.273874 pepperpepper-0.0.6.8/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.8/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.8/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.8/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.273874 pepperpepper-0.0.6.8/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.8/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.8/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.8/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.273874 pepperpepper-0.0.6.8/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.8/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.8/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.8/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.8/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.8/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.8/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.8/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.8/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.8/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.8/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.8/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.291214 pepperpepper-0.0.6.8/PepperPepper/models/
--rw-rw-rw-   0        0        0     1192 2024-05-03 07:57:17.000000 pepperpepper-0.0.6.8/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    25740 2024-05-03 08:06:15.000000 pepperpepper-0.0.6.8/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.8/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.8/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.8/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.8/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.8/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.8/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 08:07:13.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.8/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-03 08:07:13.305228 pepperpepper-0.0.6.8/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-03 08:06:28.000000 pepperpepper-0.0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.195596 pepperpepper-0.0.6.9/
+-rw-rw-rw-   0        0        0      433 2024-05-03 11:02:58.194597 pepperpepper-0.0.6.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.146159 pepperpepper-0.0.6.9/PepperPepper/
+-rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.9/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.172711 pepperpepper-0.0.6.9/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.9/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.9/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.9/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.174632 pepperpepper-0.0.6.9/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.9/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.9/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.9/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.178716 pepperpepper-0.0.6.9/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.9/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.9/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.9/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.9/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.9/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.184137 pepperpepper-0.0.6.9/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.9/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.9/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.9/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.9/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.187138 pepperpepper-0.0.6.9/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.9/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.9/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.9/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.188495 pepperpepper-0.0.6.9/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.9/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.9/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.191597 pepperpepper-0.0.6.9/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.6.9/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    29874 2024-05-03 11:02:13.000000 pepperpepper-0.0.6.9/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.9/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.9/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.9/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.192597 pepperpepper-0.0.6.9/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.9/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.9/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.9/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:02:58.194597 pepperpepper-0.0.6.9/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-03 11:02:58.000000 pepperpepper-0.0.6.9/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-03 11:02:58.000000 pepperpepper-0.0.6.9/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 11:02:58.000000 pepperpepper-0.0.6.9/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-03 11:02:58.000000 pepperpepper-0.0.6.9/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-03 11:02:58.000000 pepperpepper-0.0.6.9/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.9/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-03 11:02:58.195596 pepperpepper-0.0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-03 11:02:29.000000 pepperpepper-0.0.6.9/setup.py
```

### Comparing `pepperpepper-0.0.6.8/PepperPepper/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.9/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.9/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.9/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 from .cnn import MLPConv
 from .cnn import NiNBlock
 from .cnn import NiN
 from .cnn import InceptionBlockV1
 from .cnn import GoogLeNet
 from .cnn import ResidualBlock
 from .cnn import ResNet
+from .cnn import DenseBlock
+from .cnn import TransitionBlock
+from .cnn import DenseNet
+
+
+
 
 
 
 #from .rnn import RNNModel
 #from .transformer import TransformerModel
 #from .custom_model import CustomModel
 
@@ -36,9 +42,18 @@
    'VGG16',
    'MLPConv',
    'NiNBlock',
    'NiN',
    'InceptionBlockV1',
    'GoogLeNet',
    'ResidualBlock',
-   'ResNet'
-]
+   'ResNet',
+   'DenseBlock',
+   'TransitionBlock',
+   'DenseNet'
+]
+
+
+
+
+
+
```

### Comparing `pepperpepper-0.0.6.8/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6.9/PepperPepper/models/cnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -632,7 +632,142 @@
             if i==0 and not fist_block:
                 blk.append(ResidualBlock(in_channels, out_channels, strides=2))
             else:
                 blk.append(ResidualBlock(out_channels, out_channels))
         return blk
 
 
+
+
+"""
+11.DenseBlock的复现
+简介：一个稠密块由多个卷积块组成，每个卷积块使用相同数量的输出通道。前向传播中，将每个卷积块的输入与输出在通道上连接。
+"""
+class DenseBlock(torch.nn.Module):
+    def __init__(self, in_channels, out_channels, num_convs):
+        super(DenseBlock, self).__init__()
+        self.net = torch.nn.ModuleList([self._conv_block(in_channels + i * out_channels, out_channels) for i in range(num_convs)])
+
+    #批量生成规范层、激活层和卷积层
+    def _conv_block(self, in_channels, num_channels):
+        return torch.nn.Sequential(
+            torch.nn.BatchNorm2d(in_channels),
+            torch.nn.ReLU(inplace=True),
+            torch.nn.Conv2d(in_channels, num_channels, kernel_size=3, padding=1)
+        )
+
+
+    def forward(self, x):
+        # 实现DenseBlock中将输出与输入相连
+        features = [x]
+        for layer in self.net:
+            out = layer(torch.cat(features, dim=1))
+            features.append(out)
+        return torch.cat(features, dim=1) # 将所有输出连接在一起
+
+
+
+
+
+
+
+"""
+12.TransitionBlock
+简述：过渡层，每一个稠密块都会增加通道数，因此使用过多会过于复杂，而过度层可以控制模型复杂度，通过1x1卷积层来减小通道数，并使用步幅为2的平均汇聚层减半高度和宽度
+"""
+class TransitionBlock(torch.nn.Module):
+    def __init__(self, in_channels, out_channels):
+        super(TransitionBlock, self).__init__()
+        self.conv = torch.nn.Conv2d(in_channels, out_channels, kernel_size=1, stride=1, padding=0) # 使用1x1卷积进行特征通道数的调整
+        self.pool = torch.nn.AvgPool2d(kernel_size=2, stride=2) # 使用平均池化进行特征尺寸的减半
+
+    def forward(self, x):
+        x = self.pool(self.conv(x)) # 先通过1x1卷积调整特征通道数，然后再进行池化操作
+
+
+
+
+
+
+
+"""
+13.DenseNet
+简述：使用4个稠密块，每个稠密块可以设定包含多少个卷积层，稠密块使用过度层来调整特征图的大小
+"""
+class DenseNet(torch.nn.Module):
+    def __init__(self, in_channels=3, num_classes=1000,):
+        super(DenseNet, self).__init__()
+        # num_channels为当前的通道数，growth_rate增长率，num_convs_in_dense_block为四个稠密块包含的卷积层数
+        self.num_classs = 64
+        self.growth_rate = 32
+        self.num_convs_in_dense_block = [4, 4, 4, 4]
+        self.blk = []
+
+        #第一个模块使用单卷积层和最大汇聚层
+        self.block1 = torch.nn.Sequential(
+            torch.nn.Conv2d(in_channels, self.num_classs, kernel_size=3, stride=2, padding=3),
+            torch.nn.BatchNorm2d(64),
+            torch.nn.ReLU(),
+            torch.nn.MaxPool2d(kernel_size=3, stride=2, padding=1) # 使用最大池化进行下采样
+        )
+
+
+
+
+        # 使用4个稠密块，稠密块里的卷积层通道数即增长率设为32，所以每个稠密块将增加128个通道
+        for i, num_convs in enumerate(self.num_convs_in_dense_block):
+            # 添加一个稠密块
+            self.blk.append(DenseBlock(self.num_classs, self.growth_rate, num_convs))
+
+            # 上一个稠密块的输出通道数
+            self.num_classs = self.num_classs + self.growth_rate * num_convs
+
+            # 在稠密块直接添加一个过度层，使通道数减半
+            if i != len(self.num_convs_in_dense_block) - 1:
+                self.blk.append(TransitionBlock(self.num_classs, self.num_classs // 2))
+                self.num_classs = self.num_classs // 2
+
+
+        self.features = torch.nn.Sequential(self.block1, *self.blk, torch.nn.BatchNorm2d(self.num_classs), torch.nn.ReLU(), torch.nn.AdaptiveAvgPool2d((1, 1)))
+
+        self.classifier = torch.nn.Sequential(torch.nn.Flatten(), torch.nn.Linear(self.num_classs, num_classes))
+
+
+    def forward(self, x):
+        x = self.features(x)
+        x = self.classifier(x)
+        return x
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `pepperpepper-0.0.6.8/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.9/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.9/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.8/setup.py` & `pepperpepper-0.0.6.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6.8",
+    version="0.0.6.9",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

