# Comparing `tmp/docugami_langchain-0.0.7rc9.tar.gz` & `tmp/docugami_langchain-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugami_langchain-0.0.7rc9.tar", max compression
+gzip compressed data, was "docugami_langchain-0.0.8.tar", max compression
```

## Comparing `docugami_langchain-0.0.7rc9.tar` & `docugami_langchain-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,62 @@
--rw-r--r--   0        0        0     1072 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/LICENSE
--rw-r--r--   0        0        0      351 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/README.md
--rw-r--r--   0        0        0      669 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/__init__.py
--rw-r--r--   0        0        0      285 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/__init__.py
--rw-r--r--   0        0        0     4266 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/base.py
--rw-r--r--   0        0        0    13322 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/re_act_agent.py
--rw-r--r--   0        0        0     7878 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/re_woo_agent.py
--rw-r--r--   0        0        0     1849 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/agents/rewrite_grader_agent.py
--rw-r--r--   0        0        0    11094 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/base_runnable.py
--rw-r--r--   0        0        0      914 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/__init__.py
--rw-r--r--   0        0        0     2009 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/answer_chain.py
--rw-r--r--   0        0        0     6946 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/base.py
--rw-r--r--   0        0        0      243 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/__init__.py
--rw-r--r--   0        0        0     3255 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
--rw-r--r--   0        0        0     3849 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/summarize_chunk_chain.py
--rw-r--r--   0        0        0      291 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/__init__.py
--rw-r--r--   0        0        0     3834 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/describe_document_set_chain.py
--rw-r--r--   0        0        0     3852 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/summarize_document_chain.py
--rw-r--r--   0        0        0     3486 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/helpers.py
--rw-r--r--   0        0        0     1098 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/__init__.py
--rw-r--r--   0        0        0     2909 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
--rw-r--r--   0        0        0     3899 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_fixup_chain.py
--rw-r--r--   0        0        0     4360 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_query_explainer_chain.py
--rw-r--r--   0        0        0     8191 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_chain.py
--rw-r--r--   0        0        0     3522 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_explainer_chain.py
--rw-r--r--   0        0        0     2426 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_questions_chain.py
--rw-r--r--   0        0        0     3577 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_report_chain.py
--rw-r--r--   0        0        0      111 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/rag/__init__.py
--rw-r--r--   0        0        0     3115 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/chains/rag/simple_rag_chain.py
--rw-r--r--   0        0        0      689 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/config.py
--rw-r--r--   0        0        0      109 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0    13516 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0      674 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1075 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/key_finding.py
--rw-r--r--   0        0        0     1073 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/line_separated_list.py
--rw-r--r--   0        0        0     1992 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/soft_react_json_single_input.py
--rw-r--r--   0        0        0     2816 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/sql_finding.py
--rw-r--r--   0        0        0     4502 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/timespan.py
--rw-r--r--   0        0        0      781 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/params.py
--rw-r--r--   0        0        0        0 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/py.typed
--rw-r--r--   0        0        0      165 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/__init__.py
--rw-r--r--   0        0        0     5214 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/fused_summary.py
--rw-r--r--   0        0        0     5615 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/mappings.py
--rw-r--r--   0        0        0     5292 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/tools/reports.py
--rw-r--r--   0        0        0     5189 2024-03-17 01:01:38.632537 docugami_langchain-0.0.7rc9/docugami_langchain/tools/retrieval.py
--rw-r--r--   0        0        0     2606 2024-03-17 01:01:38.636537 docugami_langchain-0.0.7rc9/pyproject.toml
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 docugami_langchain-0.0.7rc9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/LICENSE
+-rw-r--r--   0        0        0      361 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/README.md
+-rw-r--r--   0        0        0      747 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/__init__.py
+-rw-r--r--   0        0        0     8192 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/base.py
+-rw-r--r--   0        0        0     1760 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/models.py
+-rw-r--r--   0        0        0    10775 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/re_act_agent.py
+-rw-r--r--   0        0        0     8325 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/tool_router_agent.py
+-rw-r--r--   0        0        0    16628 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/base_runnable.py
+-rw-r--r--   0        0        0     1396 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/answer_chain.py
+-rw-r--r--   0        0        0     1415 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/base.py
+-rw-r--r--   0        0        0      243 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/chunks/__init__.py
+-rw-r--r--   0        0        0     3390 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
+-rw-r--r--   0        0        0     3980 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/chunks/summarize_chunk_chain.py
+-rw-r--r--   0        0        0      291 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/documents/__init__.py
+-rw-r--r--   0        0        0     3838 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/documents/describe_document_set_chain.py
+-rw-r--r--   0        0        0     3983 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/documents/summarize_document_chain.py
+-rw-r--r--   0        0        0      647 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
+-rw-r--r--   0        0        0     3999 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_fixup_chain.py
+-rw-r--r--   0        0        0     4360 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_query_explainer_chain.py
+-rw-r--r--   0        0        0     8665 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_chain.py
+-rw-r--r--   0        0        0     3522 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_explainer_chain.py
+-rw-r--r--   0        0        0      498 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/__init__.py
+-rw-r--r--   0        0        0     3297 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/simple_rag_chain.py
+-rw-r--r--   0        0        0     4006 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/standalone_question_chain.py
+-rw-r--r--   0        0        0     4592 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/suggested_questions_chain.py
+-rw-r--r--   0        0        0     4193 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/suggested_report_chain.py
+-rw-r--r--   0        0        0     4832 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/tool_final_answer_chain.py
+-rw-r--r--   0        0        0      567 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/common.py
+-rw-r--r--   0        0        0     3147 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/data_type_detection_chain.py
+-rw-r--r--   0        0        0     3243 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/date_add_chain.py
+-rw-r--r--   0        0        0     2963 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/date_parse_chain.py
+-rw-r--r--   0        0        0     2464 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/timespan_parse_chain.py
+-rw-r--r--   0        0        0     1515 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/config.py
+-rw-r--r--   0        0        0      109 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13516 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     2798 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/history.py
+-rw-r--r--   0        0        0      797 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     4206 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/custom_react_json_single_input.py
+-rw-r--r--   0        0        0     2091 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1075 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/key_finding.py
+-rw-r--r--   0        0        0     1242 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/line_separated_list.py
+-rw-r--r--   0        0        0     2816 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/sql_finding.py
+-rw-r--r--   0        0        0      735 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/text_cleaning.py
+-rw-r--r--   0        0        0     4502 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/timespan.py
+-rw-r--r--   0        0        0      833 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/params.py
+-rw-r--r--   0        0        0      122 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/py.typed
+-rw-r--r--   0        0        0      165 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0     7829 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/retrievers/fused_summary.py
+-rw-r--r--   0        0        0     5472 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/retrievers/mappings.py
+-rw-r--r--   0        0        0      194 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/__init__.py
+-rw-r--r--   0        0        0     3657 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/common.py
+-rw-r--r--   0        0        0     7105 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/reports.py
+-rw-r--r--   0        0        0     6268 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/retrieval.py
+-rw-r--r--   0        0        0      708 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/utils/documents.py
+-rw-r--r--   0        0        0     8975 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/utils/sql.py
+-rw-r--r--   0        0        0     3389 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/utils/string_cleanup.py
+-rw-r--r--   0        0        0     2826 2024-05-04 06:11:45.834605 docugami_langchain-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 docugami_langchain-0.0.8/PKG-INFO
```

### Comparing `docugami_langchain-0.0.7rc9/LICENSE` & `docugami_langchain-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/__init__.py` & `docugami_langchain-0.0.8/docugami_langchain/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from docugami_langchain.agents import __all__ as __all_agents
 from docugami_langchain.base_runnable import __all__ as __all_base_runnable
 from docugami_langchain.chains import __all__ as __all_chains
 from docugami_langchain.document_loaders import __all__ as __all__document_loaders
 from docugami_langchain.output_parsers import __all__ as __all_output_parsers
 from docugami_langchain.params import __all__ as __all_params
 from docugami_langchain.retrievers import __all__ as __all_retrievers
+from docugami_langchain.tools import __all__ as __all_tools
 
 __all__ = (
     __all_base_runnable
     + __all_params
     + __all_agents
     + __all_chains
     + __all__document_loaders
     + __all_output_parsers
     + __all_retrievers
+    + __all_tools
 )
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/agents/rewrite_grader_agent.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/answer_chain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-# Adapted with thanks from https://github.com/langchain-ai/langgraph/blob/main/examples/rag/langgraph_agentic_rag.ipynb
-
 from typing import AsyncIterator, Optional
 
-from langchain_core.runnables import Runnable, RunnableConfig
+from langchain_core.runnables import RunnableConfig
 
-from docugami_langchain.agents.base import BaseDocugamiAgent
 from docugami_langchain.base_runnable import TracedResponse
-from docugami_langchain.params import RunnableParameters
-
+from docugami_langchain.chains.base import BaseDocugamiChain
+from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
 
-class RewriteGraderRAGAgent(BaseDocugamiAgent[dict]):
-    """
-    Agent that implements agentic RAG with the following additional optimizations:
-    1. Query Rewriting
-    2. Retrieval Grading
-    """
 
+class AnswerChain(BaseDocugamiChain[str]):
     def params(self) -> RunnableParameters:
-        raise NotImplementedError()
-
-    def runnable(self) -> Runnable:
-        """
-        Custom runnable for this chain.
-        """
-        raise NotImplementedError()
+        return RunnableParameters(
+            inputs=[
+                RunnableSingleParameter(
+                    "question",
+                    "QUESTION",
+                    "A question from the user.",
+                ),
+            ],
+            output=RunnableSingleParameter(
+                "answer",
+                "ANSWER",
+                "A helpful answer, aligned with the rules outlined above.",
+            ),
+            task_description="answers general questions",
+            additional_instructions=["- Shorter answers are better."],
+            stop_sequences=["CHAT HISTORY:", "QUESTION:", "<|eot_id|>"],
+            key_finding_output_parse=False,  # set to False for streaming
+        )
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> TracedResponse[dict]:
+    ) -> TracedResponse[str]:
         if not question:
             raise Exception("Input required: question")
 
         return super().run(
             question=question,
             config=config,
         )
 
     async def run_stream(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> AsyncIterator[TracedResponse[dict]]:
+    ) -> AsyncIterator[TracedResponse[str]]:
         if not question:
             raise Exception("Input required: question")
 
         async for item in super().run_stream(
             question=question,
             config=config,
         ):
             yield item
 
     def run_batch(  # type: ignore[override]
         self,
         inputs: list[str],
         config: Optional[RunnableConfig] = None,
-    ) -> list[dict]:
+    ) -> list[str]:
         return super().run_batch(
-            inputs=[{"question": i} for i in inputs],
+            inputs=[
+                {
+                    "question": i,
+                }
+                for i in inputs
+            ],
             config=config,
         )
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/__init__.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,52 @@
 from docugami_langchain.chains.answer_chain import AnswerChain
+from docugami_langchain.chains.base import BaseDocugamiChain
 from docugami_langchain.chains.chunks import ElaborateChunkChain, SummarizeChunkChain
-from docugami_langchain.chains.documents import DescribeDocumentSetChain, SummarizeDocumentChain
+from docugami_langchain.chains.documents import (
+    DescribeDocumentSetChain,
+    SummarizeDocumentChain,
+)
 from docugami_langchain.chains.querying import (
     DocugamiExplainedSQLQueryChain,
     SQLFixupChain,
     SQLQueryExplainerChain,
     SQLResultChain,
     SQLResultExplainerChain,
+)
+from docugami_langchain.chains.rag import (
+    SimpleRAGChain,
+    StandaloneQuestionChain,
     SuggestedQuestionsChain,
     SuggestedReportChain,
 )
-from docugami_langchain.chains.rag import SimpleRAGChain
+from docugami_langchain.chains.types import (
+    DataTypeDetectionChain,
+    DataTypes,
+    DateAddChain,
+    DateParseChain,
+    DocugamiDataType,
+    TimespanParseChain,
+)
 
 __all__ = [
     "AnswerChain",
+    "BaseDocugamiChain",
     "ElaborateChunkChain",
     "SummarizeChunkChain",
-    "SummarizeDocumentChain",
     "DescribeDocumentSetChain",
+    "SummarizeDocumentChain",
     "DocugamiExplainedSQLQueryChain",
     "SQLFixupChain",
     "SQLQueryExplainerChain",
     "SQLResultChain",
     "SQLResultExplainerChain",
+    "SimpleRAGChain",
+    "StandaloneQuestionChain",
     "SuggestedQuestionsChain",
     "SuggestedReportChain",
-    "SimpleRAGChain",
+    "DataTypeDetectionChain",
+    "DataTypes",
+    "DocugamiDataType",
+    "DateAddChain",
+    "DateParseChain",
+    "TimespanParseChain",
 ]
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/answer_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,88 @@
+from operator import itemgetter
 from typing import AsyncIterator, Optional
 
-from langchain_core.runnables import RunnableConfig
+from langchain_core.runnables import Runnable, RunnableConfig, RunnableMap
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
-from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
-
+from docugami_langchain.chains.querying.sql_query_explainer_chain import (
+    SQLQueryExplainerChain,
+)
+from docugami_langchain.chains.querying.sql_result_chain import SQLResultChain
+from docugami_langchain.chains.querying.sql_result_explainer_chain import (
+    SQLResultExplainerChain,
+)
+from docugami_langchain.params import RunnableParameters
+
+
+class DocugamiExplainedSQLQueryChain(BaseDocugamiChain[dict]):
+    sql_result_chain: SQLResultChain
+    sql_result_explainer_chain: SQLResultExplainerChain
+    sql_query_explainer_chain: Optional[SQLQueryExplainerChain]
+
+    def runnable(self) -> Runnable:
+        """
+        Custom runnable for this chain.
+        """
+
+        return RunnableMap(
+            {
+                "question": itemgetter("question"),
+                "results": self.sql_result_chain.runnable()
+                | {
+                    "question": itemgetter("question"),
+                    "sql_query": itemgetter("sql_query"),
+                    "sql_result": itemgetter("sql_result"),
+                }
+                | {
+                    "sql_query": itemgetter("sql_query"),
+                    "sql_result": itemgetter("sql_result"),
+                    "explained_sql_result": self.sql_result_explainer_chain.runnable(),
+                    "explained_sql_query": (
+                        self.sql_query_explainer_chain.runnable()
+                        if self.sql_query_explainer_chain
+                        else None
+                    ),
+                },
+            }
+        )
 
-class AnswerChain(BaseDocugamiChain[str]):
     def params(self) -> RunnableParameters:
-        return RunnableParameters(
-            inputs=[
-                RunnableSingleParameter(
-                    "question", "QUESTION", "A question from the user."
-                )
-            ],
-            output=RunnableSingleParameter(
-                "answer",
-                "ANSWER",
-                "A helpful answer, aligned with the rules outlined above",
-            ),
-            task_description="answers general questions",
-            additional_instructions=["- Shorter answers are better."],
-            key_finding_output_parse=False,  # set to False for streaming
-        )
+        raise NotImplementedError()
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> TracedResponse[str]:
+    ) -> TracedResponse[dict]:
         if not question:
             raise Exception("Input required: question")
 
         return super().run(
             question=question,
             config=config,
         )
 
     async def run_stream(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> AsyncIterator[TracedResponse[str]]:
+    ) -> AsyncIterator[TracedResponse[dict]]:
         if not question:
             raise Exception("Input required: question")
 
         async for item in super().run_stream(
             question=question,
             config=config,
         ):
             yield item
 
     def run_batch(  # type: ignore[override]
         self,
         inputs: list[str],
         config: Optional[RunnableConfig] = None,
-    ) -> list[str]:
+    ) -> list[dict]:
         return super().run_batch(
             inputs=[{"question": i} for i in inputs],
             config=config,
         )
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/elaborate_chunk_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 class ElaborateChunkChain(BaseDocugamiChain[str]):
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
                     "contents",
                     "CONTENTS",
-                    "Contents of the chunk that needs to be elaborated",
+                    "Contents of the chunk that needs to be elaborated.",
                 ),
                 RunnableSingleParameter(
                     "format",
                     "FORMAT",
                     "Format of the contents, and expected elaborated output.",
                 ),
             ],
             output=RunnableSingleParameter(
                 "elaboration",
                 "ELABORATION",
                 "Elaboration generated per the given rules.",
             ),
             task_description="elaborates some given text, while minimizing loss of key details",
-            stop_sequences=["CONTENTS:", "FORMAT:"],
+            stop_sequences=["CONTENTS:", "FORMAT:", "<|eot_id|>"],
             additional_instructions=[
                 "- Your generated elaboration should be in the same format as the given document, using the same overall schema.",
                 "- Only elaborate, don't try to change any facts in the chunk even if they appear incorrect to you.",
                 "- Include as many facts and data points from the original chunk as you can, in your elaboration.",
-                "- Pay special attention to key facts like monetary amounts, dates, addresses, names of people and companies, etc and include in your summary.",
+                "- Pay special attention to unique facts like monetary amounts, dates, time durations, addresses, names of people and companies, "
+                "phone numbers, email address, etc and include these in your elaboration to ensure it does not lose semantic value.",
                 "- Aim for the elaboration to be twice as long as the given text. Be as descriptive as possible within these limits.",
             ],
         )
 
     def run(  # type: ignore[override]
         self,
         contents: str,
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/chunks/summarize_chunk_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/documents/summarize_document_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
 from docugami_langchain.config import MIN_LENGTH_TO_SUMMARIZE
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
 
 
-class SummarizeChunkChain(BaseDocugamiChain[str]):
+class SummarizeDocumentChain(BaseDocugamiChain[str]):
     min_length_to_summarize: int = MIN_LENGTH_TO_SUMMARIZE
 
     def runnable(self) -> Runnable:
         """
         Custom runnable for this chain.
         """
         noop = RunnableLambda(lambda x: x["contents"])
@@ -33,35 +33,36 @@
 
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
                     "contents",
                     "CONTENTS",
-                    "Contents of the chunk that needs to be summarized",
+                    "Contents of the doc that needs to be summarized.",
                 ),
                 RunnableSingleParameter(
                     "format",
                     "FORMAT",
                     "Format of the contents, and expected summarized output.",
                 ),
             ],
             output=RunnableSingleParameter(
                 "summary",
                 "SUMMARY",
                 "Summary generated per the given rules.",
             ),
-            task_description="creates a summary of some given text, while minimizing loss of key details",
-            stop_sequences=["CONTENTS:", "FORMAT:"],
+            task_description="creates a summary of a given document, while minimizing loss of key details",
+            stop_sequences=["CONTENTS:", "FORMAT:", "<|eot_id|>"],
             additional_instructions=[
                 "- Your generated summary should be in the same format as the given document, using the same overall schema.",
-                "- The generated summary will be embedded and used to retrieve the raw text or table elements from a vector database.",
-                "- Only summarize, don't try to change any facts in the chunk even if they appear incorrect to you.",
-                "- Include as many facts and data points from the original chunk as you can, in your summary.",
-                "- Pay special attention to key facts like monetary amounts, dates, addresses, names of people and companies, etc and include in your summary.",
+                "- The generated summary should be up to 1 page of text in length, or shorter if the original document is short.",
+                "- Only summarize, don't try to change any facts in the document even if they appear incorrect to you.",
+                "- Include as many facts and data points from the original document as you can, in your summary.",
+                "- Pay special attention to unique facts like monetary amounts, dates, time durations, addresses, names of people and companies, "
+                "phone numbers, email address, etc and include these in your summary to ensure it does not lose semantic value.",
             ],
         )
 
     def run(  # type: ignore[override]
         self,
         contents: str,
         format: Literal["xml", "text"] = "text",
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/describe_document_set_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/documents/describe_document_set_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import AsyncIterator, Optional
 
 from langchain_core.documents import Document
 from langchain_core.runnables import Runnable, RunnableConfig, RunnableLambda
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
-from docugami_langchain.chains.helpers import formatted_summaries
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
+from docugami_langchain.utils.documents import formatted_summaries
 
 
 class DescribeDocumentSetChain(BaseDocugamiChain[str]):
     def runnable(self) -> Runnable:
         """
         Custom runnable for this chain.
         """
@@ -23,26 +23,26 @@
 
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
                     "summaries",
                     "SUMMARIES",
-                    "Summaries of representative documents from a set of documents",
+                    "Summaries of representative documents from a set of documents.",
                 ),
                 RunnableSingleParameter(
                     "docset_name",
                     "DOCSET NAME",
-                    "A user entered description for this type of document",
+                    "A user entered description for this type of document.",
                 ),
             ],
             output=RunnableSingleParameter(
                 "description",
                 "DESCRIPTION",
-                "A short general description of the given document type, using the given summaries as a guide",
+                "A short general description of the given document type, using the given summaries as a guide.",
             ),
             task_description="creates a short description of a document type, given a some sample documents as a guide",
             additional_instructions=[
                 "- Make sure your description is text only, regardless of any markup in the given sample documents.",
                 "- The generated description must apply to all documents of the given type, similar to the sample documents given, not just the exact same document.",
                 "- The generated description will be used to describe this type of document in general in a product. When users ask a question, an AI agent will use the description you produce to "
                 + "decide whether the answer for that question is likely to be found in this type of document or not.",
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/documents/summarize_document_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/chunks/summarize_chunk_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
 from docugami_langchain.config import MIN_LENGTH_TO_SUMMARIZE
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
 
 
-class SummarizeDocumentChain(BaseDocugamiChain[str]):
+class SummarizeChunkChain(BaseDocugamiChain[str]):
     min_length_to_summarize: int = MIN_LENGTH_TO_SUMMARIZE
 
     def runnable(self) -> Runnable:
         """
         Custom runnable for this chain.
         """
         noop = RunnableLambda(lambda x: x["contents"])
@@ -33,35 +33,36 @@
 
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
                     "contents",
                     "CONTENTS",
-                    "Contents of the doc that needs to be summarized",
+                    "Contents of the chunk that needs to be summarized.",
                 ),
                 RunnableSingleParameter(
                     "format",
                     "FORMAT",
                     "Format of the contents, and expected summarized output.",
                 ),
             ],
             output=RunnableSingleParameter(
                 "summary",
                 "SUMMARY",
                 "Summary generated per the given rules.",
             ),
-            task_description="creates a summary of a given document, while minimizing loss of key details",
-            stop_sequences=["CONTENTS:", "FORMAT:"],
+            task_description="creates a summary of some given text, while minimizing loss of key details",
+            stop_sequences=["CONTENTS:", "FORMAT:", "<|eot_id|>"],
             additional_instructions=[
                 "- Your generated summary should be in the same format as the given document, using the same overall schema.",
-                "- The generated summary should be up to 1 page of text in length, or shorter if the original document is short.",
-                "- Only summarize, don't try to change any facts in the document even if they appear incorrect to you.",
-                "- Include as many facts and data points from the original document as you can, in your summary.",
-                "- Pay special attention to key facts like monetary amounts, dates, addresses, names of people and companies, etc and include in your summary.",
+                "- The generated summary will be embedded and used to retrieve the raw text or table elements from a vector database.",
+                "- Only summarize, don't try to change any facts in the chunk even if they appear incorrect to you.",
+                "- Include as many facts and data points from the original chunk as you can, in your summary.",
+                "- Pay special attention to unique facts like monetary amounts, dates, time durations, addresses, names of people and companies, "
+                "phone numbers, email address, etc and include these in your summary to ensure it does not lose semantic value.",
             ],
         )
 
     def run(  # type: ignore[override]
         self,
         contents: str,
         format: Literal["xml", "text"] = "text",
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_fixup_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_fixup_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,66 +21,63 @@
                     "sql_query",
                     "INPUT SQL QUERY",
                     "SQL query with possible mistakes that should be fixed.",
                 ),
                 RunnableSingleParameter(
                     "exception",
                     "EXCEPTION",
-                    "SQL exception returned when executing the SQL query with mistakes.",
+                    "Optional SQL exception that was returned when this SQL query was executed against the table. If not provided, just ignore.",
                 ),
             ],
             output=RunnableSingleParameter(
                 "fixed_sql_query",
                 "FIXED SQL QUERY",
                 "Fixed SQL query, considering the rules and examples provided.",
             ),
             task_description="acts as a SQLite expert and given an input SQL query, fixes common SQL mistakes",
             additional_instructions=[
                 "- Fix data type mismatch in predicates",
                 "- Make sure the correct number of arguments are used for functions",
                 "- Make sure you casting to the correct data type",
                 "- Quote all column names and strings appropriately per SQLite syntax",
+                "- Make sure all column names in SELECT statements actually exist in the table (update column names if you find a near match)",
                 "- Don't select more than 10 columns to avoid making the query so long that it gets truncated",
                 "",
                 "If you see any of the above mistakes, or any other mistakes, rewrite the query to fix them. If there are no mistakes, just reproduce the original query.",
             ],
-            stop_sequences=[
-                "\n",
-                ";",
-                "|",
-            ],
+            stop_sequences=["\n", ";", "<|eot_id|>"],
             additional_runnables=[SQLFindingOutputParser()],
         )
 
     def run(  # type: ignore[override]
         self,
         table_info: str,
         sql_query: str,
-        exception: str,
+        exception: str = "",
         config: Optional[RunnableConfig] = None,
     ) -> TracedResponse[str]:
-        if not table_info or not sql_query or not exception:
-            raise Exception("Inputs required: table_info, sql_query, exception")
+        if not table_info or not sql_query:
+            raise Exception("Inputs required: table_info, sql_query")
 
         return super().run(
             table_info=table_info,
             sql_query=sql_query,
             exception=exception,
             config=config,
         )
 
     async def run_stream(  # type: ignore[override]
         self,
         table_info: str,
         sql_query: str,
-        exception: str,
+        exception: str = "",
         config: Optional[RunnableConfig] = None,
     ) -> AsyncIterator[TracedResponse[str]]:
-        if not table_info or not sql_query or not exception:
-            raise Exception("Inputs required: table_info, sql_query, exception")
+        if not table_info or not sql_query:
+            raise Exception("Inputs required: table_info, sql_query")
 
         async for item in super().run_stream(
             table_info=table_info,
             sql_query=sql_query,
             exception=exception,
             config=config,
         ):
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_query_explainer_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_query_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_chain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,124 @@
 import logging
 from operator import itemgetter
-from typing import Any, AsyncIterator, Optional
+from typing import AsyncIterator, Optional
 
 from langchain_community.utilities.sql_database import SQLDatabase
+from langchain_core.example_selectors import MaxMarginalRelevanceExampleSelector
 from langchain_core.runnables import Runnable, RunnableConfig, RunnableLambda
+from sqlglot import ParseError
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
-from docugami_langchain.chains.helpers import (
-    replace_table_name_in_select,
-    table_name_from_sql_create,
-)
 from docugami_langchain.chains.querying.sql_fixup_chain import SQLFixupChain
 from docugami_langchain.output_parsers.sql_finding import SQLFindingOutputParser
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
+from docugami_langchain.utils.sql import (
+    check_and_format_query,
+    create_example_selector,
+    get_table_info_as_create_table,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class SQLResultChain(BaseDocugamiChain[dict]):
     db: SQLDatabase
+    """The underlying SQL database that is queried by this chain."""
+
     sql_fixup_chain: Optional[SQLFixupChain] = None
+    """A chain used to fix SQL generated by this chain in case of issues."""
+
+    _example_row_selector: Optional[MaxMarginalRelevanceExampleSelector] = None
+
+    def optimize(self) -> None:
+        """
+        Optimizes the database for few shot rows selection. This is optional
+        but recommended. If you don't run optimize, then the first N rows are
+        returned in table info without considering similarity.
+        """
+        if self.embeddings:
+            self._example_row_selector = create_example_selector(
+                self.db, self.embeddings, self.examples_vectorstore_cls
+            )
 
     def runnable(self) -> Runnable:
         """
         Custom runnable for this chain.
         """
 
-        def table_info(_: Any) -> str:
+        def table_info_func(inputs: dict) -> str:
             """
             Return the table info for the database connection for this chain.
             """
-            return self.db.get_table_info()
-
-        def fix_table_name(sql_query: str) -> str:
-            """
-            Attempt to update the table name in the given query, to match the table in the
-            database connection for this chain.
-            """
-            if self.db:
-                try:
-                    table_name = table_name_from_sql_create(self.db.get_table_info())
-                    return replace_table_name_in_select(sql_query, table_name)
-                except Exception as exc:
-                    # Only warn, but continue, since this is best effort
-                    logger.warning(
-                        f"Ignored exception in table name cleanup: {str(exc)}"
-                    )
-                    pass  # nosec
-
-            # Just echo back the input if unable to fix
-            return sql_query
+            question = inputs.get("question")
+            return get_table_info_as_create_table(
+                self.db,
+                question=question,
+                example_selector=self._example_row_selector,
+            )
 
         def run_sql_query(inputs: dict, config: Optional[RunnableConfig]) -> dict:
             """
-            Runs the given query against the database connection for this chain, and returns the result.
+            Runs the given SQL query against the database connection for this chain, and returns the result.
             """
 
             question = inputs.get("question")
             sql_query = inputs.get("sql_query")
+            table_info = table_info_func({"question": question})
 
-            if not question or not sql_query:
-                raise Exception("Inputs required: question, sql_query")
+            if not question or not sql_query or not table_info:
+                raise Exception("Inputs required: question, sql_query, table_info")
 
             try:
-                # Run Raw SQL
+                sql_query = check_and_format_query(self.db, sql_query)
+
+                # Run
                 return {
                     "question": question,
                     "sql_query": sql_query,
                     "sql_result": str(self.db.run(sql_query)).strip(),
                 }
+
             except Exception as exc:
-                is_syntax_error = "syntax error" in str(exc)
+                is_syntax_error = isinstance(exc, ParseError)
+                is_syntax_error = is_syntax_error or "syntax error" in str(exc)
                 is_syntax_error = is_syntax_error or ".OperationalError" in str(exc)
 
                 if is_syntax_error and self.sql_fixup_chain:
                     # If syntax error in Raw SQL, try to fix up the SQL
+                    # giving the LLM context on the exception to aid fixup
                     fixed_sql_response = self.sql_fixup_chain.run(
-                        table_info=table_info(self),
+                        table_info=table_info,
                         sql_query=sql_query,
                         exception=str(exc),
                         config=config,  # Pass the config down to link traces in langsmith
                     )
 
                     # Run Fixed-up SQL
                     fixed_sql = fixed_sql_response.value
+                    fixed_sql = check_and_format_query(self.db, fixed_sql)
+
                     return {
                         "question": question,
                         "sql_query": fixed_sql,
                         "sql_result": str(self.db.run(fixed_sql)).strip(),
                     }
                 else:
                     raise exc
 
         return {
             "question": itemgetter("question"),
             "sql_query": {
                 "question": itemgetter("question"),
-                "table_info": RunnableLambda(table_info),
+                "table_info": RunnableLambda(table_info_func),
             }
             | super().runnable()
-            | SQLFindingOutputParser()
-            | RunnableLambda(fix_table_name),  # type: ignore
-        } | RunnableLambda(
-            run_sql_query  # type: ignore
-        )
+            | SQLFindingOutputParser(),
+        } | RunnableLambda(run_sql_query)
 
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
                     "question",
                     "QUESTION",
@@ -132,24 +142,20 @@
                 '- If the question is ambiguous or you don\'t know how to answer it in the form of a SQL QUERY, just dump the first row of the table i.e. SELECT * FROM "Table Name" LIMIT 1.',
                 "- Unless the user specifies in the question a specific number of examples to obtain, query for at most 5 results using the LIMIT clause as per SQLite.",
                 "- If needed, order the results to return the most informative data in the database.",
                 "- Never query for all columns from a table. You must query only the columns that are needed to answer the question.",
                 '- Wrap each column name in the query in double quotes (") to denote them as delimited identifiers.',
                 "- Pay attention to use only the column names you can see in the given tables. Be careful to not query for columns that do not exist.",
                 "- Pay attention to use the date('now') function to get the current date, if the question involves \"today\".",
-                """- When matching strings in WHERE clauses, always use LIKE with LOWER rather than exact string match with "=" in case the user did not fully specify complete input with the right """
+                """- When matching strings in WHERE clauses, always use LIKE with LOWER rather than exact string match with "=" since users may not fully specify complete input with the right """
                 + """casing, for example generate SELECT * from "athletes" WHERE LOWER("last name") LIKE '%jones%' instead of SELECT * from "athletes" WHERE "last name" = 'Jones'""",
                 "- Never provide any additional explanation or discussion, only output the SQLite query requested, which answers the question against the given table description.",
-                "- Always pay attention to the table name in your query, making sure it exactly matches the table description.",
-            ],
-            stop_sequences=[
-                "\n",
-                ";",
-                "|",
+                "- If example rows are given, pay special attention to them to improve your query e.g. to account for abbreviations or formatting of values.",
             ],
+            stop_sequences=["\n", ";", "<|eot_id|>"],
         )
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
     ) -> TracedResponse[dict]:
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/sql_result_explainer_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_questions_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/types/date_parse_chain.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,63 @@
-from typing import Any, AsyncIterator
-
-from langchain_community.utilities.sql_database import SQLDatabase
-from langchain_core.runnables import Runnable, RunnableLambda
+from datetime import datetime
+from typing import Any, AsyncIterator, Optional
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
-from docugami_langchain.output_parsers.line_separated_list import (
-    LineSeparatedListOutputParser,
-)
+from docugami_langchain.output_parsers.datetime import DatetimeOutputParser
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
 
+OUTPUT_FORMAT = "%m/%d/%Y"
 
-class SuggestedQuestionsChain(BaseDocugamiChain[list[str]]):
-    db: SQLDatabase
-
-    def runnable(self) -> Runnable:
-        """
-        Custom runnable for this chain.
-        """
-
-        def table_info(_: Any) -> str:
-            return self.db.get_table_info()
-
-        return {
-            "table_info": RunnableLambda(table_info),
-        } | super().runnable()
 
+class DateParseChain(BaseDocugamiChain[datetime]):
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
-                    "table_info",
-                    "TABLE DESCRIPTION",
-                    "Description of the table.",
+                    "date_text",
+                    "DATE TEXT",
+                    "The date expression that needs to be parsed, in rough natural language with possible typos or OCR glitches.",
                 ),
             ],
             output=RunnableSingleParameter(
-                "suggested_questions",
-                "SUGGESTED QUESTIONS",
-                "Some suggested questions that may be asked against the table, considering the rules and examples provided.",
+                "parsed_date",
+                "PARSED DATE",
+                f"The result of parsing the date expression, in {OUTPUT_FORMAT} format.",
             ),
-            task_description="acts as a SQLite expert and given a table description, generates some questions a user may want to ask against the table",
+            task_description=f"parses date expressions specified in rough natural language, producing output strictly in the standard {OUTPUT_FORMAT} format",
             additional_instructions=[
-                "- Base your questions only on the columns in the table.",
-                "- Generate the best 4 questions, no more than that.",
-                "- Generate questions as a list, one question per line.",
+                f"- Always produce output as a date in {OUTPUT_FORMAT} format. Never say you cannot do this.",
+                "- The input data will sometimes by messy, with typos or non-standard formats. Try to guess the date as best as you can, by trying to ignore typical typos and OCR glitches.",
+                f"- If the year is not specified, assume current year i.e. {datetime.now().year}",
+                "- If the day is not specified, assume the first of the month.",
+                "- If the date is ambiguous, assume it is the most recent date it could be.",
+                "- If multiple dates are specified, pick the first one.",
+                f"- ONLY output the parsed date expression without any commentary, explanation, or listing any assumptions. Your output must EXACTLY match the required {OUTPUT_FORMAT} format.",
             ],
-            additional_runnables=[LineSeparatedListOutputParser()],
-            stop_sequences=["\n\n", "|"],
-            key_finding_output_parse=False,  # set to False for streaming
+            additional_runnables=[DatetimeOutputParser(format=OUTPUT_FORMAT)],
+            include_output_instruction_suffix=True,
         )
 
     def run(  # type: ignore[override]
-        self,
-    ) -> TracedResponse[list[str]]:
-        return super().run()
+        self, date_text: str, config: Optional[dict] = None
+    ) -> TracedResponse[datetime]:
+        if not date_text:
+            raise Exception("Input required: date_text")
+
+        return super().run(
+            date_text=date_text,
+            config=config,
+        )
 
     async def run_stream(  # type: ignore[override]
-        self,
-    ) -> AsyncIterator[TracedResponse[list[str]]]:
+        self, **kwargs: Any
+    ) -> AsyncIterator[TracedResponse[datetime]]:
         raise NotImplementedError()
 
     def run_batch(  # type: ignore[override]
-        self,
-    ) -> list[list[str]]:
-        raise NotImplementedError()
+        self, inputs: list[str], config: Optional[dict] = None
+    ) -> list[datetime]:
+        return super().run_batch(
+            inputs=[{"date_text": i} for i in inputs],
+            config=config,
+        )
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/querying/suggested_report_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/rag/suggested_report_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,82 +2,93 @@
 from typing import AsyncIterator, Optional
 
 from langchain_core.documents import Document
 from langchain_core.runnables import Runnable, RunnableConfig, RunnableLambda
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
-from docugami_langchain.chains.helpers import formatted_summaries
+from docugami_langchain.history import chat_history_to_str
 from docugami_langchain.output_parsers.line_separated_list import (
     LineSeparatedListOutputParser,
 )
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
+from docugami_langchain.utils.documents import formatted_summaries
 
 
 class SuggestedReportChain(BaseDocugamiChain[list[str]]):
     def runnable(self) -> Runnable:
         """
         Custom runnable for this chain.
         """
 
         return {
             "summaries": itemgetter("summaries") | RunnableLambda(formatted_summaries),
+            "chat_history": itemgetter("chat_history"),
         } | super().runnable()
 
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
                     "summaries",
                     "SUMMARIES",
-                    "Summaries of representative documents from a set of documents",
+                    "Summaries of representative documents from a set of documents.",
+                ),
+                RunnableSingleParameter(
+                    "chat_history",
+                    "CHAT HISTORY",
+                    "Previous chat messages that may provide additional context for the type of columns that should be generated.",
                 ),
             ],
             output=RunnableSingleParameter(
                 "suggested_report_columns",
                 "SUGGESTED REPORT COLUMNS",
-                "Up to 20 suggested columns for an automatically generated report against documents similar to the ones provided.",
+                "Suggested columns for an automatically generated report against documents similar to the ones provided.",
             ),
             task_description="suggests columns for an automatically generated report against a set of documents, given some summaries of representative documents from the set",
             additional_instructions=[
                 "- Generate 'human-like' column labels, i.e. things a human familiar with this particular set of documents might want to know in a diagnostic report about this set of documents",
                 "- Bias towards columns highly likely to be found in all or most of the documents.",
                 "- Avoid columns that are highly likely to contain boilerplate or uninteresting information that is similar for all the documents.",
                 "- Do not include Document Name or File Name in your list, since those are included automatically by the system.",
-                "- Make sure the column names you generate are only alphanumeric, no special characters or parentheses.",
-                "- Generate suggested columns as a list, one per line.",
+                "- Make sure the column names you generate are alphanumeric, containing no special characters or parentheses.",
+                "- Generate up to 20 suggested columns as a list, one per line.",
             ],
             additional_runnables=[LineSeparatedListOutputParser()],
-            stop_sequences=["\n\n", "|"],
+            stop_sequences=["\n\n", "<|eot_id|>"],
             key_finding_output_parse=False,  # set to False for streaming
         )
 
     def run(  # type: ignore[override]
         self,
         summaries: list[Document],
+        chat_history: list[tuple[str, str]] = [],
         config: Optional[RunnableConfig] = None,
     ) -> TracedResponse[list[str]]:
         if not summaries:
             raise Exception("Input required: summaries")
 
         return super().run(
             summaries=summaries,
+            chat_history=chat_history_to_str(chat_history),
             config=config,
         )
 
     async def run_stream(  # type: ignore[override]
         self,
         summaries: list[Document],
+        chat_history: list[tuple[str, str]] = [],
         config: Optional[RunnableConfig] = None,
     ) -> AsyncIterator[TracedResponse[list[str]]]:
         if not summaries:
             raise Exception("Input required: summaries")
 
         async for item in super().run_stream(
             summaries=summaries,
+            chat_history=chat_history_to_str(chat_history),
             config=config,
         ):
             yield item
 
     def run_batch(  # type: ignore[override]
         self,
     ) -> list[list[str]]:
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/chains/rag/simple_rag_chain.py` & `docugami_langchain-0.0.8/docugami_langchain/chains/rag/simple_rag_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,19 @@
                 "ANSWER",
                 "Human readable answer to the question.",
             ),
             task_description="acts as an assistant for question-answering tasks",
             additional_instructions=[
                 "- Use only the given pieces of retrieved context to answer the question, don't make up answers.",
                 "- If you don't know the answer, just say that you don't know.",
-                "- Use three sentences maximum and keep the answer concise.",
+                "- Your answer should be concise, up to three sentences long.",
             ],
+            stop_sequences=["<|eot_id|>"],
             key_finding_output_parse=False,  # set to False for streaming
+            include_output_instruction_suffix=True,
         )
 
     def runnable(self) -> Runnable:
         """
         Custom runnable for this agent.
         """
 
@@ -84,10 +86,15 @@
 
     def run_batch(  # type: ignore[override]
         self,
         inputs: list[str],
         config: Optional[RunnableConfig] = None,
     ) -> list[str]:
         return super().run_batch(
-            inputs=[{"question": i} for i in inputs],
+            inputs=[
+                {
+                    "question": i,
+                }
+                for i in inputs
+            ],
             config=config,
         )
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/document_loaders/docugami.py` & `docugami_langchain-0.0.8/docugami_langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/__init__.py` & `docugami_langchain-0.0.8/docugami_langchain/output_parsers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from docugami_langchain.output_parsers.custom_react_json_single_input import (
+    CustomReActJsonSingleInputOutputParser,
+)
 from docugami_langchain.output_parsers.key_finding import KeyfindingOutputParser
 from docugami_langchain.output_parsers.line_separated_list import (
     LineSeparatedListOutputParser,
 )
-from docugami_langchain.output_parsers.soft_react_json_single_input import (
-    SoftReActJsonSingleInputOutputParser,
-)
 from docugami_langchain.output_parsers.sql_finding import SQLFindingOutputParser
+from docugami_langchain.output_parsers.text_cleaning import TextCleaningOutputParser
 from docugami_langchain.output_parsers.timespan import TimeSpan, TimespanOutputParser
 
 __all__ = [
     "KeyfindingOutputParser",
     "LineSeparatedListOutputParser",
-    "SoftReActJsonSingleInputOutputParser",
+    "CustomReActJsonSingleInputOutputParser",
     "SQLFindingOutputParser",
+    "TextCleaningOutputParser",
     "TimeSpan",
     "TimespanOutputParser",
 ]
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/key_finding.py` & `docugami_langchain-0.0.8/docugami_langchain/output_parsers/key_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/line_separated_list.py` & `docugami_langchain-0.0.8/docugami_langchain/output_parsers/line_separated_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import re
 
 from langchain_core.output_parsers.list import ListOutputParser
 
+from docugami_langchain.utils.string_cleanup import clean_text
+
 
 class LineSeparatedListOutputParser(ListOutputParser):
     """Parse the output of an LLM call as a line-separated list."""
 
     strip_ordinals: bool = True
     """Indicates whether list ordinals should be stripped"""
 
@@ -16,14 +18,20 @@
     def _type(self) -> str:
         """Snake-case string identifier for an output parser type."""
         return "line_separated_list_output_parser"
 
     def parse(self, text: str) -> list[str]:
         """Parse the output of an LLM call."""
 
+        text = text.strip()
+        if not text:
+            return []
+
+        text = clean_text(text)
+
         if self.ignore_pleasantry and "\n" in text and text.startswith("Sure"):
             # remove any pleasantries header
             text = "\n".join(text.splitlines()[1:])
 
         items = []
         for line in text.splitlines():
             if self.strip_ordinals:
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/sql_finding.py` & `docugami_langchain-0.0.8/docugami_langchain/output_parsers/sql_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/output_parsers/timespan.py` & `docugami_langchain-0.0.8/docugami_langchain/output_parsers/timespan.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/params.py` & `docugami_langchain-0.0.8/docugami_langchain/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,10 +19,11 @@
     output: RunnableSingleParameter
     task_description: str
     additional_instructions: list[str] = field(default_factory=lambda: [])
     stop_sequences: list[str] = field(default_factory=lambda: ["\n"])
     num_examples: int = DEFAULT_EXAMPLES_PER_PROMPT
     additional_runnables: Optional[list[Runnable]] = None
     key_finding_output_parse: bool = True
+    include_output_instruction_suffix: bool = False
 
 
 __all__ = ["RunnableSingleParameter", "RunnableParameters"]
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/retrievers/mappings.py` & `docugami_langchain-0.0.8/docugami_langchain/retrievers/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from pathlib import Path
 from typing import Optional, Union
 
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
 
-from docugami_langchain.chains import (
-    SummarizeChunkChain,
-    SummarizeDocumentChain,
-)
+from docugami_langchain.chains import SummarizeChunkChain, SummarizeDocumentChain
 from docugami_langchain.config import (
     INCLUDE_XML_TAGS,
     MAX_CHUNK_TEXT_LENGTH,
     MAX_FULL_DOCUMENT_TEXT_LENGTH,
     MIN_LENGTH_TO_SUMMARIZE,
 )
 from docugami_langchain.retrievers.fused_summary import (
@@ -119,24 +116,23 @@
     # Build separate maps of chunks, and parents
     parent_chunks_by_id: dict[str, Document] = {}
     chunks_by_source: dict[str, list[str]] = {}
     for chunk in chunks:
         chunk_id = str(chunk.metadata.get(chunk_id_key))
         chunk_source = str(chunk.metadata.get(source_key))
         parent_chunk_id = chunk.metadata.get(parent_id_key)
+
+        if chunk_source not in chunks_by_source:
+            chunks_by_source[chunk_source] = []
+
+        chunks_by_source[chunk_source].append(chunk.page_content)
+
         if not parent_chunk_id:
             # parent chunk, we will use this (for expanded context) as our chunk
             parent_chunks_by_id[chunk_id] = chunk
-        else:
-            # child chunk, we will keep track of this to build up our
-            # full document summary
-            if chunk_source not in chunks_by_source:
-                chunks_by_source[chunk_source] = []
-
-            chunks_by_source[chunk_source].append(chunk.page_content)
 
     # Build up the full docs by concatenating all the child chunks from a source
     full_docs_by_id: dict[str, Document] = {}
     full_doc_ids_by_source: dict[str, str] = {}
     for source in chunks_by_source:
         chunks_from_source = chunks_by_source[source]
         full_doc_text = "\n".join([c for c in chunks_from_source])
```

### Comparing `docugami_langchain-0.0.7rc9/docugami_langchain/tools/reports.py` & `docugami_langchain-0.0.8/docugami_langchain/tools/retrieval.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,168 @@
 import re
-import sqlite3
-import tempfile
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional
 
-import pandas as pd
-from langchain_community.tools.sql_database.tool import BaseSQLDatabaseTool
-from langchain_community.utilities.sql_database import SQLDatabase
 from langchain_core.callbacks import CallbackManagerForToolRun
+from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
-from langchain_core.tools import BaseTool
+from langchain_core.runnables import RunnableConfig
+from langchain_core.vectorstores import VectorStore
+from rerankers.models.ranker import BaseRanker
+
+from docugami_langchain.agents.models import Invocation
+from docugami_langchain.chains.documents.describe_document_set_chain import (
+    DescribeDocumentSetChain,
+)
+from docugami_langchain.chains.rag.simple_rag_chain import SimpleRAGChain
+from docugami_langchain.config import DEFAULT_RETRIEVER_K, MAX_FULL_DOCUMENT_TEXT_LENGTH
+from docugami_langchain.retrievers.fused_summary import (
+    FULL_DOC_SUMMARY_ID_KEY,
+    FusedRetrieverKeyValueFetchCallback,
+    FusedSummaryRetriever,
+    SearchType,
+)
+from docugami_langchain.tools.common import NOT_FOUND, BaseDocugamiTool
 
-from docugami_langchain.chains.querying.sql_fixup_chain import SQLFixupChain
-from docugami_langchain.chains.querying.sql_result_chain import SQLResultChain
 
+class CustomDocsetRetrievalTool(BaseDocugamiTool):
+    """A Tool that knows how to do retrieval over a docset."""
 
-class CustomReportRetrievalTool(BaseSQLDatabaseTool, BaseTool):
-    db: SQLDatabase
-    chain: SQLResultChain
-    name: str = "query_report"
+    chain: SimpleRAGChain
+    name: str = "document_answer_tool"
     description: str = ""
 
+    def to_human_readable(self, invocation: Invocation) -> str:
+        """Converts tool invocation to human readable string."""
+        return f"Searching documents: {invocation.tool_input}"
+
     def _run(
         self,
         question: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:  # type: ignore
         """Use the tool."""
-        chain_response = self.chain.run(question=question)
-        if chain_response.value:
-            sql_result = chain_response.value.get("sql_result")
-            if sql_result:
-                return str(sql_result)
 
-        return ""
+        if not question:
+            return "Please specify a question that you want to answer from this docset"
+
+        try:
+            config = None
+            if run_manager:
+                config = RunnableConfig(
+                    run_name=self.__class__.__name__,
+                    callbacks=run_manager,
+                )
+            chain_response = self.chain.run(
+                question=question,
+                config=config,
+            )
+            if chain_response.value:
+                return chain_response.value
+
+            return NOT_FOUND
+        except Exception as exc:
+            return f"There was an error. Please try a different question, or a different tool. Details: {exc}"
 
 
-def report_name_to_report_query_tool_function_name(name: str) -> str:
+def docset_name_to_direct_retrieval_tool_function_name(name: str) -> str:
     """
-    Converts a report name to a report query tool function name.
+    Converts a docset name to a direct retriever tool function name.
 
-    Report query tool function names follow these conventions:
-    1. Retrieval tool function names always start with "query_".
+    Direct retriever tool function names follow these conventions:
+    1. Retrieval tool function names always start with "document_answer_tool".
     2. The rest of the name should be a lowercased string, with underscores
        for whitespace.
-    3. Exclude any characters other than a-z (lowercase) from the function name,
-       replacing them with underscores.
+    3. Exclude any characters other than a-z (lowercase) from the function
+       name, replacing them with underscores.
     4. The final function name should not have more than one underscore together.
 
-    >>> report_name_to_report_query_tool_function_name('Earnings Calls')
-    'query_earnings_calls'
-    >>> report_name_to_report_query_tool_function_name('COVID-19   Statistics')
-    'query_covid_19_statistics'
-    >>> report_name_to_report_query_tool_function_name('2023 Market Report!!!')
-    'query_2023_market_report'
+    >>> docset_name_to_direct_retrieval_tool_function_name('Earnings Calls')
+    'document_answer_tool_earnings_calls'
+    >>> docset_name_to_direct_retrieval_tool_function_name('COVID-19   Statistics')
+    'document_answer_tool_covid_19_statistics'
+    >>> docset_name_to_direct_retrieval_tool_function_name('2023 Market Report!!!')
+    'document_answer_tool_2023_market_report'
     """
     # Replace non-letter characters with underscores and remove extra whitespaces
     name = re.sub(r"[^a-z\d]", "_", name.lower())
     # Replace whitespace with underscores and remove consecutive underscores
     name = re.sub(r"\s+", "_", name)
     name = re.sub(r"_{2,}", "_", name)
     name = name.strip("_")
 
-    return f"query_{name}"
+    return f"document_answer_tool_{name}"
 
 
-def report_details_to_report_query_tool_description(name: str, table_info: str) -> str:
-    """
-    Converts a set of chunks to a direct retriever tool description.
-    """
-    table_info = re.sub(r"\s+", " ", table_info)
-    description = (
-        f"Given a single input 'question' parameter, generates and runs a SQL query over the {name}"
-        + f" report, represented internally as the following SQL Table:\n\n{table_info}"
+def docset_details_to_direct_retrieval_tool_description(
+    name: str, description: str
+) -> str:
+    return (
+        "Pass the COMPLETE question as input to this tool."
+        + f"It implements logic to to answer questions based on information in {name} documents and outputs only the answer to your question. "
+        + "Use this tool if you think the answer is likely to come from one or a few of these documents. "
+        + description
     )
 
-    return description[:2048]  # cap to avoid failures when the description is too long
-
 
-def excel_to_sqlite_connection(
-    file_path: Union[Path, str], table_name: str
-) -> sqlite3.Connection:
-    # Create a temporary SQLite database in memory
-    conn = sqlite3.connect(":memory:")
-
-    # Verify the file path
-    file_path = Path(file_path)
-    if not (file_path.exists() and file_path.suffix.lower() == ".xlsx"):
-        raise Exception(f"Invalid file path: {file_path}")
-
-    # Read the Excel file using pandas (only the first sheet)
-    df = pd.read_excel(file_path, sheet_name=0)
-
-    # Write the table to the SQLite database
-    df.to_sql(table_name, conn, if_exists="replace", index=False)
-
-    return conn
-
-
-def connect_to_db(
-    conn: sqlite3.Connection,
-    sample_rows_in_table_info: int = 0,
-) -> SQLDatabase:
-    temp_db_file = tempfile.NamedTemporaryFile(suffix=".sqlite")
-    with sqlite3.connect(temp_db_file.name) as disk_conn:
-        conn.backup(disk_conn)  # dumps the connection to disk
-    return SQLDatabase.from_uri(
-        f"sqlite:///{temp_db_file.name}",
-        sample_rows_in_table_info=sample_rows_in_table_info,
-    )
+def summaries_to_direct_retrieval_tool_description(
+    name: str,
+    summaries: list[Document],
+    llm: BaseLanguageModel,
+    embeddings: Embeddings,
+    max_sample_documents_cutoff_length: int = MAX_FULL_DOCUMENT_TEXT_LENGTH,
+    describe_document_set_examples_file: Optional[Path] = None,
+) -> str:
+    """
+    Converts a set of chunks to a direct retriever tool description.
+    """
+    chain = DescribeDocumentSetChain(llm=llm, embeddings=embeddings)
+    chain.input_params_max_length_cutoff = max_sample_documents_cutoff_length
+    if describe_document_set_examples_file:
+        chain.load_examples(describe_document_set_examples_file)
 
+    description = chain.run(summaries=summaries, docset_name=name)
 
-def connect_to_excel(file_path: Union[Path, str], table_name: str) -> SQLDatabase:
-    return connect_to_db(excel_to_sqlite_connection(file_path, table_name))
+    return docset_details_to_direct_retrieval_tool_description(name, description.value)
 
 
-def get_retrieval_tool_for_report(
-    local_xlsx_path: Path,
-    report_name: str,
+def get_retrieval_tool_for_docset(
+    chunk_vectorstore: VectorStore,
     retrieval_tool_function_name: str,
     retrieval_tool_description: str,
-    sql_llm: BaseLanguageModel,
+    llm: BaseLanguageModel,
     embeddings: Embeddings,
-    sql_fixup_examples_file: Optional[Path] = None,
-    sql_examples_file: Optional[Path] = None,
-) -> Optional[BaseTool]:
-    if not local_xlsx_path.exists():
-        return None
-
-    db = connect_to_excel(local_xlsx_path, report_name)
-
-    fixup_chain = SQLFixupChain(llm=sql_llm, embeddings=embeddings)
-    if sql_fixup_examples_file:
-        fixup_chain.load_examples(sql_fixup_examples_file)
+    re_ranker: Optional[BaseRanker] = None,
+    fetch_full_doc_summary_callback: Optional[
+        FusedRetrieverKeyValueFetchCallback
+    ] = None,
+    fetch_parent_doc_callback: Optional[FusedRetrieverKeyValueFetchCallback] = None,
+    retrieval_k: int = DEFAULT_RETRIEVER_K,
+    full_doc_summary_id_key: str = FULL_DOC_SUMMARY_ID_KEY,
+) -> Optional[BaseDocugamiTool]:
+    """
+    Gets a retrieval tool for an agent.
+    """
 
-    sql_result_chain = SQLResultChain(
-        llm=sql_llm,
-        embeddings=embeddings,
-        db=db,
-        sql_fixup_chain=fixup_chain,
+    # Instantiate FusedSummaryRetriever with callback functions
+    retriever = FusedSummaryRetriever(
+        vectorstore=chunk_vectorstore,
+        re_ranker=re_ranker,
+        fetch_parent_doc_callback=fetch_parent_doc_callback,
+        full_doc_summary_id_key=full_doc_summary_id_key,
+        fetch_full_doc_summary_callback=fetch_full_doc_summary_callback,
+        retriever_k=retrieval_k,
+        search_type=SearchType.mmr,
     )
 
-    if sql_examples_file:
-        sql_result_chain.load_examples(sql_examples_file)
+    simple_rag_chain = SimpleRAGChain(
+        llm=llm,
+        embeddings=embeddings,
+        retriever=retriever,
+    )
 
-    return CustomReportRetrievalTool(
-        db=db,
-        chain=sql_result_chain,
+    return CustomDocsetRetrievalTool(
+        chain=simple_rag_chain,
         name=retrieval_tool_function_name,
         description=retrieval_tool_description,
-        return_direct=True,
     )
```

### Comparing `docugami_langchain-0.0.7rc9/pyproject.toml` & `docugami_langchain-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 [tool.poetry]
 name = "docugami-langchain"
-version = "0.0.7rc9"
+version = "0.0.8"
 description = "An integration package connecting Docugami and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/docugami/docugami-langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/docugami/docugami-langchain/tree/master"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain-core = ">=0.1.28"
-langchain-community = ">=0.0.25"
-langgraph = ">=0.0.26"
-dgml-utils = ">=0.3.2"
+langchain-core = ">=0.1.48"
+langchain-community = ">=0.0.36"
+langgraph = ">=0.0.39"
+dgml-utils = ">=0.3.3"
 wordtodigits = ">=1.0.2"
 python-dateutil = ">=2.9.0"
-pandas = ">=2.2.1"
+pandas = ">=2.2.2"
 pyyaml = ">=6.0.1"
 openpyxl = ">=3.1.2"
-sqlparse = ">=0.4.4"
+sqlglot = ">=23.12.2"
+tabulate = ">=0.9.0"
+rerankers = { extras = ["all"], version = ">=0.2.0" }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = ">=8.0.2"
-pytest-mock = ">=3.12.0"
-pytest-watcher = ">=0.4.1"
-pytest-asyncio = ">=0.23.5"
-sentence-transformers = ">=2.5.1"
-langchain-openai = ">=0.0.8"
-langchain-fireworks = ">=0.1.1"
+flaky = "^3.8.1"
+pytest = ">=8.1.1"
+pytest-mock = ">=3.14.0"
+pytest-watcher = ">=0.4.2"
+pytest-asyncio = ">=0.23.6"
+sentence-transformers = ">=2.7.0"
+langchain-openai = ">=0.1.3"
+langchain-fireworks = ">=0.1.2"
 faiss-cpu = ">=1.8.0"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = ">=2.2.6"
@@ -47,37 +50,40 @@
 
 [tool.poetry.group.test_integration.dependencies]
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
-ruff = ">=0.3.0"
+ruff = ">=0.4.1"
 
 [tool.poetry.group.typing.dependencies]
-mypy = ">=1.8.0"
-types-lxml = ">=2024.2.9"
-types-python-dateutil = ">=2.8.19.20240106"
-types-pyyaml = ">=6.0.12.12"
-types-requests = ">=2.31.0.20240218"
+mypy = ">=1.10.0"
+types-lxml = ">=2024.4.14"
+types-python-dateutil = ">=2.9.0.20240316"
+types-pyyaml = ">=6.0.12.20240311"
+types-requests = ">=2.31.0.20240406"
+types-regex = ">=2024.4.16.20240423"
+types-tabulate = ">=0.9.0.20240106"
 
 [tool.ruff]
 lint.select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
 ]
 line-length = 200
 
 [tool.mypy]
 disallow_untyped_defs = "True"
+disable_error_code = "typeddict-item"
 
 [[tool.mypy.overrides]]
 module = [
-    "wordtodigits", "pandas", "sqlparse", "langgraph.*",
+    "wordtodigits", "pandas", "langgraph.*", "rerankers.*", "flaky",
 ]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 omit = [
     "tests/*",
 ]
```

### Comparing `docugami_langchain-0.0.7rc9/PKG-INFO` & `docugami_langchain-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: docugami-langchain
-Version: 0.0.7rc9
+Version: 0.0.8
 Summary: An integration package connecting Docugami and LangChain
 Home-page: https://github.com/docugami/docugami-langchain
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: dgml-utils (>=0.3.2)
-Requires-Dist: langchain-community (>=0.0.25)
-Requires-Dist: langchain-core (>=0.1.28)
-Requires-Dist: langgraph (>=0.0.26)
+Requires-Dist: dgml-utils (>=0.3.3)
+Requires-Dist: langchain-community (>=0.0.36)
+Requires-Dist: langchain-core (>=0.1.48)
+Requires-Dist: langgraph (>=0.0.39)
 Requires-Dist: openpyxl (>=3.1.2)
-Requires-Dist: pandas (>=2.2.1)
+Requires-Dist: pandas (>=2.2.2)
 Requires-Dist: python-dateutil (>=2.9.0)
 Requires-Dist: pyyaml (>=6.0.1)
-Requires-Dist: sqlparse (>=0.4.4)
+Requires-Dist: rerankers[all] (>=0.2.0)
+Requires-Dist: sqlglot (>=23.12.2)
+Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: wordtodigits (>=1.0.2)
 Project-URL: Repository, https://github.com/docugami/docugami-langchain
 Project-URL: Source Code, https://github.com/docugami/docugami-langchain/tree/master
 Description-Content-Type: text/markdown
 
 # docugami-langchain
 
@@ -37,8 +39,8 @@
 
 To install with poetry:
 
 `poetry add docugami-langchain`
 
 ## Development and Testing
 
-To install with development and testing dependencies, install as `poetry install --with test,lint,typing`.
+To install with development and testing dependencies, install as `poetry install --with test,lint,typing,codespell`.
```

