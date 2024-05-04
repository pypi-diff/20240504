# Comparing `tmp/mmdit-0.0.2.tar.gz` & `tmp/mmdit-0.0.3.tar.gz`

## Comparing `mmdit-0.0.2.tar` & `mmdit-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.2/mmdit.png
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mmdit-0.0.2/mmdit/__init__.py
--rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 mmdit-0.0.2/mmdit/mmdit_pytorch.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.2/LICENSE
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.2/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0   149158 2020-02-02 00:00:00.000000 mmdit-0.0.3/mmdit.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 mmdit-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mmdit-0.0.3/mmdit/__init__.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 mmdit-0.0.3/mmdit/mmdit_pytorch.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mmdit-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mmdit-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 mmdit-0.0.3/README.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mmdit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 mmdit-0.0.3/PKG-INFO
```

### Comparing `mmdit-0.0.2/mmdit.png` & `mmdit-0.0.3/mmdit.png`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.2/.github/workflows/python-publish.yml` & `mmdit-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.2/mmdit/mmdit_pytorch.py` & `mmdit-0.0.3/mmdit/mmdit_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,24 +167,37 @@
 
         # handle optional time conditioning
 
         has_cond = exists(dim_cond)
         self.has_cond = has_cond
 
         if has_cond:
-            self.cond_dims = (
-                *((dim_text,) * 6),
-                *((dim_image,) * 6)
+            dim_gammas = (
+                *((dim_text,) * 4),
+                *((dim_image,) * 4)
             )
 
+            dim_betas = (
+                *((dim_text,) * 2),
+                *((dim_image,) * 2),
+            )
+
+            self.cond_dims = (*dim_gammas, *dim_betas)
+
+            to_cond_linear = nn.Linear(dim_cond, sum(self.cond_dims))
+
             self.to_cond = nn.Sequential(
                 nn.SiLU(),
-                nn.Linear(dim_cond, sum(self.cond_dims))
+                to_cond_linear
             )
 
+            nn.init.zeros_(to_cond_linear.weight)
+            nn.init.zeros_(to_cond_linear.bias)
+            nn.init.constant_(to_cond_linear.bias[:sum(dim_gammas)], 1.)
+
         # handle adaptive norms
 
         self.text_attn_layernorm = nn.LayerNorm(dim_text, elementwise_affine = not has_cond)
         self.image_attn_layernorm = nn.LayerNorm(dim_image, elementwise_affine = not has_cond)
 
         self.text_ff_layernorm = nn.LayerNorm(dim_text, elementwise_affine = not has_cond)
         self.image_ff_layernorm = nn.LayerNorm(dim_image, elementwise_affine = not has_cond)
@@ -211,25 +224,25 @@
         time_cond = None
     ):
         assert not (exists(time_cond) ^ self.has_cond), 'time condition must be passed in if dim_cond is set at init. it should not be passed in if not set'
 
         if self.has_cond:
             (
                 text_pre_attn_gamma,
-                text_pre_attn_beta,
                 text_post_attn_gamma,
                 text_pre_ff_gamma,
-                text_pre_ff_beta,
                 text_post_ff_gamma,
                 image_pre_attn_gamma,
-                image_pre_attn_beta,
                 image_post_attn_gamma,
                 image_pre_ff_gamma,
-                image_pre_ff_beta,
                 image_post_ff_gamma,
+                text_pre_attn_beta,
+                text_pre_ff_beta,
+                image_pre_attn_beta,
+                image_pre_ff_beta,
             ) = self.to_cond(time_cond).split(self.cond_dims, dim = -1)
 
         # handle attn adaptive layernorm
 
         text_tokens_residual = text_tokens
         image_tokens_residual = image_tokens
```

### Comparing `mmdit-0.0.2/.gitignore` & `mmdit-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.2/LICENSE` & `mmdit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.2/README.md` & `mmdit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mmdit-0.0.2/pyproject.toml` & `mmdit-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmdit"
-version = "0.0.2"
+version = "0.0.3"
 description = "MMDiT"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { file = "LICENSE" }
```

### Comparing `mmdit-0.0.2/PKG-INFO` & `mmdit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mmdit
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.3 Name: mmdit Version: 0.0.2 Summary: MMDiT Project-URL:
+Metadata-Version: 2.3 Name: mmdit Version: 0.0.3 Summary: MMDiT Project-URL:
 Homepage, https://pypi.org/project/mmdit/ Project-URL: Repository, https://
 github.com/lucidrains/mmdit Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

