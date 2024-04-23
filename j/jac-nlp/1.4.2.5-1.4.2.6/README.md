# Comparing `tmp/jac_nlp-1.4.2.5.tar.gz` & `tmp/jac_nlp-1.4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_nlp-1.4.2.5.tar", last modified: Tue Jan  9 16:44:29 2024, max compression
+gzip compressed data, was "jac_nlp-1.4.2.6.tar", last modified: Tue Apr 23 19:42:44 2024, max compression
```

## Comparing `jac_nlp-1.4.2.5.tar` & `jac_nlp-1.4.2.6.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.959098 jac_nlp-1.4.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-01-09 16:44:29.959098 jac_nlp-1.4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33031 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.927098 jac_nlp-1.4.2.5/jac_nlp/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.931098 jac_nlp-1.4.2.5/jac_nlp/action_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/bi_enc_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/cl_summer_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/paraphraser_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/sbert_sim_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/sentiment_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/summarization_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/text_seg_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/tfm_ner_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/topic_ext_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/use_enc_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/action_configs/use_qa_action_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.931098 jac_nlp-1.4.2.5/jac_nlp/bi_enc/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/bi_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/poly_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/sent_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.931098 jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.931098 jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/test_bi_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.935098 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/train_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.935098 jac_nlp-1.4.2.5/jac_nlp/cl_summer/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/cl_summer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/cl_summer/cl_summer.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/cl_summer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.935098 jac_nlp-1.4.2.5/jac_nlp/cl_summer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/cl_summer/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.935098 jac_nlp-1.4.2.5/jac_nlp/cl_summer/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/cl_summer/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/cl_summer/tests/fixtures/cl_summer.jac
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/cl_summer/tests/test_cl_summer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.935098 jac_nlp-1.4.2.5/jac_nlp/dolly/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/dolly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/dolly/dolly.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/dolly/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.935098 jac_nlp-1.4.2.5/jac_nlp/gpt2/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/gpt2/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/gpt2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/gpt2/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.935098 jac_nlp-1.4.2.5/jac_nlp/llm/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/llm/dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/llm/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/paraphraser/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/config.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/paraphraser.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/paraphraser/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/paraphraser/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/tests/fixtures/paraphraser.jac
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/paraphraser/tests/test_paraphraser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/sbert_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/test_sbert_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/sentiment/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sentiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sentiment/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/sentiment/sentiment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/summarization/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/summarization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/summarization/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/summarization/summarization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.939098 jac_nlp-1.4.2.5/jac_nlp/text_seg/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/text_seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/text_seg/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/text_seg/text_seg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/entity_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/test_tfm_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tfm_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/utils/data_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/utils/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/tfm_ner/utils/train_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/topic_ext/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/topic_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/topic_ext/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/topic_ext/config.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/topic_ext/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/topic_ext/topic_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/use_enc/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_enc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.943098 jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/fixtures/use_enc.jac
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/test_use_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_enc/use_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.947098 jac_nlp-1.4.2.5/jac_nlp/use_qa/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_qa/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.947098 jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.947098 jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/fixtures/use_qa.jac
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/test_use_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/jac_nlp/use_qa/use_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:29.947098 jac_nlp-1.4.2.5/jac_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-01-09 16:44:29.000000 jac_nlp-1.4.2.5/jac_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-01-09 16:44:29.000000 jac_nlp-1.4.2.5/jac_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 16:44:29.000000 jac_nlp-1.4.2.5/jac_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-01-09 16:44:29.000000 jac_nlp-1.4.2.5/jac_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 16:44:29.000000 jac_nlp-1.4.2.5/jac_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 16:44:29.959098 jac_nlp-1.4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-09 16:44:11.000000 jac_nlp-1.4.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.748692 jac_nlp-1.4.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-23 19:42:44.748692 jac_nlp-1.4.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33031 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.716692 jac_nlp-1.4.2.6/jac_nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.720692 jac_nlp-1.4.2.6/jac_nlp/action_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/bi_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/cl_summer_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/paraphraser_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/sbert_sim_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/sentiment_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/summarization_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/text_seg_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/tfm_ner_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/topic_ext_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/use_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/action_configs/use_qa_action_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.720692 jac_nlp-1.4.2.6/jac_nlp/bi_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/bi_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/poly_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/sent_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.720692 jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.720692 jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/test_bi_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.720692 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/train_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.720692 jac_nlp-1.4.2.6/jac_nlp/cl_summer/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/cl_summer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/cl_summer/cl_summer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/cl_summer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/cl_summer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/cl_summer/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/cl_summer/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/cl_summer/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/cl_summer/tests/fixtures/cl_summer.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/cl_summer/tests/test_cl_summer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/dolly/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/dolly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/dolly/dolly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/dolly/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/gpt2/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/gpt2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/gpt2/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/llm/dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/llm/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/paraphraser/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/paraphraser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/paraphraser/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.724692 jac_nlp-1.4.2.6/jac_nlp/paraphraser/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/tests/fixtures/paraphraser.jac
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/paraphraser/tests/test_paraphraser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/sbert_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/test_sbert_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/sentiment/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sentiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sentiment/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/sentiment/sentiment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/summarization/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/summarization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/summarization/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/summarization/summarization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/text_seg/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/text_seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/text_seg/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/text_seg/text_seg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/entity_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.728692 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/test_tfm_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tfm_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/utils/data_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/utils/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/tfm_ner/utils/train_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/topic_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/topic_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/topic_ext/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/topic_ext/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/topic_ext/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/topic_ext/topic_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/use_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_enc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/fixtures/use_enc.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/test_use_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_enc/use_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/use_qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_qa/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.732692 jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.736692 jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/fixtures/use_qa.jac
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/test_use_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/jac_nlp/use_qa/use_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.736692 jac_nlp-1.4.2.6/jac_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-23 19:42:44.000000 jac_nlp-1.4.2.6/jac_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-23 19:42:44.000000 jac_nlp-1.4.2.6/jac_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:42:44.000000 jac_nlp-1.4.2.6/jac_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-23 19:42:44.000000 jac_nlp-1.4.2.6/jac_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:42:44.000000 jac_nlp-1.4.2.6/jac_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:42:44.748692 jac_nlp-1.4.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-23 19:42:33.000000 jac_nlp-1.4.2.6/setup.py
```

### Comparing `jac_nlp-1.4.2.5/PKG-INFO` & `jac_nlp-1.4.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jac_nlp
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
-Requires-Dist: jaseci==1.4.2.5
+Requires-Dist: jaseci==1.4.2.6
 Requires-Dist: pytest<7.1,>=7.0.1
 Requires-Dist: pytest-order<1.1,>=1.0.1
 Provides-Extra: all
 Requires-Dist: transformers>=4.25.1; extra == "all"
 Requires-Dist: beautifulsoup4<4.13.0,>=4.12.2; extra == "all"
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
 Requires-Dist: sentence-transformers<2.3,>=2.2.0; extra == "all"
```

### Comparing `jac_nlp-1.4.2.5/README.md` & `jac_nlp-1.4.2.6/README.md`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/bi_enc_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/bi_enc_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/cl_summer_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/cl_summer_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/paraphraser_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/paraphraser_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/sbert_sim_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/sbert_sim_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/sentiment_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/sentiment_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/summarization_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/summarization_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/text_seg_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/text_seg_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/tfm_ner_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/tfm_ner_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/topic_ext_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/topic_ext_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/use_enc_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/use_enc_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/action_configs/use_qa_action_config.py` & `jac_nlp-1.4.2.6/jac_nlp/action_configs/use_qa_action_config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/bi_enc.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/bi_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/poly_enc.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/poly_enc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This action is inactive and not maintained for produciton usage.
 """
+
 import os
 import torch
 from typing import Dict, List, Union
 from fastapi import HTTPException
 from transformers import AutoModel, AutoConfig, AutoTokenizer
 from utils.evaluate import get_embeddings, get_inference
 from utils.models import PolyEncoder
```

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/sent_enc.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/sent_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/tests/test_bi_enc.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/tests/test_bi_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/evaluate.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/models.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/models.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/tokenizer.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/bi_enc/utils/train.py` & `jac_nlp-1.4.2.6/jac_nlp/bi_enc/utils/train.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/cl_summer/cl_summer.py` & `jac_nlp-1.4.2.6/jac_nlp/cl_summer/cl_summer.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/cl_summer/tests/test_cl_summer.py` & `jac_nlp-1.4.2.6/jac_nlp/cl_summer/tests/test_cl_summer.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/config.py` & `jac_nlp-1.4.2.6/jac_nlp/config.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/dolly/dolly.py` & `jac_nlp-1.4.2.6/jac_nlp/dolly/dolly.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/gpt2/gpt2.py` & `jac_nlp-1.4.2.6/jac_nlp/gpt2/gpt2.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/gpt2/train.py` & `jac_nlp-1.4.2.6/jac_nlp/gpt2/train.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/llm/dataset_builder.py` & `jac_nlp-1.4.2.6/jac_nlp/llm/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/llm/llm.py` & `jac_nlp-1.4.2.6/jac_nlp/llm/llm.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/paraphraser/paraphraser.py` & `jac_nlp-1.4.2.6/jac_nlp/paraphraser/paraphraser.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/paraphraser/tests/test_paraphraser.py` & `jac_nlp-1.4.2.6/jac_nlp/paraphraser/tests/test_paraphraser.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/sbert_sim/sbert_sim.py` & `jac_nlp-1.4.2.6/jac_nlp/sbert_sim/sbert_sim.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac` & `jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/sbert_sim/tests/test_sbert_sim.py` & `jac_nlp-1.4.2.6/jac_nlp/sbert_sim/tests/test_sbert_sim.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/sentiment/sentiment.py` & `jac_nlp-1.4.2.6/jac_nlp/sentiment/sentiment.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/summarization/summarization.py` & `jac_nlp-1.4.2.6/jac_nlp/summarization/summarization.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/text_seg/text_seg.py` & `jac_nlp-1.4.2.6/jac_nlp/text_seg/text_seg.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/tfm_ner/entity_utils.py` & `jac_nlp-1.4.2.6/jac_nlp/tfm_ner/entity_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac` & `jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tests/test_tfm_ner.py` & `jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tests/test_tfm_ner.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/tfm_ner/tfm_ner.py` & `jac_nlp-1.4.2.6/jac_nlp/tfm_ner/tfm_ner.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/tfm_ner/train.py` & `jac_nlp-1.4.2.6/jac_nlp/tfm_ner/train.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/tfm_ner/utils/data_tokens.py` & `jac_nlp-1.4.2.6/jac_nlp/tfm_ner/utils/data_tokens.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/topic_ext/action_utils.py` & `jac_nlp-1.4.2.6/jac_nlp/topic_ext/action_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/topic_ext/topic_ext.py` & `jac_nlp-1.4.2.6/jac_nlp/topic_ext/topic_ext.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/fixtures/use_enc.jac` & `jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/fixtures/use_enc.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/use_enc/tests/test_use_enc.py` & `jac_nlp-1.4.2.6/jac_nlp/use_enc/tests/test_use_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/use_enc/use_enc.py` & `jac_nlp-1.4.2.6/jac_nlp/use_enc/use_enc.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/fixtures/use_qa.jac` & `jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/fixtures/use_qa.jac`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/use_qa/tests/test_use_qa.py` & `jac_nlp-1.4.2.6/jac_nlp/use_qa/tests/test_use_qa.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp/use_qa/use_qa.py` & `jac_nlp-1.4.2.6/jac_nlp/use_qa/use_qa.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp.egg-info/PKG-INFO` & `jac_nlp-1.4.2.6/jac_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jac_nlp
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
-Requires-Dist: jaseci==1.4.2.5
+Requires-Dist: jaseci==1.4.2.6
 Requires-Dist: pytest<7.1,>=7.0.1
 Requires-Dist: pytest-order<1.1,>=1.0.1
 Provides-Extra: all
 Requires-Dist: transformers>=4.25.1; extra == "all"
 Requires-Dist: beautifulsoup4<4.13.0,>=4.12.2; extra == "all"
 Requires-Dist: torch<2.0.0,>=1.10.2; extra == "all"
 Requires-Dist: sentence-transformers<2.3,>=2.2.0; extra == "all"
```

### Comparing `jac_nlp-1.4.2.5/jac_nlp.egg-info/SOURCES.txt` & `jac_nlp-1.4.2.6/jac_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.2.5/jac_nlp.egg-info/requires.txt` & `jac_nlp-1.4.2.6/jac_nlp.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jaseci==1.4.2.5
+jaseci==1.4.2.6
 pytest<7.1,>=7.0.1
 pytest-order<1.1,>=1.0.1
 
 [all]
 transformers>=4.25.1
 beautifulsoup4<4.13.0,>=4.12.2
 torch<2.0.0,>=1.10.2
```

### Comparing `jac_nlp-1.4.2.5/setup.py` & `jac_nlp-1.4.2.6/setup.py`

 * *Files identical despite different names*

