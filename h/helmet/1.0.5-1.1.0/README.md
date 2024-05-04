# Comparing `tmp/helmet-1.0.5.tar.gz` & `tmp/helmet-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helmet-1.0.5.tar", max compression
+gzip compressed data, was "helmet-1.1.0.tar", max compression
```

## Comparing `helmet-1.0.5.tar` & `helmet-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1595 2024-04-30 07:26:25.313296 helmet-1.0.5/README.md
--rw-r--r--   0        0        0      497 2024-04-30 07:26:25.313296 helmet-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2652 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/explainers/__init__.py
--rw-r--r--   0        0        0     5236 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/explainers/gradients.py
--rw-r--r--   0        0        0      630 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/explainers/perturbation.py
--rw-r--r--   0        0        0       49 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/model/__init__.py
--rw-r--r--   0        0        0     3708 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/model/base_lm.py
--rw-r--r--   0        0        0     6169 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/model/dec_lm.py
--rw-r--r--   0        0        0     3949 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/updater.py
--rw-r--r--   0        0        0       79 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/utils/constants.py
--rw-r--r--   0        0        0     3277 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/utils/types.py
--rw-r--r--   0        0        0      130 2024-04-30 07:26:25.313296 helmet-1.0.5/src/helmet/utils/utils.py
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 helmet-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3116 2024-05-04 08:42:42.774084 helmet-1.1.0/README.md
+-rw-r--r--   0        0        0      445 2024-05-04 08:42:42.774084 helmet-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2980 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/explainers/__init__.py
+-rw-r--r--   0        0        0     4948 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/explainers/gradients.py
+-rw-r--r--   0        0        0      630 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/explainers/perturbation.py
+-rw-r--r--   0        0        0       49 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/model/__init__.py
+-rw-r--r--   0        0        0     3769 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/model/base_lm.py
+-rw-r--r--   0        0        0     5373 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/model/dec_lm.py
+-rw-r--r--   0        0        0     3879 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/updater.py
+-rw-r--r--   0        0        0      125 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/utils/constants.py
+-rw-r--r--   0        0        0     3623 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/utils/types.py
+-rw-r--r--   0        0        0      130 2024-05-04 08:42:42.774084 helmet-1.1.0/src/helmet/utils/utils.py
+-rw-r--r--   0        0        0     3759 1970-01-01 00:00:00.000000 helmet-1.1.0/PKG-INFO
```

### Comparing `helmet-1.0.5/src/helmet/explainers/gradients.py` & `helmet-1.1.0/src/helmet/explainers/gradients.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,9 @@
 import torch
 import numpy as np
-from captum.attr import (
-    InputXGradient, Saliency, LayerIntegratedGradients, 
-    LLMGradientAttribution, TextTokenInput, LLMAttribution, IntegratedGradients
-)
-from typing import Dict, Any
-from functools import partial
-from torch.nn import functional as F
-
-def compute_gradient(wrapper, prompt, input, output, gradient_type):
-    # TODO: add with torch.no_grad():?
-
-    def model_forward(inp, model, extra_forward_args: Dict[str, Any] = {}):
-        output = model(input_ids=inp, **extra_forward_args)
-        return F.softmax(output.logits, dim=1)
-    
-    input_embeds = wrapper.get_input_embeddings(prompt)
-    attention_mask = input["attention_mask"]
-
-    forward_func = partial(model_forward, model=wrapper.model, extra_forward_args={"attention_mask": attention_mask})
-
-    if gradient_type == "input_x_gradient":
-        # According to Luo and Specia (2024), inputxgradient has a lot of overhead because they also compute the gradients
-        # of the input based on a reference input.
-        lig = InputXGradient(forward_func)
-    else:
-        lig = Saliency(forward_func)
-    attributions = lig.attribute(inputs=input_embeds, target=output)
-    attributions = attributions.detach().cpu().numpy()
-    r = attributions[0, :, :]
-    attr = r.sum(axis=1)
-    attr = wrapper.normalize(attr)
-
-    return attr
 
 # Adapted from Interpret-LM
 # Adapted from AllenNLP Interpret and Han et al. 2020
 def register_embedding_list_hook(model, embedding_layer, embeddings_list):
     def forward_hook(module, inputs, output):
         embeddings_list.append(output.squeeze(0).clone().cpu().detach().numpy())
     handle = embedding_layer.register_forward_hook(forward_hook)
@@ -46,15 +13,14 @@
     def hook_layers(module, grad_in, grad_out):
         embeddings_gradients.append(grad_out[0].detach().cpu().numpy())
     hook = embedding_layer.register_full_backward_hook(hook_layers)
     return hook
 
 def analyze_token(wrapper, input_ids, input_mask, batch=0, correct=None, foil=None):
     # Get model gradients and input embeddings
-    torch.enable_grad()
     model = wrapper.model
     embedding_layer = wrapper.embeddings
 
     model.eval()
     embeddings_list = []
     handle = register_embedding_list_hook(model, embedding_layer, embeddings_list)
     embeddings_gradients = []
@@ -63,27 +29,26 @@
         correct = input_ids[-1]
         input_ids = input_ids[:-1]
         input_mask = input_mask[:-1]
 
     input_ids_new = torch.tensor(input_ids.clone().detach())
     input_ids_unsqueezed = input_ids_new.unsqueeze(0)
 
-    # A = model.generate(input_ids=input_ids_unsqueezed, attention_mask=input_mask)
-    A = model(input_ids=input_ids_unsqueezed, output_attentions=False)
+    with torch.enable_grad():
+        A = model(input_ids=input_ids_unsqueezed, output_attentions=False)
 
-    if foil is not None and correct != foil:
-        (A.logits[0][-1][correct]-A.logits[0][-1][foil]).backward()
-    else:
-        # Take the last logits and backpropagate the gradient
-        p = A.logits[0][-1][correct]
-        p.backward()
-    handle.remove()
-    hook.remove()
+        if foil is not None and correct != foil:
+            (A.logits[0][-1][correct]-A.logits[0][-1][foil]).backward()
+        else:
+            # Take the last logits and backpropagate the gradient
+            p = A.logits[0][-1][correct]
+            p.backward()
+        handle.remove()
+        hook.remove()
 
-    import numpy as np
     return np.array(embeddings_gradients).squeeze(), np.array(embeddings_list).squeeze()
 
 def input_x_gradient(grads, embds, normalize=False):
     input_grad = np.sum(grads * embds, axis=-1).squeeze()
 
     if normalize:
         norm = np.linalg.norm(input_grad, ord=1)
@@ -133,8 +98,32 @@
 #         wrapper.tokenizer,
 #         skip_tokens=[1],  # skip the special token for the start of the text <s>
 #     )
     
 #     res = llm_attr.attribute(input, target=output)
 #     return res.seq_attr.detach().cpu().numpy()
 
+# def compute_gradient(wrapper, prompt, input, output, gradient_type):
+#     # TODO: add with torch.no_grad():?
+
+#     def model_forward(inp, model, extra_forward_args: Dict[str, Any] = {}):
+#         output = model(input_ids=inp, **extra_forward_args)
+#         return F.softmax(output.logits, dim=1)
+    
+#     input_embeds = wrapper.get_input_embeddings(prompt)
+#     attention_mask = input["attention_mask"]
+
+#     forward_func = partial(model_forward, model=wrapper.model, extra_forward_args={"attention_mask": attention_mask})
+
+#     if gradient_type == "input_x_gradient":
+#         # According to Luo and Specia (2024), inputxgradient has a lot of overhead because they also compute the gradients
+#         # of the input based on a reference input.
+#         lig = InputXGradient(forward_func)
+#     else:
+#         lig = Saliency(forward_func)
+#     attributions = lig.attribute(inputs=input_embeds, target=output)
+#     attributions = attributions.detach().cpu().numpy()
+#     r = attributions[0, :, :]
+#     attr = r.sum(axis=1)
+#     attr = wrapper.normalize(attr)
 
+#     return attr
```

### Comparing `helmet-1.0.5/src/helmet/explainers/perturbation.py` & `helmet-1.1.0/src/helmet/explainers/perturbation.py`

 * *Files identical despite different names*

### Comparing `helmet-1.0.5/src/helmet/model/base_lm.py` & `helmet-1.1.0/src/helmet/model/base_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         self.reset_model()
         print("model loaded")
     
     def _encode_text(self, text, **kwargs):
         if isinstance(text, list):
             text = self.tokenizer.apply_chat_template(text, tokenize = False, add_generation_prompt = True)
 
-        return self.tokenizer.encode_plus(text, return_tensors="pt", **kwargs)
+        enc = self.tokenizer.encode_plus(text, return_tensors="pt", **kwargs)
+        return {k: v.to(self.device) for k, v in enc.items()}
 
     def _tokenize(self, text: str, **kwargs):
         t = self.tokenizer(text, return_tensors="pt", **kwargs)
         return t.to(self.device)
 
     def token_ids_to_string(self, output) -> str:
         # Return back the string
```

### Comparing `helmet-1.0.5/src/helmet/model/dec_lm.py` & `helmet-1.1.0/src/helmet/model/dec_lm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,106 @@
 import time
 from operator import attrgetter
 from typing import Tuple
+import numpy as np
 
 import torch
 import transformers
 
 from helmet.explainers.gradients import analyze_token, input_x_gradient
 from helmet.model.base_lm import Base_LM
-from helmet.utils.constants import ALTERNATIVES, CONTRASTIVE, SALIENCY
 from helmet.utils.types import *
 
 
 class DEC_LM(Base_LM):
-    def __init__(self, model_checkpoint: str, model: transformers.AutoModelForCausalLM, 
-                 tokenizer: transformers.PreTrainedTokenizer, url: str, project_id: str, model_config: dict = {}, device="cpu"):
+    def __init__(self, 
+                 model_checkpoint: str, 
+                 model: transformers.AutoModelForCausalLM, 
+                 tokenizer: transformers.PreTrainedTokenizer, 
+                 url: str, 
+                 project_id: str, 
+                 model_config: dict = {}, 
+                 device="cpu"):
         self.model_type = "dec"
         self.model_config = model_config
 
         try:
             assert "embeddings" in model_config, AssertionError("embeddings must be specified in model_config")
             retriever = attrgetter(model_config["embeddings"])
             embeddings = retriever(model)
             assert embeddings is not None, AssertionError(f"embeddings {model_config['embeddings']} not found in model")
         except Exception as e:
             print(e)
             raise KeyError("embeddings must be specified in model_config")
 
         super().__init__(model_checkpoint, model, tokenizer, self.model_type, url, project_id, embeddings, device)
     
-    def forward(self, inputs, generation_args, **kwargs) -> Tuple[list, AlternativesExplanation]:
-        amount_potentials = 5
-        inputs_ = self.to_device(inputs)
+    def forward(self, inputs, generation_args, **kwargs) -> Tuple[list, CertaintyExplanation]:
+        input_len = len(inputs["input_ids"][0])
 
-        input_len = len(inputs_["input_ids"][0])
-
-        output = self.model.generate(
-            **inputs_, 
+        generated_outputs = self.model.generate(
+            **inputs, 
             return_dict_in_generate=True,
-            output_scores=True, # this gets the scores, while logits are unprocessed.
-            # num_beams=5,
-            no_repeat_ngram_size=2,
-            # num_return_sequences=5,
-            # early_stopping=True,
+            output_scores=True, # this gets the scores
             **generation_args,
+            **kwargs
         )
+        
+        transition_scores = self.model.compute_transition_scores(generated_outputs.sequences, generated_outputs.scores, normalize_logits=True)
+        gen_sequences = generated_outputs.sequences[:, input_len:]
+        certainties = [float(np.exp(score.cpu().numpy())) for score in transition_scores[0]]
 
-        outputIds = output.sequences[0] #first of 5 sequence outputs
-        outs = outputIds.detach().cpu().numpy()
-        output_token_ids = outs[input_len:]
-        print("output_token_ids", output_token_ids)
-
-        scores = output.scores
-
-        alternatives_per_token = []
-        for i in range(len(scores)):
-            local_scores = scores[i][0] #only for the final sequence, thus [0]
-            # Scores is now a tensor of shape (vocab_size)
-            top_k = local_scores.topk(amount_potentials) 
-            top_k_scores = top_k.values.detach().flatten().tolist()
-            #  normalize scores
-            top_k_scores = self.normalize(top_k_scores)
-            top_k_indices = top_k.indices
-
-            tokens = self.tokenizer.convert_ids_to_tokens(top_k_indices.detach().flatten(), skip_special_tokens=True)
-            res = [{"token": token, "score": score} for token, score in zip(tokens, top_k_scores)]
-            alternatives_per_token.append(res)
+        outs = gen_sequences[0].detach().cpu().numpy() 
 
-        
-        return output_token_ids, AlternativesExplanation(alternatives_per_token)
+        return outs, CertaintyExplanation(certainties)
     
     def predict(self, prompt, generation_args, groundtruth=None, *args, **kwargs):
-        print("start of the predict function")
         start = time.time()
         input = self._encode_text(prompt)
         input_str = self.token_ids_to_string(input["input_ids"][0])
         
-        print("Input:", input_str)
+        print("Processed input:", input_str)
         
-        output_token_ids, alternatives = self.forward(input, generation_args)
+        output_token_ids, certainties = self.forward(input, generation_args)
         output_str: str = self.token_ids_to_string(output_token_ids)
 
-        print("Predicted output:", output_str)
+        print("Output:", output_str)
         
         end = time.time()
         execution_time = end - start
 
-        formatted_run = self._format_run(input_str, output_str, [alternatives], execution_time, groundtruth=groundtruth)
+        formatted_run = self._format_run(input_str, output_str, [certainties], execution_time, groundtruth=groundtruth)
 
         id = self.update_run(formatted_run)
 
         return output_str, id
 
-    def saliency_explainer(self, id: str, **kwargs) -> SaliencyExplanation:
+    def feature_attribution(self, id: str, **kwargs) -> FeatureAttributionExplainer:
         run: Run = self.get_run(id)
-        input = self._encode_text(run.input.prompt)
-        output_token_ids = self.tokenizer.convert_tokens_to_ids(run.output.tokens)
-        
+        input = self._encode_text(run.input.prompt) #on cuda
+        output_token_ids = self.tokenizer.convert_tokens_to_ids(run.output.tokens) #on cpu
+        output_token_ids = torch.tensor(output_token_ids).to(self.device)
         input_ids = input["input_ids"][0]
         attention_mask = input["attention_mask"]
 
-        merged = torch.cat((input_ids, torch.tensor(output_token_ids)), 0)
-        merged = self.to_device(merged)
+        merged = torch.cat((input_ids, output_token_ids), 0)
 
         start_index = len(input_ids)
         total_length = len(merged)
 
         result = []
         for idx in range(start_index, total_length):
             curr_input_ids = merged[:idx]
             output_id = merged[idx]
             base_saliency_matrix, base_embd_matrix = analyze_token(self, curr_input_ids, attention_mask, correct=output_id)
             gradients = input_x_gradient(base_saliency_matrix, base_embd_matrix, normalize=True)
             result.append(gradients)
             print("finished token", idx, "of", total_length)
 
-        explanation = SaliencyExplanation(input_attributions=result)
+        explanation = FeatureAttributionExplainer(input_attributions=result)
         run.explanations.append(explanation)
 
         id = self.update_run(run)
 
         return explanation
     
     def contrastive_explainer(self, id: str, alternative_str: str, **kwargs) -> ContrastiveExplanation:
@@ -143,8 +125,9 @@
         
         explanation = ContrastiveExplanation(contrastive_input=alternative_output_str, attributions=gradients)
         run.explanations.append(explanation)
 
         id = self.update_run(run)
 
         return explanation
+
```

### Comparing `helmet-1.0.5/src/helmet/updater.py` & `helmet-1.1.0/src/helmet/updater.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 import numpy
 import json
 from datetime import datetime, date
 from dateutil import parser
 
 from dacite import from_dict
-from helmet.utils.types import Run, Explanation, AlternativesExplanation, ContrastiveExplanation, SaliencyExplanation, explanation_name_to_class
+from helmet.utils.types import Run, Explanation, explanation_name_to_class
 from dataclasses import asdict
 
 numbers: tuple = tuple([numpy.int_, numpy.intc, numpy.intp, numpy.int8])
 floats: tuple =  tuple([numpy.float_, numpy.float16, numpy.float32, numpy.float64])
 
 class NumpyEncoder(json.JSONEncoder):
     """ Special json encoder for numpy types """
```

### Comparing `helmet-1.0.5/src/helmet/utils/types.py` & `helmet-1.1.0/src/helmet/utils/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Optional
-from helmet.utils.constants import SALIENCY, ALTERNATIVES, CONTRASTIVE
+from helmet.utils.constants import FEATURE_ATTRIBUTION, ALTERNATIVES, CONTRASTIVE, CERTAINTY
 
 @dataclass 
 class Attribution:
    """Attribution dataclass"""
    attribution: list[float] = field(default_factory=list)
 
 @dataclass
 class Explanation:
     """Generic explanation dataclass"""
     explanation_method: str
 
 @dataclass
-class SaliencyExplanation(Explanation):
+class FeatureAttributionExplainer(Explanation):
     """Saliency Explanation dataclass"""
     input_attributions: Attribution | list[Attribution]
     def __init__(self, input_attributions: Attribution | list[Attribution]):
         self.input_attributions = input_attributions
-        super().__init__(SALIENCY)
+        super().__init__(FEATURE_ATTRIBUTION)
     
 @dataclass
 class ContrastiveExplanation(Explanation):
     """Contrastive Explanation dataclass"""
     contrastive_input: str
     attributions: Attribution
     def __init__(self, contrastive_input: str, attributions: Attribution):
@@ -35,18 +35,27 @@
 class AlternativesExplanation(Explanation):
     """Alternatives Explanation dataclass"""
     output_alternatives: list[list[dict[str, float]]]
     def __init__(self, output_alternatives: list[list[dict[str, float]]]):
         self.output_alternatives = output_alternatives
         super().__init__(ALTERNATIVES)
 
+@dataclass
+class CertaintyExplanation(Explanation):
+    """Certainty Explanation dataclass"""
+    certainties: list[float]
+    def __init__(self, certainties: list[float]):
+        self.certainties = certainties
+        super().__init__(CERTAINTY)
+
 explanation_name_to_class = {
     ALTERNATIVES: AlternativesExplanation,
     CONTRASTIVE: ContrastiveExplanation,
-    SALIENCY: SaliencyExplanation
+    FEATURE_ATTRIBUTION: FeatureAttributionExplainer,
+    CERTAINTY: CertaintyExplanation
 }
 
 @dataclass  
 class Input:
     """Generic Prompt Class"""
     prompt: str
     input_tokens: list[str]
```

