# Comparing `tmp/swarms-4.8.2.tar.gz` & `tmp/swarms-4.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-4.8.2.tar", max compression
+gzip compressed data, was "swarms-4.8.7.tar", max compression
```

## Comparing `swarms-4.8.2.tar` & `swarms-4.8.7.tar`

### file list

```diff
@@ -1,253 +1,239 @@
--rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.8.2/LICENSE
--rw-r--r--   0        0        0    37566 2024-04-02 05:06:29.396186 swarms-4.8.2/README.md
--rw-r--r--   0        0        0     1657 2024-04-15 23:17:14.803156 swarms-4.8.2/pyproject.toml
--rw-r--r--   0        0        0      590 2024-04-02 02:30:28.406904 swarms-4.8.2/swarms/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-15 22:19:20.999687 swarms-4.8.2/swarms/agents/.DS_Store
--rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.8.2/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.8.2/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.8.2/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.8.2/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.8.2/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3503 2024-03-15 22:19:21.004191 swarms-4.8.2/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.8.2/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4971 2024-03-24 05:09:57.079682 swarms-4.8.2/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5499 2024-04-02 02:53:05.100576 swarms-4.8.2/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.8.2/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.8.2/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.8.2/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      621 2024-03-27 19:12:09.649116 swarms-4.8.2/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.8.2/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.8.2/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2827 2024-03-24 05:47:02.683694 swarms-4.8.2/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     5867 2024-03-27 19:12:09.756589 swarms-4.8.2/swarms/memory/chroma_db.py
--rw-r--r--   0        0        0     2770 2024-03-15 22:19:21.014207 swarms-4.8.2/swarms/memory/cosine_similarity.py
--rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.8.2/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3336 2024-03-15 22:19:21.014516 swarms-4.8.2/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     6125 2024-03-27 19:12:09.757820 swarms-4.8.2/swarms/memory/lanchain_chroma.py
--rw-r--r--   0        0        0     4497 2024-03-27 19:12:09.758770 swarms-4.8.2/swarms/memory/pg.py
--rw-r--r--   0        0        0     7651 2024-03-15 22:19:21.015872 swarms-4.8.2/swarms/memory/pinecone.py
--rw-r--r--   0        0        0     5738 2024-03-27 19:12:09.759612 swarms-4.8.2/swarms/memory/qdrant.py
--rw-r--r--   0        0        0     5603 2024-03-15 22:19:21.016770 swarms-4.8.2/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3841 2024-03-15 22:19:21.017420 swarms-4.8.2/swarms/memory/sqlite.py
--rw-r--r--   0        0        0     2936 2024-03-15 22:19:21.018457 swarms-4.8.2/swarms/memory/utils.py
--rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.8.2/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     6135 2024-03-15 22:19:21.019639 swarms-4.8.2/swarms/memory/weaviate_db.py
--rw-r--r--   0        0        0     2478 2024-04-05 18:37:49.855994 swarms-4.8.2/swarms/models/__init__.py
--rw-r--r--   0        0        0     2074 2024-03-27 19:58:17.874104 swarms-4.8.2/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13240 2024-03-15 22:19:21.021853 swarms-4.8.2/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12728 2024-03-15 22:19:21.022342 swarms-4.8.2/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2487 2024-03-15 22:19:21.023152 swarms-4.8.2/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3171 2024-03-15 22:19:21.023526 swarms-4.8.2/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16953 2024-03-15 22:19:21.027265 swarms-4.8.2/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10864 2024-03-15 22:19:21.028441 swarms-4.8.2/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6643 2024-03-15 22:19:21.029941 swarms-4.8.2/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-03-15 22:19:21.031788 swarms-4.8.2/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     2734 2024-03-15 22:19:21.032242 swarms-4.8.2/swarms/models/fire_function.py
--rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.8.2/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7814 2024-03-15 22:19:21.033722 swarms-4.8.2/swarms/models/gemini.py
--rw-r--r--   0        0        0     2818 2024-03-15 22:19:21.034812 swarms-4.8.2/swarms/models/gpt4_sam.py
--rw-r--r--   0        0        0    14282 2024-03-15 22:19:21.035054 swarms-4.8.2/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    13034 2024-03-15 22:19:21.035781 swarms-4.8.2/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1968 2024-03-15 22:19:21.036059 swarms-4.8.2/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5623 2024-03-15 22:19:21.036228 swarms-4.8.2/swarms/models/idefics.py
--rw-r--r--   0        0        0     7996 2024-03-15 22:19:21.036860 swarms-4.8.2/swarms/models/jina_embeds.py
--rw-r--r--   0        0        0    10752 2024-04-02 02:09:16.602464 swarms-4.8.2/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.8.2/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     6529 2024-03-15 22:19:21.038086 swarms-4.8.2/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.8.2/swarms/models/llava.py
--rw-r--r--   0        0        0     4597 2024-03-15 22:19:21.038513 swarms-4.8.2/swarms/models/medical_sam.py
--rw-r--r--   0        0        0     4324 2024-03-15 22:19:21.038800 swarms-4.8.2/swarms/models/mistral.py
--rw-r--r--   0        0        0      244 2024-03-24 04:08:38.359236 swarms-4.8.2/swarms/models/mistral_model_api.py
--rw-r--r--   0        0        0     2155 2024-03-15 22:19:21.039343 swarms-4.8.2/swarms/models/mixtral.py
--rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.8.2/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     6470 2024-03-15 22:19:21.041916 swarms-4.8.2/swarms/models/mpt.py
--rw-r--r--   0        0        0     2823 2024-03-15 22:19:21.042535 swarms-4.8.2/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.8.2/swarms/models/open_dalle.py
--rw-r--r--   0        0        0        0 2024-04-15 22:29:34.139880 swarms-4.8.2/swarms/models/open_router.py
--rw-r--r--   0        0        0    20443 2024-03-21 23:46:38.329902 swarms-4.8.2/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3175 2024-03-15 22:19:21.045986 swarms-4.8.2/swarms/models/openai_tts.py
--rw-r--r--   0        0        0     6133 2024-03-21 23:46:38.330900 swarms-4.8.2/swarms/models/palm.py
--rw-r--r--   0        0        0     1290 2024-04-05 18:37:57.323334 swarms-4.8.2/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4843 2024-03-15 22:19:21.048155 swarms-4.8.2/swarms/models/qwen.py
--rw-r--r--   0        0        0     3547 2024-03-15 22:19:21.049332 swarms-4.8.2/swarms/models/sam.py
--rw-r--r--   0        0        0    12871 2024-03-15 22:19:21.050598 swarms-4.8.2/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     7709 2024-03-15 22:19:21.050811 swarms-4.8.2/swarms/models/speecht5.py
--rw-r--r--   0        0        0     8318 2024-03-21 23:46:38.332831 swarms-4.8.2/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     5189 2024-03-15 22:19:21.051613 swarms-4.8.2/swarms/models/stable_diffusion.py
--rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.8.2/swarms/models/timm.py
--rw-r--r--   0        0        0     3990 2024-03-23 22:42:41.705709 swarms-4.8.2/swarms/models/together.py
--rw-r--r--   0        0        0      148 2024-03-15 22:19:21.053560 swarms-4.8.2/swarms/models/trocr.py
--rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.8.2/swarms/models/types.py
--rw-r--r--   0        0        0     1499 2024-03-15 22:19:21.054547 swarms-4.8.2/swarms/models/ultralytics_model.py
--rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.8.2/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.8.2/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     7678 2024-03-15 22:19:21.056747 swarms-4.8.2/swarms/models/wizard_storytelling.py
--rw-r--r--   0        0        0     9576 2024-03-15 22:19:21.057712 swarms-4.8.2/swarms/models/yarn_mistral.py
--rw-r--r--   0        0        0     2943 2024-03-15 22:19:21.058472 swarms-4.8.2/swarms/models/yi_200k.py
--rw-r--r--   0        0        0     3681 2024-03-15 22:19:21.059936 swarms-4.8.2/swarms/models/zeroscope.py
--rw-r--r--   0        0        0      775 2024-03-15 22:19:21.060753 swarms-4.8.2/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.8.2/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.8.2/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.8.2/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-03-15 22:19:21.063538 swarms-4.8.2/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.8.2/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7145 2024-03-15 22:19:21.065128 swarms-4.8.2/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.8.2/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.8.2/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.8.2/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-03-15 22:19:21.068567 swarms-4.8.2/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-03-15 22:19:21.068894 swarms-4.8.2/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.8.2/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.8.2/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.8.2/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.8.2/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.8.2/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.8.2/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.8.2/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.8.2/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.8.2/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.8.2/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-4.8.2/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.8.2/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.8.2/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.8.2/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.8.2/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.8.2/swarms/prompts/orchestrator_prompt.py
--rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.8.2/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.8.2/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.8.2/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.8.2/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-03-15 22:19:21.078885 swarms-4.8.2/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.8.2/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.8.2/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.8.2/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.8.2/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     7573 2024-03-15 22:19:21.082529 swarms-4.8.2/swarms/prompts/schema_generator.py
--rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.8.2/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3264 2024-03-15 22:19:21.083517 swarms-4.8.2/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.8.2/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.8.2/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.8.2/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.8.2/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.8.2/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-03-15 22:19:21.086266 swarms-4.8.2/swarms/prompts/tests.py
--rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.8.2/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.8.2/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.8.2/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     7134 2024-04-15 23:16:40.508533 swarms-4.8.2/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.8.2/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0     3865 2024-04-02 02:30:20.368857 swarms-4.8.2/swarms/structs/__init__.py
--rw-r--r--   0        0        0    49103 2024-04-15 23:16:41.251559 swarms-4.8.2/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.8.2/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2923 2024-03-27 19:58:17.509429 swarms-4.8.2/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     7558 2024-04-02 02:36:54.578069 swarms-4.8.2/swarms/structs/agent_rearrange.py
--rw-r--r--   0        0        0     3732 2024-03-15 22:19:21.092747 swarms-4.8.2/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     7951 2024-03-27 19:47:31.068918 swarms-4.8.2/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    11735 2024-03-15 22:19:21.093292 swarms-4.8.2/swarms/structs/autoscaler.py
--rw-r--r--   0        0        0    12262 2024-03-15 22:19:21.093668 swarms-4.8.2/swarms/structs/base.py
--rw-r--r--   0        0        0    19105 2024-03-30 07:40:24.964542 swarms-4.8.2/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12486 2024-03-27 19:12:09.737934 swarms-4.8.2/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.8.2/swarms/structs/block_wrapper.py
--rw-r--r--   0        0        0      629 2024-03-15 22:19:21.095875 swarms-4.8.2/swarms/structs/blockdevice.py
--rw-r--r--   0        0        0     3178 2024-03-15 22:19:21.096348 swarms-4.8.2/swarms/structs/blocksdict.py
--rw-r--r--   0        0        0     4887 2024-03-15 22:19:21.096911 swarms-4.8.2/swarms/structs/blockslist.py
--rw-r--r--   0        0        0     5364 2024-03-15 22:19:21.097555 swarms-4.8.2/swarms/structs/company.py
--rw-r--r--   0        0        0     4515 2024-03-15 22:19:21.097858 swarms-4.8.2/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14023 2024-03-27 19:26:23.824143 swarms-4.8.2/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12615 2024-03-15 22:19:21.099092 swarms-4.8.2/swarms/structs/debate.py
--rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.8.2/swarms/structs/document.py
--rw-r--r--   0        0        0     5433 2024-03-15 22:19:21.099780 swarms-4.8.2/swarms/structs/graph_workflow.py
--rw-r--r--   0        0        0     5066 2024-03-15 22:19:21.100307 swarms-4.8.2/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     1951 2024-03-15 22:19:21.100923 swarms-4.8.2/swarms/structs/load_balancer.py
--rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.8.2/swarms/structs/long_swarm.py
--rw-r--r--   0        0        0     7072 2024-03-15 22:19:21.101824 swarms-4.8.2/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      582 2024-03-15 22:19:21.101971 swarms-4.8.2/swarms/structs/message.py
--rw-r--r--   0        0        0     7384 2024-03-15 22:19:21.102439 swarms-4.8.2/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      867 2024-04-11 20:36:56.557766 swarms-4.8.2/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     5771 2024-03-15 22:19:21.102829 swarms-4.8.2/swarms/structs/model_parallizer.py
--rw-r--r--   0        0        0    10524 2024-03-26 17:51:23.615677 swarms-4.8.2/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-03-15 22:19:21.103669 swarms-4.8.2/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5386 2024-03-15 22:19:21.103964 swarms-4.8.2/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0     2883 2024-03-15 22:19:21.104315 swarms-4.8.2/swarms/structs/nonlinear_workflow.py
--rw-r--r--   0        0        0      364 2024-03-26 04:56:18.014859 swarms-4.8.2/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0      778 2024-03-15 22:19:21.104929 swarms-4.8.2/swarms/structs/plan.py
--rw-r--r--   0        0        0     5466 2024-03-30 18:05:25.777384 swarms-4.8.2/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     2813 2024-03-27 19:12:09.704075 swarms-4.8.2/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     4182 2024-03-21 23:46:38.336523 swarms-4.8.2/swarms/structs/schemas.py
--rw-r--r--   0        0        0     8094 2024-03-15 22:19:21.106433 swarms-4.8.2/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.8.2/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0     2894 2024-04-02 02:08:38.776074 swarms-4.8.2/swarms/structs/stackoverflow_swarm.py
--rw-r--r--   0        0        0      704 2024-03-27 19:12:09.672624 swarms-4.8.2/swarms/structs/step.py
--rw-r--r--   0        0        0    10756 2024-03-27 19:12:09.673443 swarms-4.8.2/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     5182 2024-03-27 19:47:31.068788 swarms-4.8.2/swarms/structs/swarm_redis_registry.py
--rw-r--r--   0        0        0     6470 2024-03-15 22:19:21.109619 swarms-4.8.2/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8311 2024-03-15 22:19:21.109964 swarms-4.8.2/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.8.2/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3427 2024-03-15 22:19:21.111077 swarms-4.8.2/swarms/structs/team.py
--rw-r--r--   0        0        0     3545 2024-03-15 22:19:21.112074 swarms-4.8.2/swarms/structs/utils.py
--rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.8.2/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-03-27 19:12:09.674581 swarms-4.8.2/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-4.8.2/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1087 2024-03-15 22:19:21.113750 swarms-4.8.2/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.8.2/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.8.2/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2729 2024-03-15 22:19:21.115547 swarms-4.8.2/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1996 2024-03-27 19:12:09.675144 swarms-4.8.2/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0      805 2024-03-21 23:46:38.337818 swarms-4.8.2/swarms/tools/__init__.py
--rw-r--r--   0        0        0     2647 2024-04-02 04:01:57.415991 swarms-4.8.2/swarms/tools/code_executor.py
--rw-r--r--   0        0        0     5252 2024-04-02 03:22:26.492422 swarms-4.8.2/swarms/tools/exec_tool.py
--rw-r--r--   0        0        0    14523 2024-03-24 05:11:17.316917 swarms-4.8.2/swarms/tools/format_tools.py
--rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-4.8.2/swarms/tools/function_util.py
--rw-r--r--   0        0        0      879 2024-04-03 12:10:21.544462 swarms-4.8.2/swarms/tools/interpreter.py
--rw-r--r--   0        0        0     2469 2024-03-24 05:13:04.696739 swarms-4.8.2/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.8.2/swarms/tools/tool.py
--rw-r--r--   0        0        0     6165 2024-03-15 22:19:21.121316 swarms-4.8.2/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.8.2/swarms/utils/README.md
--rw-r--r--   0        0        0     2638 2024-04-05 18:37:57.333044 swarms-4.8.2/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3537 2024-03-15 22:19:21.122933 swarms-4.8.2/swarms/utils/apa.py
--rw-r--r--   0        0        0     6071 2024-03-15 22:19:21.123535 swarms-4.8.2/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.8.2/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     6674 2024-03-15 22:19:21.125150 swarms-4.8.2/swarms/utils/code_interpreter.py
--rw-r--r--   0        0        0     1264 2024-03-15 22:19:21.125539 swarms-4.8.2/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0      808 2024-03-15 22:19:21.126204 swarms-4.8.2/swarms/utils/csv_and_pandas.py
--rw-r--r--   0        0        0     1887 2024-03-15 22:19:21.126685 swarms-4.8.2/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-03-15 22:19:21.127334 swarms-4.8.2/swarms/utils/decorators.py
--rw-r--r--   0        0        0     2342 2024-03-15 22:19:21.127636 swarms-4.8.2/swarms/utils/device_checker_cuda.py
--rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.8.2/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.8.2/swarms/utils/download_img.py
--rw-r--r--   0        0        0      690 2024-03-15 22:19:21.129208 swarms-4.8.2/swarms/utils/download_weights_from_url.py
--rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.8.2/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     3472 2024-03-15 22:19:21.130035 swarms-4.8.2/swarms/utils/execution_sandbox.py
--rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.8.2/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.8.2/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.8.2/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3286 2024-03-15 22:19:21.131635 swarms-4.8.2/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      644 2024-03-15 22:19:21.131989 swarms-4.8.2/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     1411 2024-03-15 22:19:21.132408 swarms-4.8.2/swarms/utils/function_calling_utils.py
--rw-r--r--   0        0        0     4184 2024-03-15 22:19:21.132807 swarms-4.8.2/swarms/utils/get_logger.py
--rw-r--r--   0        0        0      363 2024-03-15 22:19:21.133103 swarms-4.8.2/swarms/utils/hash.py
--rw-r--r--   0        0        0     2228 2024-03-15 22:19:21.133717 swarms-4.8.2/swarms/utils/inference_convert_utils.py
--rw-r--r--   0        0        0     2872 2024-03-15 22:19:21.133992 swarms-4.8.2/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.8.2/swarms/utils/json_utils.py
--rw-r--r--   0        0        0     1837 2024-03-15 22:19:21.134782 swarms-4.8.2/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.8.2/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     1915 2024-03-15 22:19:21.135427 swarms-4.8.2/swarms/utils/load_model_torch.py
--rw-r--r--   0        0        0     2261 2024-03-15 22:19:21.136053 swarms-4.8.2/swarms/utils/logger.py
--rw-r--r--   0        0        0    16348 2024-03-26 17:55:25.494840 swarms-4.8.2/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.8.2/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0     6723 2024-03-27 19:12:09.739420 swarms-4.8.2/swarms/utils/main.py
--rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.8.2/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0     1461 2024-03-15 22:19:21.138609 swarms-4.8.2/swarms/utils/math_eval.py
--rw-r--r--   0        0        0     1097 2024-03-15 22:19:21.139027 swarms-4.8.2/swarms/utils/pandas_to_str.py
--rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.8.2/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1199 2024-03-15 22:19:21.140224 swarms-4.8.2/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0      778 2024-03-15 22:19:21.140973 swarms-4.8.2/swarms/utils/prep_torch_model_inference.py
--rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.8.2/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1300 2024-03-15 22:19:21.141589 swarms-4.8.2/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4804 2024-03-21 23:46:38.340334 swarms-4.8.2/swarms/utils/serializable.py
--rw-r--r--   0        0        0     3034 2024-03-15 22:19:21.143281 swarms-4.8.2/swarms/utils/supervision_visualizer.py
--rw-r--r--   0        0        0      245 2024-03-15 22:19:21.144185 swarms-4.8.2/swarms/utils/torch_utils.py
--rw-r--r--   0        0        0     1308 2024-03-15 22:19:21.144686 swarms-4.8.2/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2692 2024-03-15 22:19:21.145401 swarms-4.8.2/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    40173 1970-01-01 00:00:00.000000 swarms-4.8.2/setup.py
--rw-r--r--   0        0        0    39195 1970-01-01 00:00:00.000000 swarms-4.8.2/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.8.7/LICENSE
+-rw-r--r--   0        0        0    37552 2024-04-17 20:43:58.764113 swarms-4.8.7/README.md
+-rw-r--r--   0        0        0     1800 2024-04-23 00:54:32.105628 swarms-4.8.7/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-04-02 02:30:28.406904 swarms-4.8.7/swarms/__init__.py
+-rw-r--r--   0        0        0     6148 2024-03-15 22:19:20.999687 swarms-4.8.7/swarms/agents/.DS_Store
+-rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.8.7/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.8.7/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.8.7/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.8.7/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.8.7/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3503 2024-03-15 22:19:21.004191 swarms-4.8.7/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.8.7/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4941 2024-04-18 12:43:26.447940 swarms-4.8.7/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5499 2024-04-02 02:53:05.100576 swarms-4.8.7/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.8.7/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.8.7/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.8.7/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      621 2024-03-27 19:12:09.649116 swarms-4.8.7/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.8.7/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.8.7/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2827 2024-03-24 05:47:02.683694 swarms-4.8.7/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     5867 2024-04-18 12:43:26.584739 swarms-4.8.7/swarms/memory/chroma_db.py
+-rw-r--r--   0        0        0     2742 2024-04-18 12:43:26.532818 swarms-4.8.7/swarms/memory/cosine_similarity.py
+-rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.8.7/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-4.8.7/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     6095 2024-04-18 12:43:26.587983 swarms-4.8.7/swarms/memory/lanchain_chroma.py
+-rw-r--r--   0        0        0     4475 2024-04-18 12:43:26.519175 swarms-4.8.7/swarms/memory/pg.py
+-rw-r--r--   0        0        0     7627 2024-04-18 12:42:39.431109 swarms-4.8.7/swarms/memory/pinecone.py
+-rw-r--r--   0        0        0     5738 2024-04-18 12:43:26.617809 swarms-4.8.7/swarms/memory/qdrant.py
+-rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-4.8.7/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3827 2024-04-18 12:42:39.512752 swarms-4.8.7/swarms/memory/sqlite.py
+-rw-r--r--   0        0        0     2936 2024-04-18 12:43:26.657226 swarms-4.8.7/swarms/memory/utils.py
+-rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.8.7/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     6121 2024-04-18 12:42:39.647636 swarms-4.8.7/swarms/memory/weaviate_db.py
+-rw-r--r--   0        0        0     2404 2024-04-22 23:45:03.800148 swarms-4.8.7/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-4.8.7/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13172 2024-04-18 12:43:27.185629 swarms-4.8.7/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-4.8.7/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2487 2024-03-15 22:19:21.023152 swarms-4.8.7/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3171 2024-04-18 12:43:26.791502 swarms-4.8.7/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-4.8.7/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-4.8.7/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-4.8.7/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-4.8.7/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     2734 2024-03-15 22:19:21.032242 swarms-4.8.7/swarms/models/fire_function.py
+-rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.8.7/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-4.8.7/swarms/models/gemini.py
+-rw-r--r--   0        0        0     2796 2024-04-18 12:42:39.729797 swarms-4.8.7/swarms/models/gpt4_sam.py
+-rw-r--r--   0        0        0    14214 2024-04-18 12:43:27.452395 swarms-4.8.7/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    13020 2024-04-18 12:43:27.347757 swarms-4.8.7/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1968 2024-03-15 22:19:21.036059 swarms-4.8.7/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-4.8.7/swarms/models/idefics.py
+-rw-r--r--   0        0        0     7996 2024-04-18 12:43:27.316958 swarms-4.8.7/swarms/models/jina_embeds.py
+-rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-4.8.7/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.8.7/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     6529 2024-04-18 12:43:27.304182 swarms-4.8.7/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.8.7/swarms/models/llava.py
+-rw-r--r--   0        0        0     4557 2024-04-18 12:43:27.397370 swarms-4.8.7/swarms/models/medical_sam.py
+-rw-r--r--   0        0        0     4294 2024-04-18 12:43:27.345999 swarms-4.8.7/swarms/models/mistral.py
+-rw-r--r--   0        0        0      244 2024-03-24 04:08:38.359236 swarms-4.8.7/swarms/models/mistral_model_api.py
+-rw-r--r--   0        0        0     2155 2024-03-15 22:19:21.039343 swarms-4.8.7/swarms/models/mixtral.py
+-rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.8.7/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     6448 2024-04-18 12:43:27.582607 swarms-4.8.7/swarms/models/mpt.py
+-rw-r--r--   0        0        0     2823 2024-04-18 12:43:27.453365 swarms-4.8.7/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.8.7/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2472 2024-04-17 20:43:58.873285 swarms-4.8.7/swarms/models/open_router.py
+-rw-r--r--   0        0        0    20041 2024-04-18 12:43:28.478365 swarms-4.8.7/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3175 2024-04-18 12:43:27.569100 swarms-4.8.7/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0     5961 2024-04-18 12:43:27.848709 swarms-4.8.7/swarms/models/palm.py
+-rw-r--r--   0        0        0     1521 2024-04-22 23:44:57.352370 swarms-4.8.7/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-4.8.7/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3547 2024-04-18 12:43:27.606549 swarms-4.8.7/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-4.8.7/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-4.8.7/swarms/models/speecht5.py
+-rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-4.8.7/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     5189 2024-04-18 12:43:27.897205 swarms-4.8.7/swarms/models/stable_diffusion.py
+-rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.8.7/swarms/models/timm.py
+-rw-r--r--   0        0        0     3956 2024-04-18 12:43:27.965816 swarms-4.8.7/swarms/models/together.py
+-rw-r--r--   0        0        0      148 2024-03-15 22:19:21.053560 swarms-4.8.7/swarms/models/trocr.py
+-rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.8.7/swarms/models/types.py
+-rw-r--r--   0        0        0     1485 2024-04-18 12:43:27.892853 swarms-4.8.7/swarms/models/ultralytics_model.py
+-rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.8.7/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.8.7/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     7648 2024-04-18 12:43:28.186891 swarms-4.8.7/swarms/models/wizard_storytelling.py
+-rw-r--r--   0        0        0     9546 2024-04-18 12:43:28.216830 swarms-4.8.7/swarms/models/yarn_mistral.py
+-rw-r--r--   0        0        0     2921 2024-04-18 12:42:40.582360 swarms-4.8.7/swarms/models/yi_200k.py
+-rw-r--r--   0        0        0     3681 2024-04-18 12:43:27.995338 swarms-4.8.7/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0      775 2024-03-15 22:19:21.060753 swarms-4.8.7/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.8.7/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.8.7/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.8.7/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-4.8.7/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.8.7/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7145 2024-03-15 22:19:21.065128 swarms-4.8.7/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.8.7/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.8.7/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.8.7/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-4.8.7/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-4.8.7/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.8.7/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.8.7/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.8.7/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.8.7/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.8.7/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.8.7/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.8.7/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.8.7/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.8.7/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.8.7/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-4.8.7/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.8.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.8.7/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.8.7/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.8.7/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.8.7/swarms/prompts/orchestrator_prompt.py
+-rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.8.7/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.8.7/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.8.7/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.8.7/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-4.8.7/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.8.7/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.8.7/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.8.7/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.8.7/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     7573 2024-04-18 12:43:28.296075 swarms-4.8.7/swarms/prompts/schema_generator.py
+-rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.8.7/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-4.8.7/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.8.7/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.8.7/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.8.7/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.8.7/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.8.7/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-4.8.7/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.8.7/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.8.7/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.8.7/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     7134 2024-04-18 12:43:28.263779 swarms-4.8.7/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.8.7/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0     4062 2024-04-22 17:05:28.259338 swarms-4.8.7/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    53752 2024-04-22 23:39:18.087864 swarms-4.8.7/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.8.7/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-4.8.7/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     7460 2024-04-18 12:43:28.535864 swarms-4.8.7/swarms/structs/agent_rearrange.py
+-rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-4.8.7/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-4.8.7/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12446 2024-04-22 22:34:57.654215 swarms-4.8.7/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    18739 2024-04-22 15:59:39.197542 swarms-4.8.7/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12276 2024-04-18 12:43:28.833818 swarms-4.8.7/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.8.7/swarms/structs/block_wrapper.py
+-rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-4.8.7/swarms/structs/blocks_dict.py
+-rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-4.8.7/swarms/structs/blocks_list.py
+-rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-4.8.7/swarms/structs/company.py
+-rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-4.8.7/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14037 2024-04-22 22:33:38.965703 swarms-4.8.7/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-4.8.7/swarms/structs/debate.py
+-rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.8.7/swarms/structs/document.py
+-rw-r--r--   0        0        0     5337 2024-04-18 12:42:41.464326 swarms-4.8.7/swarms/structs/graph_workflow.py
+-rw-r--r--   0        0        0     4948 2024-04-22 22:27:41.658767 swarms-4.8.7/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.8.7/swarms/structs/long_swarm.py
+-rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-4.8.7/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-4.8.7/swarms/structs/message.py
+-rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-4.8.7/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      867 2024-04-18 12:43:28.865959 swarms-4.8.7/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-4.8.7/swarms/structs/model_parallizer.py
+-rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-4.8.7/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-4.8.7/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-4.8.7/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0     2893 2024-04-18 12:43:29.126646 swarms-4.8.7/swarms/structs/nonlinear_workflow.py
+-rw-r--r--   0        0        0      379 2024-04-22 15:42:00.108678 swarms-4.8.7/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0      778 2024-03-15 22:19:21.104929 swarms-4.8.7/swarms/structs/plan.py
+-rw-r--r--   0        0        0     5268 2024-04-18 12:42:42.011555 swarms-4.8.7/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-4.8.7/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     4292 2024-04-22 16:59:54.941822 swarms-4.8.7/swarms/structs/schemas.py
+-rw-r--r--   0        0        0     6841 2024-04-22 15:58:11.142171 swarms-4.8.7/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.8.7/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0     2894 2024-04-02 02:08:38.776074 swarms-4.8.7/swarms/structs/stackoverflow_swarm.py
+-rw-r--r--   0        0        0      704 2024-03-27 19:12:09.672624 swarms-4.8.7/swarms/structs/step.py
+-rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-4.8.7/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-4.8.7/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-4.8.7/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.8.7/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3375 2024-04-18 12:43:29.501225 swarms-4.8.7/swarms/structs/team.py
+-rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-4.8.7/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7251 2024-04-18 12:42:42.381492 swarms-4.8.7/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.8.7/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-4.8.7/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-4.8.7/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-4.8.7/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.8.7/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.8.7/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2715 2024-04-18 12:43:29.717986 swarms-4.8.7/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1996 2024-03-27 19:12:09.675144 swarms-4.8.7/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1105 2024-04-22 14:25:17.851236 swarms-4.8.7/swarms/tools/__init__.py
+-rw-r--r--   0        0        0     2647 2024-04-02 04:01:57.415991 swarms-4.8.7/swarms/tools/code_executor.py
+-rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-4.8.7/swarms/tools/code_interpreter.py
+-rw-r--r--   0        0        0     5360 2024-04-18 12:43:29.866791 swarms-4.8.7/swarms/tools/exec_tool.py
+-rw-r--r--   0        0        0     3450 2024-04-18 12:42:42.695394 swarms-4.8.7/swarms/tools/execution_sandbox.py
+-rw-r--r--   0        0        0    14249 2024-04-18 12:43:30.509095 swarms-4.8.7/swarms/tools/format_tools.py
+-rw-r--r--   0        0        0     1405 2024-04-18 12:42:42.685653 swarms-4.8.7/swarms/tools/function_calling_utils.py
+-rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-4.8.7/swarms/tools/function_util.py
+-rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.8.7/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-4.8.7/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-4.8.7/swarms/tools/math_eval.py
+-rw-r--r--   0        0        0     3827 2024-04-22 23:37:59.287355 swarms-4.8.7/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.8.7/swarms/tools/tool.py
+-rw-r--r--   0        0        0     6165 2024-03-15 22:19:21.121316 swarms-4.8.7/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.8.7/swarms/utils/README.md
+-rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-4.8.7/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-4.8.7/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-4.8.7/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.8.7/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-4.8.7/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-4.8.7/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-4.8.7/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.8.7/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.8.7/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.8.7/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.8.7/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.8.7/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.8.7/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-4.8.7/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-4.8.7/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-4.8.7/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-4.8.7/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-4.8.7/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.8.7/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-4.8.7/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-4.8.7/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.8.7/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.8.7/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.8.7/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-4.8.7/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.8.7/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-4.8.7/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-4.8.7/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1308 2024-03-15 22:19:21.144686 swarms-4.8.7/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-4.8.7/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    40152 1970-01-01 00:00:00.000000 swarms-4.8.7/setup.py
+-rw-r--r--   0        0        0    39157 1970-01-01 00:00:00.000000 swarms-4.8.7/PKG-INFO
```

### Comparing `swarms-4.8.2/LICENSE` & `swarms-4.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/README.md` & `swarms-4.8.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 </div>
 
-Individual agents are barely being deployd into production because of 5 suffocating challanges: short memory, single task threading, hallucinations, high cost, and lack of collaboration.  With Multi-agent collaboration, you can effectively eliminate all of these issues. Swarms provides you with simple, reliable, and agile primitives to build your own Swarm for your specific use case. Now, Swarms is being used in production by RBC, John Deere, and many AI startups. To learn more about the unparalled benefits about multi-agent collaboration check out this github repository for research papers or book a call with me!
+Individual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups. For more information on the unparalleled benefits of multi-agent collaboration, check out this GitHub repository for research papers or schedule a call with me!
 
 ----
 
 ## Install
 `pip3 install -U swarms`
 
 ---
```

### Comparing `swarms-4.8.2/pyproject.toml` & `swarms-4.8.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,92 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "4.8.2"
+version = "4.8.7"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
-documentation = "https://swarms.apac.ai"  
-readme = "README.md" 
+documentation = "https://swarms.apac.ai"
+readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
-keywords = ["artificial intelligence", "deep learning", "optimizers", "Prompt Engineering", "swarms", "agents"]
+keywords = [
+    "artificial intelligence",
+    "deep learning",
+    "optimizers",
+    "Prompt Engineering",
+    "swarms",
+    "agents",
+]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 torch = ">=2.1.1,<3.0"
 transformers = ">= 4.39.0, <5.0.0"
 asyncio = ">=3.4.3,<4.0"
-einops = "0.7.0"
-langchain-core = "0.1.33"
 langchain-community = "0.0.29"
 langchain-experimental = "0.0.55"
 backoff = "2.2.1"
 toml = "*"
 pypdf = "4.1.0"
-httpx = "0.24.1"
 ratelimit = "2.2.1"
 loguru = "0.7.2"
 pydantic = "2.6.4"
 tenacity = "8.2.3"
 Pillow = "10.2.0"
-rich = "13.5.2"
 psutil = "*"
 sentry-sdk = "*"
 python-dotenv = "*"
 accelerate = "0.28.0"
-
-[tool.poetry.dev-dependencies]
-black = "23.3.0"
+opencv-python = "^4.9.0.80"
+yaml = "*"
+docstring_parser = "0.16"
 
 [tool.poetry.group.lint.dependencies]
+black = "^23.1.0"
 ruff = ">=0.0.249,<0.3.5"
 types-toml = "^0.10.8.1"
 types-pytz = "^2023.3.0.0"
-black = "^23.1.0"
 types-chardet = "^5.0.4.6"
 mypy-protobuf = "^3.0.0"
 
 
+[tool.poetry.group.test.dependencies]
+pytest = "^8.1.1"
+termcolor = "^2.4.0"
+pandas = "^2.2.2"
+fastapi = "^0.110.1"
+
 [tool.ruff]
-line-length = 70
-select = ["E4", "E7", "E9", "F"]
-ignore = []
-fixable = ["ALL"]
-unfixable = []
+line-length = 75
 
 [tool.black]
-line-length = 70
-target-version = ['py38']
-preview = true
+target-version = ["py38"]
+line-length = 75
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+  | docs
+)/
+'''
+
```

### Comparing `swarms-4.8.2/swarms/__init__.py` & `swarms-4.8.7/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/.DS_Store` & `swarms-4.8.7/swarms/agents/.DS_Store`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/__init__.py` & `swarms-4.8.7/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/agent_wrapper.py` & `swarms-4.8.7/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/base.py` & `swarms-4.8.7/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/developer_agents.py` & `swarms-4.8.7/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/omni_modal_agent.py` & `swarms-4.8.7/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/simple_agent.py` & `swarms-4.8.7/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/agents/tool_agent.py` & `swarms-4.8.7/swarms/agents/tool_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,11 +143,9 @@
             else:
                 raise Exception(
                     "Either model or llm should be provided to the"
                     " ToolAgent"
                 )
 
         except Exception as error:
-            logger.error(
-                f"Error running {self.name} for task: {task}"
-            )
+            logger.error(f"Error running {self.name} for task: {task}")
             raise error
```

### Comparing `swarms-4.8.2/swarms/agents/worker_agent.py` & `swarms-4.8.7/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/artifacts/base_artifact.py` & `swarms-4.8.7/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/artifacts/text_artifact.py` & `swarms-4.8.7/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/__init__.py` & `swarms-4.8.7/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/base_db.py` & `swarms-4.8.7/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/base_vectordb.py` & `swarms-4.8.7/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/chroma_db.py` & `swarms-4.8.7/swarms/memory/chroma_db.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/cosine_similarity.py` & `swarms-4.8.7/swarms/memory/cosine_similarity.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,19 +65,15 @@
             second contains corresponding cosine similarities.
     """
     if len(X) == 0 or len(Y) == 0:
         return [], []
     score_array = cosine_similarity(X, Y)
     score_threshold = score_threshold or -1.0
     score_array[score_array < score_threshold] = 0
-    top_k = min(
-        top_k or len(score_array), np.count_nonzero(score_array)
-    )
-    top_k_idxs = np.argpartition(score_array, -top_k, axis=None)[
-        -top_k:
+    top_k = min(top_k or len(score_array), np.count_nonzero(score_array))
+    top_k_idxs = np.argpartition(score_array, -top_k, axis=None)[-top_k:]
+    top_k_idxs = top_k_idxs[np.argsort(score_array.ravel()[top_k_idxs])][
+        ::-1
     ]
-    top_k_idxs = top_k_idxs[
-        np.argsort(score_array.ravel()[top_k_idxs])
-    ][::-1]
     ret_idxs = np.unravel_index(top_k_idxs, score_array.shape)
     scores = score_array.ravel()[top_k_idxs].tolist()
     return list(zip(*ret_idxs)), scores  # type: ignore
```

### Comparing `swarms-4.8.2/swarms/memory/dict_internal_memory.py` & `swarms-4.8.7/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/dict_shared_memory.py` & `swarms-4.8.7/swarms/memory/dict_shared_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         entry: Any,
     ) -> bool:
         """Add an entry to the internal memory."""
         with self.lock:
             entry_id = str(uuid.uuid4())
             data = {}
             epoch = datetime.datetime.utcfromtimestamp(0)
-            epoch = (
-                datetime.datetime.utcnow() - epoch
-            ).total_seconds()
+            epoch = (datetime.datetime.utcnow() - epoch).total_seconds()
             data[entry_id] = {
                 "agent": agent_id,
                 "epoch": epoch,
                 "score": score,
                 "cycle": agent_cycle,
                 "content": entry,
             }
```

### Comparing `swarms-4.8.2/swarms/memory/lanchain_chroma.py` & `swarms-4.8.7/swarms/memory/lanchain_chroma.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,17 +166,15 @@
 
         if type == "mmr":
             texts = self.db.max_marginal_relevance_search(
                 query=query, k=k, fetch_k=min(20, self.count)
             )
             texts = [text.page_content for text in texts]
         elif type == "cos":
-            texts = self.db.similarity_search_with_score(
-                query=query, k=k
-            )
+            texts = self.db.similarity_search_with_score(query=query, k=k)
             texts = [
                 text[0].page_content
                 for text in texts
                 if text[-1] < distance_threshold
             ]
 
         return texts
```

### Comparing `swarms-4.8.2/swarms/memory/pg.py` & `swarms-4.8.7/swarms/memory/pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,15 @@
         Initializes a new instance of the PostgresDB class.
 
         Args:
             connection_string (str): The connection string for the Postgres database.
             table_name (str): The name of the table in the database.
 
         """
-        self.engine = create_engine(
-            connection_string, *args, **kwargs
-        )
+        self.engine = create_engine(connection_string, *args, **kwargs)
         self.table_name = table_name
         self.VectorModel = self._create_vector_model()
 
     def _create_vector_model(self):
         """
         Creates the SQLAlchemy model for the vector table.
```

### Comparing `swarms-4.8.2/swarms/memory/pinecone.py` & `swarms-4.8.7/swarms/memory/pinecone.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,17 +119,15 @@
             vector_id (Optional[str], optional): _description_. Defaults to None.
             namespace (Optional[str], optional): _description_. Defaults to None.
             meta (Optional[dict], optional): _description_. Defaults to None.
 
         Returns:
             str: _description_
         """
-        vector_id = (
-            vector_id if vector_id else str_to_hash(str(vector))
-        )
+        vector_id = vector_id if vector_id else str_to_hash(str(vector))
 
         params = {"namespace": namespace} | kwargs
 
         self.index.upsert([(vector_id, vector, meta)], **params)
 
         return vector_id
```

### Comparing `swarms-4.8.2/swarms/memory/qdrant.py` & `swarms-4.8.7/swarms/memory/qdrant.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/short_term_memory.py` & `swarms-4.8.7/swarms/memory/short_term_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 import threading
 
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 
 
 class ShortTermMemory(BaseStructure):
     """Short term memory.
 
     Args:
     return_str (bool, optional): _description_. Defaults to True.
@@ -36,17 +36,15 @@
     ):
         self.return_str = return_str
         self.autosave = autosave
         self.short_term_memory = []
         self.medium_term_memory = []
         self.lock = threading.Lock()
 
-    def add(
-        self, role: str = None, message: str = None, *args, **kwargs
-    ):
+    def add(self, role: str = None, message: str = None, *args, **kwargs):
         """Add a message to the short term memory.
 
         Args:
             role (str, optional): _description_. Defaults to None.
             message (str, optional): _description_. Defaults to None.
 
         Returns:
@@ -156,17 +154,15 @@
             filename (str): _description_
         """
         try:
             with self.lock:
                 with open(filename, "w") as f:
                     json.dump(
                         {
-                            "short_term_memory": (
-                                self.short_term_memory
-                            ),
+                            "short_term_memory": (self.short_term_memory),
                             "medium_term_memory": (
                                 self.medium_term_memory
                             ),
                         },
                         f,
                     )
 
@@ -180,16 +176,14 @@
         Args:
             filename (str): _description_
         """
         try:
             with self.lock:
                 with open(filename) as f:
                     data = json.load(f)
-                self.short_term_memory = data.get(
-                    "short_term_memory", []
-                )
+                self.short_term_memory = data.get("short_term_memory", [])
                 self.medium_term_memory = data.get(
                     "medium_term_memory", []
                 )
                 logging.info(f"Loaded memory from {filename}")
         except Exception as error:
             print(f"Erorr loading memory from {filename}: {error}")
```

### Comparing `swarms-4.8.2/swarms/memory/sqlite.py` & `swarms-4.8.7/swarms/memory/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from typing import Any, List, Optional, Tuple
 
 from swarms.memory.base_vectordb import AbstractVectorDatabase
 
 try:
     import sqlite3
 except ImportError:
-    raise ImportError(
-        "Please install sqlite3 to use the SQLiteDB class."
-    )
+    raise ImportError("Please install sqlite3 to use the SQLiteDB class.")
 
 
 class SQLiteDB(AbstractVectorDatabase):
     """
     A reusable class for SQLite database operations with methods for adding,
     deleting, updating, and querying data.
```

### Comparing `swarms-4.8.2/swarms/memory/utils.py` & `swarms-4.8.7/swarms/memory/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/visual_memory.py` & `swarms-4.8.7/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/memory/weaviate_db.py` & `swarms-4.8.7/swarms/memory/weaviate_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,17 +122,15 @@
         try:
             collection = self.client.collections.get(collection_name)
             return collection.data.insert(properties)
         except Exception as error:
             print(f"Error adding object: {error}")
             raise
 
-    def query(
-        self, collection_name: str, query: str, limit: int = 10
-    ):
+    def query(self, collection_name: str, query: str, limit: int = 10):
         """Query objects from a specified collection.
 
         Args:
             collection_name (str): _description_
             query (str): _description_
             limit (int, optional): _description_. Defaults to 10.
```

### Comparing `swarms-4.8.2/swarms/models/__init__.py` & `swarms-4.8.7/swarms/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 )
 from swarms.models.popular_llms import (
     OpenAIChatLLM as OpenAIChat,
 )
 from swarms.models.popular_llms import (
     OpenAILLM as OpenAI,
 )
-from swarms.models.popular_llms import (
-    ReplicateLLM as Replicate,
-)
 from swarms.models.popular_llms import OctoAIChat
 from swarms.models.qwen import QwenVLMultiModal  # noqa: E402
 
 from swarms.models.sampling_params import SamplingParams, SamplingType
 from swarms.models.together import TogetherLLM  # noqa: E402
 from swarms.models.types import (  # noqa: E402
     AudioModality,
```

### Comparing `swarms-4.8.2/swarms/models/base_embedding_model.py` & `swarms-4.8.7/swarms/models/base_embedding_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         tokenizer: An instance of `BaseTokenizer` to use when calculating tokens.
     """
 
     model: str = None
     tokenizer: Callable = None
     chunker: Callable = None
 
-    def embed_text_artifact(
-        self, artifact: TextArtifact
-    ) -> list[float]:
+    def embed_text_artifact(self, artifact: TextArtifact) -> list[float]:
         return self.embed_string(artifact.to_text())
 
     def embed_string(self, string: str) -> list[float]:
         for attempt in self.retrying():
             with attempt:
                 if (
                     self.tokenizer
```

### Comparing `swarms-4.8.2/swarms/models/base_llm.py` & `swarms-4.8.7/swarms/models/base_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,23 +150,19 @@
 
         Args:
             tasks (List[str]): _description_
 
         Returns:
             _type_: _description_
         """
-        return await asyncio.gather(
-            *(self.arun(task) for task in tasks)
-        )
+        return await asyncio.gather(*(self.arun(task) for task in tasks))
 
     def chat(self, task: str, history: str = "") -> str:
         """Chat with the model"""
-        complete_task = (
-            task + " | " + history
-        )  # Delimiter for clarity
+        complete_task = task + " | " + history  # Delimiter for clarity
         return self.run(complete_task)
 
     def __call__(self, task: str) -> str:
         """Call the model"""
         return self.run(task)
 
     def _tokens_per_second(self) -> float:
@@ -205,17 +201,15 @@
     def enable_logging(self, log_file: str = "model.log"):
         """Initialize logging for the model."""
         logging.basicConfig(filename=log_file, level=logging.INFO)
         self.log_file = log_file
 
     def log_event(self, message: str):
         """Log an event."""
-        logging.info(
-            f"{time.strftime('%Y-%m-%d %H:%M:%S')} - {message}"
-        )
+        logging.info(f"{time.strftime('%Y-%m-%d %H:%M:%S')} - {message}")
 
     def save_checkpoint(self, checkpoint_dir: str = "checkpoints"):
         """Save the model state."""
         # This is a placeholder for actual checkpointing logic.
         if not os.path.exists(checkpoint_dir):
             os.makedirs(checkpoint_dir)
         checkpoint_path = os.path.join(
```

### Comparing `swarms-4.8.2/swarms/models/base_multimodal_model.py` & `swarms-4.8.7/swarms/models/base_multimodal_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,17 +131,15 @@
         """Get the image from the web"""
         try:
             response = requests.get(img)
             response.raise_for_status()
             image_pil = Image.open(BytesIO(response.content))
             return image_pil
         except requests.RequestException as error:
-            print(
-                f"Error fetching image from {img} and error: {error}"
-            )
+            print(f"Error fetching image from {img} and error: {error}")
             return None
 
     def encode_img(self, img: str):
         """Encode the image to base64"""
         with open(img, "rb") as image_file:
             return base64.b64encode(image_file.read()).decode("utf-8")
 
@@ -186,42 +184,36 @@
             print(f"Error processing video {error} try again")
             raise error
 
     def clear_chat_history(self):
         """Clear the chat history"""
         self.chat_history = []
 
-    def run_many(
-        self, tasks: List[str], imgs: List[str], *args, **kwargs
-    ):
+    def run_many(self, tasks: List[str], imgs: List[str], *args, **kwargs):
         """
         Run the model on multiple tasks and images all at once using concurrent
 
         Args:
             tasks (List[str]): List of tasks
             imgs (List[str]): List of image paths
 
         Returns:
             List[str]: List of responses
 
 
         """
         # Instantiate the thread pool executor
-        with ThreadPoolExecutor(
-            max_workers=self.max_workers
-        ) as executor:
+        with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
             results = executor.map(self.run, tasks, imgs)
 
         # Print the results for debugging
         for result in results:
             print(result)
 
-    def run_batch(
-        self, tasks_images: List[Tuple[str, str]]
-    ) -> List[str]:
+    def run_batch(self, tasks_images: List[Tuple[str, str]]) -> List[str]:
         """Process a batch of tasks and images"""
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = [
                 executor.submit(self.run, task, img)
                 for task, img in tasks_images
             ]
             results = [future.result() for future in futures]
@@ -240,17 +232,15 @@
 
     async def run_batch_async_with_retries(
         self, tasks_images: List[Tuple[str, str]]
     ) -> List[str]:
         """Process a batch of tasks and images asynchronously with retries"""
         loop = asyncio.get_event_loop()
         futures = [
-            loop.run_in_executor(
-                None, self.run_with_retries, task, img
-            )
+            loop.run_in_executor(None, self.run_with_retries, task, img)
             for task, img in tasks_images
         ]
         return await asyncio.gather(*futures)
 
     def unique_chat_history(self):
         """Get the unique chat history"""
         return list(set(self.chat_history))
@@ -260,17 +250,15 @@
         for i in range(self.retries):
             try:
                 return self.run(task, img)
             except Exception as error:
                 print(f"Error with the request {error}")
                 continue
 
-    def run_batch_with_retries(
-        self, tasks_images: List[Tuple[str, str]]
-    ):
+    def run_batch_with_retries(self, tasks_images: List[Tuple[str, str]]):
         """Run the model with retries"""
         for i in range(self.retries):
             try:
                 return self.run_batch(tasks_images)
             except Exception as error:
                 print(f"Error with the request {error}")
                 continue
```

### Comparing `swarms-4.8.2/swarms/models/base_tts.py` & `swarms-4.8.7/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/base_ttv.py` & `swarms-4.8.7/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/cog_vlm.py` & `swarms-4.8.7/swarms/models/cog_vlm.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,17 +295,15 @@
     ):
         """
         Generates a stream of responses using the CogVLM model in inference mode.
         It's optimized to handle continuous input-output interactions with the model in a streaming manner.
         """
         messages = params["messages"]
         temperature = float(params.get("temperature", 1.0))
-        repetition_penalty = float(
-            params.get("repetition_penalty", 1.0)
-        )
+        repetition_penalty = float(params.get("repetition_penalty", 1.0))
         top_p = float(params.get("top_p", 1.0))
         max_new_tokens = int(params.get("max_tokens", 256))
         query, history, image_list = self.process_history_and_images(
             messages
         )
 
         logger.debug(f"==== request ====\n{query}")
@@ -314,17 +312,15 @@
             self.tokenizer,
             query=query,
             history=history,
             images=[image_list[-1]],
         )
         inputs = {
             "input_ids": (
-                input_by_model["input_ids"]
-                .unsqueeze(0)
-                .to(self.device)
+                input_by_model["input_ids"].unsqueeze(0).to(self.device)
             ),
             "token_type_ids": (
                 input_by_model["token_type_ids"]
                 .unsqueeze(0)
                 .to(self.device)
             ),
             "attention_mask": (
@@ -375,17 +371,15 @@
             self.model.generate(**inputs, **gen_kwargs)
             for next_text in streamer:
                 generated_text += next_text
                 yield {
                     "text": generated_text,
                     "usage": {
                         "prompt_tokens": input_echo_len,
-                        "completion_tokens": (
-                            total_len - input_echo_len
-                        ),
+                        "completion_tokens": (total_len - input_echo_len),
                         "total_tokens": total_len,
                     },
                 }
         ret = {
             "text": generated_text,
             "usage": {
                 "prompt_tokens": input_echo_len,
@@ -433,17 +427,15 @@
                 text_content = content
 
             # Extract image data
             if isinstance(content, list):  # image
                 for item in content:
                     if isinstance(item, ImageUrlContent):
                         image_url = item.image_url.url
-                        if image_url.startswith(
-                            "data:image/jpeg;base64,"
-                        ):
+                        if image_url.startswith("data:image/jpeg;base64,"):
                             base64_encoded_image = image_url.split(
                                 "data:image/jpeg;base64,"
                             )[1]
                             image_data = base64.b64decode(
                                 base64_encoded_image
                             )
                             image = Image.open(
@@ -467,17 +459,15 @@
                             f" {text_content}"
                         )
                     formatted_history[-1] = (
                         formatted_history[-1][0],
                         text_content,
                     )
                 else:
-                    raise AssertionError(
-                        "assistant reply before user"
-                    )
+                    raise AssertionError("assistant reply before user")
             else:
                 raise AssertionError(f"unrecognized role: {role}")
 
         return last_user_query, formatted_history, image_list
 
     async def predict(self, params: dict):
         """
```

### Comparing `swarms-4.8.2/swarms/models/dalle3.py` & `swarms-4.8.7/swarms/models/dalle3.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,17 +195,15 @@
         """
         full_path = os.path.join(self.save_path, filename)
         response = requests.get(img_url)
         if response.status_code == 200:
             with open(full_path, "wb") as file:
                 file.write(response.content)
         else:
-            raise ValueError(
-                f"Failed to download image from {img_url}"
-            )
+            raise ValueError(f"Failed to download image from {img_url}")
 
     def create_variations(self, img: str):
         """
         Create variations of an image using the Dalle3 API
 
         Parameters:
         -----------
@@ -245,17 +243,15 @@
             )
             print(
                 colored(
                     f"Error running Dalle3: {error.http_status}",
                     "red",
                 )
             )
-            print(
-                colored(f"Error running Dalle3: {error.error}", "red")
-            )
+            print(colored(f"Error running Dalle3: {error.error}", "red"))
             raise error
 
     def print_dashboard(self):
         """Print the Dalle3 dashboard"""
         print(
             colored(
                 f"""Dalle3 Dashboard: 
@@ -306,17 +302,15 @@
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=max_workers
         ) as executor:
             future_to_task = {
                 executor.submit(self, task): task for task in tasks
             }
             results = []
-            for future in concurrent.futures.as_completed(
-                future_to_task
-            ):
+            for future in concurrent.futures.as_completed(future_to_task):
                 task = future_to_task[future]
                 try:
                     img = future.result()
                     results.append(img)
 
                     print(f"Task {task} completed: {img}")
                 except Exception as error:
@@ -355,13 +349,11 @@
         """Repr method for the Dalle3 class"""
         return f"Dalle3(image_url={self.image_url})"
 
     def __str__(self):
         """Str method for the Dalle3 class"""
         return f"Dalle3(image_url={self.image_url})"
 
-    @backoff.on_exception(
-        backoff.expo, Exception, max_tries=max_retries
-    )
+    @backoff.on_exception(backoff.expo, Exception, max_tries=max_retries)
     def rate_limited_call(self, task: str):
         """Rate limited call to the Dalle3 API"""
         return self.__call__(task)
```

### Comparing `swarms-4.8.2/swarms/models/distilled_whisperx.py` & `swarms-4.8.7/swarms/models/distilled_whisperx.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,15 @@
         # For async usage
         transcription = asyncio.run(model_wrapper.async_transcribe('path/to/audio.mp3'))
     """
 
     def __init__(self, model_id="distil-whisper/distil-large-v2"):
         self.device = "cuda:0" if torch.cuda.is_available() else "cpu"
         self.torch_dtype = (
-            torch.float16
-            if torch.cuda.is_available()
-            else torch.float32
+            torch.float16 if torch.cuda.is_available() else torch.float32
         )
         self.model_id = model_id
         self.model = AutoModelForSpeechSeq2Seq.from_pretrained(
             model_id,
             torch_dtype=self.torch_dtype,
             low_cpu_mem_usage=True,
             use_safetensors=True,
@@ -108,17 +106,15 @@
     async def async_transcribe(self, inputs: Union[str, dict]):
         """
         Asynchronously transcribe the given audio input using the Distil-Whisper model.
         :param inputs: A string representing the file path or a dict with audio data.
         :return: The transcribed text.
         """
         loop = asyncio.get_event_loop()
-        return await loop.run_in_executor(
-            None, self.transcribe, inputs
-        )
+        return await loop.run_in_executor(None, self.transcribe, inputs)
 
     def real_time_transcribe(self, audio_file_path, chunk_duration=5):
         """
         Simulates real-time transcription of an audio file, processing and printing results
         in chunks with colored output for readability.
 
         :param audio_file_path: Path to the audio file to be transcribed.
@@ -134,53 +130,47 @@
                 # Load the whole audio file, but process and transcribe it in chunks
                 audio_input = self.processor.audio_file_to_array(
                     audio_file_path
                 )
                 sample_rate = audio_input.sampling_rate
                 len(audio_input.array) / sample_rate
                 chunks = [
-                    audio_input.array[
-                        i : i + sample_rate * chunk_duration
-                    ]
+                    audio_input.array[i : i + sample_rate * chunk_duration]
                     for i in range(
                         0,
                         len(audio_input.array),
                         sample_rate * chunk_duration,
                     )
                 ]
 
                 print(
-                    colored(
-                        "Starting real-time transcription...", "green"
-                    )
+                    colored("Starting real-time transcription...", "green")
                 )
 
                 for i, chunk in enumerate(chunks):
                     # Process the current chunk
                     processed_inputs = self.processor(
                         chunk,
                         sampling_rate=sample_rate,
                         return_tensors="pt",
                         padding=True,
                     )
-                    processed_inputs = (
-                        processed_inputs.input_values.to(self.device)
+                    processed_inputs = processed_inputs.input_values.to(
+                        self.device
                     )
 
                     # Generate transcription for the chunk
                     logits = self.model.generate(processed_inputs)
                     transcription = self.processor.batch_decode(
                         logits, skip_special_tokens=True
                     )[0]
 
                     # Print the chunk's transcription
                     print(
-                        colored(
-                            f"Chunk {i+1}/{len(chunks)}: ", "yellow"
-                        )
+                        colored(f"Chunk {i+1}/{len(chunks)}: ", "yellow")
                         + transcription
                     )
 
                     # Wait for the chunk's duration to simulate real-time processing
                     time.sleep(chunk_duration)
 
         except Exception as e:
```

### Comparing `swarms-4.8.2/swarms/models/embeddings_base.py` & `swarms-4.8.7/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/fire_function.py` & `swarms-4.8.7/swarms/models/fire_function.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/fuyu.py` & `swarms-4.8.7/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/gemini.py` & `swarms-4.8.7/swarms/models/gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,17 +108,15 @@
             max_output_tokens=max_tokens,
             temperature=temperature,
             *args,
             **kwargs,
         )
 
         # Initialize the model
-        self.model = genai.GenerativeModel(
-            model_name, *args, **kwargs
-        )
+        self.model = genai.GenerativeModel(model_name, *args, **kwargs)
 
         # Check for the key
         if self.gemini_api_key is None:
             raise ValueError("Please provide a Gemini API key")
 
     def system_prompt_prep(
         self,
@@ -207,17 +205,15 @@
                 raise ValueError("Please provide an image to process")
             if type is None:
                 raise ValueError("Please provide the image type")
             if self.gemini_api_key is None:
                 raise ValueError("Please provide a Gemini API key")
 
             # Load the image
-            img = [
-                {"mime_type": type, "data": Path(img).read_bytes()}
-            ]
+            img = [{"mime_type": type, "data": Path(img).read_bytes()}]
         except Exception as error:
             print(f"Error processing image: {error}")
 
     def chat(
         self,
         task: str = None,
         img: str = None,
```

### Comparing `swarms-4.8.2/swarms/models/gpt4_sam.py` & `swarms-4.8.7/swarms/models/gpt4_sam.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,15 @@
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.vlm = vlm
         self.device = device
         self.return_related_marks = return_related_marks
 
-        self.sam = SegmentAnythingMarkGenerator(
-            device, *args, **kwargs
-        )
+        self.sam = SegmentAnythingMarkGenerator(device, *args, **kwargs)
         self.visualizer = MarkVisualizer(*args, **kwargs)
 
     def load_img(self, img: str) -> Any:
         """
         Loads an image from the given file path.
 
         Args:
```

### Comparing `swarms-4.8.2/swarms/models/gpt4_vision_api.py` & `swarms-4.8.7/swarms/models/gpt4_vision_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 from swarms.models.base_multimodal_model import BaseMultiModalModel
 
 try:
     import cv2
 except ImportError:
     print(
-        "OpenCV not installed. Please install OpenCV to use this"
-        " model."
+        "OpenCV not installed. Please install OpenCV to use this" " model."
     )
     raise ImportError
 
 # Load environment variables
 load_dotenv()
 openai_api_key = os.getenv("OPENAI_API_KEY")
 
@@ -244,17 +243,15 @@
 
         base64_frames = []
         while video.isOpened():
             success, frame = video.read()
             if not success:
                 break
             _, buffer = cv2.imencode(".jpg", frame)
-            base64_frames.append(
-                base64.b64encode(buffer).decode("utf-8")
-            )
+            base64_frames.append(base64.b64encode(buffer).decode("utf-8"))
 
         video.release()
         print(len(base64_frames), "frames read.")
         return base64_frames
 
     def run_with_video(
         self,
@@ -429,17 +426,15 @@
         except Exception as error:
             print(f"Error with the request {error}")
             raise error
 
     def health_check(self):
         """Health check for the GPT4Vision model"""
         try:
-            response = requests.get(
-                "https://api.openai.com/v1/engines"
-            )
+            response = requests.get("https://api.openai.com/v1/engines")
             return response.status_code == 200
         except requests.RequestException as error:
             print(f"Health check failed: {error}")
             return False
 
     def print_dashboard(self):
         dashboard = print(
```

### Comparing `swarms-4.8.2/swarms/models/huggingface.py` & `swarms-4.8.7/swarms/models/huggingface.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,17 +199,15 @@
         """Concurrently generate text for a list of prompts."""
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=max_workers
         ) as executor:
             results = list(executor.map(self.run, tasks))
         return results
 
-    def run_batch(
-        self, tasks_images: List[Tuple[str, str]]
-    ) -> List[str]:
+    def run_batch(self, tasks_images: List[Tuple[str, str]]) -> List[str]:
         """Process a batch of tasks and images"""
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = [
                 executor.submit(self.run, task, img)
                 for task, img in tasks_images
             ]
             results = [future.result() for future in futures]
```

### Comparing `swarms-4.8.2/swarms/models/huggingface_pipeline.py` & `swarms-4.8.7/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/idefics.py` & `swarms-4.8.7/swarms/models/idefics.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,17 +73,15 @@
     model.clear_chat_history()
     ```
 
     """
 
     def __init__(
         self,
-        model_name: Optional[
-            str
-        ] = "HuggingFaceM4/idefics-9b-instruct",
+        model_name: Optional[str] = "HuggingFaceM4/idefics-9b-instruct",
         device: Callable = autodetect_device,
         torch_dtype=torch.bfloat16,
         max_length: int = 100,
         batched_mode: bool = True,
         *args,
         **kwargs,
     ):
```

### Comparing `swarms-4.8.2/swarms/models/jina_embeds.py` & `swarms-4.8.7/swarms/models/jina_embeds.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/kosmos_two.py` & `swarms-4.8.7/swarms/models/kosmos_two.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
         )
 
         generated_texts = self.processor.batch_decode(
             generated_ids,
             skip_special_tokens=True,
         )[0]
 
-        processed_text, entities = (
-            self.processor.post_process_generation(generated_texts)
+        processed_text, entities = self.processor.post_process_generation(
+            generated_texts
         )
 
         return processed_text, entities
 
     # tasks
     def multimodal_grounding(self, phrase, image_url):
         task = f"<grounding><phrase> {phrase} </phrase>"
@@ -185,17 +185,15 @@
                     int(x1_norm * image_w),
                     int(y1_norm * image_h),
                     int(x2_norm * image_w),
                     int(y2_norm * image_h),
                 )
                 # draw bbox
                 # random color
-                color = tuple(
-                    np.random.randint(0, 255, size=3).tolist()
-                )
+                color = tuple(np.random.randint(0, 255, size=3).tolist())
                 new_image = cv2.rectangle(
                     new_image,
                     (orig_x1, orig_y1),
                     (orig_x2, orig_y2),
                     color,
                     box_line,
                 )
@@ -206,17 +204,15 @@
                 )
 
                 x1 = orig_x1 - l_o
                 y1 = orig_y1 - l_o
 
                 if (
                     y1
-                    < text_height
-                    + text_offset_original
-                    + 2 * text_spaces
+                    < text_height + text_offset_original + 2 * text_spaces
                 ):
                     y1 = (
                         orig_y1
                         + r_o
                         + text_height
                         + text_offset_original
                         + 2 * text_spaces
```

### Comparing `swarms-4.8.2/swarms/models/layoutlm_document_qa.py` & `swarms-4.8.7/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/llama_function_caller.py` & `swarms-4.8.7/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/llava.py` & `swarms-4.8.7/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/medical_sam.py` & `swarms-4.8.7/swarms/models/medical_sam.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,20 +111,18 @@
         box_torch = torch.as_tensor(
             box_1024, dtype=torch.float, device=img_tensor.device
         )
 
         if len(box_torch.shape) == 2:
             box_torch = box_torch[:, None, :]
 
-        sparse_embeddings, dense_embeddings = (
-            self.model.prompt_encoder(
-                points=None,
-                boxes=box_torch,
-                masks=None,
-            )
+        sparse_embeddings, dense_embeddings = self.model.prompt_encoder(
+            points=None,
+            boxes=box_torch,
+            masks=None,
         )
 
         low_res_logits, _ = self.model.mask_decoder(
             image_embeddings=img,
             image_pe=self.model.prompt_encoder.get_dense_pe(),
             sparse_prompt_embeddings=sparse_embeddings,
             dense_prompt_embeddings=dense_embeddings,
```

### Comparing `swarms-4.8.2/swarms/models/mistral.py` & `swarms-4.8.7/swarms/models/mistral.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,28 +70,26 @@
 
         self.model.to(self.device)
 
     def run(self, task: str, *args, **kwargs):
         """Run the model on a given task."""
 
         try:
-            model_inputs = self.tokenizer(
-                [task], return_tensors="pt"
-            ).to(self.device)
+            model_inputs = self.tokenizer([task], return_tensors="pt").to(
+                self.device
+            )
             generated_ids = self.model.generate(
                 **model_inputs,
                 max_length=self.max_length,
                 do_sample=self.do_sample,
                 temperature=self.temperature,
                 max_new_tokens=self.max_length,
                 **kwargs,
             )
-            output_text = self.tokenizer.batch_decode(generated_ids)[
-                0
-            ]
+            output_text = self.tokenizer.batch_decode(generated_ids)[0]
             return output_text
         except Exception as e:
             raise ValueError(f"Error running the model: {str(e)}")
 
     def chat(self, msg: str = None, streaming: bool = False):
         """
         Run chat
```

### Comparing `swarms-4.8.2/swarms/models/mixtral.py` & `swarms-4.8.7/swarms/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/moondream_mm.py` & `swarms-4.8.7/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/mpt.py` & `swarms-4.8.7/swarms/models/mpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,15 @@
         """Call the model asynchronously""" ""
         return await self.run_async(task, *args, **kwargs)
 
     def batch_generate(
         self, prompts: list, temperature: float = 1.0
     ) -> list:
         """Batch generate text"""
-        self.logger.info(
-            f"Generating text for {len(prompts)} prompts..."
-        )
+        self.logger.info(f"Generating text for {len(prompts)} prompts...")
         results = []
         with torch.autocast("cuda", dtype=torch.bfloat16):
             for prompt in prompts:
                 result = self.pipe(
                     prompt,
                     max_new_tokens=self.max_tokens,
                     do_sample=True,
```

### Comparing `swarms-4.8.2/swarms/models/nougat.py` & `swarms-4.8.7/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/open_dalle.py` & `swarms-4.8.7/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/openai_embeddings.py` & `swarms-4.8.7/swarms/models/openai_embeddings.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,17 +49,15 @@
             multiplier=1, min=min_seconds, max=max_seconds
         ),
         retry=(
             retry_if_exception_type(llm.error.Timeout)
             | retry_if_exception_type(llm.error.APIError)
             | retry_if_exception_type(llm.error.APIConnectionError)
             | retry_if_exception_type(llm.error.RateLimitError)
-            | retry_if_exception_type(
-                llm.error.ServiceUnavailableError
-            )
+            | retry_if_exception_type(llm.error.ServiceUnavailableError)
         ),
         before_sleep=before_sleep_log(logger, logging.WARNING),
     )
 
 
 def _async_retry_decorator(embeddings: OpenAIEmbeddings) -> Any:
     import llm
@@ -75,17 +73,15 @@
             multiplier=1, min=min_seconds, max=max_seconds
         ),
         retry=(
             retry_if_exception_type(llm.error.Timeout)
             | retry_if_exception_type(llm.error.APIError)
             | retry_if_exception_type(llm.error.APIConnectionError)
             | retry_if_exception_type(llm.error.RateLimitError)
-            | retry_if_exception_type(
-                llm.error.ServiceUnavailableError
-            )
+            | retry_if_exception_type(llm.error.ServiceUnavailableError)
         ),
         before_sleep=before_sleep_log(logger, logging.WARNING),
     )
 
     def wrap(func: Callable) -> Callable:
         async def wrapped_f(*args: Any, **kwargs: Any) -> Callable:
             async for _ in async_retrying:
@@ -98,23 +94,19 @@
 
 
 # https://stackoverflow.com/questions/76469415/getting-embeddings-of-length-1-from-langchain-openaiembeddings
 def _check_response(response: dict) -> dict:
     if any(len(d["embedding"]) == 1 for d in response["data"]):
         import llm
 
-        raise llm.error.APIError(
-            "OpenAI API returned an empty embedding"
-        )
+        raise llm.error.APIError("OpenAI API returned an empty embedding")
     return response
 
 
-def embed_with_retry(
-    embeddings: OpenAIEmbeddings, **kwargs: Any
-) -> Any:
+def embed_with_retry(embeddings: OpenAIEmbeddings, **kwargs: Any) -> Any:
     """Use tenacity to retry the embedding call."""
     retry_decorator = _create_retry_decorator(embeddings)
 
     @retry_decorator
     def _embed_with_retry(**kwargs: Any) -> Any:
         response = embeddings.client.create(**kwargs)
         return _check_response(response)
@@ -177,30 +169,30 @@
             text = "This is a test query."
             query_result = embeddings.embed_query(text)
 
     """
 
     client: Any = None  #: :meta private:
     model: str = "text-embedding-ada-002"
-    deployment: str = model  # to support Azure OpenAI Service custom deployment names
+    deployment: str = (
+        model  # to support Azure OpenAI Service custom deployment names
+    )
     openai_api_version: str | None = None
     # to support Azure OpenAI Service custom endpoints
     openai_api_base: str | None = None
     # to support Azure OpenAI Service custom endpoints
     openai_api_type: str | None = None
     # to support explicit proxy for OpenAI
     openai_proxy: str | None = None
     embedding_ctx_length: int = 8191
     """The maximum number of tokens to embed at once."""
     openai_api_key: str | None = None
     openai_organization: str | None = None
     allowed_special: Literal["all"] | set[str] = set()
-    disallowed_special: Literal["all"] | set[str] | Sequence[
-        str
-    ] = "all"
+    disallowed_special: Literal["all"] | set[str] | Sequence[str] = "all"
     chunk_size: int = 1000
     """Maximum number of texts to embed in each batch"""
     max_retries: int = 6
     """Maximum number of retries to make when generating."""
     request_timeout: float | tuple[float, float] | None = None
     """Timeout in seconds for the OpenAPI request."""
     headers: Any = None
@@ -224,17 +216,15 @@
     @classmethod
     def build_extra(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Build extra kwargs from additional params that were passed in."""
         all_required_field_names = get_pydantic_field_names(cls)
         extra = values.get("model_kwargs", {})
         for field_name in list(values):
             if field_name in extra:
-                raise ValueError(
-                    f"Found {field_name} supplied twice."
-                )
+                raise ValueError(f"Found {field_name} supplied twice.")
             if field_name not in all_required_field_names:
                 warnings.warn(
                     f"""WARNING! {field_name} is not default parameter.
                     {field_name} was transferred to model_kwargs.
                     Please confirm that {field_name} is what you intended."""
                 )
                 extra[field_name] = values.pop(field_name)
@@ -335,17 +325,15 @@
     def _get_len_safe_embeddings(
         self,
         texts: list[str],
         *,
         engine: str,
         chunk_size: int | None = None,
     ) -> list[list[float]]:
-        embeddings: list[list[float]] = [
-            [] for _ in range(len(texts))
-        ]
+        embeddings: list[list[float]] = [[] for _ in range(len(texts))]
         try:
             import tiktoken
         except ImportError:
             raise ImportError(
                 "Could not import tiktoken python package. "
                 "This is needed in order to for OpenAIEmbeddings. "
                 "Please install it with `pip install tiktoken`."
@@ -354,33 +342,30 @@
         tokens = []
         indices = []
         model_name = self.tiktoken_model_name or self.model
         try:
             encoding = tiktoken.encoding_for_model(model_name)
         except KeyError:
             logger.warning(
-                "Warning: model not found. Using cl100k_base"
-                " encoding."
+                "Warning: model not found. Using cl100k_base" " encoding."
             )
             model = "cl100k_base"
             encoding = tiktoken.get_encoding(model)
         for i, text in enumerate(texts):
             if self.model.endswith("001"):
                 # See: https://github.com/openai/openai-python/issues/418#issuecomment-1525939500
                 # replace newlines, which can negatively affect performance.
                 text = text.replace("\n", " ")
             token = encoding.encode(
                 text,
                 allowed_special=self.allowed_special,
                 disallowed_special=self.disallowed_special,
             )
             for j in range(0, len(token), self.embedding_ctx_length):
-                tokens.append(
-                    token[j : j + self.embedding_ctx_length]
-                )
+                tokens.append(token[j : j + self.embedding_ctx_length])
                 indices.append(i)
 
         batched_embeddings: list[list[float]] = []
         _chunk_size = chunk_size or self.chunk_size
 
         if self.show_progress_bar:
             try:
@@ -398,17 +383,15 @@
                 input=tokens[i : i + _chunk_size],
                 **self._invocation_params,
             )
             batched_embeddings.extend(
                 r["embedding"] for r in response["data"]
             )
 
-        results: list[list[list[float]]] = [
-            [] for _ in range(len(texts))
-        ]
+        results: list[list[list[float]]] = [[] for _ in range(len(texts))]
         num_tokens_in_batch: list[list[int]] = [
             [] for _ in range(len(texts))
         ]
         for i in range(len(indices)):
             results[indices[i]].append(batched_embeddings[i])
             num_tokens_in_batch[indices[i]].append(len(tokens[i]))
 
@@ -420,32 +403,28 @@
                     input="",
                     **self._invocation_params,
                 )["data"][0]["embedding"]
             else:
                 average = np.average(
                     _result, axis=0, weights=num_tokens_in_batch[i]
                 )
-            embeddings[i] = (
-                average / np.linalg.norm(average)
-            ).tolist()
+            embeddings[i] = (average / np.linalg.norm(average)).tolist()
 
         return embeddings
 
     # please refer to
     # https://github.com/openai/openai-cookbook/blob/main/examples/Embedding_long_inputs.ipynb
     async def _aget_len_safe_embeddings(
         self,
         texts: list[str],
         *,
         engine: str,
         chunk_size: int | None = None,
     ) -> list[list[float]]:
-        embeddings: list[list[float]] = [
-            [] for _ in range(len(texts))
-        ]
+        embeddings: list[list[float]] = [[] for _ in range(len(texts))]
         try:
             import tiktoken
         except ImportError:
             raise ImportError(
                 "Could not import tiktoken python package. "
                 "This is needed in order to for OpenAIEmbeddings. "
                 "Please install it with `pip install tiktoken`."
@@ -454,50 +433,45 @@
         tokens = []
         indices = []
         model_name = self.tiktoken_model_name or self.model
         try:
             encoding = tiktoken.encoding_for_model(model_name)
         except KeyError:
             logger.warning(
-                "Warning: model not found. Using cl100k_base"
-                " encoding."
+                "Warning: model not found. Using cl100k_base" " encoding."
             )
             model = "cl100k_base"
             encoding = tiktoken.get_encoding(model)
         for i, text in enumerate(texts):
             if self.model.endswith("001"):
                 # See: https://github.com/openai/openai-python/issues/418#issuecomment-1525939500
                 # replace newlines, which can negatively affect performance.
                 text = text.replace("\n", " ")
             token = encoding.encode(
                 text,
                 allowed_special=self.allowed_special,
                 disallowed_special=self.disallowed_special,
             )
             for j in range(0, len(token), self.embedding_ctx_length):
-                tokens.append(
-                    token[j : j + self.embedding_ctx_length]
-                )
+                tokens.append(token[j : j + self.embedding_ctx_length])
                 indices.append(i)
 
         batched_embeddings: list[list[float]] = []
         _chunk_size = chunk_size or self.chunk_size
         for i in range(0, len(tokens), _chunk_size):
             response = await async_embed_with_retry(
                 self,
                 input=tokens[i : i + _chunk_size],
                 **self._invocation_params,
             )
             batched_embeddings.extend(
                 r["embedding"] for r in response["data"]
             )
 
-        results: list[list[list[float]]] = [
-            [] for _ in range(len(texts))
-        ]
+        results: list[list[list[float]]] = [[] for _ in range(len(texts))]
         num_tokens_in_batch: list[list[int]] = [
             [] for _ in range(len(texts))
         ]
         for i in range(len(indices)):
             results[indices[i]].append(batched_embeddings[i])
             num_tokens_in_batch[indices[i]].append(len(tokens[i]))
 
@@ -511,17 +485,15 @@
                         **self._invocation_params,
                     )
                 )["data"][0]["embedding"]
             else:
                 average = np.average(
                     _result, axis=0, weights=num_tokens_in_batch[i]
                 )
-            embeddings[i] = (
-                average / np.linalg.norm(average)
-            ).tolist()
+            embeddings[i] = (average / np.linalg.norm(average)).tolist()
 
         return embeddings
 
     def embed_documents(
         self, texts: list[str], chunk_size: int | None = 0
     ) -> list[list[float]]:
         """Call out to OpenAI's embedding endpoint for embedding search docs.
@@ -532,17 +504,15 @@
                 specified by the class.
 
         Returns:
             List of embeddings, one for each text.
         """
         # NOTE: to keep things simple, we assume the list may contain texts longer
         #       than the maximum context and use length-safe embedding function.
-        return self._get_len_safe_embeddings(
-            texts, engine=self.deployment
-        )
+        return self._get_len_safe_embeddings(texts, engine=self.deployment)
 
     async def aembed_documents(
         self, texts: list[str], chunk_size: int | None = 0
     ) -> list[list[float]]:
         """Call out to OpenAI's embedding endpoint async for embedding search docs.
 
         Args:
```

### Comparing `swarms-4.8.2/swarms/models/openai_tts.py` & `swarms-4.8.7/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/palm.py` & `swarms-4.8.7/swarms/models/palm.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,34 +125,27 @@
 
         values["client"] = genai
 
         if (
             values["temperature"] is not None
             and not 0 <= values["temperature"] <= 1
         ):
-            raise ValueError(
-                "temperature must be in the range [0.0, 1.0]"
-            )
+            raise ValueError("temperature must be in the range [0.0, 1.0]")
 
-        if (
-            values["top_p"] is not None
-            and not 0 <= values["top_p"] <= 1
-        ):
+        if values["top_p"] is not None and not 0 <= values["top_p"] <= 1:
             raise ValueError("top_p must be in the range [0.0, 1.0]")
 
         if values["top_k"] is not None and values["top_k"] <= 0:
             raise ValueError("top_k must be positive")
 
         if (
             values["max_output_tokens"] is not None
             and values["max_output_tokens"] <= 0
         ):
-            raise ValueError(
-                "max_output_tokens must be greater than zero"
-            )
+            raise ValueError("max_output_tokens must be greater than zero")
 
         return values
 
     def _generate(
         self,
         prompts: list[str],
         stop: list[str] | None = None,
@@ -173,20 +166,16 @@
                 candidate_count=self.n,
                 **kwargs,
             )
 
             prompt_generations = []
             for candidate in completion.candidates:
                 raw_text = candidate["output"]
-                stripped_text = _strip_erroneous_leading_spaces(
-                    raw_text
-                )
-                prompt_generations.append(
-                    Generation(text=stripped_text)
-                )
+                stripped_text = _strip_erroneous_leading_spaces(raw_text)
+                prompt_generations.append(Generation(text=stripped_text))
             generations.append(prompt_generations)
 
         return LLMResult(generations=generations)
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
```

### Comparing `swarms-4.8.2/swarms/models/popular_llms.py` & `swarms-4.8.7/swarms/models/popular_llms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from langchain_community.chat_models.azure_openai import (
     AzureChatOpenAI,
 )
 from langchain_community.chat_models.openai import (
     ChatOpenAI as OpenAIChat,
 )
-from langchain_community.llms import (
-    Anthropic,
-    Cohere,
-    MosaicML,
-    OpenAI,
-    Replicate,
-)
+from langchain.llms.anthropic import Anthropic
+from langchain.llms.cohere import Cohere
+from langchain.llms.mosaicml import MosaicML
+from langchain.llms.openai import OpenAI #, OpenAIChat, AzureOpenAI
 from langchain_community.llms.octoai_endpoint import OctoAIEndpoint
-
+from langchain.llms.replicate import Replicate
 
 class AnthropicChat(Anthropic):
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
 
 
 class CohereChat(Cohere):
@@ -30,25 +27,28 @@
 
 
 class OpenAILLM(OpenAI):
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
 
 
-class ReplicateLLM(Replicate):
+class ReplicateChat(Replicate):
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
 
 
 class AzureOpenAILLM(AzureChatOpenAI):
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
 
 
 class OpenAIChatLLM(OpenAIChat):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
 
 
 class OctoAIChat(OctoAIEndpoint):
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
```

### Comparing `swarms-4.8.2/swarms/models/qwen.py` & `swarms-4.8.7/swarms/models/qwen.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,10 +135,8 @@
             response, history = self.model.chat(
                 self.tokenizer,
                 query=f"<img>{img}</img>这是什么",
                 history=None,
             )
             return response, history
         except Exception as e:
-            raise Exception(
-                "An error occurred during the chat."
-            ) from e
+            raise Exception("An error occurred during the chat.") from e
```

### Comparing `swarms-4.8.2/swarms/models/sam.py` & `swarms-4.8.7/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/sampling_params.py` & `swarms-4.8.7/swarms/models/sampling_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,15 @@
         else:
             self.stop_token_ids = list(stop_token_ids)
         self.ignore_eos = ignore_eos
         self.max_tokens = max_tokens
         self.logprobs = logprobs
         self.prompt_logprobs = prompt_logprobs
         self.skip_special_tokens = skip_special_tokens
-        self.spaces_between_special_tokens = (
-            spaces_between_special_tokens
-        )
+        self.spaces_between_special_tokens = spaces_between_special_tokens
         self.logits_processors = logits_processors
         self.include_stop_str_in_output = include_stop_str_in_output
         self._verify_args()
         if self.use_beam_search:
             self._verify_beam_search()
         else:
             self._verify_non_beam_search()
@@ -185,39 +183,31 @@
             )
         if self.temperature < 0.0:
             raise ValueError(
                 "temperature must be non-negative, got"
                 f" {self.temperature}."
             )
         if not 0.0 < self.top_p <= 1.0:
-            raise ValueError(
-                f"top_p must be in (0, 1], got {self.top_p}."
-            )
+            raise ValueError(f"top_p must be in (0, 1], got {self.top_p}.")
         if self.top_k < -1 or self.top_k == 0:
             raise ValueError(
                 "top_k must be -1 (disable), or at least 1, "
                 f"got {self.top_k}."
             )
         if not 0.0 <= self.min_p <= 1.0:
-            raise ValueError(
-                f"min_p must be in [0, 1], got {self.min_p}."
-            )
+            raise ValueError(f"min_p must be in [0, 1], got {self.min_p}.")
         if self.max_tokens is not None and self.max_tokens < 1:
             raise ValueError(
-                "max_tokens must be at least 1, got"
-                f" {self.max_tokens}."
+                "max_tokens must be at least 1, got" f" {self.max_tokens}."
             )
         if self.logprobs is not None and self.logprobs < 0:
             raise ValueError(
                 f"logprobs must be non-negative, got {self.logprobs}."
             )
-        if (
-            self.prompt_logprobs is not None
-            and self.prompt_logprobs < 0
-        ):
+        if self.prompt_logprobs is not None and self.prompt_logprobs < 0:
             raise ValueError(
                 "prompt_logprobs must be non-negative, got "
                 f"{self.prompt_logprobs}."
             )
 
     def _verify_beam_search(self) -> None:
         if self.best_of == 1:
@@ -226,21 +216,17 @@
                 f"search. Got {self.best_of}."
             )
         if self.temperature > _SAMPLING_EPS:
             raise ValueError(
                 "temperature must be 0 when using beam search."
             )
         if self.top_p < 1.0 - _SAMPLING_EPS:
-            raise ValueError(
-                "top_p must be 1 when using beam search."
-            )
+            raise ValueError("top_p must be 1 when using beam search.")
         if self.top_k != -1:
-            raise ValueError(
-                "top_k must be -1 when using beam search."
-            )
+            raise ValueError("top_k must be -1 when using beam search.")
         if self.early_stopping not in [True, False, "never"]:
             raise ValueError(
                 "early_stopping must be True, False, or 'never', "
                 f"got {self.early_stopping}."
             )
 
     def _verify_non_beam_search(self) -> None:
```

### Comparing `swarms-4.8.2/swarms/models/speecht5.py` & `swarms-4.8.7/swarms/models/speecht5.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,19 @@
         model_name="microsoft/speecht5_tts",
         vocoder_name="microsoft/speecht5_hifigan",
         dataset_name="Matthijs/cmu-arctic-xvectors",
     ):
         self.model_name = model_name
         self.vocoder_name = vocoder_name
         self.dataset_name = dataset_name
-        self.processor = SpeechT5Processor.from_pretrained(
-            self.model_name
-        )
+        self.processor = SpeechT5Processor.from_pretrained(self.model_name)
         self.model = SpeechT5ForTextToSpeech.from_pretrained(
             self.model_name
         )
-        self.vocoder = SpeechT5HifiGan.from_pretrained(
-            self.vocoder_name
-        )
+        self.vocoder = SpeechT5HifiGan.from_pretrained(self.vocoder_name)
         self.embeddings_dataset = load_dataset(
             self.dataset_name, split="validation"
         )
 
     def __call__(self, text: str, speaker_id: float = 7306):
         """Call the model on some text and return the speech."""
         speaker_embedding = torch.tensor(
@@ -117,27 +113,23 @@
     def save_speech(self, speech, filename="speech.wav"):
         """Save Speech to a file."""
         sf.write(filename, speech.numpy(), samplerate=16000)
 
     def set_model(self, model_name: str):
         """Set the model to a new model."""
         self.model_name = model_name
-        self.processor = SpeechT5Processor.from_pretrained(
-            self.model_name
-        )
+        self.processor = SpeechT5Processor.from_pretrained(self.model_name)
         self.model = SpeechT5ForTextToSpeech.from_pretrained(
             self.model_name
         )
 
     def set_vocoder(self, vocoder_name):
         """Set the vocoder to a new vocoder."""
         self.vocoder_name = vocoder_name
-        self.vocoder = SpeechT5HifiGan.from_pretrained(
-            self.vocoder_name
-        )
+        self.vocoder = SpeechT5HifiGan.from_pretrained(self.vocoder_name)
 
     def set_embeddings_dataset(self, dataset_name):
         """Set the embeddings dataset to a new dataset."""
         self.dataset_name = dataset_name
         self.embeddings_dataset = load_dataset(
             self.dataset_name, split="validation"
         )
```

### Comparing `swarms-4.8.2/swarms/models/ssd_1b.py` & `swarms-4.8.7/swarms/models/ssd_1b.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,15 @@
         https://cdn.openai.com/dall-e/encoded/feats/feats_01J9J5ZKJZJY9.png
         """
         if self.dashboard:
             self.print_dashboard()
         if task in self.cache:
             return self.cache[task]
         try:
-            img = self.pipe(
-                prompt=task, neg_prompt=neg_prompt
-            ).images[0]
+            img = self.pipe(prompt=task, neg_prompt=neg_prompt).images[0]
 
             # Generate a unique filename for the image
             img_name = f"{uuid.uuid4()}.{self.image_format}"
             img_path = os.path.join(self.save_path, img_name)
 
             # Save the image
             img.save(img_path, self.image_format)
@@ -219,17 +217,15 @@
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=max_workers
         ) as executor:
             future_to_task = {
                 executor.submit(self, task): task for task in tasks
             }
             results = []
-            for future in concurrent.futures.as_completed(
-                future_to_task
-            ):
+            for future in concurrent.futures.as_completed(future_to_task):
                 task = future_to_task[future]
                 try:
                     img = future.result()
                     results.append(img)
 
                     print(f"Task {task} completed: {img}")
                 except Exception as error:
@@ -268,13 +264,11 @@
         """Repr method for the SSD1B class"""
         return f"SSD1B(image_url={self.image_url})"
 
     def __str__(self):
         """Str method for the SSD1B class"""
         return f"SSD1B(image_url={self.image_url})"
 
-    @backoff.on_exception(
-        backoff.expo, Exception, max_tries=max_retries
-    )
+    @backoff.on_exception(backoff.expo, Exception, max_tries=max_retries)
     def rate_limited_call(self, task: str):
         """Rate limited call to the SSD1B API"""
         return self.__call__(task)
```

### Comparing `swarms-4.8.2/swarms/models/stable_diffusion.py` & `swarms-4.8.7/swarms/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/timm.py` & `swarms-4.8.7/swarms/models/timm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/together.py` & `swarms-4.8.7/swarms/models/together.py`

 * *Files 8% similar despite different names*

```diff
@@ -116,17 +116,15 @@
                 json=payload,
                 *args,
                 **kwargs,
             )
 
             out = response.json()
             content = (
-                out["choices"][0]
-                .get("message", {})
-                .get("content", None)
+                out["choices"][0].get("message", {}).get("content", None)
             )
             if self.streaming_enabled:
                 content = self.stream_response(content)
 
             return content
 
         except Exception as error:
```

### Comparing `swarms-4.8.2/swarms/models/types.py` & `swarms-4.8.7/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/ultralytics_model.py` & `swarms-4.8.7/swarms/models/ultralytics_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
     Args:
         model_name (str): The name of the model.
         *args: Variable length argument list.
         **kwargs: Arbitrary keyword arguments.
     """
 
-    def __init__(
-        self, model_name: str = "yolov8n.pt", *args, **kwargs
-    ):
+    def __init__(self, model_name: str = "yolov8n.pt", *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.model_name = model_name
 
         try:
             self.model = YOLO(model_name, *args, **kwargs)
         except Exception as e:
             raise ValueError(
```

### Comparing `swarms-4.8.2/swarms/models/vilt.py` & `swarms-4.8.7/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/vip_llava.py` & `swarms-4.8.7/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/models/wizard_storytelling.py` & `swarms-4.8.7/swarms/models/wizard_storytelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,15 @@
                     "bnb_4bit_use_double_quant": True,
                     "bnb_4bit_quant_type": "nf4",
                     "bnb_4bit_compute_dtype": torch.bfloat16,
                 }
             bnb_config = BitsAndBytesConfig(**quantization_config)
 
         try:
-            self.tokenizer = AutoTokenizer.from_pretrained(
-                self.model_id
-            )
+            self.tokenizer = AutoTokenizer.from_pretrained(self.model_id)
             self.model = AutoModelForCausalLM.from_pretrained(
                 self.model_id, quantization_config=bnb_config
             )
 
             self.model  # .to(self.device)
         except Exception as e:
             self.logger.error(
```

### Comparing `swarms-4.8.2/swarms/models/yarn_mistral.py` & `swarms-4.8.7/swarms/models/yarn_mistral.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,15 @@
                     "bnb_4bit_use_double_quant": True,
                     "bnb_4bit_quant_type": "nf4",
                     "bnb_4bit_compute_dtype": torch.bfloat16,
                 }
             bnb_config = BitsAndBytesConfig(**quantization_config)
 
         try:
-            self.tokenizer = AutoTokenizer.from_pretrained(
-                self.model_id
-            )
+            self.tokenizer = AutoTokenizer.from_pretrained(self.model_id)
             self.model = AutoModelForCausalLM.from_pretrained(
                 self.model_id,
                 quantization_config=bnb_config,
                 use_flash_attention_2=True,
                 torch_dtype=torch.bfloat16,
                 device_map="auto",
                 trust_remote_code=True,
```

### Comparing `swarms-4.8.2/swarms/models/yi_200k.py` & `swarms-4.8.7/swarms/models/yi_200k.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,17 +83,15 @@
             do_sample=True,
             repetition_penalty=self.repitition_penalty,
             no_repeat_ngram_size=self.no_repeat_ngram_size,
             temperature=self.temperature,
             top_k=self.top_k,
             top_p=self.top_p,
         )
-        return self.tokenizer.decode(
-            outputs[0], skip_special_tokens=True
-        )
+        return self.tokenizer.decode(outputs[0], skip_special_tokens=True)
 
 
 # # Example usage
 # yi34b = Yi34B200k()
 # prompt = "There's a place where time stands still. A place of breathtaking wonder, but also"
 # generated_text = yi34b(prompt)
 # print(generated_text)
```

### Comparing `swarms-4.8.2/swarms/models/zeroscope.py` & `swarms-4.8.7/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/__init__.py` & `swarms-4.8.7/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/accountant_swarm_prompts.py` & `swarms-4.8.7/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/aga.py` & `swarms-4.8.7/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/agent_output_parser.py` & `swarms-4.8.7/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/agent_prompt.py` & `swarms-4.8.7/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/agent_prompts.py` & `swarms-4.8.7/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/agent_system_prompts.py` & `swarms-4.8.7/swarms/prompts/agent_system_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/ai_research_team.py` & `swarms-4.8.7/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/autobloggen.py` & `swarms-4.8.7/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/autoswarm.py` & `swarms-4.8.7/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/base.py` & `swarms-4.8.7/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/chat_prompt.py` & `swarms-4.8.7/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/code_interpreter.py` & `swarms-4.8.7/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/code_spawner.py` & `swarms-4.8.7/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/debate.py` & `swarms-4.8.7/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/documentation.py` & `swarms-4.8.7/swarms/prompts/documentation.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/education.py` & `swarms-4.8.7/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/finance_agent_prompt.py` & `swarms-4.8.7/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/growth_agent_prompt.py` & `swarms-4.8.7/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/idea2img.py` & `swarms-4.8.7/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/legal_agent_prompt.py` & `swarms-4.8.7/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/logistics.py` & `swarms-4.8.7/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/meta_system_prompt.py` & `swarms-4.8.7/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-4.8.7/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/multi_modal_prompts.py` & `swarms-4.8.7/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-4.8.7/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/operations_agent_prompt.py` & `swarms-4.8.7/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/personal_stylist.py` & `swarms-4.8.7/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/product_agent_prompt.py` & `swarms-4.8.7/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/programming.py` & `swarms-4.8.7/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/project_manager.py` & `swarms-4.8.7/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/python.py` & `swarms-4.8.7/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/react.py` & `swarms-4.8.7/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/sales.py` & `swarms-4.8.7/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/sales_prompts.py` & `swarms-4.8.7/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/schema_generator.py` & `swarms-4.8.7/swarms/prompts/schema_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/security_team.py` & `swarms-4.8.7/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/self_operating_prompt.py` & `swarms-4.8.7/swarms/prompts/self_operating_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,15 @@
 
 def format_vision_prompt(objective, previous_action):
     """
     Format the vision prompt
     """
     if previous_action:
         previous_action = (
-            "Here was the previous action you took:"
-            f" {previous_action}"
+            "Here was the previous action you took:" f" {previous_action}"
         )
     else:
         previous_action = ""
     prompt = VISION_PROMPT.format(
         objective=objective, previous_action=previous_action
     )
     return prompt
```

### Comparing `swarms-4.8.2/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-4.8.7/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/summaries_prompts.py` & `swarms-4.8.7/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/support_agent_prompt.py` & `swarms-4.8.7/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/swarm_manager_agent.py` & `swarms-4.8.7/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/task_assignment_prompt.py` & `swarms-4.8.7/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/tests.py` & `swarms-4.8.7/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/tools.py` & `swarms-4.8.7/swarms/prompts/tools.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/urban_planning.py` & `swarms-4.8.7/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/visual_cot.py` & `swarms-4.8.7/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/worker_prompt.py` & `swarms-4.8.7/swarms/prompts/worker_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/prompts/xray_swarm_prompt.py` & `swarms-4.8.7/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/__init__.py` & `swarms-4.8.7/swarms/structs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from swarms.structs.agent import Agent
 from swarms.structs.agent_job import AgentJob
 from swarms.structs.agent_process import (
     AgentProcess,
     AgentProcessQueue,
 )
 from swarms.structs.auto_swarm import AutoSwarm, AutoSwarmRouter
-from swarms.structs.autoscaler import AutoScaler
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.structs.base_workflow import BaseWorkflow
 from swarms.structs.block_wrapper import block
 from swarms.structs.concurrent_workflow import ConcurrentWorkflow
 from swarms.structs.conversation import Conversation
 from swarms.structs.graph_workflow import GraphWorkflow
 from swarms.structs.groupchat import GroupChat, GroupChatManager
@@ -76,23 +75,28 @@
     extract_tokens_from_text,
     find_agent_by_id,
     find_token_in_text,
     parse_tasks,
 )
 from swarms.structs.agent_rearrange import AgentRearrange
 
+from swarms.structs.yaml_model import (
+    get_type_name,
+    create_yaml_schema_from_dict,
+    pydantic_type_to_yaml_schema,
+    YamlModel,
+)
 
 __all__ = [
     "Agent",
     "AgentJob",
     "AgentProcess",
     "AgentProcessQueue",
     "AutoSwarm",
     "AutoSwarmRouter",
-    "AutoScaler",
     "BaseStructure",
     "BaseSwarm",
     "BaseWorkflow",
     "block",
     "ConcurrentWorkflow",
     "Conversation",
     "GraphWorkflow",
@@ -145,8 +149,12 @@
     "distribute_tasks",
     "extract_key_from_json",
     "extract_tokens_from_text",
     "find_agent_by_id",
     "find_token_in_text",
     "parse_tasks",
     "AgentRearrange",
+    "get_type_name",
+    "create_yaml_schema_from_dict",
+    "pydantic_type_to_yaml_schema",
+    "YamlModel",
 ]
```

### Comparing `swarms-4.8.2/swarms/structs/agent.py` & `swarms-4.8.7/swarms/structs/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import json
 import logging
+from typing import Union
 import os
 import random
 import sys
 import time
 import uuid
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
@@ -15,21 +16,27 @@
 from swarms.memory.base_vectordb import AbstractVectorDatabase
 from swarms.prompts.agent_system_prompts import AGENT_SYSTEM_PROMPT_3
 from swarms.prompts.multi_modal_autonomous_instruction_prompt import (
     MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1,
 )
 from swarms.structs.conversation import Conversation
 from swarms.tools.tool import BaseTool
-from swarms.utils.code_interpreter import SubprocessCodeInterpreter
+from swarms.tools.code_interpreter import SubprocessCodeInterpreter
 from swarms.utils.data_to_text import data_to_text
 from swarms.utils.parse_code import extract_code_from_markdown
 from swarms.utils.pdf_to_text import pdf_to_text
 from swarms.tools.exec_tool import execute_tool_by_name
 from swarms.tools.code_executor import CodeExecutor
 from swarms.prompts.worker_prompt import tool_usage_worker_prompt
+from pydantic import BaseModel
+from swarms.tools.pydantic_to_json import (
+    pydantic_to_functions,
+    multi_pydantic_to_functions,
+)
+from swarms.structs.schemas import Step, ManySteps
 
 
 # Utils
 # Custom stopping condition
 def stop_when_repeats(response: str) -> bool:
     # Stop if the word stop appears in the response
     return "stop" in response.lower()
@@ -59,21 +66,25 @@
 
 
 # Step ID generator
 def step_id():
     return str(uuid.uuid1())
 
 
+# Agent output types
+agent_output_type = Union[BaseModel, dict, str]
+ToolUsageType = Union[BaseModel, Dict[str, Any]]
+
+
+# [FEAT][AGENT]
 class Agent:
     """
     Agent is the backbone to connect LLMs with tools and long term memory. Agent also provides the ability to
     ingest any type of docs like PDFs, Txts, Markdown, Json, and etc for the agent. Here is a list of features.
 
-
-
     Args:
         llm (Any): The language model to use
         template (str): The template to use
         max_loops (int): The maximum number of loops to run
         stopping_condition (Callable): The stopping condition to use
         loop_interval (int): The loop interval
         retry_attempts (int): The number of retry attempts
@@ -151,69 +162,76 @@
     >>> print(response)
     >>> # Generate a report on the financials.
 
     """
 
     def __init__(
         self,
-        id: str = agent_id,
-        llm: Any = None,
+        id: Optional[str] = agent_id,
+        llm: Optional[Any] = None,
         template: Optional[str] = None,
         max_loops: Optional[int] = 1,
         stopping_condition: Optional[Callable[[str], bool]] = None,
-        loop_interval: int = 0,
-        retry_attempts: int = 3,
-        retry_interval: int = 1,
-        return_history: bool = False,
-        stopping_token: str = None,
+        loop_interval: Optional[int] = 0,
+        retry_attempts: Optional[int] = 3,
+        retry_interval: Optional[int] = 1,
+        return_history: Optional[bool] = False,
+        stopping_token: Optional[str] = None,
         dynamic_loops: Optional[bool] = False,
-        interactive: bool = False,
-        dashboard: bool = False,
-        agent_name: str = "swarm-worker-01",
-        agent_description: str = None,
-        system_prompt: str = AGENT_SYSTEM_PROMPT_3,
+        interactive: Optional[bool] = False,
+        dashboard: Optional[bool] = False,
+        agent_name: Optional[str] = "swarm-worker-01",
+        agent_description: Optional[str] = None,
+        system_prompt: Optional[str] = AGENT_SYSTEM_PROMPT_3,
         tools: List[BaseTool] = [],
         dynamic_temperature_enabled: Optional[bool] = False,
         sop: Optional[str] = None,
         sop_list: Optional[List[str]] = None,
         saved_state_path: Optional[str] = None,
         autosave: Optional[bool] = False,
         context_length: Optional[int] = 8192,
-        user_name: str = "Human:",
+        user_name: Optional[str] = "Human:",
         self_healing_enabled: Optional[bool] = False,
         code_interpreter: Optional[bool] = False,
         multi_modal: Optional[bool] = None,
         pdf_path: Optional[str] = None,
         list_of_pdf: Optional[str] = None,
         tokenizer: Optional[Any] = None,
         long_term_memory: Optional[AbstractVectorDatabase] = None,
         preset_stopping_token: Optional[bool] = False,
-        traceback: Any = None,
-        traceback_handlers: Any = None,
+        traceback: Optional[Any] = None,
+        traceback_handlers: Optional[Any] = None,
         streaming_on: Optional[bool] = False,
         docs: List[str] = None,
-        docs_folder: str = None,
-        verbose: bool = False,
+        docs_folder: Optional[str] = None,
+        verbose: Optional[bool] = False,
         parser: Optional[Callable] = None,
         best_of_n: Optional[int] = None,
         callback: Optional[Callable] = None,
         metadata: Optional[Dict[str, Any]] = None,
         callbacks: Optional[List[Callable]] = None,
-        logger_handler: Any = sys.stderr,
+        logger_handler: Optional[Any] = sys.stderr,
         search_algorithm: Optional[Callable] = None,
         logs_to_filename: Optional[str] = None,
         evaluator: Optional[Callable] = None,
-        output_json: bool = False,
+        output_json: Optional[bool] = False,
         stopping_func: Optional[Callable] = None,
         custom_loop_condition: Optional[Callable] = None,
         sentiment_threshold: Optional[float] = None,
         custom_exit_command: Optional[str] = "exit",
         sentiment_analyzer: Optional[Callable] = None,
         limit_tokens_from_string: Optional[Callable] = None,
         custom_tools_prompt: Optional[Callable] = None,
+        tool_schema: ToolUsageType = None,
+        output_type: agent_output_type = None,
+        function_calling_type: str = "json",
+        output_cleaner: Optional[Callable] = None,
+        function_calling_format_type: Optional[str] = "OpenAI",
+        list_tool_schemas: Optional[List[BaseModel]] = None,
+        metadata_output_type: str = "json",
         *args,
         **kwargs,
     ):
         self.id = id
         self.llm = llm
         self.template = template
         self.max_loops = max_loops
@@ -266,14 +284,21 @@
         self.output_json = output_json
         self.stopping_func = stopping_func
         self.custom_loop_condition = custom_loop_condition
         self.sentiment_threshold = sentiment_threshold
         self.custom_exit_command = custom_exit_command
         self.sentiment_analyzer = sentiment_analyzer
         self.limit_tokens_from_string = limit_tokens_from_string
+        self.tool_schema = tool_schema
+        self.output_type = output_type
+        self.function_calling_type = function_calling_type
+        self.output_cleaner = output_cleaner
+        self.function_calling_format_type = function_calling_format_type
+        self.list_tool_schemas = list_tool_schemas
+        self.metadata_output_type = metadata_output_type
 
         # The max_loops will be set dynamically if the dynamic_loop
         if self.dynamic_loops:
             logger.info("Dynamic loops enabled")
             self.max_loops = "auto"
 
         # If multimodal = yes then set the sop to the multimodal sop
@@ -289,19 +314,23 @@
 
         # Initialize the code executor
         self.code_executor = SubprocessCodeInterpreter(
             debug_mode=True,
         )
 
         # If the preset stopping token is enabled then set the stopping token to the preset stopping token
-        if preset_stopping_token:
+        if preset_stopping_token is not None:
             self.stopping_token = "<DONE>"
 
+        # If the stopping function is provided then set the stopping condition to the stopping function
         self.short_memory = Conversation(
-            system_prompt=self.system_prompt, time_enabled=True
+            system_prompt=system_prompt,
+            time_enabled=True,
+            *args,
+            **kwargs
         )
 
         # If the docs exist then ingest the docs
         if self.docs:
             self.ingest_docs(self.docs)
 
         # If docs folder exists then get the docs from docs folder
@@ -322,17 +351,15 @@
                 tools_prompt = custom_tools_prompt(tools=self.tools)
 
                 self.short_memory.add(
                     role=self.agent_name, content=tools_prompt
                 )
 
             else:
-                tools_prompt = tool_usage_worker_prompt(
-                    tools=self.tools
-                )
+                tools_prompt = tool_usage_worker_prompt(tools=self.tools)
 
                 # Append the tools prompt to the short_term_memory
                 self.short_memory.add(
                     role=self.agent_name, content=tools_prompt
                 )
 
         # If the long term memory is provided then set the long term memory prompt
@@ -350,23 +377,45 @@
 
         # Set the logger handler
         if logger_handler:
             logger.add(
                 f"{self.agent_name}.log",
                 level="INFO",
                 colorize=True,
-                format=(
-                    "<green>{time}</green> <level>{message}</level>"
-                ),
+                format=("<green>{time}</green> <level>{message}</level>"),
                 backtrace=True,
                 diagnose=True,
             )
 
         # logger.info("Creating Agent {}".format(self.agent_name))
 
+        # If the tool types
+        if self.tool_schema is not None:
+            logger.info("Tool schema provided")
+            tool_schema_str = self.tool_schema_to_str(self.tool_schema)
+            
+            print(tool_schema_str)
+
+            # Add to the short memory
+            logger.info(f"Adding tool schema to memory: {tool_schema_str}")
+            self.short_memory.add(
+                role=self.user_name, content=tool_schema_str
+            )
+
+        # If a list of tool schemas:
+        if self.list_tool_schemas is not None:
+            logger.info("Tool schema provided")
+            tool_schema_str = self.tool_schemas_to_str(list_tool_schemas)
+
+            # Add to the short memory
+            logger.info(f"Adding tool schema to memory: {tool_schema_str}")
+            self.short_memory.add(
+                role=self.user_name, content=tool_schema_str
+            )
+
     def set_system_prompt(self, system_prompt: str):
         """Set the system prompt"""
         self.system_prompt = system_prompt
 
     def provide_feedback(self, feedback: str) -> None:
         """Allow users to provide feedback on the responses."""
         self.feedback.append(feedback)
@@ -399,47 +448,37 @@
                 self.llm.temperature = random.uniform(0.0, 1.0)
                 logger.info(f"Temperature: {self.llm.temperature}")
             else:
                 # Use a default temperature
                 self.llm.temperature = 0.7
         except Exception as error:
             print(
-                colored(
-                    f"Error dynamically changing temperature: {error}"
-                )
+                colored(f"Error dynamically changing temperature: {error}")
             )
 
     def format_prompt(self, template, **kwargs: Any) -> str:
         """Format the template with the provided kwargs using f-string interpolation."""
         return template.format(**kwargs)
 
     def add_task_to_memory(self, task: str):
         """Add the task to the memory"""
         try:
             logger.info(f"Adding task to memory: {task}")
             self.short_memory.add(f"{self.user_name}: {task}")
         except Exception as error:
-            print(
-                colored(
-                    f"Error adding task to memory: {error}", "red"
-                )
-            )
+            print(colored(f"Error adding task to memory: {error}", "red"))
 
     def add_message_to_memory(self, message: str):
         """Add the message to the memory"""
         try:
             logger.info(f"Adding message to memory: {message}")
-            self.short_memory.add(
-                role=self.agent_name, content=message
-            )
+            self.short_memory.add(role=self.agent_name, content=message)
         except Exception as error:
             print(
-                colored(
-                    f"Error adding message to memory: {error}", "red"
-                )
+                colored(f"Error adding message to memory: {error}", "red")
             )
 
     def add_message_to_memory_and_truncate(self, message: str):
         """Add the message to the memory and truncate"""
         self.short_memory[-1].append(message)
         self.truncate_history()
 
@@ -532,42 +571,110 @@
 
         Args:
             content (str, optional): _description_. Defaults to None.
         """
         for chunk in content:
             print(chunk, end="")
 
+    ########################## FUNCTION CALLING ##########################
+
+    def json_str_to_json(self, json_str: str):
+        """Convert a JSON string to a JSON object"""
+        return json.loads(json_str)
+
+    def json_str_to_pydantic_model(self, json_str: str, model: BaseModel):
+        """Convert a JSON string to a Pydantic model"""
+        return model.model_validate_json(json_str)
+
+    def json_str_to_dict(self, json_str: str):
+        """Convert a JSON string to a dictionary"""
+        return json.loads(json_str)
+
+    def pydantic_model_to_json_str(self, model: BaseModel):
+        return str(pydantic_to_functions(model))
+
+    def dict_to_json_str(self, dictionary: dict):
+        """Convert a dictionary to a JSON string"""
+        return json.dumps(dictionary)
+
+    def dict_to_pydantic_model(self, dictionary: dict, model: BaseModel):
+        """Convert a dictionary to a Pydantic model"""
+        return model.model_validate_json(dictionary)
+
+    # def prep_pydantic_model_for_str(self, model: BaseModel):
+    #     # Convert to Function
+    #     out = self.pydantic_model_to_json_str(model)
+
+    #     # return function_to_str(out)
+
+    def tool_schema_to_str(
+        self, tool_schema: BaseModel = None, *args, **kwargs
+    ):
+        """Convert a tool schema to a string"""
+        out = pydantic_to_functions(tool_schema)
+        return str(out)
+
+    def tool_schemas_to_str(
+        self, tool_schemas: List[BaseModel] = None, *args, **kwargs
+    ):
+        """Convert a list of tool schemas to a string"""
+        out = multi_pydantic_to_functions(tool_schemas)
+        return str(out)
+
+    def str_to_pydantic_model(self, string: str, model: BaseModel):
+        """Convert a string to a Pydantic model"""
+        return model.model_validate_json(string)
+
+    def list_str_to_pydantic_model(
+        self, list_str: List[str], model: BaseModel
+    ):
+        """Convert a list of strings to a Pydantic model"""
+        # return model.model_validate_json(list_str)
+        for string in list_str:
+            return model.model_validate_json(string)
+
+    def prepare_output_for_output_model(
+        self, output: agent_output_type = None
+    ):
+        """Prepare the output for the output model"""
+        if self.output_type == BaseModel:
+            return self.str_to_pydantic_model(output, self.output_type)
+        elif self.output_type == dict:
+            return self.dict_to_json_str(output)
+        elif self.output_type == str:
+            return output
+        else:
+            return output
+
+    ########################## FUNCTION CALLING ##########################
+
     def _history(self, user_name: str, task: str) -> str:
         """Generate the history for the history prompt
 
         Args:
             user_name (str): _description_
             task (str): _description_
 
         Returns:
             str: _description_
         """
         history = [f"{user_name}: {task}"]
         return history
 
-    def _dynamic_prompt_setup(
-        self, dynamic_prompt: str, task: str
-    ) -> str:
+    def _dynamic_prompt_setup(self, dynamic_prompt: str, task: str) -> str:
         """_dynamic_prompt_setup summary
 
         Args:
             dynamic_prompt (str): _description_
             task (str): _description_
 
         Returns:
             str: _description_
         """
-        dynamic_prompt = (
-            dynamic_prompt or self.construct_dynamic_prompt()
-        )
+        dynamic_prompt = dynamic_prompt or self.construct_dynamic_prompt()
         combined_prompt = f"{dynamic_prompt}\n{task}"
         return combined_prompt
 
     def run(
         self,
         task: Optional[str] = None,
         img: Optional[str] = None,
@@ -577,76 +684,69 @@
         """
         Run the autonomous agent loop
         """
         try:
             self.activate_autonomous_agent()
 
             if task:
-                self.short_memory.add(
-                    role=self.user_name, content=task
-                )
+                self.short_memory.add(role=self.user_name, content=task)
 
             loop_count = 0
             response = None
+            step_pool = []
 
             while (
                 self.max_loops == "auto"
                 or loop_count < self.max_loops
                 # or self.custom_loop_condition()
             ):
                 loop_count += 1
                 self.loop_count_print(loop_count, self.max_loops)
                 print("\n")
 
                 if self.dynamic_temperature_enabled:
                     self.dynamic_temperature()
 
-                task_prompt = (
-                    self.short_memory.return_history_as_string()
-                )
+                task_prompt = self.short_memory.return_history_as_string()
 
                 attempt = 0
                 success = False
                 while attempt < self.retry_attempts and not success:
                     try:
                         response_args = (
                             (task_prompt, *args)
                             if img is None
                             else (task_prompt, img, *args)
                         )
                         response = self.llm(*response_args, **kwargs)
-                        print(response)
+                        # print(response)
                         self.short_memory.add(
                             role=self.agent_name, content=response
                         )
 
                         if self.tools:
                             # Extract code from markdown
-                            response = extract_code_from_markdown(
-                                response
-                            )
+                            response = extract_code_from_markdown(response)
 
                             # Execute the tool by name
                             execute_tool_by_name(
                                 response,
                                 self.tools,
                                 stop_token=self.stopping_token,
                             )
 
                         if self.code_interpreter:
                             # Extract code from markdown
-                            extracted_code = (
-                                extract_code_from_markdown(response)
+                            extracted_code = extract_code_from_markdown(
+                                response
                             )
 
                             # Execute the code
                             # execution = execute_command(extracted_code)
-                            execution = CodeExecutor().run(
-                                extracted_code
-                            )
+                            execution = CodeExecutor().run(extracted_code)
 
                             # Add the execution to the memory
                             self.short_memory.add(
                                 role=self.agent_name,
                                 content=execution,
                             )
 
@@ -654,31 +754,27 @@
                             response = self.llm(
                                 self.short_memory.return_history_as_string(),
                                 *args,
                                 **kwargs,
                             )
 
                         if self.evaluator:
-                            evaluated_response = self.evaluator(
-                                response
-                            )
+                            evaluated_response = self.evaluator(response)
                             print(
                                 "Evaluated Response:"
                                 f" {evaluated_response}"
                             )
                             self.short_memory.add(
                                 role=self.agent_name,
                                 content=evaluated_response,
                             )
 
                         # Sentiment analysis
                         if self.sentiment_analyzer:
-                            sentiment = self.sentiment_analyzer(
-                                response
-                            )
+                            sentiment = self.sentiment_analyzer(response)
                             print(f"Sentiment: {sentiment}")
 
                             if sentiment > self.sentiment_threshold:
                                 print(
                                     f"Sentiment: {sentiment} is above"
                                     " threshold:"
                                     f" {self.sentiment_threshold}"
@@ -692,14 +788,19 @@
 
                             # print(f"Sentiment: {sentiment}")
                             self.short_memory.add(
                                 role=self.agent_name,
                                 content=sentiment,
                             )
 
+                        if self.streaming:
+                            self.streaming(response)
+                        else:
+                            print(response)
+
                         success = True  # Mark as successful to exit the retry loop
 
                     except Exception as e:
                         logger.error(
                             f"Attempt {attempt+1}: Error generating"
                             f" response: {e}"
                         )
@@ -717,17 +818,16 @@
                     if self.stopping_token in response:
                         break
                 elif (
                     self.stopping_condition is not None
                     and self._check_stopping_condition(response)
                 ):
                     break
-                elif (
-                    self.stopping_func is not None
-                    and self.stopping_func(response)
+                elif self.stopping_func is not None and self.stopping_func(
+                    response
                 ):
                     break
 
                 if self.interactive:
                     user_input = colored(input("You: "), "red")
 
                     # User-defined exit command
@@ -744,18 +844,45 @@
 
                 if self.loop_interval:
                     logger.info(
                         f"Sleeping for {self.loop_interval} seconds"
                     )
                     time.sleep(self.loop_interval)
 
+                # Save Step Metadata
+                active_step = Step(
+                    task_id=task_id(),
+                    step_id=loop_count,
+                    name=task,
+                    output=response,
+                    max_loops=self.max_loops,
+                )
+
+                step_pool.append(active_step)
+
+                # Save the step pool
+                # self.step_cache = step_pool
+
             if self.autosave:
                 logger.info("Autosaving agent state.")
                 self.save_state(self.saved_state_path)
 
+            # Apply the cleaner function to the response
+            if self.output_cleaner is not None:
+                response = self.output_cleaner(response)
+
+            # Prepare the output for the output model
+            if self.output_type is not None:
+                response = self.prepare_output_for_output_model(response)
+
+            # List of steps for this task
+            ManySteps(task_id=task_id(), steps=step_pool)
+
+            # Save Many steps
+
             return response
         except Exception as error:
             print(f"Error running agent: {error}")
             raise error
 
     def __call__(self, task: str, img: str = None, *args, **kwargs):
         """Call the agent
@@ -812,36 +939,32 @@
         Args:
             system_prompt (str): The system prompt
             history (List[str]): The history of the conversation
 
         Returns:
             str: The agent history prompt
         """
-        ltr = str(self.long_term_memory.query(query), *args, **kwargs)
+        ltr = self.long_term_memory.query(query, *args, **kwargs)
 
         context = f"""
             System: This reminds you of these events from your past: [{ltr}]
         """
-        return self.short_memory.add(
-            role=self.agent_name, content=context
-        )
+        return self.short_memory.add(role=self.agent_name, content=context)
 
     def add_memory(self, message: str):
         """Add a memory to the agent
 
         Args:
             message (str): _description_
 
         Returns:
             _type_: _description_
         """
         logger.info(f"Adding memory: {message}")
-        return self.short_memory.add(
-            role=self.agent_name, content=message
-        )
+        return self.short_memory.add(role=self.agent_name, content=message)
 
     async def run_concurrent(self, tasks: List[str], **kwargs):
         """
         Run a batch of tasks concurrently and handle an infinite level of task inputs.
 
         Args:
             tasks (List[str]): A list of tasks to run.
@@ -880,17 +1003,15 @@
             file_path (_type_): _description_
         """
         try:
             with open(file_path, "w") as f:
                 json.dump(self.short_memory, f)
             # print(f"Saved agent history to {file_path}")
         except Exception as error:
-            print(
-                colored(f"Error saving agent history: {error}", "red")
-            )
+            print(colored(f"Error saving agent history: {error}", "red"))
 
     def load(self, file_path: str):
         """
         Load the agent history from a file.
 
         Args:
             file_path (str): The path to the file containing the saved agent history.
@@ -907,43 +1028,30 @@
         return True
 
     def print_history_and_memory(self):
         """
         Prints the entire history and memory of the agent.
         Each message is colored and formatted for better readability.
         """
-        print(
-            colored(
-                "Agent History and Memory", "cyan", attrs=["bold"]
-            )
-        )
-        print(
-            colored(
-                "========================", "cyan", attrs=["bold"]
-            )
-        )
-        for loop_index, history in enumerate(
-            self.short_memory, start=1
-        ):
+        print(colored("Agent History and Memory", "cyan", attrs=["bold"]))
+        print(colored("========================", "cyan", attrs=["bold"]))
+        for loop_index, history in enumerate(self.short_memory, start=1):
             print(
-                colored(
-                    f"\nLoop {loop_index}:", "yellow", attrs=["bold"]
-                )
+                colored(f"\nLoop {loop_index}:", "yellow", attrs=["bold"])
             )
             for message in history:
                 speaker, _, message_text = message.partition(": ")
                 if "Human" in speaker:
                     print(
                         colored(f"{speaker}:", "green")
                         + f" {message_text}"
                     )
                 else:
                     print(
-                        colored(f"{speaker}:", "blue")
-                        + f" {message_text}"
+                        colored(f"{speaker}:", "blue") + f" {message_text}"
                     )
             print(colored("------------------------", "cyan"))
         print(colored("End of Agent History", "cyan", attrs=["bold"]))
 
     def step(self, task: str, **kwargs):
         """
 
@@ -966,17 +1074,15 @@
             response = self.llm(task, **kwargs)
 
             # Update the agent's history with the new interaction
             if self.interactive:
                 self.short_memory.add(
                     role=self.agent_name, content=response
                 )
-                self.short_memory.add(
-                    role=self.user_name, content=task
-                )
+                self.short_memory.add(role=self.user_name, content=task)
             else:
                 self.short_memory.add(
                     role=self.agent_name, content=response
                 )
 
             return response
         except Exception as error:
@@ -1045,17 +1151,15 @@
         self.reponse_filters.append(filter_word)
 
     def apply_reponse_filters(self, response: str) -> str:
         """
         Apply the response filters to the response
 
         """
-        logger.info(
-            f"Applying response filters to response: {response}"
-        )
+        logger.info(f"Applying response filters to response: {response}")
         for word in self.response_filters:
             response = response.replace(word, "[FILTERED]")
         return response
 
     def filtered_run(self, task: str) -> str:
         """
         # Feature 3: Response filtering
@@ -1087,17 +1191,15 @@
             file_path (str): The path to the YAML file
         """
         try:
             logger.info(f"Saving agent to YAML file: {file_path}")
             with open(file_path, "w") as f:
                 yaml.dump(self.__dict__, f)
         except Exception as error:
-            print(
-                colored(f"Error saving agent to YAML: {error}", "red")
-            )
+            print(colored(f"Error saving agent to YAML: {error}", "red"))
 
     def save_state(self, file_path: str) -> None:
         """
         Saves the current state of the agent to a JSON file, including the llm parameters.
 
         Args:
             file_path (str): The path to the JSON file where the state will be saved.
@@ -1117,33 +1219,27 @@
                     self.short_memory.return_history_as_string()
                 ),
                 "loop_interval": self.loop_interval,
                 "retry_attempts": self.retry_attempts,
                 "retry_interval": self.retry_interval,
                 "interactive": self.interactive,
                 "dashboard": self.dashboard,
-                "dynamic_temperature": (
-                    self.dynamic_temperature_enabled
-                ),
+                "dynamic_temperature": (self.dynamic_temperature_enabled),
                 "autosave": self.autosave,
                 "saved_state_path": self.saved_state_path,
                 "max_loops": self.max_loops,
             }
 
             with open(file_path, "w") as f:
                 json.dump(state, f, indent=4)
 
-            saved = colored(
-                f"Saved agent state to: {file_path}", "green"
-            )
+            saved = colored(f"Saved agent state to: {file_path}", "green")
             print(saved)
         except Exception as error:
-            print(
-                colored(f"Error saving agent state: {error}", "red")
-            )
+            print(colored(f"Error saving agent state: {error}", "red"))
 
     def state_to_str(self):
         """Transform the JSON into a string"""
         try:
             state = {
                 "agent_id": str(self.id),
                 "agent_name": self.agent_name,
@@ -1154,17 +1250,15 @@
                     self.short_memory.return_history_as_string()
                 ),
                 "loop_interval": self.loop_interval,
                 "retry_attempts": self.retry_attempts,
                 "retry_interval": self.retry_interval,
                 "interactive": self.interactive,
                 "dashboard": self.dashboard,
-                "dynamic_temperature": (
-                    self.dynamic_temperature_enabled
-                ),
+                "dynamic_temperature": (self.dynamic_temperature_enabled),
                 "autosave": self.autosave,
                 "saved_state_path": self.saved_state_path,
                 "max_loops": self.max_loops,
             }
             out = str(state)
             return out
         except Exception as error:
@@ -1205,17 +1299,15 @@
             self.loop_interval = state.get("loop_interval", 1)
             self.retry_attempts = state.get("retry_attempts", 3)
             self.retry_interval = state.get("retry_interval", 1)
             self.interactive = state.get("interactive", False)
 
             print(f"Agent state loaded from {file_path}")
         except Exception as error:
-            print(
-                colored(f"Error loading agent state: {error}", "red")
-            )
+            print(colored(f"Error loading agent state: {error}", "red"))
 
     def retry_on_failure(
         self,
         function: callable,
         retries: int = 3,
         retry_delay: int = 1,
     ):
@@ -1223,17 +1315,15 @@
         try:
             logger.info(f"Retrying function: {function}")
             attempt = 0
             while attempt < retries:
                 try:
                     return function()
                 except Exception as error:
-                    logging.error(
-                        f"Error generating response: {error}"
-                    )
+                    logging.error(f"Error generating response: {error}")
                     attempt += 1
                     time.sleep(retry_delay)
             raise Exception("All retry attempts failed")
         except Exception as error:
             print(colored(f"Error retrying function: {error}", "red"))
 
     def update_system_prompt(self, system_prompt: str):
@@ -1254,15 +1344,15 @@
 
     def update_retry_interval(self, retry_interval: int):
         """Update the retry interval"""
         self.retry_interval = retry_interval
 
     def reset(self):
         """Reset the agent"""
-        self.short_memory = {}
+        self.short_memory = None
 
     def run_code(self, code: str):
         """
         text -> parse_code by looking for code inside 6 backticks `````-> run_code
         """
         try:
             logger.info(f"Running code: {code}")
@@ -1311,17 +1401,15 @@
         Returns:
             _type_: _description_
         """
         try:
             for doc in docs:
                 data = data_to_text(doc)
 
-            return self.short_memory.add(
-                role=self.user_name, content=data
-            )
+            return self.short_memory.add(role=self.user_name, content=data)
         except Exception as error:
             print(colored(f"Error ingesting docs: {error}", "red"))
 
     def ingest_pdf(self, pdf: str):
         """Ingest the pdf into the memory
 
         Args:
@@ -1329,17 +1417,15 @@
 
         Returns:
             _type_: _description_
         """
         try:
             logger.info(f"Ingesting pdf: {pdf}")
             text = pdf_to_text(pdf)
-            return self.short_memory.add(
-                role=self.user_name, content=text
-            )
+            return self.short_memory.add(role=self.user_name, content=text)
         except Exception as error:
             print(colored(f"Error ingesting pdf: {error}", "red"))
 
     def receieve_mesage(self, name: str, message: str):
         """Receieve a message"""
         try:
             message = f"{name}: {message}"
@@ -1352,19 +1438,15 @@
     ):
         """Send a message to the agent"""
         try:
             logger.info(f"Sending agent message: {message}")
             message = f"{agent_name}: {message}"
             return self.run(message, *args, **kwargs)
         except Exception as error:
-            print(
-                colored(
-                    f"Error sending agent message: {error}", "red"
-                )
-            )
+            print(colored(f"Error sending agent message: {error}", "red"))
 
     def truncate_history(self):
         """
         Truncates the short-term memory of the agent based on the count of tokens.
 
         The method counts the tokens in the short-term memory using the tokenizer and
         compares it with the length of the memory. If the length of the memory is greater
@@ -1398,17 +1480,15 @@
             # Get the list of files then extract them and add them to the memory
             files = os.listdir(self.docs_folder)
 
             # Extract the text from the files
             for file in files:
                 text = data_to_text(file)
 
-            return self.short_memory.add(
-                role=self.user_name, content=text
-            )
+            return self.short_memory.add(role=self.user_name, content=text)
         except Exception as error:
             print(
                 colored(
                     f"Error getting docs from doc folders: {error}",
                     "red",
                 )
             )
```

### Comparing `swarms-4.8.2/swarms/structs/agent_job.py` & `swarms-4.8.7/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/agent_process.py` & `swarms-4.8.7/swarms/structs/agent_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 from pydantic import BaseModel
 
-from swarms.structs.omni_agent_types import agents
+from swarms.structs.omni_agent_types import AgentListType
 from swarms.utils.loguru_logger import logger
 from typing import Callable
 
 
 class AgentProcess(BaseModel):
     agent_id: int
     agent_name: str
@@ -50,15 +50,15 @@
     def __init__(self, max_pid: int = 1024):
         self.MAX_PID = max_pid
         self.pid_pool = [False for i in range(self.MAX_PID)]
         self.agent_process_queue = (
             []
         )  # Currently use list to simulate queue
 
-    def add(self, agents: agents):
+    def add(self, agents: AgentListType):
         """
         Adds an agent process to the queue.
 
         Args:
             agent_process (AgentProcess): The agent process to be added.
 
         Returns:
```

### Comparing `swarms-4.8.2/swarms/structs/agent_rearrange.py` & `swarms-4.8.7/swarms/structs/agent_rearrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,15 @@
         specific_tasks: dict,
     ):
         dest_agent = self.self_find_agent_by_name(dest_agent_name)
         if not dest_agent:
             return None
         task_to_run = specific_tasks.get(dest_agent_name, task)
         if self.custom_prompt:
-            out = dest_agent.run(
-                f"{task_to_run} {self.custom_prompt}"
-            )
+            out = dest_agent.run(f"{task_to_run} {self.custom_prompt}")
         else:
             out = dest_agent.run(f"{task_to_run} (from {source})")
         return out
 
     def process_flows(self, pattern, default_task, specific_tasks):
         if not self.parse_pattern(pattern):
             return None
@@ -134,17 +132,15 @@
                 task = specific_tasks.get(source, default_task)
                 source_agent = self.self_find_agent_by_name(source)
                 if source_agent:
                     result = source_agent.run(task)
                     results.append(result)
             else:
                 for destination in destinations:
-                    task = specific_tasks.get(
-                        destination, default_task
-                    )
+                    task = specific_tasks.get(destination, default_task)
                     destination_agent = self.self_find_agent_by_name(
                         destination
                     )
                     if destination_agent:
                         result = destination_agent.run(task)
                         results.append(result)
         return results
@@ -152,17 +148,15 @@
     def __call__(
         self,
         pattern: str = None,
         default_task: str = None,
         **specific_tasks,
     ):
         self.flows.clear()  # Reset previous flows
-        results = self.process_flows(
-            pattern, default_task, specific_tasks
-        )
+        results = self.process_flows(pattern, default_task, specific_tasks)
         return results
 
 
 # ## Initialize the workflow
 # agent = Agent(
 #     agent_name="t",
 #     agent_description=(
```

### Comparing `swarms-4.8.2/swarms/structs/async_workflow.py` & `swarms-4.8.7/swarms/structs/async_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,15 @@
                     raise ValueError(
                         "Either task or tasks must be provided"
                     )
 
         except Exception as error:
             logger.error(f"[ERROR][AsyncWorkflow] {error}")
 
-    async def delete(
-        self, task: Any = None, tasks: List[Task] = None
-    ):
+    async def delete(self, task: Any = None, tasks: List[Task] = None):
         """Delete a task from the workflow"""
         try:
             if task:
                 self.task_pool.remove(task)
             elif tasks:
                 for task in tasks:
                     self.task_pool.remove(task)
```

### Comparing `swarms-4.8.2/swarms/structs/auto_swarm.py` & `swarms-4.8.7/swarms/structs/auto_swarm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,13 @@
 from typing import Any, Callable, Dict, Optional, Sequence
 
-from swarms.models.base_llm import AbstractLLM
 from swarms.structs.base_swarm import BaseSwarm
 from swarms.utils.loguru_logger import logger
 
 
-class SequentialAccountingSwarm(BaseSwarm):
-    """SequentialAccountingSwarm class represents a swarm of agents that can be created automatically.
-
-    Flow:
-    name -> router -> swarm entry point
-
-    Attributes:
-        name (str, optional): The name of the swarm. Defaults to "kyegomez/sequential-accounting-swarm".
-        description (str, optional): The description of the swarm. Defaults to None.
-        verbose (bool): Whether to enable verbose mode or not. Defaults to False.
-        custom_params (dict, optional): Custom parameters for the swarm. Defaults to None.
-        iters (int, optional): The number of iterations for the swarm simulation. Defaults to 100.
-        max_agents (int, optional): The maximum number of agents in the swarm. Defaults to 100.
-        agents (Sequence[AbstractLLM], optional): The list of agents in the swarm. Defaults to None.
-
-    Methods:
-        run(task: str = None, *args, **kwargs) -> Any:
-            Run the swarm simulation.
-
-    """
-
-    def __init__(
-        self,
-        name: Optional[str] = "kyegomez/sequential-accounting-swarm",
-        description: Optional[str] = None,
-        verbose: bool = False,
-        custom_params: Optional[Dict[str, Any]] = None,
-        iters: Optional[int] = 100,
-        max_agents: Optional[int] = 100,
-        agents: Sequence[AbstractLLM] = None,
-        *args,
-        **kwargs,
-    ):
-        super().__init__()
-        self.name = name
-        self.description = description
-        self.verbose = verbose
-        self.custom_params = custom_params
-        self.iters = iters
-        self.max_agents = max_agents
-        self.agents = agents
-
-    def run(self, task: str = None, *args, **kwargs):
-        """Run the swarm simulation.
-
-        Args:
-            task (str, optional): The task to be performed by the agents. Defaults to None.
-            *args: Variable length argument list.
-            **kwargs: Arbitrary keyword arguments.
-
-        Returns:
-            Any: The final result of the swarm simulation.
-
-        """
-        for agent in self.agents:
-            out = agent.run(task, *args, **kwargs)
-            final = agent.run(out)
-
-        return final
-
-
 class AutoSwarmRouter(BaseSwarm):
     """AutoSwarmRouter class represents a router for the AutoSwarm class.
 
     This class is responsible for routing tasks to the appropriate swarm based on the provided name.
     It allows customization of the preprocessing, routing, and postprocessing of tasks.
 
     Attributes:
@@ -136,28 +74,24 @@
                     # If custom postprocess function is provided then run it
                     out = self.custom_postprocess(out)
 
                 return out
 
             if self.name in self.swarm_dict:
                 # If a match is found then send the task to the swarm
-                out = self.swarm_dict[self.name].run(
-                    task, *args, **kwargs
-                )
+                out = self.swarm_dict[self.name].run(task, *args, **kwargs)
 
                 if self.custom_postprocess:
                     # If custom postprocess function is provided then run it
                     out = self.custom_postprocess(out)
 
                 return out
 
             # If no match is found then return None
-            raise ValueError(
-                f"Swarm with name {self.name} not found."
-            )
+            raise ValueError(f"Swarm with name {self.name} not found.")
         except Exception as e:
             logger.error(f"Error: {e}")
             raise e
 
 
 class AutoSwarm(BaseSwarm):
     """AutoSwarm class represents a swarm of agents that can be created automatically.
@@ -175,27 +109,25 @@
 
     def __init__(
         self,
         name: Optional[str] = None,
         description: Optional[str] = None,
         verbose: bool = False,
         custom_params: Optional[Dict[str, Any]] = None,
-        router: Optional[AutoSwarmRouter] = None,
         custom_preprocess: Optional[Callable] = None,
         custom_postprocess: Optional[Callable] = None,
         custom_router: Optional[Callable] = None,
         *args,
         **kwargs,
     ):
         super().__init__()
         self.name = name
         self.description = description
         self.verbose = verbose
         self.custom_params = custom_params
-        self.router = router
         self.custom_preprocess = custom_preprocess
         self.custom_postprocess = custom_postprocess
         self.router = AutoSwarmRouter(
             name=name,
             description=description,
             verbose=verbose,
             custom_params=custom_params,
```

### Comparing `swarms-4.8.2/swarms/structs/base.py` & `swarms-4.8.7/swarms/structs/base_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import asyncio
 import concurrent.futures
 import json
 import os
-from abc import ABC
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import psutil
 
 try:
     import gzip
 except ImportError as error:
     print(f"Error importing gzip: {error}")
+# from pydantic import BaseModel
 
 
-class BaseStructure(ABC):
+class BaseStructure:
     """Base structure.
 
 
     Attributes:
         name (Optional[str]): _description_
         description (Optional[str]): _description_
         save_metadata (bool): _description_
@@ -55,34 +55,36 @@
         load_config: _description_
         backup_data: _description_
         monitor_resources: _description_
         run_with_resources: _description_
         run_with_resources_batched: _description_
 
     Examples:
-
+    >>> base_structure = BaseStructure()
+    >>> base_structure
+    BaseStructure(name=None, description=None, save_metadata=True, save_artifact_path='./artifacts', save_metadata_path='./metadata', save_error_path='./errors')
     """
 
     def __init__(
         self,
         name: Optional[str] = None,
         description: Optional[str] = None,
         save_metadata: bool = True,
         save_artifact_path: Optional[str] = "./artifacts",
         save_metadata_path: Optional[str] = "./metadata",
         save_error_path: Optional[str] = "./errors",
-        *args,
-        **kwargs,
     ):
+        super().__init__()
         self.name = name
         self.description = description
         self.save_metadata = save_metadata
         self.save_artifact_path = save_artifact_path
         self.save_metadata_path = save_metadata_path
         self.save_error_path = save_error_path
+        
 
     def run(self, *args, **kwargs):
         """Run the structure."""
 
     def save_to_file(self, data: Any, file_path: str):
         """Save data to file.
 
@@ -192,17 +194,15 @@
         )
         with open(file, "a") as file:
             file.write(log_message)
 
     async def run_async(self, *args, **kwargs):
         """Run the structure asynchronously."""
         loop = asyncio.get_event_loop()
-        return await loop.run_in_executor(
-            None, self.run, *args, **kwargs
-        )
+        return await loop.run_in_executor(None, self.run, *args, **kwargs)
 
     async def save_metadata_async(self, metadata: Dict[str, Any]):
         """Save metadata to file asynchronously.
 
         Args:
             metadata (Dict[str, Any]): _description_
         """
@@ -227,17 +227,15 @@
             error_message (str): _description_
         """
         loop = asyncio.get_event_loop()
         return await loop.run_in_executor(
             None, self.log_error, error_message
         )
 
-    async def save_artifact_async(
-        self, artifact: Any, artifact_name: str
-    ):
+    async def save_artifact_async(self, artifact: Any, artifact_name: str):
         """Save artifact to file asynchronously.
 
         Args:
             artifact (Any): _description_
             artifact_name (str): _description_
         """
         loop = asyncio.get_event_loop()
@@ -271,17 +269,15 @@
             event_type (str, optional): _description_. Defaults to "INFO".
         """
         loop = asyncio.get_event_loop()
         return await loop.run_in_executor(
             None, self.log_event, event, event_type
         )
 
-    async def asave_to_file(
-        self, data: Any, file: str, *args, **kwargs
-    ):
+    async def asave_to_file(self, data: Any, file: str, *args, **kwargs):
         """Save data to file asynchronously.
 
         Args:
             data (Any): _description_
             file (str): _description_
         """
         await asyncio.to_thread(
@@ -362,16 +358,15 @@
             batch_size (int, optional): _description_. Defaults to 10.
 
         Returns:
             _type_: _description_
         """
         with ThreadPoolExecutor(max_workers=batch_size) as executor:
             futures = [
-                executor.submit(self.run, data)
-                for data in batched_data
+                executor.submit(self.run, data) for data in batched_data
             ]
             return [future.result() for future in futures]
 
     def load_config(
         self, config: str = None, *args, **kwargs
     ) -> Dict[str, Any]:
         """Load config from file.
@@ -423,10 +418,13 @@
             batched_data (List[Any]): _description_
             batch_size (int, optional): _description_. Defaults to 10.
 
         Returns:
             _type_: _description_
         """
         self.monitor_resources()
-        return self.run_batched(
-            batched_data, batch_size, *args, **kwargs
-        )
+        return self.run_batched(batched_data, batch_size, *args, **kwargs)
+
+
+# x = BaseStructure()
+
+# print(x)
```

### Comparing `swarms-4.8.2/swarms/structs/base_swarm.py` & `swarms-4.8.7/swarms/structs/base_swarm.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 
 import yaml
 
 from swarms.structs.agent import Agent
 from swarms.structs.conversation import Conversation
 from swarms.utils.loguru_logger import logger
-from swarms.structs.omni_agent_types import agent
+from swarms.structs.omni_agent_types import AgentType
 
 
 class BaseSwarm(ABC):
     """
     Abstract Swarm Class for multi-agent systems
 
     Attributes:
@@ -64,67 +64,52 @@
         abatch_run: Asynchronous batch run with language model
         arun: Asynchronous run
 
     """
 
     def __init__(
         self,
-        # name: str = "Swarm",
-        agents: List[Agent] = None,
-        models: List[Any] = None,
-        max_loops: int = 200,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        agents: Optional[List[Agent]] = None,
+        models: Optional[List[Any]] = None,
+        max_loops: Optional[int] = 200,
         callbacks: Optional[Sequence[callable]] = None,
-        autosave: bool = False,
-        logging: bool = False,
-        return_metadata: bool = False,
-        metadata_filename: str = "multiagent_structure_metadata.json",
+        autosave: Optional[bool] = False,
+        logging: Optional[bool] = False,
+        return_metadata: Optional[bool] = False,
+        metadata_filename: Optional[
+            str
+        ] = "multiagent_structure_metadata.json",
         stopping_function: Optional[Callable] = None,
         stopping_condition: Optional[str] = "stop",
         stopping_condition_args: Optional[Dict] = None,
         *args,
         **kwargs,
     ):
         """Initialize the swarm with agents"""
+        self.name = name
+        self.description = description
         self.agents = agents
         self.models = models
         self.max_loops = max_loops
         self.callbacks = callbacks
         self.autosave = autosave
         self.logging = logging
         self.return_metadata = return_metadata
         self.metadata_filename = metadata_filename
         self.stopping_function = stopping_function
         self.stopping_condition = stopping_condition
         self.stopping_condition_args = stopping_condition_args
 
+        # Initialize conversation
         self.conversation = Conversation(
             time_enabled=True, *args, **kwargs
         )
 
-        # Handle the case where the agents are not provided
-        # Handle agents
-        for agent in self.agents:
-            if not isinstance(agent, Agent):
-                raise TypeError("Agents must be of type Agent.")
-
-        if self.agents is None:
-            self.agents = []
-
-        # Handle the case where the callbacks are not provided
-        if self.callbacks is None:
-            self.callbacks = []
-
-        # Handle the case where the autosave is not provided
-        if self.autosave is None:
-            self.autosave = False
-
-        # Handle the case where the logging is not provided
-        if self.logging is None:
-            self.logging = False
-
         # Handle callbacks
         if callbacks is not None:
             for callback in self.callbacks:
                 if not callable(callback):
                     raise TypeError("Callback must be callable.")
 
         # Handle autosave
@@ -150,19 +135,17 @@
         # Handle stopping condition
         if stopping_condition is not None:
             if stopping_condition_args is None:
                 stopping_condition_args = {}
             self.stopping_condition_args = stopping_condition_args
             self.stopping_condition = stopping_condition
 
-    # @abstractmethod
     def communicate(self):
         """Communicate with the swarm through the orchestrator, protocols, and the universal communication layer"""
 
-    # @abstractmethod
     def run(self):
         """Run the swarm"""
         ...
 
     def __call__(
         self,
         task,
@@ -182,104 +165,101 @@
         except Exception as error:
             logger.error(f"Error running {self.__class__.__name__}")
             raise error
 
     def step(self):
         """Step the swarm"""
 
-    # @abstractmethod
-    def add_agent(self, agent: agent):
+    def add_agent(self, agent: AgentType):
         """Add a agent to the swarm"""
+        self.agents.append(agent)
 
-    # @abstractmethod
-    def remove_agent(self, agent: agent):
+    def add_agents(self, agents: List[AgentType]):
+        """Add a list of agents to the swarm"""
+        self.agents.extend(agents)
+
+    def add_agent_by_id(self, agent_id: str):
+        """Add a agent to the swarm by id"""
+        agent = self.get_agent_by_id(agent_id)
+        self.add_agent(agent)
+
+    def remove_agent(self, agent: AgentType):
         """Remove a agent from the swarm"""
+        self.agents.remove(agent)
+
+    def get_agent_by_name(self, name: str):
+        """Get a agent by name"""
+        for agent in self.agents:
+            if agent.name == name:
+                return agent
+
+    def reset_all_agents(self):
+        """Resets the state of all agents."""
+        for agent in self.agents:
+            agent.reset()
 
-    # @abstractmethod
-    def broadcast(self, message: str, sender: Optional[agent] = None):
+    def broadcast(self, message: str, sender: Optional[AgentType] = None):
         """Broadcast a message to all agents"""
 
-    # @abstractmethod
     def reset(self):
         """Reset the swarm"""
 
-    # @abstractmethod
     def plan(self, task: str):
         """agents must individually plan using a workflow or pipeline"""
 
-    # @abstractmethod
     def direct_message(
         self,
         message: str,
-        sender: agent,
-        recipient: agent,
+        sender: AgentType,
+        recipient: AgentType,
     ):
         """Send a direct message to a agent"""
 
-    # @abstractmethod
-    def autoscaler(self, num_agents: int, agent: [agent]):
+    def autoscaler(self, num_agents: int, agent: List[AgentType]):
         """Autoscaler that acts like kubernetes for autonomous agents"""
 
-    # @abstractmethod
-    def get_agent_by_id(self, id: str) -> agent:
+    def get_agent_by_id(self, id: str) -> AgentType:
         """Locate a agent by id"""
 
-    # @abstractmethod
-    def get_agent_by_name(self, name: str) -> agent:
-        """Locate a agent by name"""
-
-    # @abstractmethod
-    def assign_task(self, agent: agent, task: Any) -> Dict:
+    def assign_task(self, agent: AgentType, task: Any) -> Dict:
         """Assign a task to a agent"""
 
-    # @abstractmethod
-    def get_all_tasks(self, agent: agent, task: Any):
+    def get_all_tasks(self, agent: AgentType, task: Any):
         """Get all tasks"""
 
-    # @abstractmethod
     def get_finished_tasks(self) -> List[Dict]:
         """Get all finished tasks"""
 
-    # @abstractmethod
     def get_pending_tasks(self) -> List[Dict]:
         """Get all pending tasks"""
 
-    # @abstractmethod
-    def pause_agent(self, agent: agent, agent_id: str):
+    def pause_agent(self, agent: AgentType, agent_id: str):
         """Pause a agent"""
 
-    # @abstractmethod
-    def resume_agent(self, agent: agent, agent_id: str):
+    def resume_agent(self, agent: AgentType, agent_id: str):
         """Resume a agent"""
 
-    # @abstractmethod
-    def stop_agent(self, agent: agent, agent_id: str):
+    def stop_agent(self, agent: AgentType, agent_id: str):
         """Stop a agent"""
 
-    # @abstractmethod
-    def restart_agent(self, agent: agent):
+    def restart_agent(self, agent: AgentType):
         """Restart agent"""
 
-    # @abstractmethod
     def scale_up(self, num_agent: int):
         """Scale up the number of agents"""
 
-    # @abstractmethod
     def scale_down(self, num_agent: int):
         """Scale down the number of agents"""
 
-    # @abstractmethod
     def scale_to(self, num_agent: int):
         """Scale to a specific number of agents"""
 
-    # @abstractmethod
-    def get_all_agents(self) -> List[agent]:
+    def get_all_agents(self) -> List[AgentType]:
         """Get all agents"""
 
-    # @abstractmethod
     def get_swarm_size(self) -> int:
         """Get the size of the swarm"""
 
     # #@abstractmethod
     def get_swarm_status(self) -> Dict:
         """Get the status of the swarm"""
 
@@ -357,17 +337,15 @@
     def run_async(self, task: Optional[str] = None, *args, **kwargs):
         """Run the swarm asynchronously
 
         Args:
             task (Optional[str], optional): _description_. Defaults to None.
         """
         loop = asyncio.get_event_loop()
-        result = loop.run_until_complete(
-            self.arun(task, *args, **kwargs)
-        )
+        result = loop.run_until_complete(self.arun(task, *args, **kwargs))
         return result
 
     def run_batch_async(self, tasks: List[str], *args, **kwargs):
         """Run the swarm asynchronously
 
         Args:
             task (Optional[str], optional): _description_. Defaults to None.
@@ -487,15 +465,14 @@
         with ThreadPoolExecutor() as executor:
             responses = executor.map(
                 lambda agent: agent(task, *args, **kwargs),
                 self.agents,
             )
         return list(responses)
 
-    # @abstractmethod
     def add_swarm_entry(self, swarm):
         """
         Add the information of a joined Swarm to the registry.
 
         Args:
             swarm (SwarmManagerBase): Instance of SwarmManagerBase representing the joined Swarm.
 
@@ -529,17 +506,15 @@
         """
         Retrieve the information the Agents which have joined the registry.
 
         Returns:
             Agent: Instance of Agent representing the retrieved Agent, or None if not found.
         """
 
-    def join_swarm(
-        self, from_entity: Agent | Agent, to_entity: Agent
-    ):
+    def join_swarm(self, from_entity: Agent | Agent, to_entity: Agent):
         """
         Add a relationship between a Swarm and an Agent or other Swarm to the registry.
 
         Args:
             from (Agent | SwarmManagerBase): Instance of Agent or SwarmManagerBase representing the source of the relationship.
         """
```

### Comparing `swarms-4.8.2/swarms/structs/base_workflow.py` & `swarms-4.8.7/swarms/structs/base_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Any, Dict, List, Optional
 
 from termcolor import colored
 
 from swarms.structs.agent import Agent
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 from swarms.structs.task import Task
 from swarms.utils.loguru_logger import logger
 
 
 class BaseWorkflow(BaseStructure):
     """
     Base class for workflows.
@@ -64,17 +64,15 @@
             ValueError: If neither task nor tasks are provided.
         """
         if task:
             self.task_pool.append(task)
         elif tasks:
             self.task_pool.extend(tasks)
         else:
-            raise ValueError(
-                "You must provide a task or a list of tasks"
-            )
+            raise ValueError("You must provide a task or a list of tasks")
 
     def add_agent(self, agent: Agent, *args, **kwargs):
         return self.agent_pool(agent)
 
     def run(self):
         """
         Abstract method to run the workflow.
@@ -118,31 +116,25 @@
         """
         Returns the results of each task in the workflow.
 
         Returns:
             Dict[str, Any]: The results of each task in the workflow
         """
         try:
-            return {
-                task.description: task.result for task in self.tasks
-            }
+            return {task.description: task.result for task in self.tasks}
         except Exception as error:
             print(
-                colored(
-                    f"Error getting task results: {error}", "red"
-                ),
+                colored(f"Error getting task results: {error}", "red"),
             )
 
     def remove_task(self, task: str) -> None:
         """Remove tasks from sequential workflow"""
         try:
             self.tasks = [
-                task
-                for task in self.tasks
-                if task.description != task
+                task for task in self.tasks if task.description != task
             ]
         except Exception as error:
             print(
                 colored(
                     f"Error removing task from workflow: {error}",
                     "red",
                 ),
@@ -173,17 +165,15 @@
         """
         try:
             for task in self.tasks:
                 if task.description == task:
                     task.kwargs.update(updates)
                     break
             else:
-                raise ValueError(
-                    f"Task {task} not found in workflow."
-                )
+                raise ValueError(f"Task {task} not found in workflow.")
         except Exception as error:
             print(
                 colored(
                     f"Error updating task in workflow: {error}", "red"
                 ),
             )
 
@@ -210,17 +200,15 @@
         """
         try:
             for task in self.tasks:
                 if task.description == task:
                     self.tasks.remove(task)
                     break
             else:
-                raise ValueError(
-                    f"Task {task} not found in workflow."
-                )
+                raise ValueError(f"Task {task} not found in workflow.")
         except Exception as error:
             print(
                 colored(
                     f"Error deleting task from workflow: {error}",
                     "red",
                 ),
             )
@@ -295,17 +283,15 @@
             print(
                 colored(
                     f"Error adding objective to workflow: {error}",
                     "red",
                 )
             )
 
-    def load_workflow_state(
-        self, filepath: str = None, **kwargs
-    ) -> None:
+    def load_workflow_state(self, filepath: str = None, **kwargs) -> None:
         """
         Loads the workflow state from a json file and restores the workflow state.
 
         Args:
             filepath (str): The path to load the workflow state from.
 
         Examples:
```

### Comparing `swarms-4.8.2/swarms/structs/block_wrapper.py` & `swarms-4.8.7/swarms/structs/block_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/blocksdict.py` & `swarms-4.8.7/swarms/structs/blocks_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional
 
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 
 
 class BlocksDict(BaseStructure):
     """
     A class representing a dictionary of blocks.
 
     Args:
```

### Comparing `swarms-4.8.2/swarms/structs/blockslist.py` & `swarms-4.8.7/swarms/structs/blocks_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, List, Optional
 
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 
 
 class BlocksList(BaseStructure):
     """
     A class representing a list of blocks.
 
     Args:
@@ -98,23 +98,19 @@
     def get_by_type(self, type: str):
         return [block for block in self.blocks if block.type == type]
 
     def get_by_id(self, id: str):
         return [block for block in self.blocks if block.id == id]
 
     def get_by_parent(self, parent: str):
-        return [
-            block for block in self.blocks if block.parent == parent
-        ]
+        return [block for block in self.blocks if block.parent == parent]
 
     def get_by_parent_id(self, parent_id: str):
         return [
-            block
-            for block in self.blocks
-            if block.parent_id == parent_id
+            block for block in self.blocks if block.parent_id == parent_id
         ]
 
     def get_by_parent_name(self, parent_name: str):
         return [
             block
             for block in self.blocks
             if block.parent_name == parent_name
```

### Comparing `swarms-4.8.2/swarms/structs/company.py` & `swarms-4.8.7/swarms/structs/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     Represents a company with a hierarchical organizational structure.
     """
 
     org_chart: List[List[Agent]]
     shared_instructions: str = None
     ceo: Optional[Agent] = None
     agents: List[Agent] = field(default_factory=list)
-    agent_interactions: Dict[str, List[str]] = field(
-        default_factory=dict
-    )
+    agent_interactions: Dict[str, List[str]] = field(default_factory=dict)
     history: Conversation = field(default_factory=Conversation)
 
     def __post_init__(self):
         self._parse_org_chart(self.org_chart)
 
     def add(self, agent: Agent) -> None:
         """
@@ -42,17 +40,15 @@
                 raise ValueError(
                     f"Agent with id {agent.id} already exists in the"
                     " company."
                 )
             self.agents.append(agent)
 
         except Exception as error:
-            logger.error(
-                f"[ERROR][CLASS: Company][METHOD: add] {error}"
-            )
+            logger.error(f"[ERROR][CLASS: Company][METHOD: add] {error}")
             raise error
 
     def get(self, agent_name: str) -> Agent:
         """
         Retrieves an agent from the company by name.
 
         Args:
@@ -69,17 +65,15 @@
                 if agent.name == agent_name:
                     return agent
             raise ValueError(
                 f"Agent with name {agent_name} does not exist in the"
                 " company."
             )
         except Exception as error:
-            logger.error(
-                f"[ERROR][CLASS: Company][METHOD: get] {error}"
-            )
+            logger.error(f"[ERROR][CLASS: Company][METHOD: get] {error}")
             raise error
 
     def remove(self, agent: Agent) -> None:
         """
         Removes an agent from the company.
 
         Args:
@@ -114,17 +108,15 @@
                         raise ValueError("1 CEO is only allowed")
                     self.ceo = node
                     self.add(node)
 
                 elif isinstance(node, list):
                     for agent in node:
                         if not isinstance(agent, Agent):
-                            raise ValueError(
-                                "Invalid agent in org chart"
-                            )
+                            raise ValueError("Invalid agent in org chart")
                         self.add(agent)
 
                     for i, agent in enumerate(node):
                         if i == len(node) - 1:
                             continue
 
                         for other_agent in node[i + 1]:
@@ -149,17 +141,15 @@
             agent2 (Agent): The second agent involved in the interaction.
 
         Returns:
             None
         """
         if agent1.ai_name not in self.agents_interactions:
             self.agents_interactions[agent1.ai_name] = []
-        self.agents_interactions[agent1.ai_name].append(
-            agent2.ai_name
-        )
+        self.agents_interactions[agent1.ai_name].append(agent2.ai_name)
 
     def run(self):
         """
         Run the company
         """
         for (
             agent_name,
```

### Comparing `swarms-4.8.2/swarms/structs/concurrent_workflow.py` & `swarms-4.8.7/swarms/structs/concurrent_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import concurrent.futures
 from dataclasses import dataclass, field
 from typing import Callable, Dict, List, Optional
 
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 from swarms.structs.task import Task
 from swarms.utils.logger import logger
 
 
 @dataclass
 class ConcurrentWorkflow(BaseStructure):
     """
@@ -31,17 +31,15 @@
     >>> workflow.tasks
     """
 
     task_pool: List[Dict] = field(default_factory=list)
     max_loops: int = 1
     max_workers: int = 5
     autosave: bool = False
-    saved_state_filepath: Optional[str] = (
-        "runs/concurrent_workflow.json"
-    )
+    saved_state_filepath: Optional[str] = "runs/concurrent_workflow.json"
     print_results: bool = False
     return_results: bool = False
     use_processes: bool = False
     stopping_condition: Optional[Callable] = None
 
     def add(self, task: Task = None, tasks: List[Task] = None):
         """Adds a task to the workflow.
@@ -85,17 +83,15 @@
             ) as executor:
                 futures = {
                     executor.submit(task.execute): task
                     for task in self.task_pool
                 }
                 results = []
 
-                for future in concurrent.futures.as_completed(
-                    futures
-                ):
+                for future in concurrent.futures.as_completed(futures):
                     task = futures[future]
                     try:
                         result = future.result()
                         if self.print_results:
                             logger.info(f"Task {task}: {result}")
                         if self.return_results:
                             results.append(result)
```

### Comparing `swarms-4.8.2/swarms/structs/conversation.py` & `swarms-4.8.7/swarms/structs/conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import json
 from typing import Optional
 
 from termcolor import colored
 
 from swarms.memory.base_db import AbstractDatabase
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 from typing import Any
 
 
 class Conversation(BaseStructure):
     """
     A class structure to represent a conversation in a chatbot. This class is used to store the conversation history.
     And, it can be used to save the conversation history to a file, load the conversation history from a file, and
@@ -79,19 +79,19 @@
         self.autosave = autosave
         self.save_filepath = save_filepath
         self.conversation_history = []
         self.tokenizer = tokenizer
         self.context_length = context_length
 
         # If system prompt is not None, add it to the conversation history
-        if self.system_prompt:
-            self.add("system", self.system_prompt)
+        if self.system_prompt is not None:
+            self.add("System: ", self.system_prompt)
 
         # If tokenizer then truncate
-        if tokenizer:
+        if tokenizer is not None:
             self.truncate_memory_with_tokenizer()
 
     def add(self, role: str, content: str, *args, **kwargs):
         """Add a message to the conversation history
 
         Args:
             role (str): The role of the speaker
@@ -335,17 +335,15 @@
 
     def delete_from_database(self, *args, **kwargs):
         """Delete the conversation history from the database"""
         self.database.delete("conversation")
 
     def update_from_database(self, *args, **kwargs):
         """Update the conversation history from the database"""
-        self.database.update(
-            "conversation", self.conversation_history
-        )
+        self.database.update("conversation", self.conversation_history)
 
     def get_from_database(self, *args, **kwargs):
         """Get the conversation history from the database"""
         return self.database.get("conversation")
 
     def execute_query_from_database(self, query, *args, **kwargs):
         """Execute a query on the database"""
```

### Comparing `swarms-4.8.2/swarms/structs/debate.py` & `swarms-4.8.7/swarms/structs/debate.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,15 @@
         self.moderator = self.players[2]
 
     def init_agents(self):
         # start: set meta prompt
         self.affirmative.system_prompt(
             self.save_file["player_meta_prompt"]
         )
-        self.negative.system_prompt(
-            self.save_file["player_meta_prompt"]
-        )
+        self.negative.system_prompt(self.save_file["player_meta_prompt"])
         self.moderator.system_prompt(
             self.save_file["moderator_meta_prompt"]
         )
 
         # start: first round debate, state opinions
         print("===== Debate Round-1 =====\n")
         self.affirmative.add_message_to_memory(
@@ -187,22 +185,18 @@
             10: "tenth",
         }
         return dct[num]
 
     def save_file_to_json(self, id):
         now = datetime.now()
         current_time = now.strftime("%Y-%m-%d_%H:%M:%S")
-        save_file_path = os.path.join(
-            self.save_file_dir, f"{id}.json"
-        )
+        save_file_path = os.path.join(self.save_file_dir, f"{id}.json")
 
         self.save_file["end_time"] = current_time
-        json_str = json.dumps(
-            self.save_file, ensure_ascii=False, indent=4
-        )
+        json_str = json.dumps(self.save_file, ensure_ascii=False, indent=4)
         with open(save_file_path, "w") as f:
             f.write(json_str)
 
     def broadcast(self, msg: str):
         """Broadcast a message to all players.
         Typical use is for the host to announce public information
```

### Comparing `swarms-4.8.2/swarms/structs/document.py` & `swarms-4.8.7/swarms/structs/document.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/graph_workflow.py` & `swarms-4.8.7/swarms/structs/graph_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 
 
 class GraphWorkflow(BaseStructure):
     """
     Represents a graph-based workflow structure.
 
     Attributes:
@@ -122,23 +122,19 @@
 
         Raises:
             ValueError: If the source node or any of the target nodes do not exist in the graph.
         """
         if from_node in self.graph:
             for condition_value, to_node in edge_dict.items():
                 if to_node in self.graph:
-                    self.graph[from_node]["edges"][
-                        to_node
-                    ] = condition
+                    self.graph[from_node]["edges"][to_node] = condition
                 else:
                     raise ValueError("Node does not exist in graph")
         else:
-            raise ValueError(
-                f"Node {from_node} does not exist in graph"
-            )
+            raise ValueError(f"Node {from_node} does not exist in graph")
 
     def run(self):
         """
         Runs the workflow and returns the graph.
 
         Returns:
             dict: The graph representing the nodes and edges.
@@ -156,17 +152,15 @@
         Args:
             node_name (_type_): _description_
 
         Raises:
             ValueError: _description_
         """
         if node_name not in self.graph:
-            raise ValueError(
-                f"Node {node_name} does not exist in graph"
-            )
+            raise ValueError(f"Node {node_name} does not exist in graph")
 
     def _check_nodes_exist(self, from_node, to_node):
         """
         Checks if the given from_node and to_node exist in the graph.
 
         Args:
             from_node: The starting node of the edge.
```

### Comparing `swarms-4.8.2/swarms/structs/groupchat.py` & `swarms-4.8.7/swarms/structs/groupchat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from dataclasses import dataclass
 from typing import Dict, List
 
+
 from swarms.structs.agent import Agent
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class GroupChat:
@@ -47,16 +48,15 @@
         raise ValueError(
             f"No agent found with a name contained in '{name}'."
         )
 
     def next_agent(self, agent: Agent) -> Agent:
         """Return the next agent in the list."""
         return self.agents[
-            (self.agent_names.index(agent.name) + 1)
-            % len(self.agents)
+            (self.agent_names.index(agent.name) + 1) % len(self.agents)
         ]
 
     def select_speaker_msg(self):
         """Return the message for selecting the next speaker."""
         return f"""
         You are in a role play game. The following roles are available:
         {self._participant_roles()}.
@@ -118,21 +118,20 @@
             messages (List[Dict]): _description_
 
         Returns:
             str: _description_
         """
         formatted_messages = []
         for message in messages:
-            formatted_message = (
-                f"'{message['role']}:{message['content']}"
-            )
+            formatted_message = f"'{message['role']}:{message['content']}"
             formatted_messages.append(formatted_message)
         return "\n".join(formatted_messages)
 
 
+@dataclass
 class GroupChatManager:
     """
     GroupChatManager
 
     Args:
         groupchat: GroupChat
         selector: Agent
@@ -141,17 +140,16 @@
     >>> from swarms import GroupChatManager
     >>> from swarms.structs.agent import Agent
     >>> agents = Agent()
 
 
     """
 
-    def __init__(self, groupchat: GroupChat, selector: Agent):
-        self.groupchat = groupchat
-        self.selector = selector
+    groupchat: GroupChat
+    selector: Agent
 
     def __call__(self, task: str):
         """Call 'GroupChatManager' instance as a function.
 
         Args:
             task (str): _description_
```

### Comparing `swarms-4.8.2/swarms/structs/long_swarm.py` & `swarms-4.8.7/swarms/structs/long_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/majority_voting.py` & `swarms-4.8.7/swarms/structs/majority_voting.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,17 +161,15 @@
 
         self.conversation = Conversation(
             time_enabled=True, *args, **kwargs
         )
 
         # If autosave is enabled, save the conversation to a file
         if self.autosave:
-            create_file(
-                str(self.conversation), "majority_voting.json"
-            )
+            create_file(str(self.conversation), "majority_voting.json")
 
         # Log the agents
         logger.info("Initializing majority voting system")
         # Length of agents
         logger.info(f"Number of agents: {len(self.agents)}")
         logger.info(
             "Agents:"
@@ -220,15 +218,13 @@
             message["content"]
             for message in self.conversation.conversation_history
             if message["role"] == "agent"
         ]
 
         # If an output parser is provided, parse the responses
         if self.output_parser is not None:
-            majority_vote = self.output_parser(
-                responses, *args, **kwargs
-            )
+            majority_vote = self.output_parser(responses, *args, **kwargs)
         else:
             majority_vote = majority_voting(responses)
 
         # Return the majority vote
         return majority_vote
```

### Comparing `swarms-4.8.2/swarms/structs/message_pool.py` & `swarms-4.8.7/swarms/structs/message_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,15 @@
         self.show_names = show_names
         self.autosave = autosave
 
         self.messages = []
 
         logger.info("MessagePool initialized")
         logger.info(f"Number of agents: {len(agents)}")
-        logger.info(
-            f"Agents: {[agent.agent_name for agent in agents]}"
-        )
+        logger.info(f"Agents: {[agent.agent_name for agent in agents]}")
         logger.info(f"moderator: {moderator.agent_name} is available")
         logger.info(f"Number of turns: {turns}")
 
     def add(
         self,
         agent: Agent,
         content: str,
@@ -184,17 +182,15 @@
             turn (int): The turn number.
 
         Returns:
             List[Dict]: The list of visible messages.
         """
         # Get the messages before the current turn
         prev_messages = [
-            message
-            for message in self.messages
-            if message["turn"] < turn
+            message for message in self.messages if message["turn"] < turn
         ]
 
         visible_messages = []
         for message in prev_messages:
             if (
                 message["visible_to"] == "all"
                 or agent.agent_name in message["visible_to"]
```

### Comparing `swarms-4.8.2/swarms/structs/meta_system_prompt.py` & `swarms-4.8.7/swarms/structs/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/model_parallizer.py` & `swarms-4.8.7/swarms/structs/model_parallizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,15 @@
             print(response)
 
     def concurrent_run(self, task: str) -> List[str]:
         """Synchronously run the task on all llms and collect responses"""
         try:
             with ThreadPoolExecutor() as executor:
                 future_to_llm = {
-                    executor.submit(llm, task): llm
-                    for llm in self.llms
+                    executor.submit(llm, task): llm for llm in self.llms
                 }
                 responses = []
                 for future in as_completed(future_to_llm):
                     try:
                         responses.append(future.result())
                     except Exception as error:
                         print(
```

### Comparing `swarms-4.8.2/swarms/structs/multi_agent_collab.py` & `swarms-4.8.7/swarms/structs/multi_agent_collab.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List
 
 import tenacity
 from langchain.output_parsers import RegexParser
 
 from swarms.structs.agent import Agent
 from swarms.utils.logger import logger
+from swarms.structs.base_swarm import BaseSwarm
 
 
 # utils
 class BidOutputParser(RegexParser):
     def get_format_instructions(self) -> str:
         return (
             "Your response should be an integrater delimited by"
@@ -20,15 +21,15 @@
 
 bid_parser = BidOutputParser(
     regex=r"<(\d+)>", output_keys=["bid"], default_output_key="bid"
 )
 
 
 # main
-class MultiAgentCollaboration:
+class MultiAgentCollaboration(BaseSwarm):
     """
     Multi-agent collaboration class.
 
     Attributes:
         agents (List[Agent]): The agents in the collaboration.
         selection_function (callable): The function that selects the next speaker.
             Defaults to select_next_speaker.
@@ -90,46 +91,38 @@
         agents: List[Agent],
         selection_function: callable = None,
         max_iters: int = 10,
         autosave: bool = True,
         saved_file_path_name: str = "multi_agent_collab.json",
         stopping_token: str = "<DONE>",
         logging: bool = True,
+        *args,
+        **kwargs,
     ):
+        super().__init__(*args, **kwargs)
         self.agents = agents
         self.select_next_speaker = selection_function
         self._step = 0
         self.max_iters = max_iters
         self.autosave = autosave
         self.saved_file_path_name = saved_file_path_name
         self.stopping_token = stopping_token
         self.results = []
         self.logger = logger
         self.logging = logging
 
-    def reset(self):
-        """Resets the state of all agents."""
-        for agent in self.agents:
-            agent.reset()
-
     def inject(self, name: str, message: str):
         """Injects a message into the multi-agent collaboration."""
         for agent in self.agents:
             agent.run(f"Name {name} and message: {message}")
         self._step += 1
 
-    def inject_agent(self, agent: Agent):
-        """Injects an agent into the multi-agent collaboration."""
-        self.agents.append(agent)
-
     def step(self) -> tuple[str, str]:
         """Steps through the multi-agent collaboration."""
-        speaker_idx = self.select_next_speaker(
-            self._step, self.agents
-        )
+        speaker_idx = self.select_next_speaker(self._step, self.agents)
         speaker = self.agents[speaker_idx]
         message = speaker.send()
         message = speaker.send()
 
         for receiver in self.agents:
             receiver.receive(speaker.name, message)
         self._step += 1
@@ -166,17 +159,15 @@
     ) -> int:
         """Selects the next speaker."""
         bids = []
         for agent in agents:
             bid = self.ask_for_bid(agent)
             bids.append(bid)
         max_value = max(bids)
-        max_indices = [
-            i for i, x in enumerate(bids) if x == max_value
-        ]
+        max_indices = [i for i, x in enumerate(bids) if x == max_value]
         idx = random.choice(max_indices)
         return idx
 
     @tenacity.retry(
         stop=tenacity.stop_after_attempt(10),
         wait=tenacity.wait_none(),
         retry=tenacity.retry_if_exception_type(ValueError),
@@ -213,62 +204,20 @@
         # => director selects next speaker
         if step % 2 == 1:
             idx = 0
         else:
             idx = director.select_next_speaker() + 1
         return idx
 
-    # def run(self, task: str):
-    #     """Runs the multi-agent collaboration."""
-    #     for step in range(self.max_iters):
-    #         speaker_idx = self.select_next_speaker_roundtable(step, self.agents)
-    #         speaker = self.agents[speaker_idx]
-    #         result = speaker.run(task)
-    #         self.results.append({"agent": speaker, "response": result})
-
-    #         if self.autosave:
-    #             self.save_state()
-    #         if result == self.stopping_token:
-    #             break
-    #     return self.results
-
-    # def run(self, task: str):
-    #     for _ in range(self.max_iters):
-    #         for step, agent, in enumerate(self.agents):
-    #             result = agent.run(task)
-    #             self.results.append({"agent": agent, "response": result})
-    #             if self.autosave:
-    #                 self.save_state()
-    #             if result == self.stopping_token:
-    #                 break
-
-    #     return self.results
-
-    # def run(self, task: str):
-    #     conversation = task
-    #     for _ in range(self.max_iters):
-    #         for agent in self.agents:
-    #             result = agent.run(conversation)
-    #             self.results.append({"agent": agent, "response": result})
-    #             conversation = result
-
-    #             if self.autosave:
-    #                 self.save()
-    #             if result == self.stopping_token:
-    #                 break
-    #     return self.results
-
     def run(self, task: str):
         conversation = task
         for _ in range(self.max_iters):
             for agent in self.agents:
                 result = agent.run(conversation)
-                self.results.append(
-                    {"agent": agent, "response": result}
-                )
+                self.results.append({"agent": agent, "response": result})
                 conversation += result
 
                 if self.autosave:
                     self.save_state()
                 if result == self.stopping_token:
                     break
 
@@ -308,20 +257,7 @@
     def __repr__(self):
         return (
             f"MultiAgentCollaboration(agents={self.agents},"
             f" selection_function={self.select_next_speaker},"
             f" max_iters={self.max_iters}, autosave={self.autosave},"
             f" saved_file_path_name={self.saved_file_path_name})"
         )
-
-    def performance(self):
-        """Tracks and reports the performance of each agent"""
-        performance_data = {}
-        for agent in self.agents:
-            performance_data[agent.name] = (
-                agent.get_performance_metrics()
-            )
-        return performance_data
-
-    def set_interaction_rules(self, rules):
-        """Sets the interaction rules for each agent"""
-        self.interaction_rules = rules
```

### Comparing `swarms-4.8.2/swarms/structs/multi_process_workflow.py` & `swarms-4.8.7/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/multi_threaded_workflow.py` & `swarms-4.8.7/swarms/structs/multi_threaded_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,15 @@
         Executes the tasks in the thread pool and returns the results.
 
         Returns:
             List: The list of results from the executed tasks.
 
         """
         results = []
-        with ThreadPoolExecutor(
-            max_workers=self.max_workers
-        ) as executor:
+        with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
             future_to_task = {}
             for _ in range(self.tasks_queue.qsize()):
                 priority_task = self.tasks_queue.get_nowait()
                 future = executor.submit(priority_task.task.execute)
                 future_to_task[future] = (
                     priority_task.task,
                     0,
@@ -123,17 +121,15 @@
                                 f"Attempt {attempt+1} failed for task"
                                 f" {task}: {str(e)}"
                             ),
                             exc_info=True,
                         )
                         if attempt + 1 < self.retry_attempts:
                             # Retry the task
-                            retry_future = executor.submit(
-                                task.execute
-                            )
+                            retry_future = executor.submit(task.execute)
                             future_to_task[retry_future] = (
                                 task,
                                 attempt + 1,
                             )
                         else:
                             logging.error(
                                 f"Task {task} failed after"
@@ -148,11 +144,9 @@
 
         Args:
             task (Task): The task whose result needs to be autosaved.
             result: The result of the task.
 
         """
         with self.lock:
-            logging.info(
-                f"Autosaving result for task {task}: {result}"
-            )
+            logging.info(f"Autosaving result for task {task}: {result}")
             # Actual autosave logic goes here
```

### Comparing `swarms-4.8.2/swarms/structs/nonlinear_workflow.py` & `swarms-4.8.7/swarms/structs/nonlinear_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 from swarms.structs.task import Task
 from swarms.utils.logger import logger  # noqa: F401
 
 
 class NonlinearWorkflow(BaseStructure):
     """
     Represents a Directed Acyclic Graph (DAG) workflow.
```

### Comparing `swarms-4.8.2/swarms/structs/plan.py` & `swarms-4.8.7/swarms/structs/plan.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/rearrange.py` & `swarms-4.8.7/swarms/structs/rearrange.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,31 +55,26 @@
                         " must have exactly one '->'."
                     )
                     return False
 
                 source_name, destinations_str = parts
                 source = self.find_agent_by_name(source_name)
                 if source is None:
-                    logging.error(
-                        f"Source agent {source_name} not found."
-                    )
+                    logging.error(f"Source agent {source_name} not found.")
                     return False
 
                 destinations_names = destinations_str.split()
                 for dest_name in destinations_names:
                     dest = self.find_agent_by_name(dest_name)
                     if dest is None:
                         logging.error(
-                            f"Destination agent {dest_name} not"
-                            " found."
+                            f"Destination agent {dest_name} not" " found."
                         )
                         return False
-                    self.flows[source.agent_name].append(
-                        dest.agent_name
-                    )
+                    self.flows[source.agent_name].append(dest.agent_name)
             return True
         except Exception as e:
             logger.error(f"Error: {e}")
             raise e
 
     def self_find_agen_by_name(self, name: str):
         """
@@ -120,28 +115,25 @@
 
                 for source, destinations in self.flows.items():
                     for dest in destinations:
                         dest_agent = self.self_find_agen_by_name(dest)
                         task = tasks.get(dest, task)
 
                         if self.custom_prompt:
-                            dest_agent.run(
-                                f"{task} {self.custom_prompt}"
-                            )
+                            dest_agent.run(f"{task} {self.custom_prompt}")
                         else:
                             dest_agent.run(f"{task} (from {source})")
             # else:
             #     raise ValueError(
             #         "No agents provided. Please provide agents to"
             #         " execute the task."
             #     )
         except Exception as e:
             logger.error(
-                f"Error: {e} try again by providing agents and"
-                " pattern"
+                f"Error: {e} try again by providing agents and" " pattern"
             )
             raise e
 
 
 # # Example usage
 # try:
 #     agents = [
```

### Comparing `swarms-4.8.2/swarms/structs/recursive_workflow.py` & `swarms-4.8.7/swarms/structs/recursive_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import List
 
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 from swarms.structs.task import Task
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class RecursiveWorkflow(BaseStructure):
@@ -35,17 +35,15 @@
         stop_token: str = "<DONE>",
         stopping_conditions: callable = None,
     ):
         self.stop_token = stop_token
         self.stopping_conditions = stopping_conditions
         self.task_pool = []
 
-        assert (
-            self.stop_token is not None
-        ), "stop_token cannot be None"
+        assert self.stop_token is not None, "stop_token cannot be None"
 
     def add(self, task: Task = None, tasks: List[Task] = None):
         """Adds a task to the workflow.
 
         Args:
             task (Task): _description_
             tasks (List[Task]): _description_
@@ -76,16 +74,13 @@
         Returns:
             None
         """
         try:
             for task in self.task_pool:
                 while True:
                     result = task.run()
-                    if (
-                        result is not None
-                        and self.stop_token in result
-                    ):
+                    if result is not None and self.stop_token in result:
                         break
                     print(f"{result}")
         except Exception as error:
             logger.warning(f"[ERROR][RecursiveWorkflow] {error}")
             raise error
```

### Comparing `swarms-4.8.2/swarms/structs/schemas.py` & `swarms-4.8.7/swarms/structs/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,16 +56,15 @@
     )
 
 
 class StepInput(BaseModel):
     step: Any = Field(
         ...,
         description=(
-            "Input parameters for the task step. Any value is"
-            " allowed."
+            "Input parameters for the task step. Any value is" " allowed."
         ),
         examples=['{\n"file_to_refactor": "models.py"\n}'],
     )
 
 
 class StepOutput(BaseModel):
     step: Any = Field(
@@ -78,17 +77,15 @@
     )
 
 
 class TaskRequestBody(BaseModel):
     input: str | None = Field(
         None,
         description="Input prompt for the task.",
-        examples=[
-            "Write the words you receive to the file 'output.txt'."
-        ],
+        examples=["Write the words you receive to the file 'output.txt'."],
     )
     additional_input: TaskInput | None = None
 
 
 class Task(TaskRequestBody):
     task_id: str = Field(
         ...,
@@ -118,44 +115,52 @@
 
 class Status(Enum):
     created = "created"
     running = "running"
     completed = "completed"
 
 
-class Step(StepRequestBody):
+class Step(BaseModel):
     task_id: str = Field(
         ...,
         description="The ID of the task this step belongs to.",
         examples=["50da533e-3904-4401-8a07-c49adf88b5eb"],
     )
-    step_id: str = Field(
+    step_id: int = Field(
         ...,
         description="The ID of the task step.",
         examples=["6bb1801a-fd80-45e8-899a-4dd723cc602e"],
     )
     name: str | None = Field(
         None,
         description="The name of the task step.",
         examples=["Write to file"],
     )
-    status: Status = Field(
-        ..., description="The status of the task step."
-    )
     output: str | None = Field(
         None,
         description="Output of the task step.",
         examples=[
             "I am going to use the write_to_file command and write"
             " Washington to a file called output.txt"
             " <write_to_file('output.txt', 'Washington')"
         ],
     )
-    additional_output: StepOutput | None = None
     artifacts: list[Artifact] = Field(
         [],
         description="A list of artifacts that the step has produced.",
     )
-    is_last: bool | None = Field(
-        False,
-        description="Whether this is the last step in the task.",
+    max_loops: int = Field(
+        1,
+        description="The maximum number of times to run the workflow.",
+    )
+
+
+class ManySteps(BaseModel):
+    task_id: str = Field(
+        ...,
+        description="The ID of the task this step belongs to.",
+        examples=["50da533e-3904-4401-8a07-c49adf88b5eb"],
+    )
+    steps: list[Step] = Field(
+        [],
+        description="A list of task steps.",
     )
```

### Comparing `swarms-4.8.2/swarms/structs/sequential_workflow.py` & `swarms-4.8.7/swarms/structs/sequential_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,17 +40,15 @@
     """
 
     name: str = None
     description: str = None
     task_pool: List[Task] = None
     max_loops: int = 1
     autosave: bool = False
-    saved_state_filepath: Optional[str] = (
-        "sequential_workflow_state.json"
-    )
+    saved_state_filepath: Optional[str] = "sequential_workflow_state.json"
     restore_state_filepath: Optional[str] = None
     dashboard: bool = False
     agents: List[Agent] = None
 
     def __post_init__(self):
         self.conversation = Conversation(
             system_prompt=f"Objective: {self.description}",
@@ -91,44 +89,14 @@
             out = agent(str(self.description))
             self.conversation.add(agent.agent_name, out)
             prompt = self.conversation.return_history_as_string()
             out = agent(prompt)
 
         return out
 
-        # try:
-        #     # If the agent is a Task instance, we include the task in kwargs for Agent.run()
-        #     # Append the task to the task_pool list
-        #     if task:
-        #         self.task_pool.append(task)
-        #         logger.info(
-        #             f"[INFO][SequentialWorkflow] Added task {task} to"
-        #             " workflow"
-        #         )
-        #     elif tasks:
-        #         for task in tasks:
-        #             self.task_pool.append(task)
-        #             logger.info(
-        #                 "[INFO][SequentialWorkflow] Added task"
-        #                 f" {task} to workflow"
-        #             )
-        #     else:
-        #         if task and tasks is not None:
-        #             # Add the task and list of tasks to the task_pool at the same time
-        #             self.task_pool.append(task)
-        #             for task in tasks:
-        #                 self.task_pool.append(task)
-
-        # except Exception as error:
-        #     logger.error(
-        #         colored(
-        #             f"Error adding task to workflow: {error}", "red"
-        #         ),
-        #     )
-
     def reset_workflow(self) -> None:
         """Resets the workflow by clearing the results of each task."""
         try:
             for task in self.task_pool:
                 task.result = None
                 logger.info(
                     f"[INFO][SequentialWorkflow] Reset task {task} in"
@@ -144,22 +112,19 @@
         Returns the results of each task in the workflow.
 
         Returns:
             Dict[str, Any]: The results of each task in the workflow
         """
         try:
             return {
-                task.description: task.result
-                for task in self.task_pool
+                task.description: task.result for task in self.task_pool
             }
         except Exception as error:
             logger.error(
-                colored(
-                    f"Error getting task results: {error}", "red"
-                ),
+                colored(f"Error getting task results: {error}", "red"),
             )
 
     def remove_task(self, task: Task) -> None:
         """Remove task_pool from sequential workflow"""
         try:
             self.task_pool.remove(task)
             logger.info(
```

### Comparing `swarms-4.8.2/swarms/structs/sermon_swarm.py` & `swarms-4.8.7/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/stackoverflow_swarm.py` & `swarms-4.8.7/swarms/structs/stackoverflow_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/step.py` & `swarms-4.8.7/swarms/structs/step.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/swarm_net.py` & `swarms-4.8.7/swarms/structs/swarm_net.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import queue
 import threading
 from typing import List, Optional
 
 # from fastapi import FastAPI
 
 from swarms.structs.agent import Agent
-from swarms.structs.base import BaseStructure
+from swarms.structs.base_structure import BaseStructure
 from swarms.utils.logger import logger  # noqa: F401
 
 
 class SwarmNetwork(BaseStructure):
     """
     SwarmNetwork class
 
@@ -128,23 +128,19 @@
         >>> from swarms.structs.agent import Agent
         >>> from swarms.structs.swarm_net import SwarmNetwork
         >>> agent = Agent()
         >>> swarm = SwarmNetwork(agents=[agent])
         >>> swarm.add_task("task")
 
         """
-        self.logger.info(
-            f"Adding task {task} to queue asynchronously"
-        )
+        self.logger.info(f"Adding task {task} to queue asynchronously")
         try:
             # Add task to queue asynchronously with asyncio
             loop = asyncio.get_running_loop()
-            await loop.run_in_executor(
-                None, self.task_queue.put, task
-            )
+            await loop.run_in_executor(None, self.task_queue.put, task)
             self.logger.info(f"Task {task} added to queue")
         except Exception as error:
             print(
                 f"Error adding task to queue: {error} try again with"
                 " a new task"
             )
             raise error
@@ -267,17 +263,15 @@
         Args:
             agent_id (_type_): _description_
         """
         self.logger.info(f"Removing agent {agent_id} from pool")
         try:
             # Remove agent from pool asynchronously with asyncio
             loop = asyncio.get_running_loop()
-            await loop.run_in_executor(
-                None, self.remove_agent, agent_id
-            )
+            await loop.run_in_executor(None, self.remove_agent, agent_id)
         except Exception as error:
             print(f"Error removing agent from pool: {error}")
             raise error
 
     def scale_up(self, num_agents: int = 1):
         """Scale up the agent pool
```

### Comparing `swarms-4.8.2/swarms/structs/swarming_architectures.py` & `swarms-4.8.7/swarms/structs/swarming_architectures.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,17 +218,15 @@
         for agent in agents:
             receive_tasks.append(
                 agent.receive_message(sender.ai_name, task)
             )
 
         await asyncio.gather(*receive_tasks)
     except Exception as error:
-        logger.error(
-            f"[ERROR][CLASS: Agent][METHOD: broadcast] {error}"
-        )
+        logger.error(f"[ERROR][CLASS: Agent][METHOD: broadcast] {error}")
         raise error
 
 
 async def one_to_one(
     sender: Agent,
     receiver: Agent,
     task: str,
@@ -246,11 +244,9 @@
 
     Returns:
         None
     """
     try:
         await receiver.receive_message(sender.ai_name, task)
     except Exception as error:
-        logger.error(
-            f"[ERROR][CLASS: Agent][METHOD: one_to_one] {error}"
-        )
+        logger.error(f"[ERROR][CLASS: Agent][METHOD: one_to_one] {error}")
         raise error
```

### Comparing `swarms-4.8.2/swarms/structs/task.py` & `swarms-4.8.7/swarms/structs/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,34 +77,30 @@
         >>> from swarms.models import OpenAIChat
         >>> agent = Agent(llm=OpenAIChat(openai_api_key=""), max_loops=1, dashboard=False)
         >>> task = Task(description="What's the weather in miami", agent=agent)
         >>> task.execute()
         >>> task.result
 
         """
-        logger.info(
-            f"[INFO][Task] Executing task: {self.description}"
-        )
+        logger.info(f"[INFO][Task] Executing task: {self.description}")
         task = self.description
         try:
             if isinstance(self.agent, Agent):
                 if self.condition is None or self.condition():
                     self.result = self.agent.run(
                         task=task,
                         *args,
                         **kwargs,
                     )
                     self.history.append(self.result)
 
                     if self.action is not None:
                         self.action()
             else:
-                self.result = self.agent.run(
-                    *self.args, **self.kwargs
-                )
+                self.result = self.agent.run(*self.args, **self.kwargs)
 
             self.history.append(self.result)
         except Exception as error:
             logger.error(f"[ERROR][Task] {error}")
 
     def run(self, *args, **kwargs):
         self.execute(*args, **kwargs)
@@ -224,28 +220,24 @@
             for task in context:
                 description = (
                     task.description
                     if task.description is not None
                     else ""
                 )
 
-                result = (
-                    task.result if task.result is not None else ""
-                )
+                result = task.result if task.result is not None else ""
 
                 # Add the context of the task to the conversation
                 new_context.add(
                     task.agent.agent_name, f"{description} {result}"
                 )
 
         elif task:
             description = (
-                task.description
-                if task.description is not None
-                else ""
+                task.description if task.description is not None else ""
             )
             result = task.result if task.result is not None else ""
             new_context.add(
                 task.agent.agent_name, f"{description} {result}"
             )
 
         prompt = new_context.return_history_as_string()
```

### Comparing `swarms-4.8.2/swarms/structs/task_queue_base.py` & `swarms-4.8.7/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/structs/team.py` & `swarms-4.8.7/swarms/structs/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         tasks (Optional[List[Task]]): List of tasks.
         agents (Optional[List[Agent]]): List of agents in this Team.
         architecture (str): Architecture that the Team will follow. Default is "sequential".
         verbose (bool): Verbose mode for the Agent Execution. Default is False.
         config (Optional[Json]): Configuration of the Team. Default is None.
     """
 
-    tasks: Optional[List[Task]] = Field(
-        None, description="List of tasks"
-    )
+    tasks: Optional[List[Task]] = Field(None, description="List of tasks")
     agents: Optional[List[Agent]] = Field(
         None, description="List of agents in this Team."
     )
     architecture = Field(
         description="architecture that the Team will follow.",
         default="sequential",
     )
@@ -47,17 +45,15 @@
             raise ValueError(
                 "Either agents and task need to be set or config."
             )
 
         if values.get("config"):
             config = json.loads(values.get("config"))
             if not config.get("agents") or not config.get("tasks"):
-                raise ValueError(
-                    "Config should have agents and tasks."
-                )
+                raise ValueError("Config should have agents and tasks.")
 
             values["agents"] = [
                 Agent(**agent) for agent in config["agents"]
             ]
 
             tasks = []
             for task in config["tasks"]:
```

### Comparing `swarms-4.8.2/swarms/structs/utils.py` & `swarms-4.8.7/swarms/structs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
         task (str, optional): _description_. Defaults to None.
 
     Returns:
         Dict[str, Any]: _description_
     """
     tasks = {}
     for line in task.split("\n"):
-        if line.startswith("<agent_id>") and line.endwith(
-            "</agent_id>"
-        ):
+        if line.startswith("<agent_id>") and line.endwith("</agent_id>"):
             agent_id, task = line[10:-11].split("><")
             tasks[agent_id] = task
     return tasks
 
 
 def find_agent_by_id(
     agent_id: str = None, agents: List[Agent] = None, *args, **kwargs
@@ -85,34 +83,30 @@
     # Check if the token is in the text
     if token in text:
         return True
     else:
         return False
 
 
-def extract_key_from_json(
-    json_response: str, key: str
-) -> Optional[str]:
+def extract_key_from_json(json_response: str, key: str) -> Optional[str]:
     """
     Extract a specific key from a JSON response.
 
     Args:
         json_response (str): The JSON response to parse.
         key (str): The key to extract.
 
     Returns:
         Optional[str]: The value of the key if it exists, None otherwise.
     """
     response_dict = json.loads(json_response)
     return response_dict.get(key)
 
 
-def extract_tokens_from_text(
-    text: str, tokens: List[str]
-) -> List[str]:
+def extract_tokens_from_text(text: str, tokens: List[str]) -> List[str]:
     """
     Extract a list of tokens from a text response.
 
     Args:
         text (str): The text to parse.
         tokens (List[str]): The tokens to extract.
```

### Comparing `swarms-4.8.2/swarms/telemetry/__init__.py` & `swarms-4.8.7/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-4.8.7/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/telemetry/check_update.py` & `swarms-4.8.7/swarms/telemetry/check_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,8 @@
     # Fetch the latest version from the PyPI API
     response = requests.get("https://pypi.org/pypi/swarms/json")
     latest_version = response.json()["info"]["version"]
 
     # Get the current version using pkg_resources
     current_version = pkg_resources.get_distribution("swarms").version
 
-    return version.parse(latest_version) > version.parse(
-        current_version
-    )
+    return version.parse(latest_version) > version.parse(current_version)
```

### Comparing `swarms-4.8.2/swarms/telemetry/log_all.py` & `swarms-4.8.7/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/telemetry/sys_info.py` & `swarms-4.8.7/swarms/telemetry/sys_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,15 @@
         swarms_verison_cmd = (
             subprocess.check_output(["swarms", "--version"])
             .decode()
             .split()[1]
         )
     except Exception as e:
         swarms_verison_cmd = str(e)
-    swarms_verison_pkg = pkg_resources.get_distribution(
-        "swarms"
-    ).version
+    swarms_verison_pkg = pkg_resources.get_distribution("swarms").version
     swarms_verison = swarms_verison_cmd, swarms_verison_pkg
     return swarms_verison
 
 
 def get_os_version():
     return platform.platform()
```

### Comparing `swarms-4.8.2/swarms/telemetry/user_utils.py` & `swarms-4.8.7/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/tools/code_executor.py` & `swarms-4.8.7/swarms/tools/code_executor.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/tools/exec_tool.py` & `swarms-4.8.7/swarms/tools/exec_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import Dict, List, NamedTuple
 
 from langchain.schema import BaseOutputParser
 from pydantic import ValidationError
 
 from swarms.tools.tool import BaseTool
 
+from swarms.utils.loguru_logger import logger
+
 
 class AgentAction(NamedTuple):
     """Action returned by AgentOutputParser."""
 
     name: str
     args: Dict
 
@@ -55,17 +57,15 @@
             preprocessed_text = preprocess_json_input(text)
             try:
                 parsed = json.loads(preprocessed_text, strict=False)
             except Exception:
                 return AgentAction(
                     name="ERROR",
                     args={
-                        "error": (
-                            f"Could not parse invalid json: {text}"
-                        )
+                        "error": (f"Could not parse invalid json: {text}")
                     },
                 )
         try:
             return AgentAction(
                 name=parsed["command"]["name"],
                 args=parsed["command"]["args"],
             )
@@ -93,26 +93,30 @@
     Returns:
         str: The result of the command execution.
     """
     output_parser = AgentOutputParser()
     # Get command name and arguments
     action = output_parser.parse(text)
     tools = {t.name: t for t in tools}
+
+    logger.info(f"Tools available: {tools}")
+
     if action.name == stop_token:
         return action.args["response"]
     if action.name in tools:
         tool = tools[action.name]
         try:
             # Check if multiple tools are used
             tool_names = [name for name in tools if name in text]
             if len(tool_names) > 1:
                 # Execute tools concurrently
                 with concurrent.futures.ThreadPoolExecutor() as executor:
                     futures = []
                     for tool_name in tool_names:
+                        logger.info(f"Executing tool: {tool_name}")
                         futures.append(
                             executor.submit(
                                 tools[tool_name].run, action.args
                             )
                         )
 
                     # Wait for all futures to complete
```

### Comparing `swarms-4.8.2/swarms/tools/format_tools.py` & `swarms-4.8.7/swarms/tools/format_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,15 @@
             response = response[len(prompt) :]
             response = response.strip().rstrip(".")
             self.debug("[generate_number]", response)
             try:
                 return float(response)
             except ValueError:
                 if iterations > 3:
-                    raise ValueError(
-                        "Failed to generate a valid number"
-                    )
+                    raise ValueError("Failed to generate a valid number")
 
                 return self.generate_number(
                     temperature=self.temperature * 1.3,
                     iterations=iterations + 1,
                 )
         elif self.llm:
             prompt = self.get_prompt()
@@ -139,17 +137,15 @@
             response = response[len(prompt) :]
             response = response.strip().rstrip(".")
             self.debug("[generate_number]", response)
             try:
                 return float(response)
             except ValueError:
                 if iterations > 3:
-                    raise ValueError(
-                        "Failed to generate a valid number"
-                    )
+                    raise ValueError("Failed to generate a valid number")
 
                 return self.generate_number(
                     temperature=self.temperature * 1.3,
                     iterations=iterations + 1,
                 )
 
         elif self.llm and self.model:
@@ -165,28 +161,22 @@
         if self.model:
             prompt = self.get_prompt()
             self.debug("[generate_boolean]", prompt, is_prompt=True)
 
             input_tensor = self.tokenizer.encode(
                 prompt, return_tensors="pt"
             )
-            output = self.model.forward(
-                input_tensor.to(self.model.device)
-            )
+            output = self.model.forward(input_tensor.to(self.model.device))
             logits = output.logits[0, -1]
 
             # todo: this assumes that "true" and "false" are both tokenized to a single token
             # this is probably not true for all tokenizers
             # this can be fixed by looking at only the first token of both "true" and "false"
-            true_token_id = self.tokenizer.convert_tokens_to_ids(
-                "true"
-            )
-            false_token_id = self.tokenizer.convert_tokens_to_ids(
-                "false"
-            )
+            true_token_id = self.tokenizer.convert_tokens_to_ids("true")
+            false_token_id = self.tokenizer.convert_tokens_to_ids("false")
 
             result = logits[true_token_id] > logits[false_token_id]
 
             self.debug("[generate_boolean]", result)
 
             return result.item()
 
@@ -223,16 +213,15 @@
             )
 
             # Some models output the prompt as part of the response
             # This removes the prompt from the response if it is present
             if (
                 len(response[0]) >= len(input_tokens[0])
                 and (
-                    response[0][: len(input_tokens[0])]
-                    == input_tokens
+                    response[0][: len(input_tokens[0])] == input_tokens
                 ).all()
             ):
                 response = response[0][len(input_tokens[0]) :]
             if response.shape[0] == 1:
                 response = response[0]
 
             response = self.tokenizer.decode(
@@ -253,16 +242,15 @@
             response = self.llm(prompt)
 
             # Some models output the prompt as part of the response
             # This removes the prompt from the response if it is present
             if (
                 len(response[0]) >= len(input_tokens[0])
                 and (
-                    response[0][: len(input_tokens[0])]
-                    == input_tokens
+                    response[0][: len(input_tokens[0])] == input_tokens
                 ).all()
             ):
                 response = response[0][len(input_tokens[0]) :]
             if response.shape[0] == 1:
                 response = response[0]
 
             self.debug("[generate_string]", "|" + response + "|")
@@ -316,17 +304,15 @@
             new_obj = {}
             if key:
                 obj[key] = new_obj
             else:
                 obj.append(new_obj)
             return self.generate_object(schema["properties"], new_obj)
         else:
-            raise ValueError(
-                f"Unsupported schema type: {schema_type}"
-            )
+            raise ValueError(f"Unsupported schema type: {schema_type}")
 
     def generate_array(
         self, item_schema: Dict[str, Any], obj: Dict[str, Any]
     ) -> list:
         if self.model:
             for _ in range(self.max_array_length):
                 # forces array to have at least one element
@@ -393,17 +379,15 @@
                     break
 
             return obj
 
     def get_prompt(self):
         template = """{prompt}\nOutput result in the following JSON schema format:\n{schema}\nResult: {progress}"""
         progress = json.dumps(self.value)
-        gen_marker_index = progress.find(
-            f'"{self.generation_marker}"'
-        )
+        gen_marker_index = progress.find(f'"{self.generation_marker}"')
         if gen_marker_index != -1:
             progress = progress[:gen_marker_index]
         else:
             raise ValueError("Failed to find generation marker")
 
         prompt = template.format(
             prompt=self.prompt,
```

### Comparing `swarms-4.8.2/swarms/tools/function_util.py` & `swarms-4.8.7/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/tools/logits_processor.py` & `swarms-4.8.7/swarms/tools/logits_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,15 @@
     LogitsWarper,
     PreTrainedTokenizer,
     StoppingCriteria,
 )
 
 
 class StringStoppingCriteria(StoppingCriteria):
-    def __init__(
-        self, tokenizer: PreTrainedTokenizer, prompt_length: int
-    ):
+    def __init__(self, tokenizer: PreTrainedTokenizer, prompt_length: int):
         self.tokenizer = tokenizer
         self.prompt_length = prompt_length
 
     def __call__(
         self,
         input_ids: torch.LongTensor,
         _,
```

### Comparing `swarms-4.8.2/swarms/tools/tool_utils.py` & `swarms-4.8.7/swarms/tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/README.md` & `swarms-4.8.7/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/__init__.py` & `swarms-4.8.7/swarms/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,62 @@
 from swarms.utils.class_args_wrapper import print_class_parameters
-from swarms.utils.code_interpreter import SubprocessCodeInterpreter
-from swarms.utils.csv_and_pandas import (
-    csv_to_dataframe,
-    dataframe_to_strings,
-)
+from swarms.tools.code_interpreter import SubprocessCodeInterpreter
 from swarms.utils.data_to_text import (
     csv_to_text,
     data_to_text,
     json_to_text,
     txt_to_text,
 )
-from swarms.utils.device_checker_cuda import check_device
 from swarms.utils.download_img import download_img_from_url
-from swarms.utils.download_weights_from_url import (
-    download_weights_from_url,
-)
 from swarms.utils.exponential_backoff import ExponentialBackoffMixin
 from swarms.utils.file_processing import (
     load_json,
     sanitize_file_path,
     zip_workspace,
     create_file_in_folder,
     zip_folders,
 )
 from swarms.utils.find_img_path import find_image_path
 from swarms.utils.json_output_parser import JsonOutputParser
 from swarms.utils.llm_metrics_decorator import metrics_decorator
-from swarms.utils.load_model_torch import load_model_torch
 from swarms.utils.markdown_message import display_markdown_message
-from swarms.utils.math_eval import math_eval
-from swarms.utils.pandas_to_str import dataframe_to_text
+from swarms.tools.math_eval import math_eval
 from swarms.utils.parse_code import extract_code_from_markdown
 from swarms.utils.pdf_to_text import pdf_to_text
-from swarms.utils.prep_torch_model_inference import (
-    prep_torch_inference,
-)
 from swarms.utils.remove_json_whitespace import (
     remove_whitespace_from_json,
     remove_whitespace_from_yaml,
 )
 from swarms.utils.save_logs import parse_log_file
-
-# from swarms.utils.supervision_visualizer import MarkVisualizer
 from swarms.utils.try_except_wrapper import try_except_wrapper
 from swarms.utils.yaml_output_parser import YamlOutputParser
 from swarms.utils.concurrent_utils import execute_concurrently
 
 
 __all__ = [
     "print_class_parameters",
     "SubprocessCodeInterpreter",
-    "csv_to_dataframe",
-    "dataframe_to_strings",
     "csv_to_text",
     "data_to_text",
     "json_to_text",
     "txt_to_text",
-    "check_device",
     "download_img_from_url",
-    "download_weights_from_url",
     "ExponentialBackoffMixin",
     "load_json",
     "sanitize_file_path",
     "zip_workspace",
     "create_file_in_folder",
     "zip_folders",
     "find_image_path",
     "JsonOutputParser",
     "metrics_decorator",
-    "load_model_torch",
     "display_markdown_message",
     "math_eval",
-    "dataframe_to_text",
     "extract_code_from_markdown",
     "pdf_to_text",
-    "prep_torch_inference",
     "remove_whitespace_from_json",
     "remove_whitespace_from_yaml",
     "parse_log_file",
     "try_except_wrapper",
     "YamlOutputParser",
     "execute_concurrently",
 ]
```

### Comparing `swarms-4.8.2/swarms/utils/apa.py` & `swarms-4.8.7/swarms/utils/apa.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,15 @@
     content: str = ""
     thought: str = ""
     plan: List[str] = field(default_factory=lambda: [])
     criticism: str = ""
     tool_name: str = ""
     tool_input: dict = field(default_factory=lambda: {})
 
-    tool_output_status: ToolCallStatus = (
-        ToolCallStatus.ToolCallSuccess
-    )
+    tool_output_status: ToolCallStatus = ToolCallStatus.ToolCallSuccess
     tool_output: str = ""
 
     def to_json(self):
         try:
             tool_output = json.loads(self.tool_output)
         except:
             tool_output = self.tool_output
@@ -120,17 +118,15 @@
             "tool_output": tool_output,
         }
 
 
 @dataclass
 class userQuery:
     task: str
-    additional_information: List[str] = field(
-        default_factory=lambda: []
-    )
+    additional_information: List[str] = field(default_factory=lambda: [])
     refine_prompt: str = field(default_factory=lambda: "")
 
     def print_self(self):
         lines = [self.task]
         for info in self.additional_information:
             lines.append(f"- {info}")
         return "\n".join(lines)
```

### Comparing `swarms-4.8.2/swarms/utils/check_function_result.py` & `swarms-4.8.7/swarms/utils/check_function_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,17 +94,15 @@
     signal.signal(signal.SIGALRM, signal_handler)
     try:
         yield
     finally:
         signal.setitimer(signal.ITIMER_REAL, 0)
 
 
-def check_function_result(
-    python_code: str, timeout: float = 5.0
-) -> Dict:
+def check_function_result(python_code: str, timeout: float = 5.0) -> Dict:
     """
     Evaluates the functional correctness of a completion by running the test
     suite provided in the problem.
 
     :param completion_id: an optional completion ID so we can match
         the results later even if execution finishes asynchronously.
     """
```

### Comparing `swarms-4.8.2/swarms/utils/class_args_wrapper.py` & `swarms-4.8.7/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/code_interpreter.py` & `swarms-4.8.7/swarms/tools/code_interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         done (threading.Event): An event that is set when the subprocess is done running code.
 
     Example:
     """
 
     def __init__(
         self,
-        start_cmd: str = "",
+        start_cmd: str = "python3",
         debug_mode: bool = False,
     ):
         self.process = None
         self.output_queue = queue.Queue()
         self.done = threading.Event()
 
     def detect_active_line(self, line):
@@ -135,16 +135,15 @@
                 if retry_count != 0:
                     # For UX, I like to hide this if it happens once. Obviously feels better to not see errors
                     # Most of the time it doesn't matter, but we should figure out why it happens frequently with:
                     # applescript
                     yield {"output": traceback.format_exc()}
                     yield {
                         "output": (
-                            "Retrying..."
-                            f" ({retry_count}/{max_retries})"
+                            "Retrying..." f" ({retry_count}/{max_retries})"
                         )
                     }
                     yield {"output": "Restarting process."}
 
                 self.start_process()
 
                 retry_count += 1
```

### Comparing `swarms-4.8.2/swarms/utils/concurrent_utils.py` & `swarms-4.8.7/swarms/utils/concurrent_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,13 @@
             results[index] = e
 
     with concurrent.futures.ThreadPoolExecutor(
         max_workers=max_workers
     ) as executor:
         futures = []
         for i, (fn, args, kwargs) in enumerate(callable_functions):
-            futures.append(
-                executor.submit(worker, fn, args, kwargs, i)
-            )
+            futures.append(executor.submit(worker, fn, args, kwargs, i))
 
         # Wait for all threads to complete
         concurrent.futures.wait(futures)
 
     return results
```

### Comparing `swarms-4.8.2/swarms/utils/data_to_text.py` & `swarms-4.8.7/swarms/utils/data_to_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     with open(file) as file:
         data = file.read()
     return data
 
 
 def md_to_text(file):
     if not os.path.exists(file):
-        raise FileNotFoundError(
-            f"No such file or directory: '{file}'"
-        )
+        raise FileNotFoundError(f"No such file or directory: '{file}'")
     with open(file) as file:
         data = file.read()
     return data
 
 
 def data_to_text(file):
     """
```

### Comparing `swarms-4.8.2/swarms/utils/decorators.py` & `swarms-4.8.7/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/disable_logging.py` & `swarms-4.8.7/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/download_img.py` & `swarms-4.8.7/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/execute_futures.py` & `swarms-4.8.7/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/execution_sandbox.py` & `swarms-4.8.7/swarms/tools/execution_sandbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         # This is just a placeholder and would require additional setup and dependencies
         # exec_in_docker(new_code)
         out = exec(new_code)
         return out
         # logging.info("Code executed successfully.")
     except Exception:
         error_message = traceback.format_exc()
-        logging.error(
-            "Code execution failed. Error: %s", error_message
-        )
+        logging.error("Code execution failed. Error: %s", error_message)
 
     # Return the new code and the error message
     return out, error_message
 
 
 def execute_code_in_sandbox(code: str, language: str = "python"):
     """
```

### Comparing `swarms-4.8.2/swarms/utils/exponential_backoff.py` & `swarms-4.8.7/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/fetch_init_params.py` & `swarms-4.8.7/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/file_processing.py` & `swarms-4.8.7/swarms/utils/file_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     Ensure the output_filename does not have .zip extension as it's added by make_archive.
     """
     temp_dir = tempfile.mkdtemp()
     # Remove .zip if present in output_filename to avoid duplication
     base_output_path = os.path.join(
         temp_dir, output_filename.replace(".zip", "")
     )
-    zip_path = shutil.make_archive(
-        base_output_path, "zip", workspace_path
-    )
+    zip_path = shutil.make_archive(base_output_path, "zip", workspace_path)
     return zip_path  # make_archive already appends .zip
 
 
 def sanitize_file_path(file_path: str):
     """
     Cleans and sanitizes the file path to be valid for Windows.
     """
@@ -58,17 +56,15 @@
         file_path (str): The path to the file to be created.
     """
     with open(file_path, "w") as file:
         file.write(content)
     return file_path
 
 
-def create_file_in_folder(
-    folder_path: str, file_name: str, content: str
-):
+def create_file_in_folder(folder_path: str, file_name: str, content: str):
     """
     Creates a file in the specified folder with the given file name and content.
 
     Args:
         folder_path (str): The path of the folder where the file will be created.
         file_name (str): The name of the file to be created.
         content (str): The content to be written to the file.
```

### Comparing `swarms-4.8.2/swarms/utils/find_img_path.py` & `swarms-4.8.7/swarms/utils/find_img_path.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,11 +14,9 @@
     pattern = r"([A-Za-z]:\\[^:\n]*?\.(png|jpg|jpeg|PNG|JPG|JPEG))|(/[^:\n]*?\.(png|jpg|jpeg|PNG|JPG|JPEG))"
     matches = [
         match.group()
         for match in re.finditer(pattern, text)
         if match.group()
     ]
     matches += [match.replace("\\", "") for match in matches if match]
-    existing_paths = [
-        match for match in matches if os.path.exists(match)
-    ]
+    existing_paths = [match for match in matches if os.path.exists(match)]
     return max(existing_paths, key=len) if existing_paths else None
```

### Comparing `swarms-4.8.2/swarms/utils/function_calling_utils.py` & `swarms-4.8.7/swarms/tools/function_calling_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import concurrent.futures
 from typing import Any, Callable, Dict, List
 from inspect import iscoroutinefunction
 import asyncio
 
 
 # Helper function to run an asynchronous function in a synchronous way
-def run_async_function_in_sync(
-    func: Callable, *args, **kwargs
-) -> Any:
+def run_async_function_in_sync(func: Callable, *args, **kwargs) -> Any:
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     coroutine = func(*args, **kwargs)
     return loop.run_until_complete(coroutine)
 
 
 # Main omni function for parallel execution
```

### Comparing `swarms-4.8.2/swarms/utils/get_logger.py` & `swarms-4.8.7/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/json_output_parser.py` & `swarms-4.8.7/swarms/utils/json_output_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,17 +72,15 @@
         """Generate formatting instructions based on the Pydantic model schema.
 
         Returns:
             A string containing formatting instructions.
         """
         schema = self.pydantic_object.schema()
         reduced_schema = {
-            k: v
-            for k, v in schema.items()
-            if k not in ["title", "type"]
+            k: v for k, v in schema.items() if k not in ["title", "type"]
         }
         schema_str = json.dumps(reduced_schema, indent=4)
 
         format_instructions = (
             f"JSON Formatting Instructions:\n{schema_str}"
         )
         return format_instructions
```

### Comparing `swarms-4.8.2/swarms/utils/json_utils.py` & `swarms-4.8.7/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/jsonl_utils.py` & `swarms-4.8.7/swarms/utils/jsonl_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,17 +30,15 @@
     else:
         with open(filename) as fp:
             for line in fp:
                 if any(not x.isspace() for x in line):
                     yield json.loads(line)
 
 
-def write_jsonl(
-    filename: str, data: Iterable[Dict], append: bool = False
-):
+def write_jsonl(filename: str, data: Iterable[Dict], append: bool = False):
     """
     Write a list of dictionaries to a JSONL file.
 
     Args:
         filename (str): The path to the output file.
         data (Iterable[Dict]): The data to be written to the file.
         append (bool, optional): If True, append to an existing file.
```

### Comparing `swarms-4.8.2/swarms/utils/llm_metrics_decorator.py` & `swarms-4.8.7/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/logger.py` & `swarms-4.8.7/swarms/utils/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     def wrapper(*args, **kwargs):
         logger.debug(
             f"Calling function {func.__name__} with args {args} and"
             f" kwargs {kwargs}"
         )
         try:
             result = func(*args, **kwargs)
-            logger.debug(
-                f"Function {func.__name__} returned {result}"
-            )
+            logger.debug(f"Function {func.__name__} returned {result}")
             return result
         except Exception as e:
             logger.error(
                 f"Function {func.__name__} raised an exception: {e}"
             )
             raise
 
@@ -69,14 +67,12 @@
         Logs a message with the specified level, task, and message.
 
         Args:
             level (int): The logging level of the message.
             task (str): The task associated with the message.
             message (str): The message to be logged.
         """
-        timestamp = datetime.datetime.now().strftime(
-            "%d/%m/%y %H:%M:%S"
-        )
+        timestamp = datetime.datetime.now().strftime("%d/%m/%y %H:%M:%S")
         formatted_message = (
             f"[{timestamp}] {level:<8} {task}\n{' ' * 29}{message}"
         )
         Logger.logger.log(level, formatted_message)
```

### Comparing `swarms-4.8.2/swarms/utils/loggers.py` & `swarms-4.8.7/swarms/utils/loggers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 from colorama import Fore, Style
 
 from swarms.utils.apa import Action, ToolCallStatus
 
 
 # from autogpt.speech import say_text
 class JsonFileHandler(logging.FileHandler):
-    def __init__(
-        self, filename, mode="a", encoding=None, delay=False
-    ):
+    def __init__(self, filename, mode="a", encoding=None, delay=False):
         """
         Initializes a new instance of the class with the specified file name, mode, encoding, and delay settings.
 
         Parameters:
             filename (str): The name of the file to be opened.
             mode (str, optional): The mode in which the file is opened. Defaults to "a" (append).
             encoding (str, optional): The encoding used to read or write the file. Defaults to None.
@@ -84,17 +82,15 @@
         log_dir = os.path.join(this_files_dir_path, "../logs")
         if not os.path.exists(log_dir):
             os.makedirs(log_dir)
 
         log_file = "activity.log"
         error_file = "error.log"
 
-        console_formatter = AutoGptFormatter(
-            "%(title_color)s %(message)s"
-        )
+        console_formatter = AutoGptFormatter("%(title_color)s %(message)s")
 
         # Create a handler for console which simulate typing
         self.typing_console_handler = TypingConsoleHandler()
         # self.typing_console_handler = ConsoleHandler()
         self.typing_console_handler.setLevel(logging.INFO)
         self.typing_console_handler.setFormatter(console_formatter)
 
@@ -377,17 +373,15 @@
             transfer_enter = "<ENTER>"
             msg_transfered = str(msg).replace("\n", transfer_enter)
             transfer_space = "<4SPACE>"
             msg_transfered = str(msg_transfered).replace(
                 "    ", transfer_space
             )
             words = msg_transfered.split()
-            words = [
-                word.replace(transfer_enter, "\n") for word in words
-            ]
+            words = [word.replace(transfer_enter, "\n") for word in words]
             words = [
                 word.replace(transfer_space, "    ") for word in words
             ]
 
             for i, word in enumerate(words):
                 print(word, end="", flush=True)
                 if i < len(words) - 1:
@@ -484,59 +478,47 @@
     Parameters:
         action (Action): The Action object to print.
 
     Returns:
         None
     """
     if action.content != "":
-        logger.typewriter_log(
-            "content:", Fore.YELLOW, f"{action.content}"
-        )
-    logger.typewriter_log(
-        "Thought:", Fore.YELLOW, f"{action.thought}"
-    )
+        logger.typewriter_log("content:", Fore.YELLOW, f"{action.content}")
+    logger.typewriter_log("Thought:", Fore.YELLOW, f"{action.thought}")
     if len(action.plan) > 0:
         logger.typewriter_log(
             "Plan:",
             Fore.YELLOW,
         )
         for line in action.plan:
             line = line.lstrip("- ")
             logger.typewriter_log("- ", Fore.GREEN, line.strip())
-    logger.typewriter_log(
-        "Criticism:", Fore.YELLOW, f"{action.criticism}"
-    )
+    logger.typewriter_log("Criticism:", Fore.YELLOW, f"{action.criticism}")
 
 
 def print_action_tool(action: Action):
     """
     Prints the details of an action tool.
 
     Args:
         action (Action): The action object containing the tool details.
 
     Returns:
         None
     """
     logger.typewriter_log("Tool:", Fore.BLUE, f"{action.tool_name}")
-    logger.typewriter_log(
-        "Tool Input:", Fore.BLUE, f"{action.tool_input}"
-    )
+    logger.typewriter_log("Tool Input:", Fore.BLUE, f"{action.tool_input}")
 
-    output = (
-        action.tool_output if action.tool_output != "" else "None"
-    )
+    output = action.tool_output if action.tool_output != "" else "None"
     logger.typewriter_log("Tool Output:", Fore.BLUE, f"{output}")
 
     color = Fore.RED
     if action.tool_output_status == ToolCallStatus.ToolCallSuccess:
         color = Fore.GREEN
-    elif (
-        action.tool_output_status == ToolCallStatus.InputCannotParsed
-    ):
+    elif action.tool_output_status == ToolCallStatus.InputCannotParsed:
         color = Fore.YELLOW
 
     logger.typewriter_log(
         "Tool Call Status:",
         Fore.BLUE,
         f"{color}{action.tool_output_status.name}{Style.RESET_ALL}",
     )
```

### Comparing `swarms-4.8.2/swarms/utils/markdown_message.py` & `swarms-4.8.7/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/math_eval.py` & `swarms-4.8.7/swarms/tools/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/parse_code.py` & `swarms-4.8.7/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/pdf_to_text.py` & `swarms-4.8.7/swarms/utils/pdf_to_text.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,17 +32,15 @@
 
             # Iterate through each page and extract text
             for page in pdf_reader.pages:
                 text += page.extract_text() + "\n"
 
             return text
     except FileNotFoundError:
-        raise FileNotFoundError(
-            f"The file at {pdf_path} was not found."
-        )
+        raise FileNotFoundError(f"The file at {pdf_path} was not found.")
     except Exception as e:
         raise Exception(
             f"An error occurred while reading the PDF file: {e}"
         )
 
 
 # Example usage
```

### Comparing `swarms-4.8.2/swarms/utils/remove_json_whitespace.py` & `swarms-4.8.7/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/save_logs.py` & `swarms-4.8.7/swarms/utils/save_logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
     Raises:
         FileNotFoundError: If the log file does not exist.
         ValueError: If a log entry does not have the correct format.
     """
     # Check if the file exists
     if not os.path.exists(filename):
-        raise FileNotFoundError(
-            f"The file {filename} does not exist."
-        )
+        raise FileNotFoundError(f"The file {filename} does not exist.")
 
     log_entries = []
 
     with open(filename) as file:
         for line in file:
             parts = line.split(" - ")
             # Check if the log entry has the correct format
```

### Comparing `swarms-4.8.2/swarms/utils/serializable.py` & `swarms-4.8.7/swarms/utils/serializable.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,17 +101,15 @@
 
             secrets.update(this.lc_secrets)
             lc_kwargs.update(this.lc_attributes)
 
         # include all secrets, even if not specified in kwargs
         # as these secrets may be passed as an environment variable instead
         for key in secrets.keys():
-            secret_value = getattr(self, key, None) or lc_kwargs.get(
-                key
-            )
+            secret_value = getattr(self, key, None) or lc_kwargs.get(key)
             if secret_value is not None:
                 lc_kwargs.update({key: secret_value})
 
         return {
             "lc": 1,
             "type": "constructor",
             "id": [*self.lc_namespace, self.__class__.__name__],
```

### Comparing `swarms-4.8.2/swarms/utils/try_except_wrapper.py` & `swarms-4.8.7/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.8.2/swarms/utils/yaml_output_parser.py` & `swarms-4.8.7/swarms/utils/yaml_output_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,15 @@
         """Generate formatting instructions based on the Pydantic model schema.
 
         Returns:
             A string containing formatting instructions.
         """
         schema = self.pydantic_object.schema()
         reduced_schema = {
-            k: v
-            for k, v in schema.items()
-            if k not in ["title", "type"]
+            k: v for k, v in schema.items() if k not in ["title", "type"]
         }
         schema_str = json.dumps(reduced_schema, indent=4)
 
         format_instructions = (
             f"YAML Formatting Instructions:\n{schema_str}"
         )
         return format_instructions
```

### Comparing `swarms-4.8.2/setup.py` & `swarms-4.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,37 +17,36 @@
 {'': ['*']}
 
 install_requires = \
 ['Pillow==10.2.0',
  'accelerate==0.28.0',
  'asyncio>=3.4.3,<4.0',
  'backoff==2.2.1',
- 'einops==0.7.0',
- 'httpx==0.24.1',
+ 'docstring_parser==0.16',
  'langchain-community==0.0.29',
- 'langchain-core==0.1.33',
  'langchain-experimental==0.0.55',
  'loguru==0.7.2',
+ 'opencv-python>=4.9.0.80,<5.0.0.0',
  'psutil',
  'pydantic==2.6.4',
  'pypdf==4.1.0',
  'python-dotenv',
  'ratelimit==2.2.1',
- 'rich==13.5.2',
  'sentry-sdk',
  'tenacity==8.2.3',
  'toml',
  'torch>=2.1.1,<3.0',
- 'transformers>=4.39.0,<5.0.0']
+ 'transformers>=4.39.0,<5.0.0',
+ 'yaml']
 
 setup_kwargs = {
     'name': 'swarms',
-    'version': '4.8.2',
+    'version': '4.8.7',
     'description': 'Swarms - Pytorch',
-    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents are barely being deployd into production because of 5 suffocating challanges: short memory, single task threading, hallucinations, high cost, and lack of collaboration.  With Multi-agent collaboration, you can effectively eliminate all of these issues. Swarms provides you with simple, reliable, and agile primitives to build your own Swarm for your specific use case. Now, Swarms is being used in production by RBC, John Deere, and many AI startups. To learn more about the unparalled benefits about multi-agent collaboration check out this github repository for research papers or book a call with me!\n\n----\n\n## Install\n`pip3 install -U swarms`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, SequentialWorkflow\n\nload_dotenv()\n\n# Load the environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Initialize the language agent\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n# Initialize the agent with the language agent\nagent1 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent2 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent3 = Agent(llm=llm, max_loops=1)\n\n# Create the workflow\nworkflow = SequentialWorkflow(max_loops=1)\n\n# Add tasks to the workflow\nworkflow.add(\n    agent1,\n    "Generate a 10,000 word blog on health and wellness.",\n)\n\n# Suppose the next task takes the output of the first task as input\nworkflow.add(\n    agent2,\n    "Summarize the generated blog",\n)\n\n# Run the workflow\nworkflow.run()\n\n# Output the results\nfor task in workflow.tasks:\n    print(f"Task: {task.description}, Result: {task.result}")\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import AbstractLLM\n\nclass vLLMLM(AbstractLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships\n\n```python\nfrom swarms import Agent, Anthropic, AgentRearrange, \n\n## Initialize the workflow\nagent = Agent(\n    agent_name="t",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    system_prompt=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent2 = Agent(\n    agent_name="t1",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Summarize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent3 = Agent(\n    agent_name="t2",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Finalize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\n\n# Rearrange the agents\nrearrange = AgentRearrange(\n    agents=[agent, agent2, agent3],\n    verbose=True,\n    # custom_prompt="Summarize the transcript",\n)\n\n# Run the workflow on a task\nresults = rearrange(\n    # pattern="t -> t1, t2 -> t2",\n    pattern="t -> t1 -> t2",\n    default_task=(\n        "Generate a transcript for a YouTube video on what swarms"\n        " are!"\n    ),\n    t="Generate a transcript for a YouTube video on what swarms are!",\n    # t2="Summarize the transcript",\n    # t3="Finalize the transcript",\n)\n# print(results)\n\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
+    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups. For more information on the unparalleled benefits of multi-agent collaboration, check out this GitHub repository for research papers or schedule a call with me!\n\n----\n\n## Install\n`pip3 install -U swarms`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, SequentialWorkflow\n\nload_dotenv()\n\n# Load the environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Initialize the language agent\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n# Initialize the agent with the language agent\nagent1 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent2 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent3 = Agent(llm=llm, max_loops=1)\n\n# Create the workflow\nworkflow = SequentialWorkflow(max_loops=1)\n\n# Add tasks to the workflow\nworkflow.add(\n    agent1,\n    "Generate a 10,000 word blog on health and wellness.",\n)\n\n# Suppose the next task takes the output of the first task as input\nworkflow.add(\n    agent2,\n    "Summarize the generated blog",\n)\n\n# Run the workflow\nworkflow.run()\n\n# Output the results\nfor task in workflow.tasks:\n    print(f"Task: {task.description}, Result: {task.result}")\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import AbstractLLM\n\nclass vLLMLM(AbstractLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships\n\n```python\nfrom swarms import Agent, Anthropic, AgentRearrange, \n\n## Initialize the workflow\nagent = Agent(\n    agent_name="t",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    system_prompt=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent2 = Agent(\n    agent_name="t1",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Summarize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent3 = Agent(\n    agent_name="t2",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Finalize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\n\n# Rearrange the agents\nrearrange = AgentRearrange(\n    agents=[agent, agent2, agent3],\n    verbose=True,\n    # custom_prompt="Summarize the transcript",\n)\n\n# Run the workflow on a task\nresults = rearrange(\n    # pattern="t -> t1, t2 -> t2",\n    pattern="t -> t1 -> t2",\n    default_task=(\n        "Generate a transcript for a YouTube video on what swarms"\n        " are!"\n    ),\n    t="Generate a transcript for a YouTube video on what swarms are!",\n    # t2="Summarize the transcript",\n    # t3="Finalize the transcript",\n)\n# print(results)\n\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/swarms',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `swarms-4.8.2/PKG-INFO` & `swarms-4.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 4.8.2
+Version: 4.8.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
@@ -17,31 +17,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: Pillow (==10.2.0)
 Requires-Dist: accelerate (==0.28.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0)
 Requires-Dist: backoff (==2.2.1)
-Requires-Dist: einops (==0.7.0)
-Requires-Dist: httpx (==0.24.1)
+Requires-Dist: docstring_parser (==0.16)
 Requires-Dist: langchain-community (==0.0.29)
-Requires-Dist: langchain-core (==0.1.33)
 Requires-Dist: langchain-experimental (==0.0.55)
 Requires-Dist: loguru (==0.7.2)
+Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: psutil
 Requires-Dist: pydantic (==2.6.4)
 Requires-Dist: pypdf (==4.1.0)
 Requires-Dist: python-dotenv
 Requires-Dist: ratelimit (==2.2.1)
-Requires-Dist: rich (==13.5.2)
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity (==8.2.3)
 Requires-Dist: toml
 Requires-Dist: torch (>=2.1.1,<3.0)
 Requires-Dist: transformers (>=4.39.0,<5.0.0)
+Requires-Dist: yaml
 Project-URL: Documentation, https://swarms.apac.ai
 Project-URL: Repository, https://github.com/kyegomez/swarms
 Description-Content-Type: text/markdown
 
 ![Swarming banner icon](images/swarmslogobanner.png)
 
 <div align="center">
@@ -52,15 +51,15 @@
 
 [![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 </div>
 
-Individual agents are barely being deployd into production because of 5 suffocating challanges: short memory, single task threading, hallucinations, high cost, and lack of collaboration.  With Multi-agent collaboration, you can effectively eliminate all of these issues. Swarms provides you with simple, reliable, and agile primitives to build your own Swarm for your specific use case. Now, Swarms is being used in production by RBC, John Deere, and many AI startups. To learn more about the unparalled benefits about multi-agent collaboration check out this github repository for research papers or book a call with me!
+Individual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups. For more information on the unparalleled benefits of multi-agent collaboration, check out this GitHub repository for research papers or schedule a call with me!
 
 ----
 
 ## Install
 `pip3 install -U swarms`
 
 ---
```

