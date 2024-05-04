# Comparing `tmp/mmdit-0.0.1.tar.gz` & `tmp/mmdit-0.0.2.tar.gz`

## Comparing `mmdit-0.0.1.tar` & `mmdit-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.1/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mmdit-0.0.1/mmdit/__init__.py
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 mmdit-0.0.1/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.1/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.1/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.2/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mmdit-0.0.2/mmdit/__init__.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 mmdit-0.0.2/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.2/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.2/PKG-INFO
```

### Comparing `mmdit-0.0.1/mmdit.png` & `mmdit-0.0.2/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.1/.github/workflows/python-publish.yml` & `mmdit-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.1/mmdit/mmdit_pytorch.py` & `mmdit-0.0.2/mmdit/mmdit_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         self,
         *,
         dim,
         dim_inputs: Tuple[int],
         dim_head = 64,
         heads = 8,
         qk_rmsnorm = False,
+        flash = False,
         attend_kwargs: dict = dict()
     ):
         super().__init__()
         """
         ein notation
 
         b - batch
@@ -59,15 +60,18 @@
         num_inputs = len(dim_inputs)
         self.num_inputs = num_inputs
 
         self.to_qkv = ModuleList([nn.Linear(dim_input, dim_inner * 3, bias = False) for dim_input in dim_inputs])
 
         self.split_heads = Rearrange('b n (qkv h d) -> qkv b h n d', h = heads, qkv = 3)
 
-        self.attend = Attend(**attend_kwargs)
+        self.attend = Attend(
+            flash = flash,
+            **attend_kwargs
+        )
 
         self.merge_heads = Rearrange('b h n d -> b n (h d)')
 
         self.to_out = ModuleList([nn.Linear(dim_inner, dim_input, bias = False) for dim_input in dim_inputs])
 
         self.qk_rmsnorm = qk_rmsnorm
         self.q_rmsnorms = (None,) * num_inputs
@@ -152,14 +156,15 @@
         dim_joint_attn,
         dim_text,
         dim_image,
         dim_cond = None,
         dim_head = 64,
         heads = 8,
         qk_rmsnorm = False,
+        flash_attn = False,
         ff_kwargs: dict = dict()
     ):
         super().__init__()
 
         # handle optional time conditioning
 
         has_cond = exists(dim_cond)
@@ -186,15 +191,16 @@
 
         # attention and feedforward
 
         self.attn = Attention(
             dim = dim_joint_attn,
             dim_inputs = (dim_text, dim_image),
             dim_head = dim_head,
-            heads = heads
+            heads = heads,
+            flash = flash_attn
         )
 
         self.text_ff = FeedForward(dim_text, **ff_kwargs)
         self.image_ff = FeedForward(dim_image, **ff_kwargs)
 
     def forward(
         self,
```

### Comparing `mmdit-0.0.1/.gitignore` & `mmdit-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.1/LICENSE` & `mmdit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.1/README.md` & `mmdit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.1/pyproject.toml` & `mmdit-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.1"
+version = "0.0.2"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.1/PKG-INFO` & `mmdit-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.1
+Version: 0.0.2
 Summary: MMDiT
 Project-URL: Homepage, https://pypi.org/project/mmdit/
 Project-URL: Repository, https://github.com/lucidrains/mmdit
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.1 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.2 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

