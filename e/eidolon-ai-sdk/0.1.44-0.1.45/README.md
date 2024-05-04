# Comparing `tmp/eidolon_ai_sdk-0.1.44.tar.gz` & `tmp/eidolon_ai_sdk-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.44.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.45.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.44.tar` & `eidolon_ai_sdk-0.1.45.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0     2569 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/README.md
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2429 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0     1311 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/audio_agent.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3025 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2710 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1434 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2329 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2864 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3717 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    13009 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1815 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     8381 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     9079 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.734536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     1823 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
--rw-r--r--   0        0        0     6440 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      601 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      614 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      597 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      595 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      586 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4638 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2562 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     9033 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     3718 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14295 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     4680 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5753 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9490 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3567 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3962 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     2421 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4477 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      974 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    23002 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14196 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4911 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6917 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-05-02 05:37:22.738536 eidolon_ai_sdk-0.1.44/logging.conf
--rw-r--r--   0        0        0     2204 2024-05-02 05:37:22.742536 eidolon_ai_sdk-0.1.44/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.44/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2429 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0     1311 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/audio_agent.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1434 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2329 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3717 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    13009 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1815 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     8381 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9079 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     1823 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
+-rw-r--r--   0        0        0     6440 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-05-03 17:57:37.333932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      586 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4638 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2562 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     9083 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     3718 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14295 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4680 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5753 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9490 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3567 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     2421 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4477 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    23002 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14196 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4911 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6917 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-05-03 17:57:37.337932 eidolon_ai_sdk-0.1.45/logging.conf
+-rw-r--r--   0        0        0     2204 2024-05-03 17:57:37.341932 eidolon_ai_sdk-0.1.45/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.45/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.44/README.md` & `eidolon_ai_sdk-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/audio_agent.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/audio_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 from collections import defaultdict
 
 from pydantic import BaseModel
 from typing import List, Any, Dict, AsyncIterator, Set
 
-from eidolon_ai_client.client import Machine, Agent, AgentResponseIterator
+from eidolon_ai_client.client import Machine, Agent, AgentResponseIterator, Process
 from eidolon_ai_sdk.cpu.agent_call_history import AgentCallHistory
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.logic_unit import LogicUnit
 from eidolon_ai_client.events import StreamEvent, ObjectOutputEvent
 from eidolon_ai_sdk.system.fn_handler import FnHandler
 from eidolon_ai_sdk.system.reference_model import Specable
 from eidolon_ai_client.util.logger import logger
@@ -178,15 +178,15 @@
 
     # todo, this needs to create history record before iterating
     def _process_tool(self, agent: Agent, action: str, allowed_pids: Set[str], call_context: CallContext):
         def fn(_self, conversation_id: str, body):
             if conversation_id not in allowed_pids:
                 raise ValueError(f"Conversation id {conversation_id} not allowed for action {action}")
             return RecordAgentResponseIterator(
-                agent.process(conversation_id).stream_action(action, body), call_context.process_id, call_context.thread_id
+                Process(machine=agent.machine, process_id=conversation_id).stream_action(agent.agent, action, body), call_context.process_id, call_context.thread_id
             )
 
         return fn
 
 
 # todo, it would be nice to work this into the client automatically
 class RecordAgentResponseIterator(AgentResponseIterator):
```

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.45/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/logging.conf` & `eidolon_ai_sdk-0.1.45/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.44/pyproject.toml` & `eidolon_ai_sdk-0.1.45/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.44"
+version = "0.1.45"
 description = "An Open Source Agent Services Framework"
 authors = [ "Luke Lalor <lukehlalor@gmail.com>",]
 readme = "README.md"
 include = [ "logging.conf",]
 
 [tool.ruff]
 line-length = 121
 
 [tool.eidolon]
 update-tag = "sdk"
-last-update-hash = "325c68e5b44c82bfe8ec088c9932910da86868a3"
+last-update-hash = "f1d98f85339c3a6390fbd9851e75d6fc7e06d3c3"
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
 Website = "https://www.eidolonai.com/"
 
 [tool.poetry.scripts]
 eidolon-server = "eidolon_ai_sdk.bin.agent_http_server:main"
@@ -57,15 +57,15 @@
 httpx-sse = "^0.4.0"
 sse-starlette = "^2.0.0"
 dill = "^0.3.8"
 opentelemetry-instrumentation-fastapi = "^0.44b0"
 opentelemetry-instrumentation-logging = "^0.44b0"
 opentelemetry-sdk = "^1.23.0"
 eidolon-ai-mistralai = "^0.1.6a"
-eidolon-ai-client = "^0.1.12"
+eidolon-ai-client = "^0.1.13"
 eidolon-ai-usage-client = "^0.1.6"
 boto3 = "^1.34.74"
 azure-identity = "^1.16.0"
 playwright = "^1.43.0"
 
 [tool.pytest.ini_options]
 pythonpath = "project"
```

### Comparing `eidolon_ai_sdk-0.1.44/PKG-INFO` & `eidolon_ai_sdk-0.1.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.44
+Version: 0.1.45
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0)
 Requires-Dist: boto3 (>=1.34.74,<2.0.0)
 Requires-Dist: boto3-stubs[essential] (>=1.34.74,<2.0.0)
 Requires-Dist: chromadb (>=0.4.18,<0.5.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: eidolon-ai-client (>=0.1.12,<0.2.0)
+Requires-Dist: eidolon-ai-client (>=0.1.13,<0.2.0)
 Requires-Dist: eidolon-ai-mistralai (>=0.1.6a,<0.2.0)
 Requires-Dist: eidolon-ai-usage-client (>=0.1.6,<0.2.0)
 Requires-Dist: esprima (>=4.0.1,<5.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
```

