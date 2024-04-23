# Comparing `tmp/ipex_llm-2.1.0b20240421-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240422-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5348037 bytes, number of entries: 218
+Zip file size: 5263605 bytes, number of entries: 186
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3091 b- defN 24-Apr-17 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,71 +38,71 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-Apr-21 15:08 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Apr-21 15:08 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   460288 b- defN 24-Apr-21 15:08 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   852992 b- defN 24-Apr-21 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856064 b- defN 24-Apr-21 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   843776 b- defN 24-Apr-21 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-Apr-21 15:08 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   520192 b- defN 24-Apr-21 15:08 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   485888 b- defN 24-Apr-21 15:08 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   460800 b- defN 24-Apr-21 15:08 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   545792 b- defN 24-Apr-21 15:08 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   520704 b- defN 24-Apr-21 15:08 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   540160 b- defN 24-Apr-21 15:08 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   515072 b- defN 24-Apr-21 15:08 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   577024 b- defN 24-Apr-21 15:08 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   551936 b- defN 24-Apr-21 15:08 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Apr-21 15:08 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   514560 b- defN 24-Apr-21 15:08 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Apr-21 15:08 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   125952 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128000 b- defN 24-Apr-21 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Apr-21 15:08 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   551424 b- defN 24-Apr-21 15:08 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-Apr-22 15:08 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-Apr-22 15:08 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   460288 b- defN 24-Apr-22 15:08 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   852992 b- defN 24-Apr-22 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856064 b- defN 24-Apr-22 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   843776 b- defN 24-Apr-22 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-Apr-22 15:08 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   520192 b- defN 24-Apr-22 15:08 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   485888 b- defN 24-Apr-22 15:08 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   460800 b- defN 24-Apr-22 15:08 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   545792 b- defN 24-Apr-22 15:08 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   520704 b- defN 24-Apr-22 15:08 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   540160 b- defN 24-Apr-22 15:08 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   515072 b- defN 24-Apr-22 15:08 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   577024 b- defN 24-Apr-22 15:08 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   551936 b- defN 24-Apr-22 15:08 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-Apr-22 15:08 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   514560 b- defN 24-Apr-22 15:08 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-Apr-22 15:08 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-Apr-22 15:08 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-Apr-22 15:08 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-Apr-22 15:08 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-Apr-22 15:08 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   125952 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128000 b- defN 24-Apr-22 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-Apr-22 15:08 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   551424 b- defN 24-Apr-22 15:08 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    11371 b- defN 24-Mar-27 11:49 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
--rw-------  2.0 unx     8692 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/vllm_worker.py
+-rw-------  2.0 unx    11232 b- defN 24-Apr-22 15:07 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    69847 b- defN 24-Apr-18 12:34 ipex_llm/transformers/convert.py
--rw-------  2.0 unx    14274 b- defN 24-Apr-07 15:05 ipex_llm/transformers/convert_ipex.py
+-rw-------  2.0 unx    70437 b- defN 24-Apr-22 15:07 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    14334 b- defN 24-Apr-22 15:07 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4533 b- defN 24-Apr-03 15:07 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     3289 b- defN 24-Apr-18 12:34 ipex_llm/transformers/lisa.py
 -rw-------  2.0 unx     5429 b- defN 24-Mar-25 11:36 ipex_llm/transformers/loader.py
--rw-------  2.0 unx    14719 b- defN 24-Apr-17 15:07 ipex_llm/transformers/lookup.py
+-rw-------  2.0 unx    14775 b- defN 24-Apr-22 15:07 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    38388 b- defN 24-Apr-18 12:34 ipex_llm/transformers/low_bit_linear.py
 -rw-------  2.0 unx    36157 b- defN 24-Apr-18 12:34 ipex_llm/transformers/model.py
 -rw-------  2.0 unx     6921 b- defN 24-Mar-25 11:36 ipex_llm/transformers/modelling_bigdl.py
 -rw-------  2.0 unx    14770 b- defN 24-Mar-25 11:36 ipex_llm/transformers/qlora.py
 -rw-------  2.0 unx    16567 b- defN 24-Mar-25 11:36 ipex_llm/transformers/relora.py
--rw-------  2.0 unx    55517 b- defN 24-Apr-19 15:09 ipex_llm/transformers/speculative.py
+-rw-------  2.0 unx    55625 b- defN 24-Apr-22 15:07 ipex_llm/transformers/speculative.py
 -rw-------  2.0 unx     8404 b- defN 24-Mar-25 11:36 ipex_llm/transformers/training_patch.py
 -rw-------  2.0 unx    13931 b- defN 24-Apr-18 12:34 ipex_llm/transformers/utils.py
 -rw-------  2.0 unx     7611 b- defN 24-Mar-25 11:36 ipex_llm/transformers/xpu_customize_fwd.py
 -rw-------  2.0 unx      875 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/__init__.py
 -rw-------  2.0 unx     2172 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/act.py
 -rw-------  2.0 unx     8861 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq.py
 -rw-------  2.0 unx     4422 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq_config.py
@@ -146,14 +146,15 @@
 -rw-------  2.0 unx    17973 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptj.py
 -rw-------  2.0 unx     6219 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptneox.py
 -rw-------  2.0 unx    11647 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/internlm.py
 -rw-------  2.0 unx    97385 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/llama.py
 -rw-------  2.0 unx    45181 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/mistral.py
 -rw-------  2.0 unx    27273 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/mixtral.py
 -rw-------  2.0 unx     9540 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mpt.py
+-rw-------  2.0 unx     7685 b- defN 24-Apr-22 15:07 ipex_llm/transformers/models/phi.py
 -rw-------  2.0 unx     6268 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/phixtral.py
 -rw-------  2.0 unx    32349 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen.py
 -rw-------  2.0 unx    32725 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen2.py
 -rw-------  2.0 unx    30334 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen2_moe.py
 -rw-------  2.0 unx    11832 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen_vl.py
 -rw-------  2.0 unx     6135 b- defN 24-Mar-29 11:38 ipex_llm/transformers/models/rwkv4.py
 -rw-------  2.0 unx    10722 b- defN 24-Apr-09 15:06 ipex_llm/transformers/models/rwkv5.py
@@ -168,53 +169,20 @@
 -rw-------  2.0 unx     2477 b- defN 24-Mar-25 11:36 ipex_llm/utils/ipex_importer.py
 -rw-------  2.0 unx     2259 b- defN 24-Mar-25 11:36 ipex_llm/utils/isa_checker.py
 -rw-------  2.0 unx     7129 b- defN 24-Mar-25 11:36 ipex_llm/utils/lazy_load_torch.py
 -rw-------  2.0 unx     1556 b- defN 24-Mar-25 11:36 ipex_llm/utils/utils.py
 -rw-------  2.0 unx      988 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/__init__.py
 -rw-------  2.0 unx     2872 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/lazyimport.py
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
--rw-------  2.0 unx    16868 b- defN 24-Apr-07 15:05 ipex_llm/vllm/config.py
--rw-------  2.0 unx     2801 b- defN 24-Mar-25 11:36 ipex_llm/vllm/logger.py
--rw-------  2.0 unx     6048 b- defN 24-Mar-25 11:36 ipex_llm/vllm/outputs.py
--rw-------  2.0 unx    10871 b- defN 24-Mar-25 11:36 ipex_llm/vllm/sampling_params.py
--rw-------  2.0 unx    13481 b- defN 24-Mar-25 11:36 ipex_llm/vllm/sequence.py
--rw-------  2.0 unx     1946 b- defN 24-Mar-25 11:36 ipex_llm/vllm/utils.py
--rw-------  2.0 unx     2338 b- defN 24-Mar-25 11:36 ipex_llm/vllm/core/policy.py
--rw-------  2.0 unx    18616 b- defN 24-Apr-02 11:36 ipex_llm/vllm/core/scheduler.py
--rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/vllm/engine/__init__.py
--rw-------  2.0 unx    12045 b- defN 24-Mar-25 11:36 ipex_llm/vllm/engine/arg_utils.py
--rw-------  2.0 unx    20743 b- defN 24-Mar-25 11:36 ipex_llm/vllm/engine/async_llm_engine.py
--rw-------  2.0 unx    30354 b- defN 24-Mar-25 11:36 ipex_llm/vllm/engine/llm_engine.py
--rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/vllm/entrypoints/__init__.py
--rw-------  2.0 unx     4462 b- defN 24-Mar-25 11:36 ipex_llm/vllm/entrypoints/api_server.py
--rw-------  2.0 unx    10346 b- defN 24-Mar-25 11:36 ipex_llm/vllm/entrypoints/llm.py
--rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/vllm/entrypoints/openai/__init__.py
--rw-------  2.0 unx    28607 b- defN 24-Mar-25 11:36 ipex_llm/vllm/entrypoints/openai/api_server.py
--rw-------  2.0 unx     7642 b- defN 24-Mar-25 11:36 ipex_llm/vllm/entrypoints/openai/openai_protocol.py
--rw-------  2.0 unx     3737 b- defN 24-Mar-25 11:36 ipex_llm/vllm/entrypoints/openai/protocol.py
--rw-------  2.0 unx      682 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/__init__.py
--rw-------  2.0 unx     3642 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/input_metadata.py
--rw-------  2.0 unx     5372 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/model_loader.py
--rw-------  2.0 unx     1630 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/utils.py
--rw-------  2.0 unx    22574 b- defN 24-Apr-02 11:36 ipex_llm/vllm/model_executor/layers/bigdl_sampler.py
--rw-------  2.0 unx    11431 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_baichuan.py
--rw-------  2.0 unx     8964 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_chatglm.py
--rw-------  2.0 unx    11428 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_llama.py
--rw-------  2.0 unx     8770 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_mistral.py
--rw-------  2.0 unx     8675 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_mixtral.py
--rw-------  2.0 unx     7699 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_model.py
--rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/__init__.py
--rw-------  2.0 unx     8707 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/tokenizer.py
--rw-------  2.0 unx    13950 b- defN 24-Mar-25 11:36 ipex_llm/vllm/worker/worker.py
--rw-------  2.0 unx      585 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/__init__.py
--rw-------  2.0 unx     7208 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/model_convert.py
--rw-------  2.0 unx      747 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/engine/__init__.py
--rw-------  2.0 unx     5715 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/engine/engine.py
--rw-------  2.0 unx    10475 b- defN 24-Apr-18 12:34 ipex_llm/vllm2/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4400 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    20723 b- defN 24-Apr-21 15:08 ipex_llm-2.1.0b20240421.dist-info/RECORD
-218 files, 13087091 bytes uncompressed, 5314911 bytes compressed:  59.4%
+-rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
+-rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
+-rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
+-rw-------  2.0 unx     5714 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/engine.py
+-rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240422.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240422.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4400 b- defN 24-Apr-22 15:08 ipex_llm-2.1.0b20240422.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-Apr-22 15:08 ipex_llm-2.1.0b20240422.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-Apr-22 15:08 ipex_llm-2.1.0b20240422.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-Apr-22 15:08 ipex_llm-2.1.0b20240422.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17635 b- defN 24-Apr-22 15:08 ipex_llm-2.1.0b20240422.dist-info/RECORD
+186 files, 12788365 bytes uncompressed, 5235425 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -447,14 +447,17 @@
 
 Filename: ipex_llm/transformers/models/mixtral.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/mpt.py
 Comment: 
 
+Filename: ipex_llm/transformers/models/phi.py
+Comment: 
+
 Filename: ipex_llm/transformers/models/phixtral.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/qwen.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/qwen2.py
@@ -513,143 +516,44 @@
 
 Filename: ipex_llm/utils/common/lazyimport.py
 Comment: 
 
 Filename: ipex_llm/utils/common/log4Error.py
 Comment: 
 
-Filename: ipex_llm/vllm/config.py
+Filename: ipex_llm/vllm/__init__.py
 Comment: 
 
-Filename: ipex_llm/vllm/logger.py
-Comment: 
-
-Filename: ipex_llm/vllm/outputs.py
-Comment: 
-
-Filename: ipex_llm/vllm/sampling_params.py
-Comment: 
-
-Filename: ipex_llm/vllm/sequence.py
-Comment: 
-
-Filename: ipex_llm/vllm/utils.py
-Comment: 
-
-Filename: ipex_llm/vllm/core/policy.py
-Comment: 
-
-Filename: ipex_llm/vllm/core/scheduler.py
+Filename: ipex_llm/vllm/model_convert.py
 Comment: 
 
 Filename: ipex_llm/vllm/engine/__init__.py
 Comment: 
 
-Filename: ipex_llm/vllm/engine/arg_utils.py
-Comment: 
-
-Filename: ipex_llm/vllm/engine/async_llm_engine.py
-Comment: 
-
-Filename: ipex_llm/vllm/engine/llm_engine.py
-Comment: 
-
-Filename: ipex_llm/vllm/entrypoints/__init__.py
-Comment: 
-
-Filename: ipex_llm/vllm/entrypoints/api_server.py
-Comment: 
-
-Filename: ipex_llm/vllm/entrypoints/llm.py
-Comment: 
-
-Filename: ipex_llm/vllm/entrypoints/openai/__init__.py
+Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm/vllm/entrypoints/openai/openai_protocol.py
-Comment: 
-
-Filename: ipex_llm/vllm/entrypoints/openai/protocol.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/__init__.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/input_metadata.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/model_loader.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/utils.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/layers/bigdl_sampler.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/models/bigdl_baichuan.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/models/bigdl_chatglm.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/models/bigdl_llama.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/models/bigdl_mistral.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/models/bigdl_mixtral.py
-Comment: 
-
-Filename: ipex_llm/vllm/model_executor/models/bigdl_model.py
-Comment: 
-
-Filename: ipex_llm/vllm/transformers_utils/__init__.py
-Comment: 
-
-Filename: ipex_llm/vllm/transformers_utils/tokenizer.py
-Comment: 
-
-Filename: ipex_llm/vllm/worker/worker.py
-Comment: 
-
-Filename: ipex_llm/vllm2/__init__.py
-Comment: 
-
-Filename: ipex_llm/vllm2/model_convert.py
-Comment: 
-
-Filename: ipex_llm/vllm2/engine/__init__.py
-Comment: 
-
-Filename: ipex_llm/vllm2/engine/engine.py
-Comment: 
-
-Filename: ipex_llm/vllm2/entrypoints/openai/api_server.py
-Comment: 
-
-Filename: ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240422.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240422.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240421.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240422.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240421.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240422.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240421.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240422.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240421.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240422.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240421.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240422.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,16 +6375,18 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	sub    0x66(%eip),%esp        # 0x1800056a1
-   18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
+   180005634:	in     $0x7c,%eax
+   180005636:	es data16 add %al,(%rax)
+   18000563a:	add    %al,(%rax)
+   18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
    18000567e:	add    %al,(%rax)
    180005680:	add    %eax,(%rax)
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180052e48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053400
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000052e48
@@ -109410,17 +109410,19 @@
    18005c7ba:	add    $0x180,%eax
    18005c7bf:	add    %dh,0x56(%rax)
    18005c7c2:	add    $0x180,%eax
    18005c7c7:	add    %bh,0x56(%rax)
    18005c7ca:	add    $0x180,%eax
    18005c7cf:	add    %al,(%rax)
    18005c7d1:	add    %al,(%rax)
-   18005c7d3:	add    %ah,0x2b(%rdi)
-   18005c7d6:	and    $0x66,%eax
-   18005c7db:	add    %cl,0x50000000(%rip)        # 0x1d005c7e1
+   18005c7d3:	add    %ah,%ch
+   18005c7d5:	jl     0x18005c7fd
+   18005c7d7:	data16 add %al,(%rax)
+   18005c7da:	add    %al,(%rax)
+   18005c7dc:	or     $0x50000000,%eax
    18005c7e1:	add    (%rax),%eax
    18005c7e3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7e9:	mov    $0x5,%ecx
 	...
    18005c7fe:	add    %al,(%rax)
    18005c800:	adc    %dl,%ch
    18005c802:	add    $0x180,%eax
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,16 +5058,18 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	sub    0x66(%eip),%esp        # 0x180004a41
-   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
+   1800049d4:	in     $0x7c,%eax
+   1800049d6:	es data16 add %al,(%rax)
+   1800049da:	add    %al,(%rax)
+   1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a5a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:16 2024
+Time/Date		Mon Apr 22 15:06:14 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005ae00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a5a8
@@ -120845,17 +120845,18 @@
    18006307d:	add    %al,(%rax)
    18006307f:	add    %bh,0x18005c6(%rax)
    180063085:	add    %al,(%rax)
    180063087:	add    %al,%al
    180063089:	movb   $0x0,0x180(%rip)        # 0x180063210
    180063090:	add    %al,(%rax)
    180063092:	add    %al,(%rax)
-   180063094:	push   $0x66252b
-   180063099:	add    %al,(%rax)
-   18006309b:	add    %cl,0x50000000(%rip)        # 0x1d00630a1
+   180063094:	out    %al,$0x7c
+   180063096:	es data16 add %al,(%rax)
+   18006309a:	add    %al,(%rax)
+   18006309c:	or     $0x50000000,%eax
    1800630a1:	add    (%rax),%eax
    1800630a3:	add    %al,0x2f040006(,%rdi,1)
    1800630aa:	(bad)
 	...
    1800630ff:	add    %bh,0x40(%rax)
    180063102:	(bad)
    180063103:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180058c38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:07:21 2024
+Time/Date		Mon Apr 22 15:07:22 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000058c38
@@ -114727,17 +114727,19 @@
    1800626ed:	add    %al,(%rax)
    1800626ef:	add    %dh,-0x4a(%rax)
    1800626f2:	add    $0x180,%eax
    1800626f7:	add    %bh,-0x4a(%rax)
    1800626fa:	add    $0x180,%eax
    1800626ff:	add    %al,(%rax)
    180062701:	add    %al,(%rax)
-   180062703:	add    %ch,0x66252b(%rcx)
-   180062709:	add    %al,(%rax)
-   18006270b:	add    %cl,0x50000000(%rip)        # 0x1d0062711
+   180062703:	add    %ch,(%rdx)
+   180062705:	jge    0x18006272d
+   180062707:	data16 add %al,(%rax)
+   18006270a:	add    %al,(%rax)
+   18006270c:	or     $0x50000000,%eax
    180062711:	add    (%rax),%eax
    180062713:	add    %ah,(%rax)
    180062715:	xor    %eax,(%rsi)
    180062717:	add    %ah,(%rax)
    180062719:	(bad)
    18006271a:	(bad)
 	...
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180053058
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:02:49 2024
+Time/Date		Mon Apr 22 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053600
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000053058
@@ -109461,17 +109461,19 @@
    18005c79a:	add    $0x180,%eax
    18005c79f:	add    %dh,0x56(%rax)
    18005c7a2:	add    $0x180,%eax
    18005c7a7:	add    %bh,0x56(%rax)
    18005c7aa:	add    $0x180,%eax
    18005c7af:	add    %al,(%rax)
    18005c7b1:	add    %al,(%rax)
-   18005c7b3:	add    %bl,0x66252a(%rcx)
-   18005c7b9:	add    %al,(%rax)
-   18005c7bb:	add    %cl,0x50000000(%rip)        # 0x1d005c7c1
+   18005c7b3:	add    %dl,(%rcx)
+   18005c7b5:	jl     0x18005c7dd
+   18005c7b7:	data16 add %al,(%rax)
+   18005c7ba:	add    %al,(%rax)
+   18005c7bc:	or     $0x50000000,%eax
    18005c7c1:	add    (%rax),%eax
    18005c7c3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7c9:	mov    $0x5,%ebx
 	...
    18005c7fe:	add    %al,(%rax)
    18005c800:	adc    %dl,%ch
    18005c802:	add    $0x180,%eax
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180060428
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:07:21 2024
+Time/Date		Mon Apr 22 15:07:22 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060c00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000060428
@@ -126192,17 +126192,18 @@
    180068fb5:	add    %al,(%rax)
    180068fb7:	add    %al,%al
    180068fb9:	es (bad)
    180068fbb:	addb   $0x0,(%rcx)
    180068fbe:	add    %al,(%rax)
    180068fc0:	add    %al,(%rax)
    180068fc2:	add    %al,(%rax)
-   180068fc4:	test   $0x66252b,%eax
-   180068fc9:	add    %al,(%rax)
-   180068fcb:	add    %cl,0x50000000(%rip)        # 0x1d0068fd1
+   180068fc4:	sub    0x26(%rbp),%bh
+   180068fc7:	data16 add %al,(%rax)
+   180068fca:	add    %al,(%rax)
+   180068fcc:	or     $0x50000000,%eax
    180068fd1:	add    (%rax),%eax
    180068fd3:	add    %al,(%rsp,%rbx,4)
    180068fd6:	(bad)
    180068fd7:	add    %al,(%rsp,%rcx,4)
    180068fda:	(bad)
 	...
    180068fff:	add    %bh,-0x61(%rax)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a7b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:02:49 2024
+Time/Date		Mon Apr 22 15:02:42 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b000
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a7b8
@@ -121007,17 +121007,18 @@
    18006305d:	add    %al,(%rax)
    18006305f:	add    %bh,0x18005c6(%rax)
    180063065:	add    %al,(%rax)
    180063067:	add    %al,%al
    180063069:	movb   $0x0,0x180(%rip)        # 0x1800631f0
    180063070:	add    %al,(%rax)
    180063072:	add    %al,(%rax)
-   180063074:	cltd
-   180063075:	sub    0x66(%rip),%ah        # 0x1800630e1
-   18006307b:	add    %cl,0x50000000(%rip)        # 0x1d0063081
+   180063074:	adc    0x66(%rsi,%riz,1),%bh
+   180063078:	add    %al,(%rax)
+   18006307a:	add    %al,(%rax)
+   18006307c:	or     $0x50000000,%eax
    180063081:	add    (%rax),%eax
    180063083:	add    %al,0x31040006(,%rdi,1)
    18006308a:	(bad)
 	...
    1800630ff:	add    %bh,0x40(%rax)
    180063102:	(bad)
    180063103:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005f138
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:07:21 2024
+Time/Date		Mon Apr 22 15:07:22 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005f800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005f138
@@ -124880,17 +124880,18 @@
    180068096:	add    %al,(%rax)
    180068098:	rclb   $1,(%rsi)
    18006809a:	(bad)
    18006809b:	addb   $0x0,(%rcx)
    18006809e:	add    %al,(%rax)
    1800680a0:	add    %al,(%rax)
    1800680a2:	add    %al,(%rax)
-   1800680a4:	test   $0x66252b,%eax
-   1800680a9:	add    %al,(%rax)
-   1800680ab:	add    %cl,0x50000000(%rip)        # 0x1d00680b1
+   1800680a4:	sub    0x26(%rbp),%bh
+   1800680a7:	data16 add %al,(%rax)
+   1800680aa:	add    %al,(%rax)
+   1800680ac:	or     $0x50000000,%eax
    1800680b1:	add    (%rax),%eax
    1800680b3:	add    %al,(%rax)
    1800680b5:	lea    (%rsi),%eax
    1800680b7:	add    %al,(%rax)
    1800680b9:	jns    0x1800680c1
 	...
    1800680ff:	add    %dh,-0x70(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800594c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:02:49 2024
+Time/Date		Mon Apr 22 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059c00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000594c8
@@ -119683,17 +119683,18 @@
    180062140:	enter  $0x5b6,$0x80
    180062144:	add    %eax,(%rax)
    180062146:	add    %al,(%rax)
    180062148:	shlb   $1,0x18005(%rsi)
    18006214e:	add    %al,(%rax)
    180062150:	add    %al,(%rax)
    180062152:	add    %al,(%rax)
-   180062154:	cltd
-   180062155:	sub    0x66(%rip),%ah        # 0x1800621c1
-   18006215b:	add    %cl,0x50000000(%rip)        # 0x1d0062161
+   180062154:	adc    %edi,0x66(%rsi,%riz,1)
+   180062158:	add    %al,(%rax)
+   18006215a:	add    %al,(%rax)
+   18006215c:	or     $0x50000000,%eax
    180062161:	add    (%rax),%eax
    180062163:	add    %al,-0x7ffff9d3(%rax)
    180062169:	sbb    $0x6,%eax
 	...
    18006217e:	add    %al,(%rax)
    180062180:	lock xor %al,(%rsi)
    180062183:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180066598
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:07:20 2024
+Time/Date		Mon Apr 22 15:07:22 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000066c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000066598
@@ -135439,17 +135439,18 @@
    18006fbe5:	add    %al,(%rax)
    18006fbe7:	add    %al,%al
    18006fbe9:	xchg   %al,(%rsi)
    18006fbeb:	addb   $0x0,(%rcx)
    18006fbee:	add    %al,(%rax)
    18006fbf0:	add    %al,(%rax)
    18006fbf2:	add    %al,(%rax)
-   18006fbf4:	test   $0x2b,%al
-   18006fbf6:	and    $0x66,%eax
-   18006fbfb:	add    %cl,0x50000000(%rip)        # 0x1d006fc01
+   18006fbf4:	sub    0x26(%rbp),%bh
+   18006fbf7:	data16 add %al,(%rax)
+   18006fbfa:	add    %al,(%rax)
+   18006fbfc:	or     $0x50000000,%eax
    18006fc01:	add    (%rax),%eax
    18006fc03:	add    %dl,%al
    18006fc05:	or     $0xfdd00007,%eax
    18006fc0a:	(bad)
 	...
    18006fc7f:	add    %al,0x11(%rax)
    18006fc82:	(bad)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800609b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:02:49 2024
+Time/Date		Mon Apr 22 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061000
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000609b8
@@ -130151,17 +130151,18 @@
    180069cb5:	add    %al,(%rax)
    180069cb7:	add    %al,%al
    180069cb9:	es (bad)
    180069cbb:	addb   $0x0,(%rcx)
    180069cbe:	add    %al,(%rax)
    180069cc0:	add    %al,(%rax)
    180069cc2:	add    %al,(%rax)
-   180069cc4:	cltd
-   180069cc5:	sub    0x66(%rip),%ah        # 0x180069d31
-   180069ccb:	add    %cl,0x50000000(%rip)        # 0x1d0069cd1
+   180069cc4:	adc    %edi,0x66(%rsi,%riz,1)
+   180069cc8:	add    %al,(%rax)
+   180069cca:	add    %al,(%rax)
+   180069ccc:	or     $0x50000000,%eax
    180069cd1:	add    (%rax),%eax
    180069cd3:	add    %dl,-0x52(%rax)
    180069cd6:	(bad)
    180069cd7:	add    %dl,-0x5e(%rax)
    180069cda:	(bad)
 	...
    180069cff:	add    %al,%al
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,16 +5355,18 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	sub    0x66(%eip),%esp        # 0x180004aa1
-   180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
+   180004a34:	in     $0x7c,%eax
+   180004a36:	es data16 add %al,(%rax)
+   180004a3a:	add    %al,(%rax)
+   180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
    180004a7e:	add    %al,(%rax)
    180004a80:	add    %eax,(%rax)
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800592b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:16 2024
+Time/Date		Mon Apr 22 15:06:14 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059a00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000592b8
@@ -119535,17 +119535,18 @@
    180062160:	enter  $0x5b6,$0x80
    180062164:	add    %eax,(%rax)
    180062166:	add    %al,(%rax)
    180062168:	shlb   $1,0x18005(%rsi)
    18006216e:	add    %al,(%rax)
    180062170:	add    %al,(%rax)
    180062172:	add    %al,(%rax)
-   180062174:	push   $0x66252b
-   180062179:	add    %al,(%rax)
-   18006217b:	add    %cl,0x50000000(%rip)        # 0x1d0062181
+   180062174:	out    %al,$0x7c
+   180062176:	es data16 add %al,(%rax)
+   18006217a:	add    %al,(%rax)
+   18006217c:	or     $0x50000000,%eax
    180062181:	add    (%rax),%eax
    180062183:	add    %al,(%rax)
    180062185:	cs (bad)
    180062187:	add    %al,(%rax)
    180062189:	sbb    $0x6,%al
 	...
    1800621ff:	add    %dh,0x31(%rax)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,16 +25509,18 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	sub    0x66(%eip),%esp        # 0x140014b31
-   140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
+   140014ac4:	in     $0x7c,%eax
+   140014ac6:	es data16 add %al,(%rax)
+   140014aca:	add    %al,(%rax)
+   140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
    140014ad9:	rex add %eax,(%rax)
 	...
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:03:17 2024
+Time/Date		Mon Apr 22 15:03:09 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189024,15 +189024,15 @@
    140093ea5:	add    %al,(%rax)
    140093ea7:	add    %al,(%rax)
    140093ea9:	cltd
    140093eaa:	or     %al,0x1(%rax)
    140093ead:	add    %al,(%rax)
    140093eaf:	add    %al,(%rax)
    140093eb1:	add    %al,(%rax)
-   140093eb3:	add    %dh,0x66252a(%rbp)
+   140093eb3:	add    %ch,0x66267c(%rip)        # 0x1406f6535
    140093eb9:	add    %al,(%rax)
    140093ebb:	add    %cl,-0x34000000(%rip)        # 0x10c093ec1
    140093ec1:	add    (%rax),%eax
    140093ec3:	add    %dl,(%rax)
    140093ec5:	jae    0x140093ed0
    140093ec7:	add    %dl,(%rax)
    140093ec9:	movsxd (%rcx),%ecx
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,16 +24136,18 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	sub    0x66(%eip),%esp        # 0x140013f61
-   140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
+   140013ef4:	in     $0x7c,%eax
+   140013ef6:	es data16 add %al,(%rax)
+   140013efa:	add    %al,(%rax)
+   140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
    140013f81:	add    %r8,0x1(%r8)
    140013f85:	add    %al,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,16 +24679,18 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	sub    0x66(%eip),%esp        # 0x140014031
-   140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
+   140013fc4:	in     $0x7c,%eax
+   140013fc6:	es data16 add %al,(%rax)
+   140013fca:	add    %al,(%rax)
+   140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
 	...
    140013fff:	add    %ah,0x140014d(%rax)
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,17 +40341,19 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %ah,0x2b(%rdi)
-   14001f126:	and    $0x66,%eax
-   14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
+   14001f123:	add    %ah,%ch
+   14001f125:	jl     0x14001f14d
+   14001f127:	data16 add %al,(%rax)
+   14001f12a:	add    %al,(%rax)
+   14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
 	...
    14001f180:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000acc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32227,17 +32227,19 @@
    1400191a5:	add    %al,(%rax)
    1400191a7:	add    %al,(%rax)
    1400191a9:	push   %rbp
    1400191aa:	add    %eax,0x1(%rax)
    1400191ad:	add    %al,(%rax)
    1400191af:	add    %al,(%rax)
    1400191b1:	add    %al,(%rax)
-   1400191b3:	add    %ah,0x2b(%rdi)
-   1400191b6:	and    $0x66,%eax
-   1400191bb:	add    %cl,0x20000000(%rip)        # 0x1600191c1
+   1400191b3:	add    %ah,%ch
+   1400191b5:	jl     0x1400191dd
+   1400191b7:	data16 add %al,(%rax)
+   1400191ba:	add    %al,(%rax)
+   1400191bc:	or     $0x20000000,%eax
    1400191c1:	add    (%rax),%eax
    1400191c3:	add    %dh,-0x5f(%rax)
    1400191c6:	add    %eax,(%rax)
    1400191c8:	jo     0x140019159
    1400191ca:	add    %eax,(%rax)
 	...
    140019200:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:02:49 2024
+Time/Date		Mon Apr 22 15:02:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32344,17 +32344,19 @@
    140019185:	add    %al,(%rax)
    140019187:	add    %al,(%rax)
    140019189:	push   %rbp
    14001918a:	add    %eax,0x1(%rax)
    14001918d:	add    %al,(%rax)
    14001918f:	add    %al,(%rax)
    140019191:	add    %al,(%rax)
-   140019193:	add    %bl,0x66252a(%rcx)
-   140019199:	add    %al,(%rax)
-   14001919b:	add    %cl,0x20000000(%rip)        # 0x1600191a1
+   140019193:	add    %dl,(%rcx)
+   140019195:	jl     0x1400191bd
+   140019197:	data16 add %al,(%rax)
+   14001919a:	add    %al,(%rax)
+   14001919c:	or     $0x20000000,%eax
    1400191a1:	add    (%rax),%eax
    1400191a3:	add    %dh,-0x5f(%rax)
    1400191a6:	add    %eax,(%rax)
    1400191a8:	jo     0x14001913b
    1400191aa:	add    %eax,(%rax)
 	...
    140019200:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:14 2024
+Time/Date		Mon Apr 22 15:06:12 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27188,17 +27188,19 @@
    140015f80:	push   $0x1400123
    140015f85:	add    %al,(%rax)
    140015f87:	add    %dh,0x23(%rax)
    140015f8a:	add    %eax,0x1(%rax)
    140015f8d:	add    %al,(%rax)
    140015f8f:	add    %al,(%rax)
    140015f91:	add    %al,(%rax)
-   140015f93:	add    %ah,0x2b(%rsi)
-   140015f96:	and    $0x66,%eax
-   140015f9b:	add    %cl,-0x70000000(%rip)        # 0xd0015fa1
+   140015f93:	add    %ah,%ah
+   140015f95:	jl     0x140015fbd
+   140015f97:	data16 add %al,(%rax)
+   140015f9a:	add    %al,(%rax)
+   140015f9c:	or     $0x90000000,%eax
    140015fa1:	add    (%rax),%eax
    140015fa3:	add    %ch,0x65(%rax)
    140015fa6:	add    %eax,(%rax)
    140015fa8:	push   $0x153
 	...
    140015ffd:	add    %al,(%rax)
    140015fff:	add    %bl,(%rax)
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:02:48 2024
+Time/Date		Mon Apr 22 15:02:40 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27296,17 +27296,19 @@
    140015f60:	push   $0x1400123
    140015f65:	add    %al,(%rax)
    140015f67:	add    %dh,0x23(%rax)
    140015f6a:	add    %eax,0x1(%rax)
    140015f6d:	add    %al,(%rax)
    140015f6f:	add    %al,(%rax)
    140015f71:	add    %al,(%rax)
-   140015f73:	add    %bl,0x66252a(%rax)
-   140015f79:	add    %al,(%rax)
-   140015f7b:	add    %cl,-0x70000000(%rip)        # 0xd0015f81
+   140015f73:	add    %dl,(%rax)
+   140015f75:	jl     0x140015f9d
+   140015f77:	data16 add %al,(%rax)
+   140015f7a:	add    %al,(%rax)
+   140015f7c:	or     $0x90000000,%eax
    140015f81:	add    (%rax),%eax
    140015f83:	add    %ch,0x65(%rax)
    140015f86:	add    %eax,(%rax)
    140015f88:	push   $0x155
 	...
    140015ffd:	add    %al,(%rax)
    140015fff:	add    %bl,(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:14 2024
+Time/Date		Mon Apr 22 15:06:12 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28454,17 +28454,19 @@
    14001706d:	add    %al,(%rax)
    14001706f:	add    %cl,0x1400133(%rax)
    140017075:	add    %al,(%rax)
    140017077:	add    %dl,0x1400133(%rax)
    14001707d:	add    %al,(%rax)
    14001707f:	add    %al,(%rax)
    140017081:	add    %al,(%rax)
-   140017083:	add    %ah,0x2b(%rsi)
-   140017086:	and    $0x66,%eax
-   14001708b:	add    %cl,-0x70000000(%rip)        # 0xd0017091
+   140017083:	add    %ah,%ah
+   140017085:	jl     0x1400170ad
+   140017087:	data16 add %al,(%rax)
+   14001708a:	add    %al,(%rax)
+   14001708c:	or     $0x90000000,%eax
    140017091:	add    (%rax),%eax
    140017093:	add    %ch,0x1(%rsi,%rsi,2)
    140017097:	add    %ch,0x1(%rdx,%riz,2)
 	...
    1400170ff:	add    %ah,(%rax)
    140017101:	jp     0x140017104
    140017103:	rex add %eax,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:02:48 2024
+Time/Date		Mon Apr 22 15:02:40 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28600,17 +28600,19 @@
    14001704d:	add    %al,(%rax)
    14001704f:	add    %cl,0x1400133(%rax)
    140017055:	add    %al,(%rax)
    140017057:	add    %dl,0x1400133(%rax)
    14001705d:	add    %al,(%rax)
    14001705f:	add    %al,(%rax)
    140017061:	add    %al,(%rax)
-   140017063:	add    %bl,0x66252a(%rax)
-   140017069:	add    %al,(%rax)
-   14001706b:	add    %cl,-0x70000000(%rip)        # 0xd0017071
+   140017063:	add    %dl,(%rax)
+   140017065:	jl     0x14001708d
+   140017067:	data16 add %al,(%rax)
+   14001706a:	add    %al,(%rax)
+   14001706c:	or     $0x90000000,%eax
    140017071:	add    (%rax),%eax
    140017073:	add    %ch,%ah
    140017075:	jne    0x140017078
    140017077:	add    %ch,%ah
    140017079:	add    %eax,%gs:(%rax)
    14001707c:	add    %al,(%rax)
    14001707e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32545,17 +32545,19 @@
    1400192a5:	add    %al,(%rax)
    1400192a7:	add    %al,(%rax)
    1400192a9:	push   %rbp
    1400192aa:	add    %eax,0x1(%rax)
    1400192ad:	add    %al,(%rax)
    1400192af:	add    %al,(%rax)
    1400192b1:	add    %al,(%rax)
-   1400192b3:	add    %ah,0x2b(%rdi)
-   1400192b6:	and    $0x66,%eax
-   1400192bb:	add    %cl,0x20000000(%rip)        # 0x1600192c1
+   1400192b3:	add    %ah,%ch
+   1400192b5:	jl     0x1400192dd
+   1400192b7:	data16 add %al,(%rax)
+   1400192ba:	add    %al,(%rax)
+   1400192bc:	or     $0x20000000,%eax
    1400192c1:	add    (%rax),%eax
    1400192c3:	add    %bh,0x1(%rdx,%riz,4)
    1400192c7:	add    %bh,0x1(%rdx,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
 	...
    140019309:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Sun Apr 21 15:02:49 2024
+Time/Date		Mon Apr 22 15:02:40 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32652,17 +32652,19 @@
    140019285:	add    %al,(%rax)
    140019287:	add    %al,(%rax)
    140019289:	push   %rbp
    14001928a:	add    %eax,0x1(%rax)
    14001928d:	add    %al,(%rax)
    14001928f:	add    %al,(%rax)
    140019291:	add    %al,(%rax)
-   140019293:	add    %bl,0x66252a(%rcx)
-   140019299:	add    %al,(%rax)
-   14001929b:	add    %cl,0x20000000(%rip)        # 0x1600192a1
+   140019293:	add    %dl,(%rax)
+   140019295:	jl     0x1400192bd
+   140019297:	data16 add %al,(%rax)
+   14001929a:	add    %al,(%rax)
+   14001929c:	or     $0x20000000,%eax
    1400192a1:	add    (%rax),%eax
    1400192a3:	add    %bh,0x1(%rdx,%riz,4)
    1400192a7:	add    %bh,0x1(%rsp,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
 	...
    140019309:	add    %al,(%rax)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,16 +4028,18 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	sub    0x66(%eip),%esp        # 0x180004671
-   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
+   180004604:	in     $0x7c,%eax
+   180004606:	es data16 add %al,(%rax)
+   18000460a:	add    %al,(%rax)
+   18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800607a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sun Apr 21 15:06:15 2024
+Time/Date		Mon Apr 22 15:06:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060e00
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000607a8
@@ -129991,16 +129991,18 @@
    180069cd5:	add    %al,(%rax)
    180069cd7:	add    %al,%al
    180069cd9:	es (bad)
    180069cdb:	addb   $0x0,(%rcx)
    180069cde:	add    %al,(%rax)
    180069ce0:	add    %al,(%rax)
    180069ce2:	add    %al,(%rax)
-   180069ce4:	sub    0x66(%eip),%esp        # 0x180069d51
-   180069ceb:	add    %cl,0x50000000(%rip)        # 0x1d0069cf1
+   180069ce4:	in     $0x7c,%eax
+   180069ce6:	es data16 add %al,(%rax)
+   180069cea:	add    %al,(%rax)
+   180069cec:	or     $0x50000000,%eax
    180069cf1:	add    (%rax),%eax
    180069cf3:	add    %dl,-0x52(%rax)
    180069cf6:	(bad)
    180069cf7:	add    %dl,-0x60(%rax)
    180069cfa:	(bad)
    180069cfb:	add    %al,(%rax)
    180069cfd:	add    %al,(%rax)
```

## ipex_llm/serving/fastchat/vllm_worker.py

```diff
@@ -25,33 +25,26 @@
 import argparse
 import asyncio
 import json
 from typing import List
 
 from fastapi import FastAPI, Request, BackgroundTasks
 from fastapi.responses import StreamingResponse, JSONResponse
-import torch
 import uvicorn
-# from vllm import AsyncLLMEngine
-# from vllm.engine.arg_utils import AsyncEngineArgs
-# from vllm.sampling_params import SamplingParams
-# from vllm.utils import random_uuid
-from ipex_llm.vllm.engine.async_llm_engine import AsyncLLMEngine
-from ipex_llm.vllm.engine.arg_utils import AsyncEngineArgs
-from ipex_llm.vllm.sampling_params import SamplingParams
-from ipex_llm.vllm.utils import random_uuid
-
-import numpy as np
+from ipex_llm.vllm.engine import IPEXLLMAsyncLLMEngine as AsyncLLMEngine
+from vllm.engine.arg_utils import AsyncEngineArgs
+from vllm.sampling_params import SamplingParams
+from vllm.utils import random_uuid
 
+from fastchat.serve.base_model_worker import BaseModelWorker
 from fastchat.serve.model_worker import (
-    BaseModelWorker,
     logger,
     worker_id,
 )
-from fastchat.utils import get_context_length
+from fastchat.utils import get_context_length, is_partial_stop
 
 
 app = FastAPI()
 
 
 class VLLMWorker(BaseModelWorker):
     def __init__(
@@ -73,85 +66,133 @@
             model_path,
             model_names,
             limit_worker_concurrency,
             conv_template,
         )
 
         logger.info(
-            f"Loading the model {self.model_names} on worker {worker_id}, worker type: vLLM worker."
+            f"Loading the model {self.model_names} on worker {worker_id}, "
+            f"worker type: vLLM worker..."
         )
         self.tokenizer = llm_engine.engine.tokenizer
+        # This is to support vllm >= 0.2.7 where TokenizerGroup was introduced
+        # and llm_engine.engine.tokenizer was no longer a raw tokenizer
+        if hasattr(self.tokenizer, "tokenizer"):
+            self.tokenizer = llm_engine.engine.tokenizer.tokenizer
         self.context_len = get_context_length(llm_engine.engine.model_config.hf_config)
 
         if not no_register:
             self.init_heart_beat()
 
     async def generate_stream(self, params):
         self.call_ct += 1
 
         context = params.pop("prompt")
         request_id = params.pop("request_id")
         temperature = float(params.get("temperature", 1.0))
         top_p = float(params.get("top_p", 1.0))
+        top_k = params.get("top_k", -1.0)
+        presence_penalty = float(params.get("presence_penalty", 0.0))
+        frequency_penalty = float(params.get("frequency_penalty", 0.0))
         max_new_tokens = params.get("max_new_tokens", 256)
         stop_str = params.get("stop", None)
         stop_token_ids = params.get("stop_token_ids", None) or []
         if self.tokenizer.eos_token_id is not None:
             stop_token_ids.append(self.tokenizer.eos_token_id)
         echo = params.get("echo", True)
-        ignore_eos = params.get('ignore_eos', False)
+        use_beam_search = params.get("use_beam_search", False)
+        best_of = params.get("best_of", None)
+
+        request = params.get("request", None)
 
         # Handle stop_str
         stop = set()
         if isinstance(stop_str, str) and stop_str != "":
             stop.add(stop_str)
         elif isinstance(stop_str, list) and stop_str != []:
             stop.update(stop_str)
 
         for tid in stop_token_ids:
             if tid is not None:
-                stop.add(self.tokenizer.decode(tid))
+                s = self.tokenizer.decode(tid)
+                if s != "":
+                    stop.add(s)
 
         # make sampling params in vllm
         top_p = max(top_p, 1e-5)
         if temperature <= 1e-5:
             top_p = 1.0
+
         sampling_params = SamplingParams(
             n=1,
             temperature=temperature,
             top_p=top_p,
-            use_beam_search=False,
+            use_beam_search=use_beam_search,
             stop=list(stop),
+            stop_token_ids=stop_token_ids,
             max_tokens=max_new_tokens,
-            ignore_eos=ignore_eos,
+            top_k=top_k,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            best_of=best_of,
         )
         results_generator = engine.generate(context, sampling_params, request_id)
 
         async for request_output in results_generator:
             prompt = request_output.prompt
             if echo:
                 text_outputs = [
                     prompt + output.text for output in request_output.outputs
                 ]
             else:
                 text_outputs = [output.text for output in request_output.outputs]
             text_outputs = " ".join(text_outputs)
-            finish_reason = request_output.outputs[0].finish_reason
-            output_token_latency = request_output.outputs[0].output_token_latency
-            first_token_latency = output_token_latency[0]
-            if len(output_token_latency) > 1:
-                rest_token_time = np.mean(output_token_latency[1:])
-            else:
-                rest_token_time = None
-            # Note: usage is not supported yet
-            ret = {"text": text_outputs, "error_code": 0, "usage": {},
-                   "finish_reason": finish_reason, "first_token_time": first_token_latency,
-                   "rest_token_time": rest_token_time}
+
+            partial_stop = any(is_partial_stop(text_outputs, i) for i in stop)
+            # prevent yielding partial stop sequence
+            if partial_stop:
+                continue
+
+            aborted = False
+            if request and await request.is_disconnected():
+                await engine.abort(request_id)
+                request_output.finished = True
+                aborted = True
+                for output in request_output.outputs:
+                    output.finish_reason = "abort"
+
+            prompt_tokens = len(request_output.prompt_token_ids)
+            completion_tokens = sum(
+                len(output.token_ids) for output in request_output.outputs
+            )
+            ret = {
+                "text": text_outputs,
+                "error_code": 0,
+                "usage": {
+                    "prompt_tokens": prompt_tokens,
+                    "completion_tokens": completion_tokens,
+                    "total_tokens": prompt_tokens + completion_tokens,
+                },
+                "cumulative_logprob": [
+                    output.cumulative_logprob for output in request_output.outputs
+                ],
+                "finish_reason": request_output.outputs[0].finish_reason
+                if len(request_output.outputs) == 1
+                else [output.finish_reason for output in request_output.outputs],
+            }
+            # Emit twice here to ensure a 'finish_reason' with empty
+            # content in the OpenAI API response.
+            # This aligns with the behavior of model_worker.
+            if request_output.finished:
+                yield (json.dumps({**ret, **{"finish_reason": None}}) + "\0").encode()
             yield (json.dumps(ret) + "\0").encode()
 
+            if aborted:
+                break
+
     async def generate(self, params):
         async for x in self.generate_stream(params):
             pass
         return json.loads(x[:-1].decode())
 
 
 def release_worker_semaphore():
@@ -176,25 +217,27 @@
 
 @app.post("/worker_generate_stream")
 async def api_generate_stream(request: Request):
     params = await request.json()
     await acquire_worker_semaphore()
     request_id = random_uuid()
     params["request_id"] = request_id
+    params["request"] = request
     generator = worker.generate_stream(params)
     background_tasks = create_background_tasks(request_id)
     return StreamingResponse(generator, background=background_tasks)
 
 
 @app.post("/worker_generate")
 async def api_generate(request: Request):
     params = await request.json()
     await acquire_worker_semaphore()
     request_id = random_uuid()
     params["request_id"] = request_id
+    params["request"] = request
     output = await worker.generate(params)
     release_worker_semaphore()
     await engine.abort(request_id)
     return JSONResponse(output)
 
 
 @app.post("/worker_get_status")
@@ -222,37 +265,56 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21002)
     parser.add_argument("--worker-address", type=str, default="http://localhost:21002")
     parser.add_argument(
         "--controller-address", type=str, default="http://localhost:21001"
     )
-    parser.add_argument("--model-path", type=str, default="lmsys/vicuna-7b-v1.3")
+    parser.add_argument("--model-path", type=str, default="lmsys/vicuna-7b-v1.5")
     parser.add_argument(
         "--model-names",
         type=lambda s: s.split(","),
         help="Optional display comma separated names",
     )
     parser.add_argument("--limit-worker-concurrency", type=int, default=1024)
     parser.add_argument("--no-register", action="store_true")
     parser.add_argument("--num-gpus", type=int, default=1)
     parser.add_argument(
         "--conv-template", type=str, default=None, help="Conversation prompt template."
     )
+    parser.add_argument(
+        "--load-in-low-bit", type=str, default="sym_int4", help="Low-bit quantization format"
+    )
+    parser.add_argument(
+        "--trust_remote_code",
+        action="store_false",
+        default=True,
+        help="Trust remote code (e.g., from HuggingFace) when"
+        "downloading the model and tokenizer.",
+    )
+    parser.add_argument(
+        "--gpu_memory_utilization",
+        type=float,
+        default=0.9,
+        help="The ratio (between 0 and 1) of GPU memory to"
+        "reserve for the model weights, activations, and KV cache. Higher"
+        "values will increase the KV cache size and thus improve the model's"
+        "throughput. However, if the value is too high, it may cause out-of-"
+        "memory (OOM) errors.",
+    )
 
     parser = AsyncEngineArgs.add_cli_args(parser)
     args = parser.parse_args()
     if args.model_path:
         args.model = args.model_path
-    # if args.num_gpus > 1:
-    #     args.tensor_parallel_size = args.num_gpus
+    if args.num_gpus > 1:
+        args.tensor_parallel_size = args.num_gpus
 
-    # By default, we are creating a CPU asyncEngineArgs.
     engine_args = AsyncEngineArgs.from_cli_args(args)
-    engine = AsyncLLMEngine.from_engine_args(engine_args)
+    engine = AsyncLLMEngine.from_engine_args(engine_args, load_in_low_bit=args.load_in_low_bit)
     worker = VLLMWorker(
         args.controller_address,
         args.worker_address,
         worker_id,
         args.model_path,
         args.model_names,
         args.limit_worker_concurrency,
```

## ipex_llm/transformers/convert.py

```diff
@@ -646,14 +646,17 @@
     ):
         from ipex_llm.transformers.models.bert import merge_qkv
         model.apply(merge_qkv)
     # for starcoder2
     if model.config.model_type == "starcoder2":
         from ipex_llm.transformers.models.starcoder2 import merge_qkv
         model.apply(merge_qkv)
+    if model.config.model_type == "phi":
+        from ipex_llm.transformers.models.phi import merge_qkv
+        model.apply(merge_qkv)
     if model.config.model_type == "qwen":
         rope_base = model.config.rotary_emb_base
         from accelerate.big_modeling import init_empty_weights
 
         def split_qkv_proj_func(module):
             if "QWenAttention" in module.__class__.__name__:
                 c_attn_weight = module.c_attn.weight.data
@@ -1411,15 +1414,22 @@
         # starcoder2
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
         from ipex_llm.transformers.models.starcoder2 import attention_forward
         from ipex_llm.transformers.models.starcoder2 import model_forward
         convert_forward(model, module.Starcoder2Attention, attention_forward)
         convert_forward(model, module.Starcoder2Model, model_forward)
-
+    elif model.config.model_type == 'phi':
+        # for phi-2
+        modeling_module_name = model.__class__.__module__
+        module = importlib.import_module(modeling_module_name)
+        from ipex_llm.transformers.models.phi import attention_forward
+        from ipex_llm.transformers.models.phi import model_forward
+        convert_forward(model, module.PhiAttention, attention_forward)
+        convert_forward(model, module.PhiModel, model_forward)
     elif model.config.model_type == 'yuan':
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
         from ipex_llm.transformers.models.yuan import yuan_attention_forward
         # from ipex_llm.transformers.models.yuan import yuan_mlp_forward
         convert_forward(model,
                         module.YuanAttention,
```

## ipex_llm/transformers/convert_ipex.py

```diff
@@ -146,15 +146,16 @@
 
     is_tpp = _using_tpp()
 
     _ipex_optimize_rmsnorm(model, rms_classes, is_tpp=is_tpp, is_woq=is_woq)
     _ipex_optimize_attention(model, is_tpp=is_tpp, is_woq=is_woq)
     _ipex_optimize_decoder(model, is_tpp=is_tpp, is_woq=is_woq)
 
-    model.register_forward_hook(output_hook, with_kwargs=True)
+    # need to register_forward_hook after torch.jit.trace
+    # model.register_forward_hook(output_hook, with_kwargs=True)
     return model
 
 
 def _ipex_jit(model):
     from intel_extension_for_pytorch.transformers.optimize import (
         get_dummy_input,
         _set_optimized_model_for_generation
```

## ipex_llm/transformers/lookup.py

```diff
@@ -312,15 +312,16 @@
             self.n_matched += max_matched - 1
             self.n_drafted += candidate_length
 
             # Clean up target model KV cache
             if max_of_max_matched != max_matched:
                 output_ids = output_ids[:, :max_matched]
                 new_cache_size = max_of_max_matched - max_matched
-                past_key_values = _crop_past_key_values(self, past_key_values, new_cache_size)
+                past_key_values = _crop_past_key_values(self, past_key_values,
+                                                        new_cache_size)
 
             input_ids = torch.cat((input_ids, output_ids), dim=-1)
 
             step += output_ids.size(1)
             step_verify += 1
 
         # Stop on eos and remove content after eos
```

## ipex_llm/transformers/speculative.py

```diff
@@ -447,27 +447,28 @@
                 past_key_values[i] = (new_cache_k.transpose(1, 2), new_cache_v.transpose(1, 2))
             else:
                 past_key_values[i] = (new_cache_k, new_cache_v)
     return past_key_values, not enough_kv_room
 
 
 def _crop_past_key_values(self, past_key_values, new_cache_size, _enable_ipex=False):
-    from ipex_llm.transformers.kv import DynamicFp8Cache, DynamicNormalCache
-    if isinstance(past_key_values, (DynamicFp8Cache, DynamicNormalCache)):
-        if hasattr(past_key_values, "_seen_tokens"):
-            past_key_values._seen_tokens -= new_cache_size
-        else:
-            past_key_values.seen_tokens -= new_cache_size
+    if version.parse(trans_version) >= version.parse("4.36.0"):
+        from ipex_llm.transformers.kv import DynamicFp8Cache, DynamicNormalCache
+        if isinstance(past_key_values, (DynamicFp8Cache, DynamicNormalCache)):
+            if hasattr(past_key_values, "_seen_tokens"):
+                past_key_values._seen_tokens -= new_cache_size
+            else:
+                past_key_values.seen_tokens -= new_cache_size
 
-        for i, k in enumerate(past_key_values.key_cache):
-            past_key_values.key_cache[i] = k[:, :, :-new_cache_size, :]
-        for i, v in enumerate(past_key_values.value_cache):
-            past_key_values.value_cache[i] = v[:, :, :-new_cache_size, :]
+            for i, k in enumerate(past_key_values.key_cache):
+                past_key_values.key_cache[i] = k[:, :, :-new_cache_size, :]
+            for i, v in enumerate(past_key_values.value_cache):
+                past_key_values.value_cache[i] = v[:, :, :-new_cache_size, :]
 
-        return past_key_values
+            return past_key_values
 
     if _enable_ipex:
         cur_len = past_key_values[0][0].size(1)
         delta = new_cache_size
         tmp = torch.empty(1, (cur_len - delta), (cur_len - delta), 1,
                           dtype=torch.long).contiguous()
         past_key_values = [[tmp, key_cache, value_cache, beam_idx]
```

## ipex_llm/vllm/engine/__init__.py

```diff
@@ -8,7 +8,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+from .engine import IPEXLLMAsyncLLMEngine, IPEXLLMLLMEngine, IPEXLLMClass
+__all__ = [
+    "IPEXLLMAsyncLLMEngine",
+    "IPEXLLMLLMEngine",
+    "IPEXLLMClass",
+]
```

## ipex_llm/vllm/entrypoints/openai/api_server.py

```diff
@@ -1,685 +1,82 @@
-#
-# Copyright 2016 The BigDL Authors.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Some parts of this file is adapted from
-# https://github.com/vllm-project/vllm/blob/v0.2.1.post1/vllm/entrypoints/openai/api_server.py
-# which is licensed under Apache License 2.0
-#
-# Copyright 2023 The vLLM team. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# Adapted from
-# https://github.com/lm-sys/FastChat/blob/168ccc29d3f7edc50823016105c024fe2282732a/fastchat/serve/openai_api_server.py
-#
-# bigdl-llm Intel specified code change
-#
-
 import argparse
 import asyncio
 import json
-import time
-from http import HTTPStatus
-from typing import AsyncGenerator, Dict, List, Optional, Tuple, Union
+from contextlib import asynccontextmanager
+import os
+import importlib
+import inspect
+import ssl
 
+from prometheus_client import make_asgi_app
 import fastapi
 import uvicorn
+from http import HTTPStatus
 from fastapi import Request
 from fastapi.exceptions import RequestValidationError
 from fastapi.middleware.cors import CORSMiddleware
-from fastapi.responses import JSONResponse, StreamingResponse
-from packaging import version
-import numpy as np
-
-from ipex_llm.vllm.engine.arg_utils import AsyncEngineArgs
-from ipex_llm.vllm.engine.async_llm_engine import AsyncLLMEngine
-from ipex_llm.vllm.entrypoints.openai.protocol import (
-    CompletionResponse, CompletionResponseChoice,
-    CompletionResponseStreamChoice, CompletionStreamResponse,
-    ChatCompletionResponse, ChatCompletionResponseChoice, ChatMessage,
-    DeltaMessage, ErrorResponse, LogProbs, ModelCard, ModelPermission,
-    UsageInfo)
-from ipex_llm.vllm.entrypoints.openai.openai_protocol import (
-    CompletionRequest, ChatCompletionRequest,
-    ChatCompletionResponseStreamChoice, ChatCompletionStreamResponse,
-    ModelList)
-from ipex_llm.vllm.logger import init_logger
-from ipex_llm.vllm.outputs import RequestOutput
-from ipex_llm.vllm.sampling_params import SamplingParams
-from ipex_llm.vllm.transformers_utils.tokenizer import get_tokenizer
-import uuid
-from ipex_llm.utils.common import invalidInputError
+from fastapi.responses import JSONResponse, StreamingResponse, Response
 
-try:
-    import fastchat
-    from fastchat.conversation import Conversation, SeparatorStyle
-    from fastchat.model.model_adapter import get_conversation_template
-    _fastchat_available = True
-except ImportError:
-    _fastchat_available = False
+import vllm
+from vllm.engine.arg_utils import AsyncEngineArgs
+from vllm.entrypoints.openai.protocol import (CompletionRequest,
+                                              ChatCompletionRequest,
+                                              ErrorResponse)
+from vllm.logger import init_logger
+from vllm.entrypoints.openai.serving_chat import OpenAIServingChat
+from vllm.entrypoints.openai.serving_completion import OpenAIServingCompletion
+from vllm.entrypoints.openai.serving_engine import LoRA
+from ipex_llm.vllm.engine import IPEXLLMAsyncLLMEngine
+from ipex_llm.utils.common import invalidInputError
 
 TIMEOUT_KEEP_ALIVE = 5  # seconds
 
+openai_serving_chat: OpenAIServingChat = None
+openai_serving_completion: OpenAIServingCompletion = None
 logger = init_logger(__name__)
-served_model = None
-app = fastapi.FastAPI()
-engine = None
-
-
-def random_uuid() -> str:
-    return str(uuid.uuid4().hex)
-
-
-def create_error_response(status_code: HTTPStatus,
-                          message: str) -> JSONResponse:
-    return JSONResponse(ErrorResponse(message=message,
-                                      type="invalid_request_error").dict(),
-                        status_code=status_code.value)
-
-
-@app.exception_handler(RequestValidationError)
-async def validation_exception_handler(request, exc):  # pylint: disable=unused-argument
-    return create_error_response(HTTPStatus.BAD_REQUEST, str(exc))
-
-
-async def check_model(request) -> Optional[JSONResponse]:
-    if request.model == served_model:
-        return
-    ret = create_error_response(
-        HTTPStatus.NOT_FOUND,
-        f"The model `{request.model}` does not exist.",
-    )
-    return ret
-
-
-async def get_gen_prompt(request) -> str:
-    if not _fastchat_available:
-        invalidInputError(
-            False,
-            "fastchat is not installed. Please install fastchat to use "
-            "the chat completion and conversation APIs: `$ pip install fschat`"
-        )
-    if version.parse(fastchat.__version__) < version.parse("0.2.23"):
-        invalidInputError(
-            False,
-            f"fastchat version is low. Current version: {fastchat.__version__} "
-            "Please upgrade fastchat to use: `$ pip install -U fschat`")
-
-    conv = get_conversation_template(request.model)
-    conv = Conversation(
-        name=conv.name,
-        system_template=conv.system_template,
-        system_message=conv.system_message,
-        roles=conv.roles,
-        messages=list(conv.messages),  # prevent in-place modification
-        offset=conv.offset,
-        sep_style=SeparatorStyle(conv.sep_style),
-        sep=conv.sep,
-        sep2=conv.sep2,
-        stop_str=conv.stop_str,
-        stop_token_ids=conv.stop_token_ids,
-    )
-
-    if isinstance(request.messages, str):
-        prompt = request.messages
-    else:
-        for message in request.messages:
-            msg_role = message["role"]
-            if msg_role == "system":
-                conv.system_message = message["content"]
-            elif msg_role == "user":
-                conv.append_message(conv.roles[0], message["content"])
-            elif msg_role == "assistant":
-                conv.append_message(conv.roles[1], message["content"])
-            else:
-                invalidInputError(False, f"Unknown role: {msg_role}")
-
-        # Add a blank message for the assistant.
-        conv.append_message(conv.roles[1], None)
-        prompt = conv.get_prompt()
-
-    return prompt
-
-
-async def check_length(
-    request: Union[ChatCompletionRequest, CompletionRequest],
-    prompt: Optional[str]=None,
-    prompt_ids: Optional[List[int]]=None
-) -> Tuple[List[int], Optional[JSONResponse]]:
-    invalidInputError((not (prompt is None and prompt_ids is None)
-                      and not (prompt is not None and prompt_ids is not None)
-                       ), "Either prompt or prompt_ids should be provided.")
-    if prompt_ids is not None:
-        input_ids = prompt_ids
-    else:
-        input_ids = tokenizer(prompt).input_ids
-    token_num = len(input_ids)
-
-    if request.max_tokens is None:
-        request.max_tokens = max_model_len - token_num
-    if token_num + request.max_tokens > max_model_len:
-        return input_ids, create_error_response(
-            HTTPStatus.BAD_REQUEST,
-            f"This model's maximum context length is {max_model_len} tokens. "
-            f"However, you requested {request.max_tokens + token_num} tokens "
-            f"({token_num} in the messages, "
-            f"{request.max_tokens} in the completion). "
-            f"Please reduce the length of the messages or completion.",
-        )
-    else:
-        return input_ids, None
-
-
-@app.get("/v1/models")
-async def show_available_models():
-    """Show available models. Right now we only have one model."""
-    model_cards = [
-        ModelCard(id=served_model,
-                  root=served_model,
-                  permission=[ModelPermission()])
-    ]
-    return ModelList(data=model_cards)
-
-
-def create_logprobs(token_ids: List[int],
-                    id_logprobs: List[Dict[int, float]],
-                    initial_text_offset: int = 0) -> LogProbs:
-    """Create OpenAI-style logprobs."""
-    logprobs = LogProbs()
-    last_token_len = 0
-    for token_id, id_logprob in zip(token_ids, id_logprobs):
-        token = tokenizer.convert_ids_to_tokens(token_id)
-        logprobs.tokens.append(token)
-        logprobs.token_logprobs.append(id_logprob[token_id])
-        if len(logprobs.text_offset) == 0:
-            logprobs.text_offset.append(initial_text_offset)
-        else:
-            logprobs.text_offset.append(logprobs.text_offset[-1] +
-                                        last_token_len)
-        last_token_len = len(token)
-
-        logprobs.top_logprobs.append({
-            tokenizer.convert_ids_to_tokens(i): p
-            for i, p in id_logprob.items()
-        })
-    return logprobs
 
 
-@app.post("/v1/chat/completions")
-async def create_chat_completion(request: ChatCompletionRequest,
-                                 raw_request: Request):
-    """Completion API similar to OpenAI's API.
+@asynccontextmanager
+async def lifespan(app: fastapi.FastAPI):
 
-    See  https://platform.openai.com/docs/api-reference/chat/create
-    for the API specification. This API mimics the OpenAI ChatCompletion API.
+    async def _force_log():
+        while True:
+            await asyncio.sleep(10)
+            await engine.do_log_stats()
 
-    NOTE: Currently we do not support the following features:
-        - function_call (Users should implement this by themselves)
-        - logit_bias (to be supported by vLLM engine)
-    """
-    logger.info(f"Received chat completion request: {request}")
-
-    error_check_ret = await check_model(request)
-    if error_check_ret is not None:
-        return error_check_ret
-
-    if request.logit_bias is not None and len(request.logit_bias) > 0:
-        # TODO: support logit_bias in vLLM engine.
-        return create_error_response(HTTPStatus.BAD_REQUEST,
-                                     "logit_bias is not currently supported")
-
-    prompt = await get_gen_prompt(request)
-    token_ids, error_check_ret = await check_length(request, prompt=prompt)
-    if error_check_ret is not None:
-        return error_check_ret
-
-    model_name = request.model
-    request_id = f"cmpl-{random_uuid()}"
-    created_time = int(time.monotonic())
-    try:
-        sampling_params = SamplingParams(
-            n=request.n,
-            presence_penalty=request.presence_penalty,
-            frequency_penalty=request.frequency_penalty,
-            temperature=request.temperature,
-            top_p=request.top_p,
-            stop=request.stop,
-            stop_token_ids=request.stop_token_ids,
-            max_tokens=request.max_tokens,
-            best_of=request.best_of,
-            top_k=request.top_k,
-            ignore_eos=request.ignore_eos,
-            use_beam_search=request.use_beam_search,
-            skip_special_tokens=request.skip_special_tokens,
-        )
-    except ValueError as e:
-        return create_error_response(HTTPStatus.BAD_REQUEST, str(e))
-
-    result_generator = engine.generate(prompt, sampling_params, request_id,
-                                       token_ids)
-
-    def create_stream_response_json(
-        index: int,
-        text: str,
-        finish_reason: Optional[str] = None,
-        output_token_latency: Optional[List[float]] = None,
-    ) -> str:
-        if output_token_latency is None:
-            choice_data = ChatCompletionResponseStreamChoice(
-                index=index,
-                delta=DeltaMessage(content=text),
-                finish_reason=finish_reason,
-            )
-        elif len(output_token_latency) == 1:
-            # bigdl-llm change start
-            # summary: add token-time recording related logic
-            # other modifications follow the same logic
-            choice_data = ChatCompletionResponseStreamChoice(
-                index=index,
-                delta=DeltaMessage(content=text),
-                finish_reason=finish_reason,
-                first_token_time=output_token_latency[0])
-        else:
-            choice_data = ChatCompletionResponseStreamChoice(
-                index=index,
-                delta=DeltaMessage(content=text),
-                finish_reason=finish_reason,
-                first_token_time=output_token_latency[0],
-                rest_token_time=np.mean(output_token_latency[1:]))
-            # bigdl-llm change end
-        response = ChatCompletionStreamResponse(
-            id=request_id,
-            created=created_time,
-            model=model_name,
-            choices=[choice_data],
-        )
-        response_json = response.json(ensure_ascii=False)
-
-        return response_json
-
-    async def completion_stream_generator() -> AsyncGenerator[str, None]:
-        # First chunk with role
-        for i in range(request.n):
-            choice_data = ChatCompletionResponseStreamChoice(
-                index=i,
-                delta=DeltaMessage(role="assistant"),
-                finish_reason=None,
-                output_token_latency=None,
-            )
-            chunk = ChatCompletionStreamResponse(id=request_id,
-                                                 choices=[choice_data],
-                                                 model=model_name)
-            data = chunk.json(exclude_unset=True, ensure_ascii=False)
-            yield f"data: {data}\n\n"
-
-        previous_texts = [""] * request.n
-        previous_num_tokens = [0] * request.n
-        async for res in result_generator:
-            res: RequestOutput
-            for output in res.outputs:
-                i = output.index
-                delta_text = output.text[len(previous_texts[i]):]
-                previous_texts[i] = output.text
-                previous_num_tokens[i] = len(output.token_ids)
-                response_json = create_stream_response_json(
-                    index=i,
-                    text=delta_text,
-                    output_token_latency=output.output_token_latency,
-                )
-                yield f"data: {response_json}\n\n"
-                if output.finish_reason is not None:
-                    response_json = create_stream_response_json(
-                        index=i,
-                        text="",
-                        finish_reason=output.finish_reason,
-                        output_token_latency=output.output_token_latency,
-                    )
-                    yield f"data: {response_json}\n\n"
-        yield "data: [DONE]\n\n"
+    if not engine_args.disable_log_stats:
+        asyncio.create_task(_force_log())
 
-    # Streaming response
-    if request.stream:
-        return StreamingResponse(completion_stream_generator(),
-                                 media_type="text/event-stream")
+    yield
 
-    # Non-streaming response
-    final_res: RequestOutput = None
-    async for res in result_generator:
-        if await raw_request.is_disconnected():
-            # Abort the request if the client disconnects.
-            await engine.abort(request_id)
-            return create_error_response(HTTPStatus.BAD_REQUEST,
-                                         "Client disconnected")
-        final_res = res
-    invalidInputError(final_res is not None, "final result should not be None")
-    choices = []
-    for output in final_res.outputs:
-        if output.output_token_latency is None:
-            choice_data = ChatCompletionResponseChoice(
-                index=output.index,
-                message=ChatMessage(role="assistant", content=output.text),
-                finish_reason=output.finish_reason,
-            )
-        else:
-            choice_data = ChatCompletionResponseChoice(
-                index=output.index,
-                message=ChatMessage(role="assistant", content=output.text),
-                finish_reason=output.finish_reason,
-                first_token_time=output.output_token_latency[0],
-                rest_token_time=np.mean(output.output_token_latency[1:]),
-            )
-        choices.append(choice_data)
-
-    num_prompt_tokens = len(final_res.prompt_token_ids)
-    num_generated_tokens = sum(
-        len(output.token_ids) for output in final_res.outputs)
-    usage = UsageInfo(
-        prompt_tokens=num_prompt_tokens,
-        completion_tokens=num_generated_tokens,
-        total_tokens=num_prompt_tokens + num_generated_tokens,
-    )
-    response = ChatCompletionResponse(
-        id=request_id,
-        created=created_time,
-        model=model_name,
-        choices=choices,
-        usage=usage,
-    )
 
-    if request.stream:
-        # When user requests streaming but we don't stream, we still need to
-        # return a streaming response with a single event.
-        response_json = response.json(ensure_ascii=False)
-
-        async def fake_stream_generator() -> AsyncGenerator[str, None]:
-            yield f"data: {response_json}\n\n"
-            yield "data: [DONE]\n\n"
+app = fastapi.FastAPI(lifespan=lifespan)
 
-        return StreamingResponse(fake_stream_generator(),
-                                 media_type="text/event-stream")
 
-    return response
+class LoRAParserAction(argparse.Action):
 
+    def __call__(self, parser, namespace, values, option_string=None):
+        lora_list = []
+        for item in values:
+            name, path = item.split('=')
+            lora_list.append(LoRA(name, path))
+        setattr(namespace, self.dest, lora_list)
 
-@app.post("/v1/completions")
-async def create_completion(request: CompletionRequest, raw_request: Request):
-    """Completion API similar to OpenAI's API.
 
-    See https://platform.openai.com/docs/api-reference/completions/create
-    for the API specification. This API mimics the OpenAI Completion API.
-
-    NOTE: Currently we do not support the following features:
-        - echo (since the vLLM engine does not currently support
-          getting the logprobs of prompt tokens)
-        - suffix (the language models we currently support do not support
-          suffix)
-        - logit_bias (to be supported by vLLM engine)
-    """
-    logger.info(f"Received completion request: {request}")
-
-    error_check_ret = await check_model(request)
-    if error_check_ret is not None:
-        return error_check_ret
-
-    if request.echo:
-        # We do not support echo since the vLLM engine does not
-        # currently support getting the logprobs of prompt tokens.
-        return create_error_response(HTTPStatus.BAD_REQUEST,
-                                     "echo is not currently supported")
-
-    if request.suffix is not None:
-        # The language models we currently support do not support suffix.
-        return create_error_response(HTTPStatus.BAD_REQUEST,
-                                     "suffix is not currently supported")
-
-    if request.logit_bias is not None and len(request.logit_bias) > 0:
-        # TODO: support logit_bias in vLLM engine.
-        return create_error_response(HTTPStatus.BAD_REQUEST,
-                                     "logit_bias is not currently supported")
-
-    model_name = request.model
-    request_id = f"cmpl-{random_uuid()}"
-
-    use_token_ids = False
-    if isinstance(request.prompt, list):
-        if len(request.prompt) == 0:
-            return create_error_response(HTTPStatus.BAD_REQUEST,
-                                         "please provide at least one prompt")
-        first_element = request.prompt[0]
-        if isinstance(first_element, int):
-            use_token_ids = True
-            prompt = request.prompt
-        elif isinstance(first_element, (str, list)):
-            # TODO: handles multiple prompt case in list[list[int]]
-            if len(request.prompt) > 1:
-                return create_error_response(
-                    HTTPStatus.BAD_REQUEST,
-                    "multiple prompts in a batch is not currently supported")
-            use_token_ids = not isinstance(first_element, str)
-            prompt = request.prompt[0]
-    else:
-        prompt = request.prompt
-
-    if use_token_ids:
-        _, error_check_ret = await check_length(request, prompt_ids=prompt)
-    else:
-        token_ids, error_check_ret = await check_length(request, prompt=prompt)
-    if error_check_ret is not None:
-        return error_check_ret
-
-    created_time = int(time.monotonic())
-    try:
-        sampling_params = SamplingParams(
-            n=request.n,
-            best_of=request.best_of,
-            presence_penalty=request.presence_penalty,
-            frequency_penalty=request.frequency_penalty,
-            temperature=request.temperature,
-            top_p=request.top_p,
-            top_k=request.top_k,
-            stop=request.stop,
-            stop_token_ids=request.stop_token_ids,
-            ignore_eos=request.ignore_eos,
-            max_tokens=request.max_tokens,
-            logprobs=request.logprobs,
-            use_beam_search=request.use_beam_search,
-            skip_special_tokens=request.skip_special_tokens,
-        )
-    except ValueError as e:
-        return create_error_response(HTTPStatus.BAD_REQUEST, str(e))
-
-    if use_token_ids:
-        result_generator = engine.generate(None,
-                                           sampling_params,
-                                           request_id,
-                                           prompt_token_ids=prompt)
-    else:
-        result_generator = engine.generate(prompt, sampling_params, request_id,
-                                           token_ids)
-
-    # Similar to the OpenAI API, when n != best_of, we do not stream the
-    # results. In addition, we do not stream the results when use beam search.
-    stream = (request.stream
-              and (request.best_of is None or request.n == request.best_of)
-              and not request.use_beam_search)
-
-    def create_stream_response_json(
-        index: int,
-        text: str,
-        logprobs: Optional[LogProbs] = None,
-        finish_reason: Optional[str] = None,
-        output_token_latency: Optional[List[float]] = None,
-    ) -> str:
-        if output_token_latency is None:
-            choice_data = CompletionResponseStreamChoice(
-                index=index,
-                text=text,
-                logprobs=logprobs,
-                finish_reason=finish_reason,
-            )
-        elif len(output_token_latency) == 1:
-            choice_data = CompletionResponseStreamChoice(
-                index=index,
-                text=text,
-                logprobs=logprobs,
-                finish_reason=finish_reason,
-                first_token_time=output_token_latency[0])
-        else:
-            choice_data = CompletionResponseStreamChoice(
-                index=index,
-                text=text,
-                logprobs=logprobs,
-                finish_reason=finish_reason,
-                first_token_time=output_token_latency[0],
-                rest_token_time=np.mean(output_token_latency[1:]),
-            )
-        response = CompletionStreamResponse(
-            id=request_id,
-            created=created_time,
-            model=model_name,
-            choices=[choice_data],
-        )
-        response_json = response.json(ensure_ascii=False)
-
-        return response_json
-
-    async def completion_stream_generator() -> AsyncGenerator[str, None]:
-        previous_texts = [""] * request.n
-        previous_num_tokens = [0] * request.n
-        async for res in result_generator:
-            res: RequestOutput
-            for output in res.outputs:
-                i = output.index
-                delta_text = output.text[len(previous_texts[i]):]
-                if request.logprobs is not None:
-                    logprobs = create_logprobs(
-                        output.token_ids[previous_num_tokens[i]:],
-                        output.logprobs[previous_num_tokens[i]:],
-                        len(previous_texts[i]))
-                else:
-                    logprobs = None
-                previous_texts[i] = output.text
-                previous_num_tokens[i] = len(output.token_ids)
-                response_json = create_stream_response_json(
-                    index=i,
-                    text=delta_text,
-                    logprobs=logprobs,
-                    output_token_latency=output.output_token_latency,
-                )
-                yield f"data: {response_json}\n\n"
-                if output.finish_reason is not None:
-                    logprobs = (LogProbs()
-                                if request.logprobs is not None else None)
-                    response_json = create_stream_response_json(
-                        index=i,
-                        text="",
-                        logprobs=logprobs,
-                        finish_reason=output.finish_reason,
-                        output_token_latency=output.output_token_latency,
-                    )
-                    yield f"data: {response_json}\n\n"
-        yield "data: [DONE]\n\n"
-
-    # Streaming response
-    if stream:
-        return StreamingResponse(completion_stream_generator(),
-                                 media_type="text/event-stream")
-
-    # Non-streaming response
-    final_res: RequestOutput = None
-    async for res in result_generator:
-        if await raw_request.is_disconnected():
-            # Abort the request if the client disconnects.
-            await engine.abort(request_id)
-            return create_error_response(HTTPStatus.BAD_REQUEST,
-                                         "Client disconnected")
-        final_res = res
-    invalidInputError(final_res is not None, "final result should not be None")
-    choices = []
-    for output in final_res.outputs:
-        if request.logprobs is not None:
-            logprobs = create_logprobs(output.token_ids, output.logprobs)
-        else:
-            logprobs = None
-        if output.output_token_latency is None:
-            choice_data = CompletionResponseChoice(
-                index=output.index,
-                text=output.text,
-                logprobs=logprobs,
-                finish_reason=output.finish_reason,
-            )
-        else:
-            choice_data = CompletionResponseChoice(
-                index=output.index,
-                text=output.text,
-                logprobs=logprobs,
-                finish_reason=output.finish_reason,
-                first_token_time=output.output_token_latency[0],
-                rest_token_time=np.mean(output.output_token_latency[1:]),
-            )
-        choices.append(choice_data)
-
-    num_prompt_tokens = len(final_res.prompt_token_ids)
-    num_generated_tokens = sum(
-        len(output.token_ids) for output in final_res.outputs)
-    usage = UsageInfo(
-        prompt_tokens=num_prompt_tokens,
-        completion_tokens=num_generated_tokens,
-        total_tokens=num_prompt_tokens + num_generated_tokens,
-    )
-    response = CompletionResponse(
-        id=request_id,
-        created=created_time,
-        model=model_name,
-        choices=choices,
-        usage=usage,
-    )
-
-    if request.stream:
-        # When user requests streaming but we don't stream, we still need to
-        # return a streaming response with a single event.
-        response_json = response.json(ensure_ascii=False)
-
-        async def fake_stream_generator() -> AsyncGenerator[str, None]:
-            yield f"data: {response_json}\n\n"
-            yield "data: [DONE]\n\n"
-
-        return StreamingResponse(fake_stream_generator(),
-                                 media_type="text/event-stream")
-
-    return response
-
-
-if __name__ == "__main__":
+def parse_args():
     parser = argparse.ArgumentParser(
         description="vLLM OpenAI-Compatible RESTful API server.")
     parser.add_argument("--host", type=str, default=None, help="host name")
     parser.add_argument("--port", type=int, default=8000, help="port number")
+    parser.add_argument(
+        "--uvicorn-log-level",
+        type=str,
+        default="info",
+        choices=['debug', 'info', 'warning', 'error', 'critical', 'trace'],
+        help="log level for uvicorn")
     parser.add_argument("--allow-credentials",
                         action="store_true",
                         help="allow credentials")
     parser.add_argument("--allowed-origins",
                         type=json.loads,
                         default=["*"],
                         help="allowed origins")
@@ -687,47 +84,202 @@
                         type=json.loads,
                         default=["*"],
                         help="allowed methods")
     parser.add_argument("--allowed-headers",
                         type=json.loads,
                         default=["*"],
                         help="allowed headers")
+    parser.add_argument("--api-key",
+                        type=str,
+                        default=None,
+                        help="If provided, the server will require this key "
+                        "to be presented in the header.")
     parser.add_argument("--served-model-name",
                         type=str,
                         default=None,
                         help="The model name used in the API. If not "
                         "specified, the model name will be the same as "
                         "the huggingface name.")
+    parser.add_argument(
+        "--lora-modules",
+        type=str,
+        default=None,
+        nargs='+',
+        action=LoRAParserAction,
+        help="LoRA module configurations in the format name=path. "
+        "Multiple modules can be specified.")
+    parser.add_argument("--chat-template",
+                        type=str,
+                        default=None,
+                        help="The file path to the chat template, "
+                        "or the template in single-line form "
+                        "for the specified model")
+    parser.add_argument("--response-role",
+                        type=str,
+                        default="assistant",
+                        help="The role name to return if "
+                        "`request.add_generation_prompt=true`.")
+    parser.add_argument("--ssl-keyfile",
+                        type=str,
+                        default=None,
+                        help="The file path to the SSL key file")
+    parser.add_argument("--ssl-certfile",
+                        type=str,
+                        default=None,
+                        help="The file path to the SSL cert file")
+    parser.add_argument("--ssl-ca-certs",
+                        type=str,
+                        default=None,
+                        help="The CA certificates file")
+    parser.add_argument(
+        "--ssl-cert-reqs",
+        type=int,
+        default=int(ssl.CERT_NONE),
+        help="Whether client certificate is required (see stdlib ssl module's)"
+    )
+    parser.add_argument(
+        "--root-path",
+        type=str,
+        default=None,
+        help="FastAPI root_path when app is behind a path based routing proxy")
+    parser.add_argument(
+        "--middleware",
+        type=str,
+        action="append",
+        default=[],
+        help="Additional ASGI middleware to apply to the app. "
+        "We accept multiple --middleware arguments. "
+        "The value should be an import path. "
+        "If a function is provided, vLLM will add it to the server "
+        "using @app.middleware('http'). "
+        "If a class is provided, vLLM will add it to the server "
+        "using app.add_middleware(). ")
+    parser.add_argument(
+        "--load-in-low-bit",
+        type=str,
+        default="sym_int4",
+        help="Low-bit quantization for IPEX-LLM models")
 
     parser = AsyncEngineArgs.add_cli_args(parser)
-    args = parser.parse_args()
+    return parser.parse_args()
+
+
+# Add prometheus asgi middleware to route /metrics requests
+metrics_app = make_asgi_app()
+app.mount("/metrics", metrics_app)
+
+
+@app.exception_handler(RequestValidationError)
+async def validation_exception_handler(_, exc):
+    err = openai_serving_chat.create_error_response(message=str(exc))
+    return JSONResponse(err.model_dump(), status_code=HTTPStatus.BAD_REQUEST)
+
+
+@app.get("/health")
+async def health() -> Response:
+    """Health check."""
+    await openai_serving_chat.engine.check_health()
+    return Response(status_code=200)
+
+
+@app.get("/v1/models")
+async def show_available_models():
+    models = await openai_serving_chat.show_available_models()
+    return JSONResponse(content=models.model_dump())
+
+
+@app.get("/version")
+async def show_version():
+    ver = {"version": vllm.__version__}
+    return JSONResponse(content=ver)
+
+
+@app.post("/v1/chat/completions")
+async def create_chat_completion(request: ChatCompletionRequest,
+                                 raw_request: Request):
+    generator = await openai_serving_chat.create_chat_completion(
+        request, raw_request)
+    if isinstance(generator, ErrorResponse):
+        return JSONResponse(content=generator.model_dump(),
+                            status_code=generator.code)
+    if request.stream:
+        return StreamingResponse(content=generator,
+                                 media_type="text/event-stream")
+    else:
+        return JSONResponse(content=generator.model_dump())
+
+
+@app.post("/v1/completions")
+async def create_completion(request: CompletionRequest, raw_request: Request):
+    generator = await openai_serving_completion.create_completion(
+        request, raw_request)
+    if isinstance(generator, ErrorResponse):
+        return JSONResponse(content=generator.model_dump(),
+                            status_code=generator.code)
+    if request.stream:
+        return StreamingResponse(content=generator,
+                                 media_type="text/event-stream")
+    else:
+        return JSONResponse(content=generator.model_dump())
+
+
+if __name__ == "__main__":
+    args = parse_args()
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=args.allowed_origins,
         allow_credentials=args.allow_credentials,
         allow_methods=args.allowed_methods,
         allow_headers=args.allowed_headers,
     )
 
+    token = os.environ.get("VLLM_API_KEY") or args.api_key
+    if token:
+        @app.middleware("http")
+        async def authentication(request: Request, call_next):
+            if not request.url.path.startswith("/v1"):
+                return await call_next(request)
+            if request.headers.get("Authorization") != "Bearer " + token:
+                return JSONResponse(content={"error": "Unauthorized"},
+                                    status_code=401)
+            return await call_next(request)
+
+    for middleware in args.middleware:
+        module_path, object_name = middleware.rsplit(".", 1)
+        imported = getattr(importlib.import_module(module_path), object_name)
+        if inspect.isclass(imported):
+            app.add_middleware(imported)
+        elif inspect.iscoroutinefunction(imported):
+            app.middleware("http")(imported)
+        else:
+            invalidInputError(False, (f"Invalid middleware {middleware}. "
+                              f"Must be a function or a class."))
+
+    logger.info(f"vLLM API server version {vllm.__version__}")
     logger.info(f"args: {args}")
 
     if args.served_model_name is not None:
         served_model = args.served_model_name
     else:
         served_model = args.model
 
     engine_args = AsyncEngineArgs.from_cli_args(args)
-    engine = AsyncLLMEngine.from_engine_args(engine_args)
-    engine_model_config = asyncio.run(engine.get_model_config())
-    max_model_len = engine_model_config.max_model_len
-
-    # A separate tokenizer to map token IDs to strings.
-    tokenizer = get_tokenizer(engine_args.tokenizer,
-                              tokenizer_mode=engine_args.tokenizer_mode,
-                              trust_remote_code=engine_args.trust_remote_code)
+    engine = IPEXLLMAsyncLLMEngine.from_engine_args(engine_args,
+                                                    load_in_low_bit=args.load_in_low_bit)
+    openai_serving_chat = OpenAIServingChat(engine, served_model,
+                                            args.response_role,
+                                            args.lora_modules,
+                                            args.chat_template)
+    openai_serving_completion = OpenAIServingCompletion(
+        engine, served_model, args.lora_modules)
 
+    app.root_path = args.root_path
     uvicorn.run(app,
                 host=args.host,
                 port=args.port,
-                log_level="info",
-                timeout_keep_alive=TIMEOUT_KEEP_ALIVE)
+                log_level=args.uvicorn_log_level,
+                timeout_keep_alive=TIMEOUT_KEEP_ALIVE,
+                ssl_keyfile=args.ssl_keyfile,
+                ssl_certfile=args.ssl_certfile,
+                ssl_ca_certs=args.ssl_ca_certs,
+                ssl_cert_reqs=args.ssl_cert_reqs)
```

## Comparing `ipex_llm/vllm/entrypoints/__init__.py` & `ipex_llm/vllm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
```

## Comparing `ipex_llm/vllm2/model_convert.py` & `ipex_llm/vllm/model_convert.py`

 * *Files identical despite different names*

## Comparing `ipex_llm/vllm2/engine/engine.py` & `ipex_llm/vllm/engine/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from vllm.engine.llm_engine import LLMEngine
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.engine.arg_utils import AsyncEngineArgs, EngineArgs
 from vllm.engine.ray_utils import initialize_ray_cluster
 from vllm.entrypoints.llm import LLM
 from vllm.utils import Counter
 
-from ipex_llm.vllm2.model_convert import _ipex_llm_convert
+from ipex_llm.vllm.model_convert import _ipex_llm_convert
 from ipex_llm.utils.common import invalidInputError
 
 
 class IPEXLLMAsyncLLMEngine(AsyncLLMEngine):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

## Comparing `ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240422.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240422.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240421.dist-info/METADATA` & `ipex_llm-2.1.0b20240422.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240421
+Version: 2.1.0b20240422
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240421) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240422) ; extra == 'cpp'
 Provides-Extra: serving
 Requires-Dist: py-cpuinfo ; extra == 'serving'
 Requires-Dist: fschat[model_worker,webui] (==0.2.36) ; extra == 'serving'
 Requires-Dist: protobuf ; extra == 'serving'
 Provides-Extra: xpu
 Requires-Dist: py-cpuinfo ; extra == 'xpu'
 Requires-Dist: protobuf ; extra == 'xpu'
@@ -39,47 +39,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240421) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240421) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240422) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240422) ; extra == 'xpu'
 Provides-Extra: xpu-2-0
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
 Requires-Dist: protobuf ; extra == 'xpu-2-0'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
 Requires-Dist: tabulate ; extra == 'xpu-2-0'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
 Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240421) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240421) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240422) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240422) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240421) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240421) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240422) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240422) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240421.dist-info/RECORD` & `ipex_llm-2.1.0b20240422.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -38,70 +38,70 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=ZkOop2NrTlLf6sKCFWGGExGoOhjAEkpKTO-AVl2QxVM,36352
-ipex_llm/libs/bloom.dll,sha256=E02GE8sqGkmXtdKFFz4azolzvrhzHNQLuF2uw9PHCMw,460288
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=7e9FMUPjf6EIgZUZPDZ30kaZqkeheUdclWhKBGUAB30,852992
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=0PDUtA5warS-tf0RI8MIvdz13NEyohhuv9sR3YnViUI,856064
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=-pDZnJkObvcSbgWmKohPZoeeXRJiKnPDsQXwdDMA69g,843776
-ipex_llm/libs/gptneox-api.dll,sha256=CURBvu1-YJUH-RNmM0RI89MTJAmDSL3x6sKtK4i_vGA,24576
-ipex_llm/libs/gptneox.dll,sha256=6iOydIoF_NHuYjHO4PhmcHSXtMiK_CMeA1TarL9qGSE,520192
-ipex_llm/libs/libbloom_avx.dll,sha256=X5k8VRgYhpHyGiX6KCffvEKG0zDjOAYqXxxLPO0UsYQ,485888
-ipex_llm/libs/libbloom_vnni.dll,sha256=8uVDkWmRLN4fzWnh4aLuFUKdm3dZqF-yJAfx3eVAmHc,460800
-ipex_llm/libs/libgptneox_avx.dll,sha256=q-gz9en4cP13eWKf3bVz4OKCqIE6GRvptCi2M_8VO2o,545792
-ipex_llm/libs/libgptneox_vnni.dll,sha256=CIhG1CQKHTj93V5k4VdBoADXcOAcK9GsedAHHNNAX2g,520704
-ipex_llm/libs/libllama_avx.dll,sha256=jqW3w-FVtyFvaMi4QoQTFXA6Rr-3kuFQj_2JsOtw6yk,540160
-ipex_llm/libs/libllama_vnni.dll,sha256=nVf5Yc5ZzeHOnnPNVPdCMRKQPFX7zC-6oGz9cK7qW94,515072
-ipex_llm/libs/libstarcoder_avx.dll,sha256=iAgsHRa2g22tTpYfGT0WNDwMt2IBvy20dt1pXIeBtAk,577024
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=CzWwAKBOUt7cMXVQFG_aNonwglkHNxBDOhQF-xw1Di0,551936
-ipex_llm/libs/llama-api.dll,sha256=TtBBevciqsxTfb4nrK1Pk4J4osP7KETPg76ItYHm_gY,25088
-ipex_llm/libs/llama.dll,sha256=uJvNt5_90aVWwlC-QtePjq7gkJIWL2lOcfp7Km-TaKo,514560
-ipex_llm/libs/main-bloom.exe,sha256=vhyLpebr8qpgY8N2uT8c1Pc0_d-xI8uVlYIAEyIWAnk,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=9TmJ5ZzokFImV2wb4uHXOzlX3hzcE6BoDgJ9abKxb8g,726016
-ipex_llm/libs/main-gptneox.exe,sha256=efW8AzNTxAXfL7YtQLMFicyYDpu9QbP6b3gqpDbYtm0,98816
-ipex_llm/libs/main-llama.exe,sha256=UxLg0d9ZrER6_jJ5cLnX33d_qMcgzbPoae5tuLrI0qo,99840
-ipex_llm/libs/main-starcoder.exe,sha256=nE37zf2f6d5iddUyGyX9TlSK7hVZwz9SMgl_-rdz-do,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=izbDkxvfP1sUDc0s5q0RtpKy7yCtQqG1sSe0Tfrxqd8,125952
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=V-vSD7J_QY0Wtyc5mjfBgjhMHSsdoFSYsatBjuTLb5s,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=mLXthXl0kGYjmi0AEyw6FiZXGbFAa5t3o9rsA3Sgk40,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=ojeATK03mgoJYKbQy7MLjQ1GS5Ha6vlG0XDYQj8IyPA,104448
-ipex_llm/libs/quantize-llama.exe,sha256=5qpQSiAbr8kRc41kSIXZMMF6b47UQTkVHFBiyanboPo,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=z2nzd8ACgTVXIjPziGw8XrwwHt84umbyPWNDV29ylCQ,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=Z2fjFudTOkKAPneI9XJ1fuNgTZOv74J9IyRaUIo4bIQ,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=l2RlRdm0BzlexIg3BIMhJmgTSnfRHKlq8L332KONpnE,128000
-ipex_llm/libs/starcoder-api.dll,sha256=3kIsK50EG74cwbxmcekQNnfaCKKwSh0Dknm9XMNvCpo,21504
-ipex_llm/libs/starcoder.dll,sha256=rh1HkdLL7-WybMScqEGt-Q0S4tvEqADTrfHeJBjf5yA,551424
+ipex_llm/libs/bloom-api.dll,sha256=pY06fEK1BNo1t06_Ek7JoNyWxf5mydZd9vj1Pts7TUE,36352
+ipex_llm/libs/bloom.dll,sha256=qf5PEsjzp-iYeiNqySod_Qb5aRuCUBCA9kSW7hbL70I,460288
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=HKk7JR10-xDm-MXXd0zD_3jY_Vo49HEcj3oHMwTOR6M,852992
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=YGsV9nOUzT7-q66lukpI8ZHAe6us79NKCOTYFTmTIlw,856064
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=ctMIlI1308BF_5uVay3-bK0lTi-vPubMOaXmw8PlemU,843776
+ipex_llm/libs/gptneox-api.dll,sha256=8P2CBgUHqVMWYzXGfLerCIfhLgMc-8fxjqfyt-q43lk,24576
+ipex_llm/libs/gptneox.dll,sha256=UMVqeLT6N4N2w_eT8bAvAXOl3S2wC8O5Yq23FZYyjRg,520192
+ipex_llm/libs/libbloom_avx.dll,sha256=f0yp69cyfP9AOkZAMccufncea_kJ5q_kE8OvABQIAoQ,485888
+ipex_llm/libs/libbloom_vnni.dll,sha256=UyKkXSfo-8hB3nb2XyF_eChOdRL-pbsGuqGRNnN-Dyg,460800
+ipex_llm/libs/libgptneox_avx.dll,sha256=ZRGgFR_-GFtCTnjNimKhRcXwTRrtmMWJgZmXQ6iMd70,545792
+ipex_llm/libs/libgptneox_vnni.dll,sha256=SzA6Uljx7Mlq9Nm010519FDgN2JNcPOIyqKWk_lqVj0,520704
+ipex_llm/libs/libllama_avx.dll,sha256=KqsXt3l65MtoiHLOg_R6eJYPYP7Etfssm--38Cs2dAg,540160
+ipex_llm/libs/libllama_vnni.dll,sha256=jcyXTZYfVDU5UyamskAaChGOjh5O5Lx2f0dwpwR1GVE,515072
+ipex_llm/libs/libstarcoder_avx.dll,sha256=Q2X-pskdigUCriWX875p5dCPRBP45E6HdcYetwAwUrE,577024
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=t7qGh0HNJ4z5IoZUdQZ7XCd4rBoKmCVMer_boWtDx80,551936
+ipex_llm/libs/llama-api.dll,sha256=-5z8lMT4__lHU9orgKW_uiXmH9z739WPxZQSzKdERkI,25088
+ipex_llm/libs/llama.dll,sha256=uUtypCd2G81mXK743ztBcl3gTbC4Thz_QFvuE--TYXw,514560
+ipex_llm/libs/main-bloom.exe,sha256=0EEHQxf8vp_k2nuROwljh6CcG-t86bwI1n-vx-HM5hc,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=j3mtodHv80JmnkltqWq5sR9G7zRuxOAb7ADEZ5CbmQA,726016
+ipex_llm/libs/main-gptneox.exe,sha256=Z-Pp8zSz6VkPgAPjxyNdzRC85V9R9Sh2i6F6gqRpOmQ,98816
+ipex_llm/libs/main-llama.exe,sha256=opbql2-9I7TOFYYmW_gikTuDlj6Lw2aGb193yHD2_co,99840
+ipex_llm/libs/main-starcoder.exe,sha256=GoKaoQfAWRkZQ9gjgPa0LAVoj-VosfsmwNZOS6JoMMA,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=H8yO6VHkNgy66xxZsYsxuyrW6m70t9hdUvz8DX6h198,125952
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=juyU4jq8mdwpmHXpGjigyKK3TboeT1a2JpN74thsGvs,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=F70T41B2otH6rQ9bXFV436YGTmKbCb549QWJCY2XzEM,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=YNSm7T_otLgW9syLOZL4yMVixwyCk__sCar-4BF5NEc,104448
+ipex_llm/libs/quantize-llama.exe,sha256=PtGngS4R79D5gWku6lNMThRXJ4YycWeVm6FtBG1UMfs,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=x8wZawQrNWGv-e05i-2XVFwU8RYfwb-0Ln1HJvluK9A,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=SFPVxvpnE5oD7gkMAAQhFbA7x6Ba77C5oJpT-izVSWM,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=WKhORqa2YvIVtuCZNhYm26c2Yt71tuF3TMTd_YdDIgE,128000
+ipex_llm/libs/starcoder-api.dll,sha256=v56clFvrHaEsp_fT9y7vxeeqWMBB1jVgGjYANqw-jas,21504
+ipex_llm/libs/starcoder.dll,sha256=pG3TuVDELAOpeQoHF8BR8ETn4gt650J2mdEcPU97mCQ,551424
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=LNMHFYgJqna-4TfIYH7zfKElUXIYMqE0J0ICHpvMGPk,11371
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
-ipex_llm/serving/fastchat/vllm_worker.py,sha256=x22OLdf0IdvuzHHVspczXb4q6bq4GNldtc3YdZsNGUs,8692
+ipex_llm/serving/fastchat/vllm_worker.py,sha256=AKQSXstaNztTViXnWFVwgH_EmPsQzdTSuijNFldOnDk,11232
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=5LgfS8pKiMhKdx1BDKw_kBVpArT13bTIvnKfSPy3OI4,69847
-ipex_llm/transformers/convert_ipex.py,sha256=HcG4efY4nK_uFHCVL9wYKlINHTcXdWYQEMrJNcmjQRE,14274
+ipex_llm/transformers/convert.py,sha256=Pel8w2gQdL5Cj0WHj_RRx7HhpzmZ3xyRoYbWFBl2D80,70437
+ipex_llm/transformers/convert_ipex.py,sha256=34aAqZ_TXrdu-Pf4eWebSxvbnu4lg3pJEc5Wd_KA0aQ,14334
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=rllcXh7wQAtyLsXWg8BxAYJuIwTBp9aRElnKifCFWRg,4533
 ipex_llm/transformers/lisa.py,sha256=F5WxbtXQ7RdKulj83h_2DnEIgKiKGZf7zvOmg6QBl2s,3289
 ipex_llm/transformers/loader.py,sha256=mC9-RuJGIvpSdP0eyDQ3OY2q1SFTwM-TDlcv2ZSVNIo,5429
-ipex_llm/transformers/lookup.py,sha256=--9zJiNFvsEwtg7gdZAtsBVhewGDQvCdYZ-lkPmBxXo,14719
+ipex_llm/transformers/lookup.py,sha256=dvQkkovR6DvoEuaHzgyFHPmeS0Yk3Gm-T2Nm0QirywE,14775
 ipex_llm/transformers/low_bit_linear.py,sha256=ifclEZ2AAh5ZN3G6fHy-8K9NgRRHJcg6rg0z7lZwaZw,38388
 ipex_llm/transformers/model.py,sha256=hHExQLCrSntBXY8c9FXGgIMQNiL8BQ99ll4GoglGFM0,36157
 ipex_llm/transformers/modelling_bigdl.py,sha256=AqbRwpSAiHmKUo2FGOiwKtytlh-35NWb6eDy7YyNzoo,6921
 ipex_llm/transformers/qlora.py,sha256=WwHn2NXwx8SM6k7_xK1veppWiwL3g5PKihrbC3SPm-g,14770
 ipex_llm/transformers/relora.py,sha256=-dYzUV0P-IhO2jFdnzN9-v_sFzJpRj3ZwN9eCJzOoCw,16567
-ipex_llm/transformers/speculative.py,sha256=_-zqypaWWvNppbtAbnzJg3J_0QhC2Slmnad7_zhAJZs,55517
+ipex_llm/transformers/speculative.py,sha256=SfRf7mkRD4rzJn7XcZrBZaqwEbRMwkNZeNwihFmTNCo,55625
 ipex_llm/transformers/training_patch.py,sha256=4_eQ2uCtGOnRVC2iPkzquuYnvERdneBb7Ovu_pc-VCA,8404
 ipex_llm/transformers/utils.py,sha256=DZJ4Tz-WVeGORkE_Ld8YYCz4WrePiQvtfwPOK5KJlnE,13931
 ipex_llm/transformers/xpu_customize_fwd.py,sha256=wFpIhs5F6tkNs8gBOrLxWdhLzO3EDHovVkERPIAoAvg,7611
 ipex_llm/transformers/awq/__init__.py,sha256=Du5gu3-eeAkeDO_dEMBTzrDBA66DSN3uL3-rn8WGXQw,875
 ipex_llm/transformers/awq/act.py,sha256=YwomJzOOKwkKtzGrm4L4kwBstBLO1Z8SK4CKi8PSYVQ,2172
 ipex_llm/transformers/awq/awq.py,sha256=cGyRQJWwAEJtOtdSbsBoQ33KX_Ie0pv5OJHC0ACEELE,8861
 ipex_llm/transformers/awq/awq_config.py,sha256=SDZJUCAxuphwwnGqjLrbCJIo4KmFmiNgZOeKJI4DmvY,4422
@@ -145,14 +145,15 @@
 ipex_llm/transformers/models/gptj.py,sha256=TTIx461X2nOcIkrAcZhEf7d7mjJ3yvEC9KLVc1-hrpc,17973
 ipex_llm/transformers/models/gptneox.py,sha256=MVVdTbxV2oGzpCCzBMUy6oysVlnMtohJkl7SiC0xMAA,6219
 ipex_llm/transformers/models/internlm.py,sha256=mHyKQswtAHpT8R44gVvH7N57jjbk_GNtxjZWJy7ioog,11647
 ipex_llm/transformers/models/llama.py,sha256=6vQqOVYlquXh404SLTqucu8QOQDpH9fGDST4TwlIAoM,97385
 ipex_llm/transformers/models/mistral.py,sha256=GC0qaiQ1P-eOOmbvHoiaDziB2LFjhf8srll0fkr7c6M,45181
 ipex_llm/transformers/models/mixtral.py,sha256=qHeOIz8t7dTIPS9yu3QaOiN5jrUzDZ6NU9_wR6bb47U,27273
 ipex_llm/transformers/models/mpt.py,sha256=z02NwHogJZVh-Mk4sYoIzR90SFIKhoNN_-ifsD907TQ,9540
+ipex_llm/transformers/models/phi.py,sha256=i2IWpShCej-da32iZWTYVYVT5WuEqKVYFfiaiqDOYJg,7685
 ipex_llm/transformers/models/phixtral.py,sha256=4B_2iE26GlzTVdaemd6mwYQ8mp4Yo4Yq9DgSFkF0yvc,6268
 ipex_llm/transformers/models/qwen.py,sha256=JLUFrgJ3cD_2iG_pqov5zZmkZDhZUZ9Lg9bgQYJCcWk,32349
 ipex_llm/transformers/models/qwen2.py,sha256=NFLzgdvBcj5cdmCeJi0lqXz4c0JfBioZK_im2Ysynac,32725
 ipex_llm/transformers/models/qwen2_moe.py,sha256=Wv9oU1vOx087DeC4BSVLtrAAdKKnyk2y1czzhfG7ncc,30334
 ipex_llm/transformers/models/qwen_vl.py,sha256=8uu4OS-KipkMxUZxCnjjx28LfIwdqz2ue-Ul1ZwtdO0,11832
 ipex_llm/transformers/models/rwkv4.py,sha256=Kzu6QlEi0KDXiJrfoZ71TI_D2nju2-sOeaKSZqdJz8U,6135
 ipex_llm/transformers/models/rwkv5.py,sha256=nNtWQROVAUc82SClzHrbaYVsr6CALnlVos0I2TX0YUc,10722
@@ -167,52 +168,19 @@
 ipex_llm/utils/ipex_importer.py,sha256=sZro19_QZGr7oKiTq4P_i0CMUrDFlQkc7Ple9mV38CA,2477
 ipex_llm/utils/isa_checker.py,sha256=SisZ32B1G7meZvgRKZcani1WevIhMwum7nilZ3sHgXY,2259
 ipex_llm/utils/lazy_load_torch.py,sha256=MCZZr1NWwxOZQt-3OthNBxMxdN2jiRbvyXwJkrIKAhM,7129
 ipex_llm/utils/utils.py,sha256=jfDRc622QF2U2YZpmqo0evnaElHbVBDoRZqH_6hUXmI,1556
 ipex_llm/utils/common/__init__.py,sha256=pV_8I-oa8RrHSCJg6ADBY_Tre6vXCqAMyhfpj1UhvYE,988
 ipex_llm/utils/common/lazyimport.py,sha256=AOxkmsRnqpr9zEGA5_0baqrWGhdWBmIgyKO8cwF33u4,2872
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
-ipex_llm/vllm/config.py,sha256=OM6b-um5n6hRJZY7C4G9fNg9W4glz81uN_O5mYi9vN0,16868
-ipex_llm/vllm/logger.py,sha256=M58jOmSP2DAOv-9P3itndAf2oOGoezcS5yPbO9u591w,2801
-ipex_llm/vllm/outputs.py,sha256=b3ppf4FXQa8DpksGTrgdRP4vTD0Z0nqmkMQD4wGElhk,6048
-ipex_llm/vllm/sampling_params.py,sha256=TBus65w2gqU6j5CPydnwexHJNZu9a2w87WacOtQTC_I,10871
-ipex_llm/vllm/sequence.py,sha256=7Jkhvj9hkktD4sZr27vm3pVhd9rhbJA6GKG-Qqbo-Zs,13481
-ipex_llm/vllm/utils.py,sha256=UT2q9Q8ry4U7_4IFhW9Ii69Mo4bhIC_wJ1aHghTeuo4,1946
-ipex_llm/vllm/core/policy.py,sha256=FRPpx4qkZ1kd3S0LtzlXDBKW_W6l1vWMCtzaF4Vw3fM,2338
-ipex_llm/vllm/core/scheduler.py,sha256=Ub42UVY5qhHVCStg8LbayI7VhtKNHmjazJpSrndC-3o,18616
-ipex_llm/vllm/engine/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
-ipex_llm/vllm/engine/arg_utils.py,sha256=RrpGZXOOR8S1xGKgqTw94kIaXuS2liayyClruvTKkHo,12045
-ipex_llm/vllm/engine/async_llm_engine.py,sha256=xP4-R1YeWjt3v8tCd_3xStaAWomk7P6NSDrmMH1JavY,20743
-ipex_llm/vllm/engine/llm_engine.py,sha256=qSWMzXaIh8F7dKREN0qcFuRYTWEsNtSZHhv0LhkI7i0,30354
-ipex_llm/vllm/entrypoints/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
-ipex_llm/vllm/entrypoints/api_server.py,sha256=Y54ZVE4v5J34LCeC_jcQTWNlK5pwgM_MDNqzA7HQ0Mo,4462
-ipex_llm/vllm/entrypoints/llm.py,sha256=_SCiYZ7O5xeYHoB96TU7RAM6rBp9D7R9kUYtBw2CqlM,10346
-ipex_llm/vllm/entrypoints/openai/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
-ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=oST9oJJLFWPvN6ryzDyGQYM8wqmxsODJb-wPEFjCghU,28607
-ipex_llm/vllm/entrypoints/openai/openai_protocol.py,sha256=z798WFwB6KlhjmYJxFw4350BLhv8el4ip1S0qVQ2wwY,7642
-ipex_llm/vllm/entrypoints/openai/protocol.py,sha256=RwDW5Fxa0CivyWFj_mV8Lm_59o139uXg7hpYLqUPSaA,3737
-ipex_llm/vllm/model_executor/__init__.py,sha256=9C_YDoM62uXvwGFMTwITcYAOpy7zS-MaLbBDrb1_T2Q,682
-ipex_llm/vllm/model_executor/input_metadata.py,sha256=6VKtWjAD8mM9PeZ3Wy0m0zaLT5XPYAAx4eY3qFkWzlE,3642
-ipex_llm/vllm/model_executor/model_loader.py,sha256=UmWM0tlb4igBA49wLtwwekdQrHhL3UsCHgQ0V5guBuM,5372
-ipex_llm/vllm/model_executor/utils.py,sha256=Xj596gvRdfog8Cokk58sWWburJqcAendsu7X0zBfxHM,1630
-ipex_llm/vllm/model_executor/layers/bigdl_sampler.py,sha256=UkX57lEHFnPHExP7fHBbmXdk6GJesOMYUMTdg67hblA,22574
-ipex_llm/vllm/model_executor/models/bigdl_baichuan.py,sha256=XdHjfP-dCm9dOs49JdpJ1y8CPrhnrq4zWIiyHidO6UY,11431
-ipex_llm/vllm/model_executor/models/bigdl_chatglm.py,sha256=y54a6CD5DN5yINdg4_VXLM_86k03rJmMEtx1I9iYieQ,8964
-ipex_llm/vllm/model_executor/models/bigdl_llama.py,sha256=8mjFjUWXql-pmoibwlGLWpPmHAD-_bpwcnAm8V1GIxA,11428
-ipex_llm/vllm/model_executor/models/bigdl_mistral.py,sha256=slF_zjHXFrQUxB-Qsl_vc0AKbnnfC_ahfdDAKGGt7HE,8770
-ipex_llm/vllm/model_executor/models/bigdl_mixtral.py,sha256=AKRYNG366ZMpjORC30IOak2OdctqKS0TG1Y4FKv7XdE,8675
-ipex_llm/vllm/model_executor/models/bigdl_model.py,sha256=ysQ3UNwUDLIZVEPtVd_ADQHeRCN2INYQeFlVIZP8qy4,7699
-ipex_llm/vllm/transformers_utils/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
-ipex_llm/vllm/transformers_utils/tokenizer.py,sha256=PKmEi1ROhf9dKRa-7AuKYwvAY-htP-ZIAz4HhNqhokU,8707
-ipex_llm/vllm/worker/worker.py,sha256=eifKuzefL9HC1R62P0mCYBsZlclo_5hQf01vFgc6mFA,13950
-ipex_llm/vllm2/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
-ipex_llm/vllm2/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
-ipex_llm/vllm2/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
-ipex_llm/vllm2/engine/engine.py,sha256=4jQucwE46X_Bn2dA7uzjWKSJWeSiDZ76-9XW7WHJHAA,5715
-ipex_llm/vllm2/entrypoints/openai/api_server.py,sha256=M7pwasNK1J6kTTrcFgbxgXmKnPWUA4D6cw89EeA7Vw0,10475
-ipex_llm-2.1.0b20240421.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240421.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240421.dist-info/METADATA,sha256=hStuh9WEFKa8RJtkCJQQ_H4UllPv1qxrR9r798WjsgA,4400
-ipex_llm-2.1.0b20240421.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240421.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240421.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240421.dist-info/RECORD,,
+ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
+ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
+ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
+ipex_llm/vllm/engine/engine.py,sha256=G6Zyvl2vYVQD_WodYiPxKPkkG6iVxF_EeB4bNtUPCyY,5714
+ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
+ipex_llm-2.1.0b20240422.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240422.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240422.dist-info/METADATA,sha256=2qk7i0whxfnZHbFhYUIfy6us4Xhy4xYFHbqnXvfFFV0,4400
+ipex_llm-2.1.0b20240422.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240422.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240422.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240422.dist-info/RECORD,,
```

