# Comparing `tmp/opencompass-0.2.2.tar.gz` & `tmp/opencompass-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opencompass-0.2.2.tar", last modified: Thu Feb  8 06:05:10 2024, max compression
+gzip compressed data, was "dist/opencompass-0.2.3.tar", last modified: Tue Mar 12 03:53:43 2024, max compression
```

## Comparing `opencompass-0.2.2.tar` & `opencompass-0.2.3.tar`

### file list

```diff
@@ -1,387 +1,407 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    20968 2024-02-08 06:05:10.000000 opencompass-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-02-08 06:05:00.000000 opencompass-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/FinanceIQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/GaokaoBench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/cmp_GCP_D.py
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/cmp_KSP.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/cmp_TSP_D.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/hard_GCP.py
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/hard_MSP.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/hard_TSP.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/p_BSP.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/p_EDP.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/p_SPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/NPHardEval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/TheoremQA.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/advglue.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/afqmcd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/agieval/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/agieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/constructions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16445 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/dataset_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/math_equivalence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/agieval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/anli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/anthropics_evals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/arc.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/ax.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/bbh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/boolq.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/bustum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/c3.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/ceval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/chid.py
--rw-r--r--   0 runner    (1001) docker     (127)    20323 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cibench.py
--rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/circular.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/civilcomments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/clozeTest_maxmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cluewsc.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cmb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cmmlu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cmnli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cmrc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/commonsenseqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/commonsenseqa_cn.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/copa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/crowspairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/crowspairs_cn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/csl.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/cvalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/drcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/drop.py
--rw-r--r--   0 runner    (1001) docker     (127)    15872 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/ds1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/ds1000_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/eprstmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/flores.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/game24.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/govrepcrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/gpqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/gsm8k.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/gsm_hard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/hellaswag.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/humaneval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/humaneval_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/humanevalx.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/hungarian_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_codedebug.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_coderun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_endia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_enmc.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_enqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_ensum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_mathcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_mathfind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_retrievekv.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_retrievenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_retrievepasskey.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_zhqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/infinitebench/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/iwslt2017.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/jigsawmultilingual.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/kaoshi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/lambada.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/lawbench/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/lawbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/lawbench/lawbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/lcsts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/leval/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_coursera.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_financial_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_gov_report_summ.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_gsm100.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_legal_contract_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_meeting_summ.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_multidoc_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_narrattive_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_natural_question.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_news_summ.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_paper_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_patent_summ.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_review_summ.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_scientific_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_topic_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_tpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/leval/leval_tvshow_summ.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/lmeval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/longbench/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_2wikim_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_dureader.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_gov_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_hotpot_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_lcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_lsht.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_multi_news.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_multifieldqa_en.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_multifieldqa_zh.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_musique.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_narrative_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_passage_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_passage_retrieval_en.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_passage_retrieval_zh.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_qasper.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_qmsum.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_repobench.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_samsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_trec.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_trivia_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/longbench/longbench_vcsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/mastermath2024v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/math.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/math401.py
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/math_intern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/mathbench.py
--rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/mbpp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/medbench/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/constructions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/dataset_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/math_equivalence.py
--rw-r--r--   0 runner    (1001) docker     (127)    21958 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/medbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/medbench/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/mmlu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/multirc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/narrativeqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/natural_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/natural_question_cn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/obqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/piqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/py150.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/qasper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/qaspercut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/race.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/realtoxicprompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/reasonbench/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/reasonbench/ReasonBenchDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/reasonbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/rolebench.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/safety.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/scibench.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/siqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/squad20.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/storycloze.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/strategyqa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/subjective/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/alignbench.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/compass_arena.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/corev2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25234 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/creationbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/information_retrival.py
--rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/mtbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/multiround.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/subjective/subjective_cmp.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/summedits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/summscreen.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/svamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/tabmwp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/teval/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/teval/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/evaluators/instruct_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/evaluators/planning_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/evaluators/reason_retrieve_understand_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/evaluators/review_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/datasets/teval/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/utils/convert_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/utils/format_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/utils/meta_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/teval/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/tnews.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/triviaqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/triviaqarc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/truthfulqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/tydiqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/wic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/wikibench.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/winograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/winogrande.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/wnli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/wsc.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/xcopa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/xiezhi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/xlsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/datasets/xsum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/metrics/dump_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/metrics/mme_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/metrics/seedbench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/accessory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/ai360_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/alaya.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/baichuan_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/baidu_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19050 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/base_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/bytedance_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/models/claude_api/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/claude_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/claude_api/claude_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/claude_api/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/glm.py
--rw-r--r--   0 runner    (1001) docker     (127)    33985 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/intern_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/lagent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/lightllm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/minimax_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/modelscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/moonshot_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/nanbeige_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/pangu_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/qwen_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/sensetime_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/turbomind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/turbomind_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/turbomind_tis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/xunfei_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/zhipuai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/models/zhipuai_v2_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/openicl/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_dataset_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_agent_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_aucroc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_circular_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_em_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_hf_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_jieba_rouge_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_misc_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_toxic_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_evaluator/lm_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_agent_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_attack_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_base_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_chat_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_clp_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_gen_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_ll_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_mink_percent_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_ppl_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_ppl_only_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_sc_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_tot_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_base_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_bm25_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_dpp_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_fix_k_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_mdl_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_random_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_topk_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_votek_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_zero_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/openicl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/openicl/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/partitioners/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/mm_naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/num_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/size.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/sub_naive.py
--rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/partitioners/sub_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9409 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/runners/dlc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/runners/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/runners/local_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/runners/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/runners/slurm_sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/summarizers/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/circular.py
--rw-r--r--   0 runner    (1001) docker     (127)    18153 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/default.py
--rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/multi_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/summarizers/subjective/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/alignmentbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/alpacaeval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/compass_arena.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/corev2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/creationbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/information_retrival.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/mtbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/multiround.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/subjective_post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/subjective/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/summarizers/summarizer_pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/llm_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/mm_infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/openicl_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/openicl_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/openicl_infer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/tasks/subjective_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/abbr.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/lark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/text_postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-08 06:05:00.000000 opencompass-0.2.2/opencompass/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20968 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-08 06:05:10.000000 opencompass-0.2.2/opencompass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 06:05:10.000000 opencompass-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-08 06:05:00.000000 opencompass-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-03-12 03:53:43.000000 opencompass-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-03-12 03:53:33.000000 opencompass-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/FinanceIQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/GaokaoBench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/cmp_GCP_D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/cmp_KSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/cmp_TSP_D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/hard_GCP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/hard_MSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/hard_TSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/p_BSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/p_EDP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/p_SPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/NPHardEval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/OpenFinData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/TheoremQA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/advglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/afqmcd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/agieval/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/agieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16445 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/dataset_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/math_equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/agieval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/anli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/anthropics_evals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/ax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/bbh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/boolq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/bustum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/c3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/ceval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/chid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20323 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cibench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15035 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/civilcomments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/clozeTest_maxmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cluewsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cmb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cmmlu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cmnli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cmrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/commonsenseqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/commonsenseqa_cn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/copa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/crowspairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/crowspairs_cn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/csl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/cvalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/drcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15872 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/ds1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/ds1000_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/eprstmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/flores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/game24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/govrepcrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/gpqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/gsm8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/gsm_hard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/hellaswag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/humaneval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/humaneval_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/humanevalx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/hungarian_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_codedebug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_coderun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_endia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_enmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_enqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_ensum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_mathcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_mathfind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_retrievekv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_retrievenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_retrievepasskey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_zhqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/infinitebench/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/iwslt2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/jigsawmultilingual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/kaoshi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lambada.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/lawbench/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lawbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lawbench/lawbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lcsts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/leval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_coursera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_financial_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_gov_report_summ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_gsm100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_legal_contract_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_meeting_summ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_multidoc_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_narrattive_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_natural_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_news_summ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_paper_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_patent_summ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_review_summ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_scientific_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_topic_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_tpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/leval/leval_tvshow_summ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lmeval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/longbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_2wikim_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_dureader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_gov_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_hotpot_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_lcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_lsht.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_multi_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_multifieldqa_en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_multifieldqa_zh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_musique.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_narrative_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_passage_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_passage_retrieval_en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_passage_retrieval_zh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_qasper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_qmsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_repobench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_samsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_trec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_trivia_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/longbench/longbench_vcsum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/lveval/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12371 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_cmrc_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_dureader_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_factrecall_en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_factrecall_zh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_hotpotwikiqa_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_lic_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_loogle_CR_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_loogle_MIR_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_loogle_SD_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_multifieldqa_en_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/lveval/lveval_multifieldqa_zh_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/mastermath2024v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/math401.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/math_intern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/mathbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17152 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/mbpp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/medbench/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/dataset_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/math_equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21958 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/medbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/medbench/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/mmlu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/multirc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/narrativeqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/natural_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/natural_question_cn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/obqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/piqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/py150.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/qasper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/qaspercut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/race.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/realtoxicprompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/reasonbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/reasonbench/ReasonBenchDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/reasonbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/rolebench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/safety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/scibench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/siqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/squad20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/storycloze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/strategyqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/subjective/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/alignbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/compass_arena.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/corev2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25234 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/creationbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/information_retrival.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/mtbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/multiround.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/subjective/subjective_cmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/summedits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/summscreen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/svamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/tabmwp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/teval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/teval/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/evaluators/instruct_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/evaluators/planning_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/evaluators/reason_retrieve_understand_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/evaluators/review_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/datasets/teval/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/utils/convert_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/utils/format_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/utils/meta_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/teval/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/tnews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/triviaqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/triviaqarc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/truthfulqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/tydiqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/wic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/wikibench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/winograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/winogrande.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/wnli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/wsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/xcopa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/xiezhi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/xlsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/datasets/xsum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/metrics/dump_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/metrics/mme_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/metrics/seedbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/accessory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/ai360_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/alaya.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/baichuan_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/baidu_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19050 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/bytedance_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/models/claude_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/claude_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/claude_api/claude_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/claude_api/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/gemini_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33985 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/intern_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/krgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/lagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/lightllm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/lmdeploy_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/minimax_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/modelscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/moonshot_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/nanbeige_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16867 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/pangu_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/qwen_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/sensetime_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/turbomind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/turbomind_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/turbomind_tis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/xunfei_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/zhipuai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/models/zhipuai_v2_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/openicl/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_dataset_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_agent_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_aucroc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_circular_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_em_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_hf_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_jieba_rouge_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_misc_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_plugin_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_toxic_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_evaluator/lm_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_agent_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_attack_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_base_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15603 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_chat_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_clp_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_gen_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8894 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_ll_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_mink_percent_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_ppl_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_ppl_only_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_sc_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_tot_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_base_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_bm25_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_dpp_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_fix_k_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_mdl_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_random_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_topk_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_votek_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_zero_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/openicl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/openicl/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/partitioners/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/mm_naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/num_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/sub_naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10855 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/partitioners/sub_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/runners/dlc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/runners/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8903 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/runners/local_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/runners/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/runners/slurm_sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/summarizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18153 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/multi_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28602 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/needlebench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/summarizers/subjective/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/alignmentbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/alpacaeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/compass_arena.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/corev2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/creationbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/information_retrival.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/mtbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/multiround.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/subjective_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/subjective/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/summarizers/summarizer_pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/llm_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/mm_infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/openicl_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/openicl_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/openicl_infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11547 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/tasks/subjective_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/abbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/lark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/text_postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-12 03:53:33.000000 opencompass-0.2.3/opencompass/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-12 03:53:43.000000 opencompass-0.2.3/opencompass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 03:53:43.000000 opencompass-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-03-12 03:53:33.000000 opencompass-0.2.3/setup.py
```

### Comparing `opencompass-0.2.2/PKG-INFO` & `opencompass-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencompass
-Version: 0.2.2
+Version: 0.2.3
 Summary: A comprehensive toolkit for large model evaluation
 Home-page: https://github.com/open-compass/opencompass
 Author: OpenCompass Contributors
 Maintainer: OpenCompass Authors
 License: Apache License 2.0
 Description: <div align="center">
           <img src="docs/en/_static/image/logo.svg" width="500px"/>
@@ -13,39 +13,38 @@
         
         [![docs](https://readthedocs.org/projects/opencompass/badge)](https://opencompass.readthedocs.io/en)
         [![license](https://img.shields.io/github/license/InternLM/opencompass.svg)](https://github.com/open-compass/opencompass/blob/main/LICENSE)
         
         <!-- [![PyPI](https://badge.fury.io/py/opencompass.svg)](https://pypi.org/project/opencompass/) -->
         
         [🌐Website](https://opencompass.org.cn/) |
+        [📖CompassHub](https://hub.opencompass.org.cn/home) |
+        [📊CompassRank](https://rank.opencompass.org.cn/home) |
         [📘Documentation](https://opencompass.readthedocs.io/en/latest/) |
         [🛠️Installation](https://opencompass.readthedocs.io/en/latest/get_started/installation.html) |
         [🤔Reporting Issues](https://github.com/open-compass/opencompass/issues/new/choose)
         
         English | [简体中文](README_zh-CN.md)
         
         </div>
         
         <p align="center">
             👋 join us on <a href="https://discord.gg/KKwfEbFj7U" target="_blank">Discord</a> and <a href="https://r.vansin.top/?r=opencompass" target="_blank">WeChat</a>
         </p>
         
-        ## 📣 OpenCompass 2023 LLM Annual Leaderboard
+        ## 📣 OpenCompass 2.0
         
-        We are honored to have witnessed the tremendous progress of artificial general intelligence together with the community in the past year, and we are also very pleased that **OpenCompass** can help numerous developers and users.
+        We are thrilled to introduce OpenCompass 2.0, an advanced suite featuring three key components: [CompassKit](https://github.com/open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://rank.opencompass.org.cn/home).
+        ![oc20](https://github.com/tonysy/opencompass/assets/7881589/90dbe1c0-c323-470a-991e-2b37ab5350b2)
         
-        We announce the launch of the **OpenCompass 2023 LLM Annual Leaderboard** plan. We expect to release the annual leaderboard of the LLMs in January 2024, systematically evaluating the performance of LLMs in various capabilities such as language, knowledge, reasoning, creation, long-text, and agents.
+        **CompassRank** has been significantly enhanced into the leaderboards that now incorporates both open-source benchmarks and proprietary benchmarks. This upgrade allows for a more comprehensive evaluation of models across the industry.
         
-        At that time, we will release rankings for both open-source models and commercial API models, aiming to provide a comprehensive, objective, and neutral reference for the industry and research community.
+        **CompassHub** presents a pioneering benchmark browser interface, designed to simplify and expedite the exploration and utilization of an extensive array of benchmarks for researchers and practitioners alike. To enhance the visibility of your own benchmark within the community, we warmly invite you to contribute it to CompassHub. You may initiate the submission process by clicking [here](https://hub.opencompass.org.cn/dataset-submit).
         
-        We sincerely invite various large models to join the OpenCompass to showcase their performance advantages in different fields. At the same time, we also welcome researchers and developers to provide valuable suggestions and contributions to jointly promote the development of the LLMs. If you have any questions or needs, please feel free to [contact us](mailto:opencompass@pjlab.org.cn). In addition, relevant evaluation contents, performance statistics, and evaluation methods will be open-source along with the leaderboard release.
-        
-        We have provided the more details of the CompassBench 2023 in [Doc](docs/zh_cn/advanced_guides/compassbench_intro.md).
-        
-        Let's look forward to the release of the OpenCompass 2023 LLM Annual Leaderboard!
+        **CompassKit** is a powerful collection of evaluation toolkits specifically tailored for Large Language Models and Large Vision-language Models. It provides an extensive set of tools to assess and measure the performance of these complex models effectively. Welcome to try our toolkits for in your research and products.
         
         ## 🧭	Welcome
         
         to **OpenCompass**!
         
         Just like a compass guides us on our journey, OpenCompass will guide you through the complex landscape of evaluating large language models. With its powerful algorithms and intuitive interface, OpenCompass makes it easy to assess the quality and effectiveness of your NLP models.
         
@@ -56,20 +55,20 @@
         > **Attention**<br />
         > We launch the OpenCompass Collaboration project, welcome to support diverse evaluation benchmarks into OpenCompass!
         > Clike [Issue](https://github.com/open-compass/opencompass/issues/248) for more information.
         > Let's work together to build a more powerful OpenCompass toolkit!
         
         ## 🚀 What's New <a><img width="35" height="20" src="https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png"></a>
         
+        - **\[2024.02.29\]** We supported the MT-Bench, AlpacalEval and AlignBench, more information can be found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/subjective_evaluation.html) 🔥🔥🔥.
+        - **\[2024.01.30\]** We release OpenCompass 2.0. Click  [CompassKit](https://github.com/open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://rank.opencompass.org.cn/home) for more information ! 🔥🔥🔥.
         - **\[2024.01.17\]** We supported the evaluation of [InternLM2](https://github.com/open-compass/opencompass/blob/main/configs/eval_internlm2_keyset.py) and [InternLM2-Chat](https://github.com/open-compass/opencompass/blob/main/configs/eval_internlm2_chat_keyset.py), InternLM2 showed extremely strong performance in these tests, welcome to try! 🔥🔥🔥.
         - **\[2024.01.17\]** We supported the needle in a haystack test with multiple needles, more information can be found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/needleinahaystack_eval.html#id8) 🔥🔥🔥.
-        - **\[2023.12.28\]** We have enabled seamless evaluation of all models developed using [LLaMA2-Accessory](https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for comprehensive LLM development. 🔥🔥🔥.
-        - **\[2023.12.22\]** We have released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more details! 🔥🔥🔥.
-        - **\[2023.12.10\]** We have released [VLMEvalKit](https://github.com/open-compass/VLMEvalKit), a toolkit for evaluating vision-language models (VLMs), currently support 20+ VLMs and 7 multi-modal benchmarks (including MMBench series).
-        - **\[2023.12.10\]** We have supported Mistral AI's MoE LLM: **Mixtral-8x7B-32K**. Welcome to [MixtralKit](https://github.com/open-compass/MixtralKit) for more details about inference and evaluation.
+        - **\[2023.12.28\]** We have enabled seamless evaluation of all models developed using [LLaMA2-Accessory](https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for comprehensive LLM development.
+        - **\[2023.12.22\]** We have released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more details!
         
         > [More](docs/en/notes/news.md)
         
         ## ✨ Introduction
         
         ![image](https://github.com/open-compass/opencompass/assets/22607038/f45fe125-4aed-4f8c-8fe8-df4efb41a8ea)
         
@@ -83,15 +82,15 @@
         
         - **Modular design with high extensibility**: Want to add new models or datasets, customize an advanced task division strategy, or even support a new cluster management system? Everything about OpenCompass can be easily expanded!
         
         - **Experiment management and reporting mechanism**: Use config files to fully record each experiment, and support real-time reporting of results.
         
         ## 📊 Leaderboard
         
-        We provide [OpenCompass Leaderboard](https://opencompass.org.cn/rank) for the community to rank all public models and API models. If you would like to join the evaluation, please provide the model repository URL or a standard API interface to the email address `opencompass@pjlab.org.cn`.
+        We provide [OpenCompass Leaderboard](https://rank.opencompass.org.cn/home) for the community to rank all public models and API models. If you would like to join the evaluation, please provide the model repository URL or a standard API interface to the email address `opencompass@pjlab.org.cn`.
         
         <p align="right"><a href="#top">🔝Back to top</a></p>
         
         ## 🛠️ Installation
         
         Below are the steps for quick installation and datasets preparation.
         
@@ -118,16 +117,16 @@
         # also please install requiresments packages via `pip install -r requirements/api.txt` for API models if needed.
         ```
         
         ### 📂 Data Preparation
         
         ```bash
         # Download dataset to data/ folder
-        wget https://github.com/open-compass/opencompass/releases/download/0.1.8.rc1/OpenCompassData-core-20231110.zip
-        unzip OpenCompassData-core-20231110.zip
+        wget https://github.com/open-compass/opencompass/releases/download/0.2.2.rc1/OpenCompassData-core-20240207.zip
+        unzip OpenCompassData-core-20240207.zip
         ```
         
         Some third-party features, like Humaneval and Llama, may require additional steps to work properly, for detailed steps please refer to the [Installation Guide](https://opencompass.readthedocs.io/en/latest/get_started/installation.html).
         
         <p align="right"><a href="#top">🔝Back to top</a></p>
         
         ## 🏗️ ️Evaluation
@@ -424,18 +423,14 @@
               </td>
             </tr>
         </td>
             </tr>
           </tbody>
         </table>
         
-        ## OpenCompass Ecosystem
-        
-        <p align="right"><a href="#top">🔝Back to top</a></p>
-        
         ## 📖 Model Support
         
         <table align="center">
           <tbody>
             <tr align="center" valign="bottom">
               <td>
                 <b>Open-source Models</b>
@@ -457,20 +452,22 @@
         - [Baichuan](https://github.com/baichuan-inc)
         - [WizardLM](https://github.com/nlpxucan/WizardLM)
         - [ChatGLM2](https://github.com/THUDM/ChatGLM2-6B)
         - [ChatGLM3](https://github.com/THUDM/ChatGLM3-6B)
         - [TigerBot](https://github.com/TigerResearch/TigerBot)
         - [Qwen](https://github.com/QwenLM/Qwen)
         - [BlueLM](https://github.com/vivo-ai-lab/BlueLM)
+        - [Gemma](https://huggingface.co/google/gemma-7b)
         - ...
         
         </td>
         <td>
         
         - OpenAI
+        - Gemini
         - Claude
         - ZhipuAI(ChatGLM)
         - Baichuan
         - ByteDance(YunQue)
         - Huawei(PanGu)
         - 360
         - Baidu(ERNIEBot)
@@ -485,26 +482,26 @@
           </tbody>
         </table>
         
         <p align="right"><a href="#top">🔝Back to top</a></p>
         
         ## 🔜 Roadmap
         
-        - [ ] Subjective Evaluation
+        - [x] Subjective Evaluation
           - [ ] Release CompassAreana
-          - [ ] Subjective evaluation dataset.
+          - [x] Subjective evaluation.
         - [x] Long-context
-          - [ ] Long-context evaluation with extensive datasets.
+          - [x] Long-context evaluation with extensive datasets.
           - [ ] Long-context leaderboard.
-        - [ ] Coding
+        - [x] Coding
           - [ ] Coding evaluation leaderboard.
           - [x] Non-python language evaluation service.
-        - [ ] Agent
+        - [x] Agent
           - [ ] Support various agenet framework.
-          - [ ] Evaluation of tool use of the LLMs.
+          - [x] Evaluation of tool use of the LLMs.
         - [x] Robustness
           - [x] Support various attack method
         
         ## 👷‍♂️ Contributing
         
         We appreciate all contributions to improving OpenCompass. Please refer to the [contributing guideline](https://opencompass.readthedocs.io/en/latest/notes/contribution_guide.html) for the best practice.
```

#### html2text {}

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1 Name: opencompass Version: 0.2.2 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opencompass Version: 0.2.3 Summary: A comprehensive
 toolkit for large model evaluation Home-page: https://github.com/open-compass/
 opencompass Author: OpenCompass Contributors Maintainer: OpenCompass Authors
 License: Apache License 2.0 Description:
                        [docs/en/_static/image/logo.svg]
 
     [![docs](https://readthedocs.org/projects/opencompass/badge)](https://
    opencompass.readthedocs.io/en) [![license](https://img.shields.io/github/
 license/InternLM/opencompass.svg)](https://github.com/open-compass/opencompass/
        blob/main/LICENSE) [ðWebsite](https://opencompass.org.cn/) |
-     [ðDocumentation](https://opencompass.readthedocs.io/en/latest/) |
-[ð ï¸Installation](https://opencompass.readthedocs.io/en/latest/get_started/
- installation.html) | [ð¤Reporting Issues](https://github.com/open-compass/
-   opencompass/issues/new/choose) English | [ç®ä½ä¸­æ](README_zh-CN.md)
+   [ðCompassHub](https://hub.opencompass.org.cn/home) | [ðCompassRank]
+     (https://rank.opencompass.org.cn/home) | [ðDocumentation](https://
+    opencompass.readthedocs.io/en/latest/) | [ð ï¸Installation](https://
+    opencompass.readthedocs.io/en/latest/get_started/installation.html) |
+[ð¤Reporting Issues](https://github.com/open-compass/opencompass/issues/new/
+               choose) English | [ç®ä½ä¸­æ](README_zh-CN.md)
                       ð join us on _D_i_s_c_o_r_d and _W_e_C_h_a_t
-## ð£ OpenCompass 2023 LLM Annual Leaderboard We are honored to have
-witnessed the tremendous progress of artificial general intelligence together
-with the community in the past year, and we are also very pleased that
-**OpenCompass** can help numerous developers and users. We announce the launch
-of the **OpenCompass 2023 LLM Annual Leaderboard** plan. We expect to release
-the annual leaderboard of the LLMs in January 2024, systematically evaluating
-the performance of LLMs in various capabilities such as language, knowledge,
-reasoning, creation, long-text, and agents. At that time, we will release
-rankings for both open-source models and commercial API models, aiming to
-provide a comprehensive, objective, and neutral reference for the industry and
-research community. We sincerely invite various large models to join the
-OpenCompass to showcase their performance advantages in different fields. At
-the same time, we also welcome researchers and developers to provide valuable
-suggestions and contributions to jointly promote the development of the LLMs.
-If you have any questions or needs, please feel free to [contact us](mailto:
-opencompass@pjlab.org.cn). In addition, relevant evaluation contents,
-performance statistics, and evaluation methods will be open-source along with
-the leaderboard release. We have provided the more details of the CompassBench
-2023 in [Doc](docs/zh_cn/advanced_guides/compassbench_intro.md). Let's look
-forward to the release of the OpenCompass 2023 LLM Annual Leaderboard! ## ð§­
-Welcome to **OpenCompass**! Just like a compass guides us on our journey,
-OpenCompass will guide you through the complex landscape of evaluating large
-language models. With its powerful algorithms and intuitive interface,
-OpenCompass makes it easy to assess the quality and effectiveness of your NLP
-models. ð©ð©ð© Explore opportunities at OpenCompass! We're currently
-**hiring full-time researchers/engineers and interns**. If you're passionate
-about LLM and OpenCompass, don't hesitate to reach out to us via [email]
-(mailto:zhangsongyang@pjlab.org.cn). We'd love to hear from you! ð¥ð¥ð¥
-We are delighted to announce that **the OpenCompass has been recommended by the
-Meta AI**, click [Get Started](https://ai.meta.com/llama/get-started/
-#validation) of Llama for more information. > **Attention**
+## ð£ OpenCompass 2.0 We are thrilled to introduce OpenCompass 2.0, an
+advanced suite featuring three key components: [CompassKit](https://github.com/
+open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and
+[CompassRank](https://rank.opencompass.org.cn/home). ![oc20](https://
+github.com/tonysy/opencompass/assets/7881589/90dbe1c0-c323-470a-991e-
+2b37ab5350b2) **CompassRank** has been significantly enhanced into the
+leaderboards that now incorporates both open-source benchmarks and proprietary
+benchmarks. This upgrade allows for a more comprehensive evaluation of models
+across the industry. **CompassHub** presents a pioneering benchmark browser
+interface, designed to simplify and expedite the exploration and utilization of
+an extensive array of benchmarks for researchers and practitioners alike. To
+enhance the visibility of your own benchmark within the community, we warmly
+invite you to contribute it to CompassHub. You may initiate the submission
+process by clicking [here](https://hub.opencompass.org.cn/dataset-submit).
+**CompassKit** is a powerful collection of evaluation toolkits specifically
+tailored for Large Language Models and Large Vision-language Models. It
+provides an extensive set of tools to assess and measure the performance of
+these complex models effectively. Welcome to try our toolkits for in your
+research and products. ## ð§­ Welcome to **OpenCompass**! Just like a compass
+guides us on our journey, OpenCompass will guide you through the complex
+landscape of evaluating large language models. With its powerful algorithms and
+intuitive interface, OpenCompass makes it easy to assess the quality and
+effectiveness of your NLP models. ð©ð©ð© Explore opportunities at
+OpenCompass! We're currently **hiring full-time researchers/engineers and
+interns**. If you're passionate about LLM and OpenCompass, don't hesitate to
+reach out to us via [email](mailto:zhangsongyang@pjlab.org.cn). We'd love to
+hear from you! ð¥ð¥ð¥ We are delighted to announce that **the OpenCompass
+has been recommended by the Meta AI**, click [Get Started](https://ai.meta.com/
+llama/get-started/#validation) of Llama for more information. > **Attention**
 > We launch the OpenCompass Collaboration project, welcome to support diverse
 evaluation benchmarks into OpenCompass! > Clike [Issue](https://github.com/
 open-compass/opencompass/issues/248) for more information. > Let's work
 together to build a more powerful OpenCompass toolkit! ## ð What's New
 [https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-
-4fe0-bbba-39ffb77730be.png]- **\[2024.01.17\]** We supported the evaluation of
-[InternLM2](https://github.com/open-compass/opencompass/blob/main/configs/
-eval_internlm2_keyset.py) and [InternLM2-Chat](https://github.com/open-compass/
-opencompass/blob/main/configs/eval_internlm2_chat_keyset.py), InternLM2 showed
-extremely strong performance in these tests, welcome to try! ð¥ð¥ð¥. -
-**\[2024.01.17\]** We supported the needle in a haystack test with multiple
-needles, more information can be found [here](https://
+4fe0-bbba-39ffb77730be.png]- **\[2024.02.29\]** We supported the MT-Bench,
+AlpacalEval and AlignBench, more information can be found [here](https://
 opencompass.readthedocs.io/en/latest/advanced_guides/
+subjective_evaluation.html) ð¥ð¥ð¥. - **\[2024.01.30\]** We release
+OpenCompass 2.0. Click [CompassKit](https://github.com/open-compass),
+[CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://
+rank.opencompass.org.cn/home) for more information ! ð¥ð¥ð¥. - **\
+[2024.01.17\]** We supported the evaluation of [InternLM2](https://github.com/
+open-compass/opencompass/blob/main/configs/eval_internlm2_keyset.py) and
+[InternLM2-Chat](https://github.com/open-compass/opencompass/blob/main/configs/
+eval_internlm2_chat_keyset.py), InternLM2 showed extremely strong performance
+in these tests, welcome to try! ð¥ð¥ð¥. - **\[2024.01.17\]** We supported
+the needle in a haystack test with multiple needles, more information can be
+found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/
 needleinahaystack_eval.html#id8) ð¥ð¥ð¥. - **\[2023.12.28\]** We have
 enabled seamless evaluation of all models developed using [LLaMA2-Accessory]
 (https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for
-comprehensive LLM development. ð¥ð¥ð¥. - **\[2023.12.22\]** We have
-released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step
-evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our
-[Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more
-details! ð¥ð¥ð¥. - **\[2023.12.10\]** We have released [VLMEvalKit]
-(https://github.com/open-compass/VLMEvalKit), a toolkit for evaluating vision-
-language models (VLMs), currently support 20+ VLMs and 7 multi-modal benchmarks
-(including MMBench series). - **\[2023.12.10\]** We have supported Mistral AI's
-MoE LLM: **Mixtral-8x7B-32K**. Welcome to [MixtralKit](https://github.com/open-
-compass/MixtralKit) for more details about inference and evaluation. > [More]
+comprehensive LLM development. - **\[2023.12.22\]** We have released [T-Eval]
+(https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark
+to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://
+open-compass.github.io/T-Eval/leaderboard.html) for more details! > [More]
 (docs/en/notes/news.md) ## â¨ Introduction ![image](https://github.com/open-
 compass/opencompass/assets/22607038/f45fe125-4aed-4f8c-8fe8-df4efb41a8ea)
 OpenCompass is a one-stop platform for large model evaluation, aiming to
 provide a fair, open, and reproducible benchmark for large model evaluation.
 Its main features include: - **Comprehensive support for models and datasets**:
 Pre-support for 20+ HuggingFace and API models, a model evaluation scheme of
 70+ datasets with about 400,000 questions, comprehensively evaluating the
@@ -84,33 +84,34 @@
 shot, and chain-of-thought evaluations, combined with standard or dialogue-type
 prompt templates, to easily stimulate the maximum performance of various
 models. - **Modular design with high extensibility**: Want to add new models or
 datasets, customize an advanced task division strategy, or even support a new
 cluster management system? Everything about OpenCompass can be easily expanded!
 - **Experiment management and reporting mechanism**: Use config files to fully
 record each experiment, and support real-time reporting of results. ## ð
-Leaderboard We provide [OpenCompass Leaderboard](https://opencompass.org.cn/
-rank) for the community to rank all public models and API models. If you would
-like to join the evaluation, please provide the model repository URL or a
-standard API interface to the email address `opencompass@pjlab.org.cn`.
+Leaderboard We provide [OpenCompass Leaderboard](https://
+rank.opencompass.org.cn/home) for the community to rank all public models and
+API models. If you would like to join the evaluation, please provide the model
+repository URL or a standard API interface to the email address
+`opencompass@pjlab.org.cn`.
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ð ï¸ Installation Below are the steps for quick installation and datasets
 preparation. ### ð» Environment Setup #### Open-source Models with GPU
 ```bash conda create --name opencompass python=3.10 pytorch torchvision
 pytorch-cuda -c nvidia -c pytorch -y conda activate opencompass git clone
 https://github.com/open-compass/opencompass opencompass cd opencompass pip
 install -e . ``` #### API Models with CPU-only ```bash conda create -
 n opencompass python=3.10 pytorch torchvision torchaudio cpuonly -c pytorch -
 y conda activate opencompass git clone https://github.com/open-compass/
 opencompass opencompass cd opencompass pip install -e . # also please install
 requiresments packages via `pip install -r requirements/api.txt` for API models
 if needed. ``` ### ð Data Preparation ```bash # Download dataset to data/
 folder wget https://github.com/open-compass/opencompass/releases/download/
-0.1.8.rc1/OpenCompassData-core-20231110.zip unzip OpenCompassData-core-
-20231110.zip ``` Some third-party features, like Humaneval and Llama, may
+0.2.2.rc1/OpenCompassData-core-20240207.zip unzip OpenCompassData-core-
+20240207.zip ``` Some third-party features, like Humaneval and Llama, may
 require additional steps to work properly, for detailed steps please refer to
 the [Installation Guide](https://opencompass.readthedocs.io/en/latest/
 get_started/installation.html).
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ðï¸ ï¸Evaluation After ensuring that OpenCompass is installed correctly
 according to the above steps and the datasets are prepared, you can evaluate
 the performance of the LLaMA-7b model on the MMLU and C-Eval datasets using the
@@ -165,52 +166,51 @@
 DROP - OpenBookQA - NarrativeQA -       JigsawMultilingual
 SQuAD2.0 CCoonntteenntt    Qasper              - TruthfulQA
 SSuummmmaarryy - CSL -                         RRoobbuussttnneessss -
 LCSTS - XSum -                          AdvGLUE
 SummScreen CCoonntteenntt
 AAnnaallyyssiiss - EPRSTMT
 - LAMBADA - TNEWS
-## OpenCompass Ecosystem
-                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ð Model Support
-                OOppeenn--ssoouurrccee MMooddeellss                            AAPPII MMooddeellss
-- [InternLM](https://github.com/         - OpenAI - Claude - ZhipuAI(ChatGLM) -
-InternLM/InternLM) - [LLaMA](https://    Baichuan - ByteDance(YunQue) - Huawei
-github.com/facebookresearch/llama) -     (PanGu) - 360 - Baidu(ERNIEBot) -
-[Vicuna](https://github.com/lm-sys/      MiniMax(ABAB-Chat) - SenseTime(nova) -
-FastChat) - [Alpaca](https://github.com/ Xunfei(Spark) - â¦â¦
-tatsu-lab/stanford_alpaca) - [Baichuan]
-(https://github.com/baichuan-inc) -
-[WizardLM](https://github.com/nlpxucan/
-WizardLM) - [ChatGLM2](https://
-github.com/THUDM/ChatGLM2-6B) -
+               OOppeenn--ssoouurrccee MMooddeellss                            AAPPII MMooddeellss
+- [InternLM](https://github.com/        - OpenAI - Gemini - Claude - ZhipuAI
+InternLM/InternLM) - [LLaMA](https://   (ChatGLM) - Baichuan - ByteDance
+github.com/facebookresearch/llama) -    (YunQue) - Huawei(PanGu) - 360 - Baidu
+[Vicuna](https://github.com/lm-sys/     (ERNIEBot) - MiniMax(ABAB-Chat) -
+FastChat) - [Alpaca](https://           SenseTime(nova) - Xunfei(Spark) -
+github.com/tatsu-lab/stanford_alpaca) - â¦â¦
+[Baichuan](https://github.com/baichuan-
+inc) - [WizardLM](https://github.com/
+nlpxucan/WizardLM) - [ChatGLM2](https:/
+/github.com/THUDM/ChatGLM2-6B) -
 [ChatGLM3](https://github.com/THUDM/
 ChatGLM3-6B) - [TigerBot](https://
 github.com/TigerResearch/TigerBot) -
-[Qwen](https://github.com/QwenLM/Qwen) -
-[BlueLM](https://github.com/vivo-ai-lab/
-BlueLM) - ...
-                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
-## ð Roadmap - [ ] Subjective Evaluation - [ ] Release CompassAreana - [ ]
-Subjective evaluation dataset. - [x] Long-context - [ ] Long-context evaluation
-with extensive datasets. - [ ] Long-context leaderboard. - [ ] Coding - [ ]
-Coding evaluation leaderboard. - [x] Non-python language evaluation service. -
-[ ] Agent - [ ] Support various agenet framework. - [ ] Evaluation of tool use
-of the LLMs. - [x] Robustness - [x] Support various attack method ##
-ð·ââï¸ Contributing We appreciate all contributions to improving
-OpenCompass. Please refer to the [contributing guideline](https://
-opencompass.readthedocs.io/en/latest/notes/contribution_guide.html) for the
-best practice. ## ð¤ Acknowledgements Some code in this project is cited and
-modified from [OpenICL](https://github.com/Shark-NLP/OpenICL). Some datasets
-and prompt implementations are modified from [chain-of-thought-hub](https://
-github.com/FranxYao/chain-of-thought-hub) and [instruct-eval](https://
-github.com/declare-lab/instruct-eval). ## ðï¸ Citation ```bibtex @misc
-{2023opencompass, title={OpenCompass: A Universal Evaluation Platform for
-Foundation Models}, author={OpenCompass Contributors}, howpublished = {\url
-{https://github.com/open-compass/opencompass}}, year={2023} } ```
+[Qwen](https://github.com/QwenLM/Qwen)
+- [BlueLM](https://github.com/vivo-ai-
+lab/BlueLM) - [Gemma](https://
+huggingface.co/google/gemma-7b) - ...
+                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
+## ð Roadmap - [x] Subjective Evaluation - [ ] Release CompassAreana - [x]
+Subjective evaluation. - [x] Long-context - [x] Long-context evaluation with
+extensive datasets. - [ ] Long-context leaderboard. - [x] Coding - [ ] Coding
+evaluation leaderboard. - [x] Non-python language evaluation service. - [x]
+Agent - [ ] Support various agenet framework. - [x] Evaluation of tool use of
+the LLMs. - [x] Robustness - [x] Support various attack method ## ð·ââï¸
+Contributing We appreciate all contributions to improving OpenCompass. Please
+refer to the [contributing guideline](https://opencompass.readthedocs.io/en/
+latest/notes/contribution_guide.html) for the best practice. ## ð¤
+Acknowledgements Some code in this project is cited and modified from [OpenICL]
+(https://github.com/Shark-NLP/OpenICL). Some datasets and prompt
+implementations are modified from [chain-of-thought-hub](https://github.com/
+FranxYao/chain-of-thought-hub) and [instruct-eval](https://github.com/declare-
+lab/instruct-eval). ## ðï¸ Citation ```bibtex @misc{2023opencompass, title=
+{OpenCompass: A Universal Evaluation Platform for Foundation Models}, author=
+{OpenCompass Contributors}, howpublished = {\url{https://github.com/open-
+compass/opencompass}}, year={2023} } ```
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 Keywords: AI,NLP,in-context learning,large language
 model,evaluation,benchmark,llm Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Requires-Python: >=3.8.0 Description-
```

### Comparing `opencompass-0.2.2/README.md` & `opencompass-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,39 +5,38 @@
 
 [![docs](https://readthedocs.org/projects/opencompass/badge)](https://opencompass.readthedocs.io/en)
 [![license](https://img.shields.io/github/license/InternLM/opencompass.svg)](https://github.com/open-compass/opencompass/blob/main/LICENSE)
 
 <!-- [![PyPI](https://badge.fury.io/py/opencompass.svg)](https://pypi.org/project/opencompass/) -->
 
 [🌐Website](https://opencompass.org.cn/) |
+[📖CompassHub](https://hub.opencompass.org.cn/home) |
+[📊CompassRank](https://rank.opencompass.org.cn/home) |
 [📘Documentation](https://opencompass.readthedocs.io/en/latest/) |
 [🛠️Installation](https://opencompass.readthedocs.io/en/latest/get_started/installation.html) |
 [🤔Reporting Issues](https://github.com/open-compass/opencompass/issues/new/choose)
 
 English | [简体中文](README_zh-CN.md)
 
 </div>
 
 <p align="center">
     👋 join us on <a href="https://discord.gg/KKwfEbFj7U" target="_blank">Discord</a> and <a href="https://r.vansin.top/?r=opencompass" target="_blank">WeChat</a>
 </p>
 
-## 📣 OpenCompass 2023 LLM Annual Leaderboard
+## 📣 OpenCompass 2.0
 
-We are honored to have witnessed the tremendous progress of artificial general intelligence together with the community in the past year, and we are also very pleased that **OpenCompass** can help numerous developers and users.
+We are thrilled to introduce OpenCompass 2.0, an advanced suite featuring three key components: [CompassKit](https://github.com/open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://rank.opencompass.org.cn/home).
+![oc20](https://github.com/tonysy/opencompass/assets/7881589/90dbe1c0-c323-470a-991e-2b37ab5350b2)
 
-We announce the launch of the **OpenCompass 2023 LLM Annual Leaderboard** plan. We expect to release the annual leaderboard of the LLMs in January 2024, systematically evaluating the performance of LLMs in various capabilities such as language, knowledge, reasoning, creation, long-text, and agents.
+**CompassRank** has been significantly enhanced into the leaderboards that now incorporates both open-source benchmarks and proprietary benchmarks. This upgrade allows for a more comprehensive evaluation of models across the industry.
 
-At that time, we will release rankings for both open-source models and commercial API models, aiming to provide a comprehensive, objective, and neutral reference for the industry and research community.
+**CompassHub** presents a pioneering benchmark browser interface, designed to simplify and expedite the exploration and utilization of an extensive array of benchmarks for researchers and practitioners alike. To enhance the visibility of your own benchmark within the community, we warmly invite you to contribute it to CompassHub. You may initiate the submission process by clicking [here](https://hub.opencompass.org.cn/dataset-submit).
 
-We sincerely invite various large models to join the OpenCompass to showcase their performance advantages in different fields. At the same time, we also welcome researchers and developers to provide valuable suggestions and contributions to jointly promote the development of the LLMs. If you have any questions or needs, please feel free to [contact us](mailto:opencompass@pjlab.org.cn). In addition, relevant evaluation contents, performance statistics, and evaluation methods will be open-source along with the leaderboard release.
-
-We have provided the more details of the CompassBench 2023 in [Doc](docs/zh_cn/advanced_guides/compassbench_intro.md).
-
-Let's look forward to the release of the OpenCompass 2023 LLM Annual Leaderboard!
+**CompassKit** is a powerful collection of evaluation toolkits specifically tailored for Large Language Models and Large Vision-language Models. It provides an extensive set of tools to assess and measure the performance of these complex models effectively. Welcome to try our toolkits for in your research and products.
 
 ## 🧭	Welcome
 
 to **OpenCompass**!
 
 Just like a compass guides us on our journey, OpenCompass will guide you through the complex landscape of evaluating large language models. With its powerful algorithms and intuitive interface, OpenCompass makes it easy to assess the quality and effectiveness of your NLP models.
 
@@ -48,20 +47,20 @@
 > **Attention**<br />
 > We launch the OpenCompass Collaboration project, welcome to support diverse evaluation benchmarks into OpenCompass!
 > Clike [Issue](https://github.com/open-compass/opencompass/issues/248) for more information.
 > Let's work together to build a more powerful OpenCompass toolkit!
 
 ## 🚀 What's New <a><img width="35" height="20" src="https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png"></a>
 
+- **\[2024.02.29\]** We supported the MT-Bench, AlpacalEval and AlignBench, more information can be found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/subjective_evaluation.html) 🔥🔥🔥.
+- **\[2024.01.30\]** We release OpenCompass 2.0. Click  [CompassKit](https://github.com/open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://rank.opencompass.org.cn/home) for more information ! 🔥🔥🔥.
 - **\[2024.01.17\]** We supported the evaluation of [InternLM2](https://github.com/open-compass/opencompass/blob/main/configs/eval_internlm2_keyset.py) and [InternLM2-Chat](https://github.com/open-compass/opencompass/blob/main/configs/eval_internlm2_chat_keyset.py), InternLM2 showed extremely strong performance in these tests, welcome to try! 🔥🔥🔥.
 - **\[2024.01.17\]** We supported the needle in a haystack test with multiple needles, more information can be found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/needleinahaystack_eval.html#id8) 🔥🔥🔥.
-- **\[2023.12.28\]** We have enabled seamless evaluation of all models developed using [LLaMA2-Accessory](https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for comprehensive LLM development. 🔥🔥🔥.
-- **\[2023.12.22\]** We have released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more details! 🔥🔥🔥.
-- **\[2023.12.10\]** We have released [VLMEvalKit](https://github.com/open-compass/VLMEvalKit), a toolkit for evaluating vision-language models (VLMs), currently support 20+ VLMs and 7 multi-modal benchmarks (including MMBench series).
-- **\[2023.12.10\]** We have supported Mistral AI's MoE LLM: **Mixtral-8x7B-32K**. Welcome to [MixtralKit](https://github.com/open-compass/MixtralKit) for more details about inference and evaluation.
+- **\[2023.12.28\]** We have enabled seamless evaluation of all models developed using [LLaMA2-Accessory](https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for comprehensive LLM development.
+- **\[2023.12.22\]** We have released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more details!
 
 > [More](docs/en/notes/news.md)
 
 ## ✨ Introduction
 
 ![image](https://github.com/open-compass/opencompass/assets/22607038/f45fe125-4aed-4f8c-8fe8-df4efb41a8ea)
 
@@ -75,15 +74,15 @@
 
 - **Modular design with high extensibility**: Want to add new models or datasets, customize an advanced task division strategy, or even support a new cluster management system? Everything about OpenCompass can be easily expanded!
 
 - **Experiment management and reporting mechanism**: Use config files to fully record each experiment, and support real-time reporting of results.
 
 ## 📊 Leaderboard
 
-We provide [OpenCompass Leaderboard](https://opencompass.org.cn/rank) for the community to rank all public models and API models. If you would like to join the evaluation, please provide the model repository URL or a standard API interface to the email address `opencompass@pjlab.org.cn`.
+We provide [OpenCompass Leaderboard](https://rank.opencompass.org.cn/home) for the community to rank all public models and API models. If you would like to join the evaluation, please provide the model repository URL or a standard API interface to the email address `opencompass@pjlab.org.cn`.
 
 <p align="right"><a href="#top">🔝Back to top</a></p>
 
 ## 🛠️ Installation
 
 Below are the steps for quick installation and datasets preparation.
 
@@ -110,16 +109,16 @@
 # also please install requiresments packages via `pip install -r requirements/api.txt` for API models if needed.
 ```
 
 ### 📂 Data Preparation
 
 ```bash
 # Download dataset to data/ folder
-wget https://github.com/open-compass/opencompass/releases/download/0.1.8.rc1/OpenCompassData-core-20231110.zip
-unzip OpenCompassData-core-20231110.zip
+wget https://github.com/open-compass/opencompass/releases/download/0.2.2.rc1/OpenCompassData-core-20240207.zip
+unzip OpenCompassData-core-20240207.zip
 ```
 
 Some third-party features, like Humaneval and Llama, may require additional steps to work properly, for detailed steps please refer to the [Installation Guide](https://opencompass.readthedocs.io/en/latest/get_started/installation.html).
 
 <p align="right"><a href="#top">🔝Back to top</a></p>
 
 ## 🏗️ ️Evaluation
@@ -416,18 +415,14 @@
       </td>
     </tr>
 </td>
     </tr>
   </tbody>
 </table>
 
-## OpenCompass Ecosystem
-
-<p align="right"><a href="#top">🔝Back to top</a></p>
-
 ## 📖 Model Support
 
 <table align="center">
   <tbody>
     <tr align="center" valign="bottom">
       <td>
         <b>Open-source Models</b>
@@ -449,20 +444,22 @@
 - [Baichuan](https://github.com/baichuan-inc)
 - [WizardLM](https://github.com/nlpxucan/WizardLM)
 - [ChatGLM2](https://github.com/THUDM/ChatGLM2-6B)
 - [ChatGLM3](https://github.com/THUDM/ChatGLM3-6B)
 - [TigerBot](https://github.com/TigerResearch/TigerBot)
 - [Qwen](https://github.com/QwenLM/Qwen)
 - [BlueLM](https://github.com/vivo-ai-lab/BlueLM)
+- [Gemma](https://huggingface.co/google/gemma-7b)
 - ...
 
 </td>
 <td>
 
 - OpenAI
+- Gemini
 - Claude
 - ZhipuAI(ChatGLM)
 - Baichuan
 - ByteDance(YunQue)
 - Huawei(PanGu)
 - 360
 - Baidu(ERNIEBot)
@@ -477,26 +474,26 @@
   </tbody>
 </table>
 
 <p align="right"><a href="#top">🔝Back to top</a></p>
 
 ## 🔜 Roadmap
 
-- [ ] Subjective Evaluation
+- [x] Subjective Evaluation
   - [ ] Release CompassAreana
-  - [ ] Subjective evaluation dataset.
+  - [x] Subjective evaluation.
 - [x] Long-context
-  - [ ] Long-context evaluation with extensive datasets.
+  - [x] Long-context evaluation with extensive datasets.
   - [ ] Long-context leaderboard.
-- [ ] Coding
+- [x] Coding
   - [ ] Coding evaluation leaderboard.
   - [x] Non-python language evaluation service.
-- [ ] Agent
+- [x] Agent
   - [ ] Support various agenet framework.
-  - [ ] Evaluation of tool use of the LLMs.
+  - [x] Evaluation of tool use of the LLMs.
 - [x] Robustness
   - [x] Support various attack method
 
 ## 👷‍♂️ Contributing
 
 We appreciate all contributions to improving OpenCompass. Please refer to the [contributing guideline](https://opencompass.readthedocs.io/en/latest/notes/contribution_guide.html) for the best practice.
```

#### html2text {}

```diff
@@ -1,75 +1,75 @@
                        [docs/en/_static/image/logo.svg]
 
     [![docs](https://readthedocs.org/projects/opencompass/badge)](https://
    opencompass.readthedocs.io/en) [![license](https://img.shields.io/github/
 license/InternLM/opencompass.svg)](https://github.com/open-compass/opencompass/
        blob/main/LICENSE) [ðWebsite](https://opencompass.org.cn/) |
-     [ðDocumentation](https://opencompass.readthedocs.io/en/latest/) |
-[ð ï¸Installation](https://opencompass.readthedocs.io/en/latest/get_started/
- installation.html) | [ð¤Reporting Issues](https://github.com/open-compass/
-   opencompass/issues/new/choose) English | [ç®ä½ä¸­æ](README_zh-CN.md)
+   [ðCompassHub](https://hub.opencompass.org.cn/home) | [ðCompassRank]
+     (https://rank.opencompass.org.cn/home) | [ðDocumentation](https://
+    opencompass.readthedocs.io/en/latest/) | [ð ï¸Installation](https://
+    opencompass.readthedocs.io/en/latest/get_started/installation.html) |
+[ð¤Reporting Issues](https://github.com/open-compass/opencompass/issues/new/
+               choose) English | [ç®ä½ä¸­æ](README_zh-CN.md)
                       ð join us on _D_i_s_c_o_r_d and _W_e_C_h_a_t
-## ð£ OpenCompass 2023 LLM Annual Leaderboard We are honored to have
-witnessed the tremendous progress of artificial general intelligence together
-with the community in the past year, and we are also very pleased that
-**OpenCompass** can help numerous developers and users. We announce the launch
-of the **OpenCompass 2023 LLM Annual Leaderboard** plan. We expect to release
-the annual leaderboard of the LLMs in January 2024, systematically evaluating
-the performance of LLMs in various capabilities such as language, knowledge,
-reasoning, creation, long-text, and agents. At that time, we will release
-rankings for both open-source models and commercial API models, aiming to
-provide a comprehensive, objective, and neutral reference for the industry and
-research community. We sincerely invite various large models to join the
-OpenCompass to showcase their performance advantages in different fields. At
-the same time, we also welcome researchers and developers to provide valuable
-suggestions and contributions to jointly promote the development of the LLMs.
-If you have any questions or needs, please feel free to [contact us](mailto:
-opencompass@pjlab.org.cn). In addition, relevant evaluation contents,
-performance statistics, and evaluation methods will be open-source along with
-the leaderboard release. We have provided the more details of the CompassBench
-2023 in [Doc](docs/zh_cn/advanced_guides/compassbench_intro.md). Let's look
-forward to the release of the OpenCompass 2023 LLM Annual Leaderboard! ## ð§­
-Welcome to **OpenCompass**! Just like a compass guides us on our journey,
-OpenCompass will guide you through the complex landscape of evaluating large
-language models. With its powerful algorithms and intuitive interface,
-OpenCompass makes it easy to assess the quality and effectiveness of your NLP
-models. ð©ð©ð© Explore opportunities at OpenCompass! We're currently
-**hiring full-time researchers/engineers and interns**. If you're passionate
-about LLM and OpenCompass, don't hesitate to reach out to us via [email]
-(mailto:zhangsongyang@pjlab.org.cn). We'd love to hear from you! ð¥ð¥ð¥
-We are delighted to announce that **the OpenCompass has been recommended by the
-Meta AI**, click [Get Started](https://ai.meta.com/llama/get-started/
-#validation) of Llama for more information. > **Attention**
+## ð£ OpenCompass 2.0 We are thrilled to introduce OpenCompass 2.0, an
+advanced suite featuring three key components: [CompassKit](https://github.com/
+open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and
+[CompassRank](https://rank.opencompass.org.cn/home). ![oc20](https://
+github.com/tonysy/opencompass/assets/7881589/90dbe1c0-c323-470a-991e-
+2b37ab5350b2) **CompassRank** has been significantly enhanced into the
+leaderboards that now incorporates both open-source benchmarks and proprietary
+benchmarks. This upgrade allows for a more comprehensive evaluation of models
+across the industry. **CompassHub** presents a pioneering benchmark browser
+interface, designed to simplify and expedite the exploration and utilization of
+an extensive array of benchmarks for researchers and practitioners alike. To
+enhance the visibility of your own benchmark within the community, we warmly
+invite you to contribute it to CompassHub. You may initiate the submission
+process by clicking [here](https://hub.opencompass.org.cn/dataset-submit).
+**CompassKit** is a powerful collection of evaluation toolkits specifically
+tailored for Large Language Models and Large Vision-language Models. It
+provides an extensive set of tools to assess and measure the performance of
+these complex models effectively. Welcome to try our toolkits for in your
+research and products. ## ð§­ Welcome to **OpenCompass**! Just like a compass
+guides us on our journey, OpenCompass will guide you through the complex
+landscape of evaluating large language models. With its powerful algorithms and
+intuitive interface, OpenCompass makes it easy to assess the quality and
+effectiveness of your NLP models. ð©ð©ð© Explore opportunities at
+OpenCompass! We're currently **hiring full-time researchers/engineers and
+interns**. If you're passionate about LLM and OpenCompass, don't hesitate to
+reach out to us via [email](mailto:zhangsongyang@pjlab.org.cn). We'd love to
+hear from you! ð¥ð¥ð¥ We are delighted to announce that **the OpenCompass
+has been recommended by the Meta AI**, click [Get Started](https://ai.meta.com/
+llama/get-started/#validation) of Llama for more information. > **Attention**
 > We launch the OpenCompass Collaboration project, welcome to support diverse
 evaluation benchmarks into OpenCompass! > Clike [Issue](https://github.com/
 open-compass/opencompass/issues/248) for more information. > Let's work
 together to build a more powerful OpenCompass toolkit! ## ð What's New
 [https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-
-4fe0-bbba-39ffb77730be.png]- **\[2024.01.17\]** We supported the evaluation of
-[InternLM2](https://github.com/open-compass/opencompass/blob/main/configs/
-eval_internlm2_keyset.py) and [InternLM2-Chat](https://github.com/open-compass/
-opencompass/blob/main/configs/eval_internlm2_chat_keyset.py), InternLM2 showed
-extremely strong performance in these tests, welcome to try! ð¥ð¥ð¥. -
-**\[2024.01.17\]** We supported the needle in a haystack test with multiple
-needles, more information can be found [here](https://
+4fe0-bbba-39ffb77730be.png]- **\[2024.02.29\]** We supported the MT-Bench,
+AlpacalEval and AlignBench, more information can be found [here](https://
 opencompass.readthedocs.io/en/latest/advanced_guides/
+subjective_evaluation.html) ð¥ð¥ð¥. - **\[2024.01.30\]** We release
+OpenCompass 2.0. Click [CompassKit](https://github.com/open-compass),
+[CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://
+rank.opencompass.org.cn/home) for more information ! ð¥ð¥ð¥. - **\
+[2024.01.17\]** We supported the evaluation of [InternLM2](https://github.com/
+open-compass/opencompass/blob/main/configs/eval_internlm2_keyset.py) and
+[InternLM2-Chat](https://github.com/open-compass/opencompass/blob/main/configs/
+eval_internlm2_chat_keyset.py), InternLM2 showed extremely strong performance
+in these tests, welcome to try! ð¥ð¥ð¥. - **\[2024.01.17\]** We supported
+the needle in a haystack test with multiple needles, more information can be
+found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/
 needleinahaystack_eval.html#id8) ð¥ð¥ð¥. - **\[2023.12.28\]** We have
 enabled seamless evaluation of all models developed using [LLaMA2-Accessory]
 (https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for
-comprehensive LLM development. ð¥ð¥ð¥. - **\[2023.12.22\]** We have
-released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step
-evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our
-[Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more
-details! ð¥ð¥ð¥. - **\[2023.12.10\]** We have released [VLMEvalKit]
-(https://github.com/open-compass/VLMEvalKit), a toolkit for evaluating vision-
-language models (VLMs), currently support 20+ VLMs and 7 multi-modal benchmarks
-(including MMBench series). - **\[2023.12.10\]** We have supported Mistral AI's
-MoE LLM: **Mixtral-8x7B-32K**. Welcome to [MixtralKit](https://github.com/open-
-compass/MixtralKit) for more details about inference and evaluation. > [More]
+comprehensive LLM development. - **\[2023.12.22\]** We have released [T-Eval]
+(https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark
+to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://
+open-compass.github.io/T-Eval/leaderboard.html) for more details! > [More]
 (docs/en/notes/news.md) ## â¨ Introduction ![image](https://github.com/open-
 compass/opencompass/assets/22607038/f45fe125-4aed-4f8c-8fe8-df4efb41a8ea)
 OpenCompass is a one-stop platform for large model evaluation, aiming to
 provide a fair, open, and reproducible benchmark for large model evaluation.
 Its main features include: - **Comprehensive support for models and datasets**:
 Pre-support for 20+ HuggingFace and API models, a model evaluation scheme of
 70+ datasets with about 400,000 questions, comprehensively evaluating the
@@ -80,33 +80,34 @@
 shot, and chain-of-thought evaluations, combined with standard or dialogue-type
 prompt templates, to easily stimulate the maximum performance of various
 models. - **Modular design with high extensibility**: Want to add new models or
 datasets, customize an advanced task division strategy, or even support a new
 cluster management system? Everything about OpenCompass can be easily expanded!
 - **Experiment management and reporting mechanism**: Use config files to fully
 record each experiment, and support real-time reporting of results. ## ð
-Leaderboard We provide [OpenCompass Leaderboard](https://opencompass.org.cn/
-rank) for the community to rank all public models and API models. If you would
-like to join the evaluation, please provide the model repository URL or a
-standard API interface to the email address `opencompass@pjlab.org.cn`.
+Leaderboard We provide [OpenCompass Leaderboard](https://
+rank.opencompass.org.cn/home) for the community to rank all public models and
+API models. If you would like to join the evaluation, please provide the model
+repository URL or a standard API interface to the email address
+`opencompass@pjlab.org.cn`.
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ð ï¸ Installation Below are the steps for quick installation and datasets
 preparation. ### ð» Environment Setup #### Open-source Models with GPU
 ```bash conda create --name opencompass python=3.10 pytorch torchvision
 pytorch-cuda -c nvidia -c pytorch -y conda activate opencompass git clone
 https://github.com/open-compass/opencompass opencompass cd opencompass pip
 install -e . ``` #### API Models with CPU-only ```bash conda create -
 n opencompass python=3.10 pytorch torchvision torchaudio cpuonly -c pytorch -
 y conda activate opencompass git clone https://github.com/open-compass/
 opencompass opencompass cd opencompass pip install -e . # also please install
 requiresments packages via `pip install -r requirements/api.txt` for API models
 if needed. ``` ### ð Data Preparation ```bash # Download dataset to data/
 folder wget https://github.com/open-compass/opencompass/releases/download/
-0.1.8.rc1/OpenCompassData-core-20231110.zip unzip OpenCompassData-core-
-20231110.zip ``` Some third-party features, like Humaneval and Llama, may
+0.2.2.rc1/OpenCompassData-core-20240207.zip unzip OpenCompassData-core-
+20240207.zip ``` Some third-party features, like Humaneval and Llama, may
 require additional steps to work properly, for detailed steps please refer to
 the [Installation Guide](https://opencompass.readthedocs.io/en/latest/
 get_started/installation.html).
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ðï¸ ï¸Evaluation After ensuring that OpenCompass is installed correctly
 according to the above steps and the datasets are prepared, you can evaluate
 the performance of the LLaMA-7b model on the MMLU and C-Eval datasets using the
@@ -161,46 +162,45 @@
 DROP - OpenBookQA - NarrativeQA -       JigsawMultilingual
 SQuAD2.0 CCoonntteenntt    Qasper              - TruthfulQA
 SSuummmmaarryy - CSL -                         RRoobbuussttnneessss -
 LCSTS - XSum -                          AdvGLUE
 SummScreen CCoonntteenntt
 AAnnaallyyssiiss - EPRSTMT
 - LAMBADA - TNEWS
-## OpenCompass Ecosystem
-                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ð Model Support
-                OOppeenn--ssoouurrccee MMooddeellss                            AAPPII MMooddeellss
-- [InternLM](https://github.com/         - OpenAI - Claude - ZhipuAI(ChatGLM) -
-InternLM/InternLM) - [LLaMA](https://    Baichuan - ByteDance(YunQue) - Huawei
-github.com/facebookresearch/llama) -     (PanGu) - 360 - Baidu(ERNIEBot) -
-[Vicuna](https://github.com/lm-sys/      MiniMax(ABAB-Chat) - SenseTime(nova) -
-FastChat) - [Alpaca](https://github.com/ Xunfei(Spark) - â¦â¦
-tatsu-lab/stanford_alpaca) - [Baichuan]
-(https://github.com/baichuan-inc) -
-[WizardLM](https://github.com/nlpxucan/
-WizardLM) - [ChatGLM2](https://
-github.com/THUDM/ChatGLM2-6B) -
+               OOppeenn--ssoouurrccee MMooddeellss                            AAPPII MMooddeellss
+- [InternLM](https://github.com/        - OpenAI - Gemini - Claude - ZhipuAI
+InternLM/InternLM) - [LLaMA](https://   (ChatGLM) - Baichuan - ByteDance
+github.com/facebookresearch/llama) -    (YunQue) - Huawei(PanGu) - 360 - Baidu
+[Vicuna](https://github.com/lm-sys/     (ERNIEBot) - MiniMax(ABAB-Chat) -
+FastChat) - [Alpaca](https://           SenseTime(nova) - Xunfei(Spark) -
+github.com/tatsu-lab/stanford_alpaca) - â¦â¦
+[Baichuan](https://github.com/baichuan-
+inc) - [WizardLM](https://github.com/
+nlpxucan/WizardLM) - [ChatGLM2](https:/
+/github.com/THUDM/ChatGLM2-6B) -
 [ChatGLM3](https://github.com/THUDM/
 ChatGLM3-6B) - [TigerBot](https://
 github.com/TigerResearch/TigerBot) -
-[Qwen](https://github.com/QwenLM/Qwen) -
-[BlueLM](https://github.com/vivo-ai-lab/
-BlueLM) - ...
-                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
-## ð Roadmap - [ ] Subjective Evaluation - [ ] Release CompassAreana - [ ]
-Subjective evaluation dataset. - [x] Long-context - [ ] Long-context evaluation
-with extensive datasets. - [ ] Long-context leaderboard. - [ ] Coding - [ ]
-Coding evaluation leaderboard. - [x] Non-python language evaluation service. -
-[ ] Agent - [ ] Support various agenet framework. - [ ] Evaluation of tool use
-of the LLMs. - [x] Robustness - [x] Support various attack method ##
-ð·ââï¸ Contributing We appreciate all contributions to improving
-OpenCompass. Please refer to the [contributing guideline](https://
-opencompass.readthedocs.io/en/latest/notes/contribution_guide.html) for the
-best practice. ## ð¤ Acknowledgements Some code in this project is cited and
-modified from [OpenICL](https://github.com/Shark-NLP/OpenICL). Some datasets
-and prompt implementations are modified from [chain-of-thought-hub](https://
-github.com/FranxYao/chain-of-thought-hub) and [instruct-eval](https://
-github.com/declare-lab/instruct-eval). ## ðï¸ Citation ```bibtex @misc
-{2023opencompass, title={OpenCompass: A Universal Evaluation Platform for
-Foundation Models}, author={OpenCompass Contributors}, howpublished = {\url
-{https://github.com/open-compass/opencompass}}, year={2023} } ```
+[Qwen](https://github.com/QwenLM/Qwen)
+- [BlueLM](https://github.com/vivo-ai-
+lab/BlueLM) - [Gemma](https://
+huggingface.co/google/gemma-7b) - ...
+                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
+## ð Roadmap - [x] Subjective Evaluation - [ ] Release CompassAreana - [x]
+Subjective evaluation. - [x] Long-context - [x] Long-context evaluation with
+extensive datasets. - [ ] Long-context leaderboard. - [x] Coding - [ ] Coding
+evaluation leaderboard. - [x] Non-python language evaluation service. - [x]
+Agent - [ ] Support various agenet framework. - [x] Evaluation of tool use of
+the LLMs. - [x] Robustness - [x] Support various attack method ## ð·ââï¸
+Contributing We appreciate all contributions to improving OpenCompass. Please
+refer to the [contributing guideline](https://opencompass.readthedocs.io/en/
+latest/notes/contribution_guide.html) for the best practice. ## ð¤
+Acknowledgements Some code in this project is cited and modified from [OpenICL]
+(https://github.com/Shark-NLP/OpenICL). Some datasets and prompt
+implementations are modified from [chain-of-thought-hub](https://github.com/
+FranxYao/chain-of-thought-hub) and [instruct-eval](https://github.com/declare-
+lab/instruct-eval). ## ðï¸ Citation ```bibtex @misc{2023opencompass, title=
+{OpenCompass: A Universal Evaluation Platform for Foundation Models}, author=
+{OpenCompass Contributors}, howpublished = {\url{https://github.com/open-
+compass/opencompass}}, year={2023} } ```
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
```

### Comparing `opencompass-0.2.2/opencompass/datasets/FinanceIQ.py` & `opencompass-0.2.3/opencompass/datasets/FinanceIQ.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/GaokaoBench.py` & `opencompass-0.2.3/opencompass/datasets/GaokaoBench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/cmp_GCP_D.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/cmp_GCP_D.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/cmp_KSP.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/cmp_KSP.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/cmp_TSP_D.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/cmp_TSP_D.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/hard_GCP.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/hard_GCP.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/hard_MSP.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/hard_MSP.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/hard_TSP.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/hard_TSP.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/p_BSP.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/p_BSP.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/p_EDP.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/p_EDP.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/p_SPP.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/p_SPP.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/prompts.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/prompts.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/NPHardEval/utils.py` & `opencompass-0.2.3/opencompass/datasets/NPHardEval/utils.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/__init__.py` & `opencompass-0.2.3/opencompass/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,39 +43,41 @@
 from .gsm8k import *  # noqa: F401, F403
 from .gsm_hard import *  # noqa: F401, F403
 from .hellaswag import *  # noqa: F401, F403
 from .huggingface import *  # noqa: F401, F403
 from .humaneval import *  # noqa: F401, F403
 from .humanevalx import *  # noqa: F401, F403
 from .hungarian_math import *  # noqa: F401, F403
-from .IFEval import *  # noqa: F401, F403
+from .IFEval.ifeval import IFEvalDataset, IFEvaluator  # noqa: F401, F403
 from .infinitebench import *  # noqa: F401, F403
 from .iwslt2017 import *  # noqa: F401, F403
 from .jigsawmultilingual import *  # noqa: F401, F403
 from .jsonl import JsonlDataset  # noqa: F401, F403
 from .kaoshi import KaoshiDataset, KaoshiEvaluator  # noqa: F401, F403
 from .lambada import *  # noqa: F401, F403
 from .lawbench import *  # noqa: F401, F403
 from .lcsts import *  # noqa: F401, F403
 from .leval import *  # noqa: F401, F403
 from .longbench import *  # noqa: F401, F403
+from .lveval import *  # noqa: F401, F403
 from .mastermath2024v1 import *  # noqa: F401, F403
 from .math import *  # noqa: F401, F403
 from .math401 import *  # noqa: F401, F403
 from .math_intern import *  # noqa: F401, F403
 from .mathbench import *  # noqa: F401, F403
 from .mbpp import *  # noqa: F401, F403
 from .medbench import *  # noqa: F401, F403
 from .mmlu import *  # noqa: F401, F403
 from .multirc import *  # noqa: F401, F403
 from .narrativeqa import *  # noqa: F401, F403
 from .natural_question import *  # noqa: F401, F403
 from .natural_question_cn import *  # noqa: F401, F403
 from .NPHardEval import *  # noqa: F401, F403
 from .obqa import *  # noqa: F401, F403
+from .OpenFinData import *  # noqa: F401, F403
 from .piqa import *  # noqa: F401, F403
 from .py150 import *  # noqa: F401, F403
 from .qasper import *  # noqa: F401, F403
 from .qaspercut import *  # noqa: F401, F403
 from .race import *  # noqa: F401, F403
 from .realtoxicprompts import *  # noqa: F401, F403
 from .reasonbench import ReasonBenchDataset  # noqa: F401, F403
```

### Comparing `opencompass-0.2.2/opencompass/datasets/advglue.py` & `opencompass-0.2.3/opencompass/datasets/advglue.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/agieval/agieval.py` & `opencompass-0.2.3/opencompass/datasets/agieval/agieval.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/agieval/constructions.py` & `opencompass-0.2.3/opencompass/datasets/agieval/constructions.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/agieval/dataset_loader.py` & `opencompass-0.2.3/opencompass/datasets/agieval/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/agieval/evaluation.py` & `opencompass-0.2.3/opencompass/datasets/agieval/evaluation.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/agieval/math_equivalence.py` & `opencompass-0.2.3/opencompass/datasets/agieval/math_equivalence.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/agieval/post_process.py` & `opencompass-0.2.3/opencompass/datasets/agieval/post_process.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/agieval/utils.py` & `opencompass-0.2.3/opencompass/datasets/agieval/utils.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/anthropics_evals.py` & `opencompass-0.2.3/opencompass/datasets/anthropics_evals.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/arc.py` & `opencompass-0.2.3/opencompass/datasets/arc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/ax.py` & `opencompass-0.2.3/opencompass/datasets/ax.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/base.py` & `opencompass-0.2.3/opencompass/datasets/base.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/bbh.py` & `opencompass-0.2.3/opencompass/datasets/bbh.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/boolq.py` & `opencompass-0.2.3/opencompass/datasets/boolq.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/c3.py` & `opencompass-0.2.3/opencompass/datasets/c3.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cb.py` & `opencompass-0.2.3/opencompass/datasets/cb.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/ceval.py` & `opencompass-0.2.3/opencompass/datasets/ceval.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/chid.py` & `opencompass-0.2.3/opencompass/datasets/chid.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cibench.py` & `opencompass-0.2.3/opencompass/datasets/cibench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/circular.py` & `opencompass-0.2.3/opencompass/datasets/circular.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/civilcomments.py` & `opencompass-0.2.3/opencompass/datasets/civilcomments.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/clozeTest_maxmin.py` & `opencompass-0.2.3/opencompass/datasets/clozeTest_maxmin.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cluewsc.py` & `opencompass-0.2.3/opencompass/datasets/cluewsc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cmb.py` & `opencompass-0.2.3/opencompass/datasets/cmb.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cmmlu.py` & `opencompass-0.2.3/opencompass/datasets/cmmlu.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cmnli.py` & `opencompass-0.2.3/opencompass/datasets/cmnli.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cmrc.py` & `opencompass-0.2.3/opencompass/datasets/cmrc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/commonsenseqa.py` & `opencompass-0.2.3/opencompass/datasets/commonsenseqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/commonsenseqa_cn.py` & `opencompass-0.2.3/opencompass/datasets/commonsenseqa_cn.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/crowspairs.py` & `opencompass-0.2.3/opencompass/datasets/crowspairs.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/crowspairs_cn.py` & `opencompass-0.2.3/opencompass/datasets/crowspairs_cn.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/csl.py` & `opencompass-0.2.3/opencompass/datasets/csl.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/custom.py` & `opencompass-0.2.3/opencompass/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/cvalues.py` & `opencompass-0.2.3/opencompass/datasets/cvalues.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/drcd.py` & `opencompass-0.2.3/opencompass/datasets/drcd.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/drop.py` & `opencompass-0.2.3/opencompass/datasets/drop.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/ds1000.py` & `opencompass-0.2.3/opencompass/datasets/ds1000.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/ds1000_interpreter.py` & `opencompass-0.2.3/opencompass/datasets/ds1000_interpreter.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/eprstmt.py` & `opencompass-0.2.3/opencompass/datasets/eprstmt.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/flores.py` & `opencompass-0.2.3/opencompass/datasets/flores.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/game24.py` & `opencompass-0.2.3/opencompass/datasets/game24.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/govrepcrs.py` & `opencompass-0.2.3/opencompass/datasets/govrepcrs.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/gpqa.py` & `opencompass-0.2.3/opencompass/datasets/lambada.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,45 @@
-import copy
-import csv
-import os
-
-from datasets import Dataset
-
-from opencompass.openicl import BaseEvaluator
-from opencompass.registry import LOAD_DATASET
+import json
+import re
+import string
+
+from datasets import Dataset, DatasetDict
+
+from opencompass.openicl.icl_evaluator import BaseEvaluator
+from opencompass.registry import ICL_EVALUATORS, LOAD_DATASET
+from opencompass.utils.text_postprocessors import general_postprocess
 
 from .base import BaseDataset
 
 
 @LOAD_DATASET.register_module()
-class GPQADataset(BaseDataset):
+class lambadaDataset(BaseDataset):
 
     @staticmethod
-    def load(path: str, name: str):
-        cnt = 0
-        data = []
-        data_new = []
-        with open(os.path.join(path, name), 'r', encoding='utf-8') as f:
-            reader = csv.reader(f, delimiter=',')
-            for row in reader:
-                if row[7] == 'Question':
-                    continue
-                cnt = cnt + 1
-                question = row[7]
-                A = row[8]
-                B = row[9]
-                C = row[10]
-                D = row[11]
-                options = [row[8], row[9], row[10], row[11]]
-                answer = 'A'
-
-                data.append({
-                    'question': question,
-                    'A': A,
-                    'B': B,
-                    'C': C,
-                    'D': D,
-                    'options': options,
-                    'answer': answer
-                })
-
-                circular_patterns = ['ABCD', 'BCDA', 'CDAB', 'DABC']  # 更新选项顺序
-                c = circular_patterns[cnt % 4]
-                line = copy.deepcopy(data[cnt - 1])
-                tmp = line['A']
-                for i in range(4):
-                    line['ABCD'[i]] = line['options'][ord(c[i]) - ord('A')]
-
-                for i in range(4):
-                    if line['ABCD'[i]] == tmp:
-                        line['answer'] = 'ABCD'[i]
-                        break
-                data_new.append(line)
-
-        dataset = Dataset.from_list(data_new)
+    def load(path):
+        dataset = []
+        with open(path, 'r', encoding='utf-8') as f:
+            for line in f:
+                dataset.append(json.loads(line))
+        dataset = Dataset.from_list(dataset)
+        return DatasetDict({'test': dataset})
 
-        return dataset
 
+@ICL_EVALUATORS.register_module()
+class LambadaEvaluator(BaseEvaluator):
 
-class GPQAEvaluator(BaseEvaluator):
+    def __init__(self) -> None:
+        super().__init__()
 
     def score(self, predictions, references):
         if len(predictions) != len(references):
             return {
-                'error': 'predictions and references have different length'
+                'error': 'predictions and references have different '
+                'length'
             }
-        correct = 0
-        count = 0
-        details = []
-        for i, j in zip(predictions, references):
-            detail = {'pred': i, 'answer': j, 'correct': False}
-            count += 1
-            if i == j:
-                correct += 1
-                detail['correct'] = True
-            details.append(detail)
-        result = {'accuracy': 100 * correct / count, 'details': details}
-        return result
+        score = 0.0
+        for pred, refer in zip(predictions, references):
+            pred = pred.strip().split(' ')[0]
+            pred = re.split(f'[{string.punctuation}]', pred)[0]
+            score += general_postprocess(pred) == general_postprocess(refer)
+        score = 100.0 * score / len(predictions)
+        return dict(accuracy=score)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `opencompass-0.2.2/opencompass/datasets/gsm8k.py` & `opencompass-0.2.3/opencompass/datasets/gsm8k.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/gsm_hard.py` & `opencompass-0.2.3/opencompass/datasets/gsm_hard.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/hellaswag.py` & `opencompass-0.2.3/opencompass/datasets/hellaswag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os.path as osp
 
-from datasets import Dataset
+from datasets import Dataset, DatasetDict
 
 from opencompass.registry import LOAD_DATASET
 
 from .base import BaseDataset
 
 
 @LOAD_DATASET.register_module()
@@ -67,14 +67,40 @@
                     'D': data['choices'][3],
                     'gold': data['gold'],
                 })
         dataset = Dataset.from_list(dataset)
         return dataset
 
 
+@LOAD_DATASET.register_module()
+class hellaswagDatasetwithICE(BaseDataset):
+
+    @staticmethod
+    def load(path):
+        dataset_dict = DatasetDict()
+        for split, filename in [
+            ['train', 'hellaswag_train_sampled25.jsonl'],
+            ['val', 'hellaswag.jsonl'],
+        ]:
+            dataset = []
+            with open(osp.join(path, filename), 'r', encoding='utf-8') as f:
+                for line in f:
+                    data = json.loads(line)
+                    dataset.append({
+                        'ctx': data['query'].split(': ', 1)[-1],
+                        'A': data['choices'][0],
+                        'B': data['choices'][1],
+                        'C': data['choices'][2],
+                        'D': data['choices'][3],
+                        'label': 'ABCD'[data['gold']],
+                    })
+            dataset_dict[split] = Dataset.from_list(dataset)
+        return dataset_dict
+
+
 class hellaswagDatasetClean(BaseDataset):
 
     # load the contamination annotations of CEval from
     # https://github.com/liyucheng09/Contamination_Detector
     @staticmethod
     def load_contamination_annotations(path, split='val'):
         import requests
```

### Comparing `opencompass-0.2.2/opencompass/datasets/humaneval.py` & `opencompass-0.2.3/opencompass/datasets/humaneval.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,18 +152,21 @@
     return text
 
 
 def humaneval_postprocess_v2(text: str) -> str:
     """This is an advanced version of previous postprocess to handle more
     situations, better to use this one."""
     try:
-        # for chatGLM raw text
-        text = eval(text)
+        # for chatGLM related text
+        eval_text = eval(text)
     except Exception:
         pass
+    else:
+        if isinstance(eval_text, str):
+            text = eval_text
     text = text.lstrip('\n')
     if '```' in text:
         blocks = re.findall(r'```(.*?)```', text, re.DOTALL)
         if len(blocks) == 0:
             text = text.split('```')[1]  # fall back to default strategy
         else:
             text = blocks[0]  # fetch the first code block
```

### Comparing `opencompass-0.2.2/opencompass/datasets/humaneval_multi.py` & `opencompass-0.2.3/opencompass/datasets/humaneval_multi.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/humanevalx.py` & `opencompass-0.2.3/opencompass/datasets/humanevalx.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/__init__.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/__init__.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_codedebug.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_codedebug.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_coderun.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_coderun.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_endia.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_endia.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_enmc.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_enmc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_enqa.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_enqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_ensum.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_ensum.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_mathcalc.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_mathcalc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_mathfind.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_mathfind.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_retrievekv.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_retrievekv.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_retrievenumber.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_retrievenumber.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_retrievepasskey.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_retrievepasskey.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/infinitebench/infinitebench_zhqa.py` & `opencompass-0.2.3/opencompass/datasets/infinitebench/infinitebench_zhqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/jigsawmultilingual.py` & `opencompass-0.2.3/opencompass/datasets/jigsawmultilingual.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/kaoshi.py` & `opencompass-0.2.3/opencompass/datasets/kaoshi.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/lambada.py` & `opencompass-0.2.3/opencompass/datasets/OpenFinData.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import json
-import re
-import string
+import os.path as osp
 
-from datasets import Dataset, DatasetDict
+from datasets import Dataset
 
 from opencompass.openicl.icl_evaluator import BaseEvaluator
 from opencompass.registry import ICL_EVALUATORS, LOAD_DATASET
-from opencompass.utils.text_postprocessors import general_postprocess
 
 from .base import BaseDataset
 
 
 @LOAD_DATASET.register_module()
-class lambadaDataset(BaseDataset):
+class OpenFinDataDataset(BaseDataset):
 
     @staticmethod
-    def load(path):
-        dataset = []
-        with open(path, 'r', encoding='utf-8') as f:
-            for line in f:
-                dataset.append(json.loads(line))
-        dataset = Dataset.from_list(dataset)
-        return DatasetDict({'test': dataset})
+    def load(path: str, name: str):
+        with open(osp.join(path, f'{name}.json'), 'r') as f:
+            data = json.load(f)
+            return Dataset.from_list(data)
 
 
 @ICL_EVALUATORS.register_module()
-class LambadaEvaluator(BaseEvaluator):
+class OpenFinDataKWEvaluator(BaseEvaluator):
 
-    def __init__(self) -> None:
+    def __init__(self, ):
         super().__init__()
 
     def score(self, predictions, references):
-        if len(predictions) != len(references):
-            return {
-                'error': 'predictions and references have different '
-                'length'
-            }
-        score = 0.0
-        for pred, refer in zip(predictions, references):
-            pred = pred.strip().split(' ')[0]
-            pred = re.split(f'[{string.punctuation}]', pred)[0]
-            score += general_postprocess(pred) == general_postprocess(refer)
-        score = 100.0 * score / len(predictions)
-        return dict(accuracy=score)
+        assert len(predictions) == len(references)
+
+        scores = []
+        results = dict()
+
+        for i in range(len(references)):
+            all_hit = True
+            judgement = references[i].split('、')
+            for item in judgement:
+                if item not in predictions[i]:
+                    all_hit = False
+                    break
+            if all_hit:
+                scores.append(True)
+            else:
+                scores.append(False)
+
+        results['accuracy'] = round(sum(scores) / len(scores), 4) * 100
+        return results
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opencompass-0.2.2/opencompass/datasets/lawbench/lawbench.py` & `opencompass-0.2.3/opencompass/datasets/lawbench/lawbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/lcsts.py` & `opencompass-0.2.3/opencompass/datasets/lcsts.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/__init__.py` & `opencompass-0.2.3/opencompass/datasets/leval/__init__.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/evaluators.py` & `opencompass-0.2.3/opencompass/datasets/leval/evaluators.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_coursera.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_coursera.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_financial_qa.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_financial_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_gov_report_summ.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_gov_report_summ.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_gsm100.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_gsm100.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_legal_contract_qa.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_legal_contract_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_meeting_summ.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_meeting_summ.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_multidoc_qa.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_multidoc_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_narrattive_qa.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_narrattive_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_natural_question.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_natural_question.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_news_summ.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_news_summ.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_paper_assistant.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_paper_assistant.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_patent_summ.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_patent_summ.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_quality.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_quality.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_review_summ.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_review_summ.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_scientific_qa.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_scientific_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_topic_retrieval.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_topic_retrieval.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_tpo.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_tpo.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/leval/leval_tvshow_summ.py` & `opencompass-0.2.3/opencompass/datasets/leval/leval_tvshow_summ.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/__init__.py` & `opencompass-0.2.3/opencompass/datasets/longbench/__init__.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/evaluators.py` & `opencompass-0.2.3/opencompass/datasets/longbench/evaluators.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_2wikim_qa.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_2wikim_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_dureader.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_dureader.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_gov_report.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_gov_report.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_hotpot_qa.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_hotpot_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_lcc.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_lcc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_lsht.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_lsht.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_multi_news.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_multi_news.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_multifieldqa_en.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_multifieldqa_en.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_multifieldqa_zh.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_multifieldqa_zh.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_musique.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_musique.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_narrative_qa.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_narrative_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_passage_count.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_passage_count.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_passage_retrieval_en.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_passage_retrieval_en.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_passage_retrieval_zh.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_passage_retrieval_zh.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_qasper.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_qasper.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_qmsum.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_qmsum.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_repobench.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_repobench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_samsum.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_samsum.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_trec.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_trec.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_trivia_qa.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_trivia_qa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/longbench/longbench_vcsum.py` & `opencompass-0.2.3/opencompass/datasets/longbench/longbench_vcsum.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/mastermath2024v1.py` & `opencompass-0.2.3/opencompass/datasets/mastermath2024v1.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/math.py` & `opencompass-0.2.3/opencompass/datasets/math.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/math401.py` & `opencompass-0.2.3/opencompass/datasets/math401.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/math_intern.py` & `opencompass-0.2.3/opencompass/datasets/math_intern.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/mathbench.py` & `opencompass-0.2.3/opencompass/datasets/mathbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/mbpp.py` & `opencompass-0.2.3/opencompass/datasets/mbpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,23 +209,23 @@
                 futures = []
                 for i, (refer, pred) in enumerate(zip(references,
                                                       predictions)):
                     pred = self._process_answer(pred)
                     programs = self._process_test(refer, pred)
                     future = executor.submit(execution, programs, i, 3)
                     futures.append(future)
+                    details[str(i)] = {}
+                    details[str(i)]['origin'] = predictions[i]
+                    details[str(i)]['programs'] = programs
 
                 from tqdm import tqdm
                 for future in tqdm(as_completed(futures), total=len(futures)):
                     index, key = future.result()
                     result[key] += 1
-                    details[str(index)] = {
-                        'programs': predictions[index],
-                        'result': key
-                    }
+                    details[str(index)]['result'] = key
 
             result['score'] = result['pass'] / len(predictions) * 100
             result['details'] = details
             return result
         else:
             try:
                 from evalplus.data import write_jsonl
```

### Comparing `opencompass-0.2.2/opencompass/datasets/medbench/constructions.py` & `opencompass-0.2.3/opencompass/datasets/medbench/constructions.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/medbench/dataset_loader.py` & `opencompass-0.2.3/opencompass/datasets/medbench/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/medbench/evaluation.py` & `opencompass-0.2.3/opencompass/datasets/medbench/evaluation.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/medbench/math_equivalence.py` & `opencompass-0.2.3/opencompass/datasets/medbench/math_equivalence.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/medbench/medbench.py` & `opencompass-0.2.3/opencompass/datasets/medbench/medbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/medbench/post_process.py` & `opencompass-0.2.3/opencompass/datasets/medbench/post_process.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/medbench/utils.py` & `opencompass-0.2.3/opencompass/datasets/medbench/utils.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/mmlu.py` & `opencompass-0.2.3/opencompass/datasets/mmlu.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/multirc.py` & `opencompass-0.2.3/opencompass/datasets/multirc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/narrativeqa.py` & `opencompass-0.2.3/opencompass/datasets/narrativeqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/natural_question.py` & `opencompass-0.2.3/opencompass/datasets/natural_question.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         processed_answers = [[general_postprocess(j).lower() for j in i]
                              for i in references]
 
         details = []
         cnt = 0
         for pred, cand_ans in zip(processed_predictions, processed_answers):
             detail = {'pred': pred, 'answer': cand_ans, 'correct': False}
-            cnt += int(any([cand == pred for cand in cand_ans]))
-            if int(any([cand == pred for cand in cand_ans])):
-                detail['correct'] = True
+            # is_correct = any([cand == pred for cand in cand_ans])
+            is_correct = any([cand in pred for cand in cand_ans])
+            cnt += int(is_correct)
+            detail['correct'] = is_correct
             details.append(detail)
         score = cnt / len(predictions) * 100
 
         return {'score': score, 'details': details}
```

### Comparing `opencompass-0.2.2/opencompass/datasets/natural_question_cn.py` & `opencompass-0.2.3/opencompass/datasets/natural_question_cn.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/obqa.py` & `opencompass-0.2.3/opencompass/datasets/obqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/piqa.py` & `opencompass-0.2.3/opencompass/datasets/piqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/py150.py` & `opencompass-0.2.3/opencompass/datasets/py150.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/qasper.py` & `opencompass-0.2.3/opencompass/datasets/qasper.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/qaspercut.py` & `opencompass-0.2.3/opencompass/datasets/qaspercut.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/race.py` & `opencompass-0.2.3/opencompass/datasets/race.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/realtoxicprompts.py` & `opencompass-0.2.3/opencompass/datasets/realtoxicprompts.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/reasonbench/ReasonBenchDataset.py` & `opencompass-0.2.3/opencompass/datasets/reasonbench/ReasonBenchDataset.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/record.py` & `opencompass-0.2.3/opencompass/datasets/record.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/rolebench.py` & `opencompass-0.2.3/opencompass/datasets/rolebench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/safety.py` & `opencompass-0.2.3/opencompass/datasets/safety.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/scibench.py` & `opencompass-0.2.3/opencompass/datasets/scibench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/siqa.py` & `opencompass-0.2.3/opencompass/datasets/siqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/squad20.py` & `opencompass-0.2.3/opencompass/datasets/squad20.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/storycloze.py` & `opencompass-0.2.3/opencompass/datasets/storycloze.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/strategyqa.py` & `opencompass-0.2.3/opencompass/datasets/strategyqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/alignbench.py` & `opencompass-0.2.3/opencompass/datasets/subjective/alignbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/compass_arena.py` & `opencompass-0.2.3/opencompass/datasets/subjective/compass_arena.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/corev2.py` & `opencompass-0.2.3/opencompass/datasets/subjective/corev2.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/creationbench.py` & `opencompass-0.2.3/opencompass/datasets/subjective/creationbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/information_retrival.py` & `opencompass-0.2.3/opencompass/datasets/subjective/information_retrival.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/mtbench.py` & `opencompass-0.2.3/opencompass/datasets/subjective/mtbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/multiround.py` & `opencompass-0.2.3/opencompass/datasets/subjective/multiround.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/subjective/subjective_cmp.py` & `opencompass-0.2.3/opencompass/datasets/subjective/subjective_cmp.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/summscreen.py` & `opencompass-0.2.3/opencompass/datasets/summscreen.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/svamp.py` & `opencompass-0.2.3/opencompass/datasets/svamp.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/tabmwp.py` & `opencompass-0.2.3/opencompass/datasets/tabmwp.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/__init__.py` & `opencompass-0.2.3/opencompass/datasets/teval/__init__.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/evaluators/instruct_evaluator.py` & `opencompass-0.2.3/opencompass/datasets/teval/evaluators/instruct_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/evaluators/planning_evaluator.py` & `opencompass-0.2.3/opencompass/datasets/teval/evaluators/planning_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/evaluators/reason_retrieve_understand_evaluator.py` & `opencompass-0.2.3/opencompass/datasets/teval/evaluators/reason_retrieve_understand_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/evaluators/review_evaluator.py` & `opencompass-0.2.3/opencompass/datasets/teval/evaluators/review_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/schema.py` & `opencompass-0.2.3/opencompass/datasets/teval/schema.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/utils/convert_results.py` & `opencompass-0.2.3/opencompass/datasets/teval/utils/convert_results.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/utils/format_load.py` & `opencompass-0.2.3/opencompass/datasets/teval/utils/format_load.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/teval/utils/template.py` & `opencompass-0.2.3/opencompass/datasets/teval/utils/template.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/tnews.py` & `opencompass-0.2.3/opencompass/datasets/tnews.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/triviaqa.py` & `opencompass-0.2.3/opencompass/datasets/triviaqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/triviaqarc.py` & `opencompass-0.2.3/opencompass/datasets/triviaqarc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/truthfulqa.py` & `opencompass-0.2.3/opencompass/datasets/truthfulqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/tydiqa.py` & `opencompass-0.2.3/opencompass/datasets/tydiqa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/wic.py` & `opencompass-0.2.3/opencompass/datasets/wic.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/wikibench.py` & `opencompass-0.2.3/opencompass/datasets/wikibench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/winograd.py` & `opencompass-0.2.3/opencompass/datasets/winograd.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/wnli.py` & `opencompass-0.2.3/opencompass/datasets/wnli.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/wsc.py` & `opencompass-0.2.3/opencompass/datasets/wsc.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/xcopa.py` & `opencompass-0.2.3/opencompass/datasets/xcopa.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/xiezhi.py` & `opencompass-0.2.3/opencompass/datasets/xiezhi.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/xlsum.py` & `opencompass-0.2.3/opencompass/datasets/xlsum.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/datasets/xsum.py` & `opencompass-0.2.3/opencompass/datasets/xsum.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/metrics/dump_results.py` & `opencompass-0.2.3/opencompass/metrics/dump_results.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/metrics/mme_score.py` & `opencompass-0.2.3/opencompass/metrics/mme_score.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/metrics/seedbench.py` & `opencompass-0.2.3/opencompass/metrics/seedbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/__init__.py` & `opencompass-0.2.3/opencompass/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 from .alaya import AlayaLM  # noqa: F401
 from .baichuan_api import BaiChuan  # noqa: F401
 from .baidu_api import ERNIEBot  # noqa: F401
 from .base import BaseModel, LMTemplateParser  # noqa
 from .base_api import APITemplateParser, BaseAPIModel  # noqa
 from .bytedance_api import ByteDance  # noqa: F401
 from .claude_api import Claude  # noqa: F401
+from .gemini_api import Gemini, GeminiAllesAPIN  # noqa: F401, F403
 from .glm import GLM130B  # noqa: F401, F403
 from .huggingface import HuggingFace  # noqa: F401, F403
 from .huggingface import HuggingFaceCausalLM  # noqa: F401, F403
 from .huggingface import HuggingFaceChatGLM3  # noqa: F401, F403
 from .intern_model import InternLM  # noqa: F401, F403
+from .krgpt_api import KrGPT  # noqa: F401
 from .lightllm_api import LightllmAPI  # noqa: F401
 from .llama2 import Llama2, Llama2Chat  # noqa: F401, F403
+from .lmdeploy_pytorch import LmdeployPytorchModel  # noqa: F401
 from .minimax_api import MiniMax  # noqa: F401
 from .mixtral import Mixtral  # noqa: F401
 from .modelscope import ModelScope, ModelScopeCausalLM  # noqa: F401, F403
 from .moonshot_api import MoonShot  # noqa: F401
 from .nanbeige_api import Nanbeige  # noqa: F401
 from .openai_api import OpenAI  # noqa: F401
 from .pangu_api import PanGu  # noqa: F401
```

### Comparing `opencompass-0.2.2/opencompass/models/accessory.py` & `opencompass-0.2.3/opencompass/models/accessory.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/ai360_api.py` & `opencompass-0.2.3/opencompass/models/ai360_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/alaya.py` & `opencompass-0.2.3/opencompass/models/alaya.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/baichuan_api.py` & `opencompass-0.2.3/opencompass/models/baichuan_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/baidu_api.py` & `opencompass-0.2.3/opencompass/models/baidu_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/base.py` & `opencompass-0.2.3/opencompass/models/base.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/base_api.py` & `opencompass-0.2.3/opencompass/models/base_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/bytedance_api.py` & `opencompass-0.2.3/opencompass/models/bytedance_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/claude_api/claude_api.py` & `opencompass-0.2.3/opencompass/models/claude_api/claude_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/claude_api/postprocessors.py` & `opencompass-0.2.3/opencompass/models/claude_api/postprocessors.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/glm.py` & `opencompass-0.2.3/opencompass/models/glm.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/huggingface.py` & `opencompass-0.2.3/opencompass/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/intern_model.py` & `opencompass-0.2.3/opencompass/models/intern_model.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/lagent.py` & `opencompass-0.2.3/opencompass/models/lagent.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/langchain.py` & `opencompass-0.2.3/opencompass/models/langchain.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/lightllm_api.py` & `opencompass-0.2.3/opencompass/models/lightllm_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import json
+import re
 from concurrent.futures import ThreadPoolExecutor
 from typing import Dict, List, Optional
 
 import numpy as np
 import requests
 
 from opencompass.registry import MODELS
 from opencompass.utils.logging import get_logger
 
-from .base_api import BaseAPIModel
+from .base import BaseModel
+from .base_api import TokenBucket
 
 
 @MODELS.register_module()
-class LightllmAPI(BaseAPIModel):
+class LightllmAPI(BaseModel):
 
     is_api: bool = True
 
     def __init__(
             self,
             path: str = 'LightllmAPI',
             url: str = 'http://localhost:8080/generate',
-            max_seq_len: int = 2048,
             meta_template: Optional[Dict] = None,
+            rate_per_worker: int = 2,
             retry: int = 2,
             generation_kwargs: Optional[Dict] = dict(),
     ):
 
         super().__init__(path=path,
-                         max_seq_len=max_seq_len,
                          meta_template=meta_template,
-                         retry=retry,
                          generation_kwargs=generation_kwargs)
         self.logger = get_logger()
         self.url = url
+        self.retry = retry
         self.generation_kwargs = generation_kwargs
         self.max_out_len = self.generation_kwargs.get('max_new_tokens', 1024)
+        self.meta_template = meta_template
+        self.token_bucket = TokenBucket(rate_per_worker, False)
 
     def generate(self, inputs: List[str], max_out_len: int,
                  **kwargs) -> List[str]:
         """Generate results given a list of inputs.
 
         Args:
             inputs (List[str]): A list of strings or PromptDicts.
@@ -146,7 +149,37 @@
             except requests.JSONDecodeError:
                 self.logger.error('JsonDecode error, got',
                                   str(raw_response.content))
             max_num_retries += 1
         raise RuntimeError('Calling LightllmAPI failed after retrying for '
                            f'{max_num_retries} times. Check the logs for '
                            'details.')
+
+    def wait(self):
+        """Wait till the next query can be sent.
+
+        Applicable in both single-thread and multi-thread environments.
+        """
+        return self.token_bucket.get_token()
+
+    def get_token_len(self, prompt: str) -> int:
+        """Get lengths of the tokenized string. Only English and Chinese
+        characters are counted for now. Users are encouraged to override this
+        method if more accurate length is needed.
+
+        Args:
+            prompt (str): Input string.
+
+        Returns:
+            int: Length of the input tokens
+        """
+
+        english_parts = re.findall(r'[A-Za-z0-9]+', prompt)
+        chinese_parts = re.findall(r'[\u4e00-\u9FFF]+', prompt)
+
+        # Count English words
+        english_count = sum(len(part.split()) for part in english_parts)
+
+        # Count Chinese words
+        chinese_count = sum(len(part) for part in chinese_parts)
+
+        return english_count + chinese_count
```

### Comparing `opencompass-0.2.2/opencompass/models/llama2.py` & `opencompass-0.2.3/opencompass/models/llama2.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/minimax_api.py` & `opencompass-0.2.3/opencompass/models/minimax_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/mixtral.py` & `opencompass-0.2.3/opencompass/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/modelscope.py` & `opencompass-0.2.3/opencompass/models/modelscope.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/moonshot_api.py` & `opencompass-0.2.3/opencompass/models/moonshot_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/nanbeige_api.py` & `opencompass-0.2.3/opencompass/models/nanbeige_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/openai_api.py` & `opencompass-0.2.3/opencompass/models/openai_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -235,14 +235,15 @@
                 continue
             try:
                 return response['choices'][0]['message']['content'].strip()
             except KeyError:
                 if 'error' in response:
                     if response['error']['code'] == 'rate_limit_exceeded':
                         time.sleep(1)
+                        self.logger.warn('Rate limit exceeded, retrying...')
                         continue
                     elif response['error']['code'] == 'insufficient_quota':
                         self.invalid_keys.add(key)
                         self.logger.warn(f'insufficient_quota key: {key}')
                         continue
 
                     self.logger.error('Find error message in response: ',
@@ -411,14 +412,21 @@
                     'msgCode'] == '10000':
                 data = response['data']
                 choices = data['choices']
                 if choices is None:
                     self.logger.error(data)
                 else:
                     return choices[0]['message']['content'].strip()
+            try:
+                match = re.match(r'Error code: \d+ - (.*)', response['data'])
+                err = eval(match.group(1))['error']
+                if err['code'] == 'content_filter' and err['status'] == 400:
+                    return err['message']
+            except Exception:
+                pass
             self.logger.error(response['msg'])
             self.logger.error(response)
             time.sleep(1)
 
         raise RuntimeError('API call failed.')
 
     def get_token_len(self, prompt: str) -> int:
```

### Comparing `opencompass-0.2.2/opencompass/models/pangu_api.py` & `opencompass-0.2.3/opencompass/models/pangu_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/qwen_api.py` & `opencompass-0.2.3/opencompass/models/qwen_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/sensetime_api.py` & `opencompass-0.2.3/opencompass/models/sensetime_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/turbomind.py` & `opencompass-0.2.3/opencompass/models/turbomind.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from concurrent.futures import ThreadPoolExecutor
 from typing import Dict, List, Optional, Union
 
+import numpy as np
+
 from opencompass.models.base import BaseModel
 from opencompass.utils.logging import get_logger
 from opencompass.utils.prompt import PromptList
 
 PromptType = Union[PromptList, str]
 
 
@@ -157,7 +159,33 @@
             _, output_ids, _ = outputs
             response = self.tokenizer.decode(output_ids)
             response = valid_str(response)
         # used to trim
         if end_str:
             response = response.split(end_str)[0]
         return response
+
+    def get_ppl(self,
+                inputs: List[str],
+                mask_length: Optional[List[int]] = None) -> List[float]:
+        """Get perplexity scores given a list of inputs.
+
+        Args:
+            inputs (List[str]): A list of strings.
+            mask_length (Optional[List[int]]): A list of mask lengths. If
+                provided, the perplexity scores will be calculated with the
+                first mask_length[i] tokens masked out. It's okay to skip
+                its implementation if advanced features in PPLInfernecer is
+                not needed.
+
+        Returns:
+            np.ndarray:  The perplexity scores in shape of (N,)
+        """
+        assert isinstance(
+            inputs, List), f'List(str) is expected, but got {type(inputs)}'
+        results = []
+        for text in inputs:
+            input_ids = self.tokenizer.encode(text)
+            res = self.generators[0].get_ppl(input_ids)
+            results.append(res)
+        results = np.concatenate(results)
+        return results
```

### Comparing `opencompass-0.2.2/opencompass/models/turbomind_api.py` & `opencompass-0.2.3/opencompass/models/turbomind_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,49 +16,51 @@
     for invalid_char in invalid_chars:
         bstr = bstr.replace(invalid_char, b'')
     ret = bstr.decode(encoding=coding, errors='ignore')
     return ret
 
 
 class TurboMindAPIModel(BaseModel):
-    """Model wrapper for TurboMind Triton Inference Server gRPC API.
+    """Model wrapper for lmdeploy api server.
 
     Args:
-        path (str): The name of OpenAI's model.
-        tis_addr (str): The address (ip:port format) of turbomind's
-            triton inference server
+        api_addr (str): The address (ip:port format) of lmdeploy's
+            api server.
         max_seq_len (int): The maximum allowed sequence length of a model.
             Note that the length of prompt + generated tokens shall not exceed
             this value. Defaults to 2048.
         meta_template (Dict, optional): The model's meta prompt
             template if needed, in case the requirement of injecting or
             wrapping of any meta instructions.
+        end_str (str, optional): Whether to trim generated strings with end_str
+            if the model has special ending strings that are not handled well.
+            Defaults to None.
     """
 
     is_api: bool = True
 
-    def __init__(
-        self,
-        path: str,
-        api_addr: str = 'http://0.0.0.0:23333',
-        max_seq_len: int = 2048,
-        meta_template: Optional[Dict] = None,
-    ):
-        super().__init__(path=path,
+    def __init__(self,
+                 api_addr: str = 'http://0.0.0.0:23333',
+                 max_seq_len: int = 2048,
+                 meta_template: Optional[Dict] = None,
+                 end_str: Optional[str] = None,
+                 **kwargs):
+        super().__init__(path='',
                          max_seq_len=max_seq_len,
                          meta_template=meta_template)
         from lmdeploy.serve.openai.api_client import APIClient
         self.chatbot = APIClient(api_addr)
         self.model_name = self.chatbot.available_models[0]
         self.logger = get_logger()
         self.template_parser = LMTemplateParser(meta_template)
         self.eos_token_id = None
         if meta_template and 'eos_token_id' in meta_template:
             self.eos_token_id = meta_template['eos_token_id']
         self.api_addr = api_addr
+        self.end_str = end_str
 
     def generate(
         self,
         inputs: List[str or PromptList],
         max_out_len: int = 512,
         temperature: float = 1.0,
     ) -> List[str]:
@@ -69,39 +71,43 @@
                 The PromptDict should be organized in OpenCompass'
                 API format.
             max_out_len (int): The maximum length of the output.
             temperature (float): What sampling temperature to use,
                 between 0 and 2. Higher values like 0.8 will make the output
                 more random, while lower values like 0.2 will make it more
                 focused and deterministic. Defaults to 0.7.
-
+            end_str (str, optional): Whether to trim generated strings
+                with end_str if the model has special ending strings
+                that are not handled well.
+                Defaults to None.
         Returns:
             List[str]: A list of generated strings.
         """
 
         with ThreadPoolExecutor() as executor:
             results = list(
                 executor.map(self._generate, inputs,
                              [max_out_len] * len(inputs),
-                             [temperature] * len(inputs)))
+                             [temperature] * len(inputs),
+                             [self.end_str] * len(inputs)))
         return results
 
     def get_token_len(self, prompt: str) -> int:
         input_ids, length = self.chatbot.encode(prompt)
         return length
 
     def wait(self):
         """Wait till the next query can be sent.
 
         Applicable in both single-thread and multi-thread environments.
         """
         return self.token_bucket.get_token()
 
     def _generate(self, prompt: str or PromptList, max_out_len: int,
-                  temperature: float) -> str:
+                  temperature: float, end_str: str) -> str:
         """Generate results given a list of inputs.
 
         Args:
             prompt (str or PromptList): A string or PromptDict.
                 The PromptDict should be organized in OpenCompass'
                 API format.
             max_out_len (int): The maximum length of the output.
@@ -123,8 +129,10 @@
                 model=self.model_name,
                 max_tokens=max_out_len,
                 temperature=temperature,
                 top_p=0.8,
                 top_k=1):
             response += output['choices'][0]['text']
         response = valid_str(response)
+        if end_str:
+            response = response.split(end_str)[0]
         return response
```

### Comparing `opencompass-0.2.2/opencompass/models/turbomind_tis.py` & `opencompass-0.2.3/opencompass/models/turbomind_tis.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/vllm.py` & `opencompass-0.2.3/opencompass/models/vllm.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/xunfei_api.py` & `opencompass-0.2.3/opencompass/models/xunfei_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/zhipuai_api.py` & `opencompass-0.2.3/opencompass/models/zhipuai_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/models/zhipuai_v2_api.py` & `opencompass-0.2.3/opencompass/models/zhipuai_v2_api.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_dataset_reader.py` & `opencompass-0.2.3/opencompass/openicl/icl_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/__init__.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,9 +3,10 @@
 from .icl_base_evaluator import BaseEvaluator  # noqa
 from .icl_circular_evaluator import CircularEvaluator  # noqa
 from .icl_em_evaluator import EMEvaluator  # noqa
 from .icl_hf_evaluator import *  # noqa
 from .icl_jieba_rouge_evaluator import JiebaRougeEvaluator  # noqa
 from .icl_misc_evaluator import AverageMinKEvaluator  # noqa
 from .icl_misc_evaluator import AveragePPLEvaluator  # noqa
+from .icl_plugin_evaluator import TEvalEvaluator  # noqa
 from .icl_toxic_evaluator import ToxicEvaluator  # noqa
 from .lm_evaluator import LMEvaluator  # noqa
```

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_agent_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_agent_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_aucroc_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_aucroc_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_circular_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_circular_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_em_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_em_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_hf_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_hf_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_jieba_rouge_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_jieba_rouge_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/icl_toxic_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/icl_toxic_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_evaluator/lm_evaluator.py` & `opencompass-0.2.3/opencompass/openicl/icl_evaluator/lm_evaluator.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/__init__.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/__init__.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_agent_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_agent_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_attack_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_attack_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_base_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_base_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_chat_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_chat_inferencer.py`

 * *Files 23% similar despite different names*

```diff
@@ -168,31 +168,37 @@
 
     def __init__(
             self,
             model,
             output_json_filepath: Optional[str] = './icl_inference_output',
             output_json_filename: Optional[str] = 'predictions',
             save_every: Optional[int] = 1,
+            temperature: Optional[float] = 0.0,
+            do_sample: Optional[bool] = False,
             infer_mode: str = 'last',
+            max_out_len: int = 512,
             **kwargs) -> None:
         super().__init__(
             model=model,
             output_json_filename=output_json_filename,
             output_json_filepath=output_json_filepath,
             **kwargs,
         )
         assert infer_mode in ['last', 'every', 'every_with_gt']
         self.infer_mode = infer_mode
+        self.temperature = temperature
+        self.do_sample = do_sample
         self.model: BaseModel
         self._set_meta_template(self.model)
 
         if self.model.is_api and save_every is None:
             save_every = 1
         self.save_every = save_every
         self.dialogue_mode = False
+        self.max_out_len = max_out_len
 
     def _set_meta_template(self, model):
         origin = model.template_parser
         if isinstance(origin, _APITemplateParser):
             model.template_parser = APITemplateParser(origin.meta_template)
         if isinstance(origin, _LMTemplateParser):
             model.template_parser = LMTemplateParser(origin.meta_template)
@@ -326,16 +332,16 @@
 
     def infer_last(self, chat: List[dict], index: int, output_handler):
         assistant_indices = [
             i for i, item in enumerate(chat) if item['role'] == 'assistant'
         ]
 
         history = chat[:assistant_indices[-1]]
-        output = self.model.generate_from_template([history],
-                                                   max_out_len=512)[0]
+        output = self.model.generate_from_template(
+            [history], max_out_len=self.max_out_len)[0]
         output_handler.save_results(
             origin_prompt=history,
             prediction=output,
             idx=index,
             gold=chat[assistant_indices[-1]]['content'],
         )
 
@@ -343,16 +349,24 @@
         assistant_indices = [
             i for i, item in enumerate(chat) if item['role'] == 'assistant'
         ]
         index_copy = index
 
         for i in assistant_indices:
             history = chat[:i]
-            output = self.model.generate_from_template([history],
-                                                       max_out_len=512)[0]
+            if self.do_sample:
+                output = self.model.generate_from_template(
+                    [history],
+                    do_sample=self.do_sample,
+                    temperature=self.temperature,
+                    max_out_len=self.max_out_len)[0]
+            else:
+                output = self.model.generate_from_template(
+                    [history], do_sample=False,
+                    max_out_len=self.max_out_len)[0]
             chat[i]['content'] = output
             if not self.dialogue_mode:
                 output_handler.save_multiround_results(
                     origin_prompt=history[-1]['content'],
                     prediction=output,
                     idx=index,
                     gold=chat[i]['content'],
@@ -381,16 +395,16 @@
                             output_handler):
         assistant_indices = [
             i for i, item in enumerate(chat) if item['role'] == 'assistant'
         ]
 
         for i in assistant_indices:
             history = chat[:i]
-            output = self.model.generate_from_template([history],
-                                                       max_out_len=512)[0]
+            output = self.model.generate_from_template(
+                [history], max_out_len=self.max_out_len)[0]
             output_handler.save_multiround_results(
                 origin_prompt=history[-1]['content'],
                 prediction=output,
                 idx=index,
                 gold=chat[i]['content'],
             )
             index += 1
```

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_clp_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_clp_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_gen_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_gen_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_ll_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_ll_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_mink_percent_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_mink_percent_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_ppl_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_ppl_inferencer.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,17 @@
                 prompt = retriever.generate_label_prompt(
                     idx,
                     ice[idx],
                     label,
                     ice_template=ice_template,
                     prompt_template=prompt_template,
                     remain_sep=normalizing_str is not None)
+                prompt_token_num = self.model.get_token_len_from_template(
+                    prompt, mode='ppl')
                 if self.max_seq_len is not None:
-                    prompt_token_num = self.model.get_token_len_from_template(
-                        prompt, mode='ppl')
                     while len(ice_idx_list[idx]
                               ) > 0 and prompt_token_num > self.max_seq_len:
                         ice_idx_list[idx] = ice_idx_list[idx][:-1]
                         ice[idx] = retriever.generate_ice(
                             ice_idx_list[idx], ice_template=ice_template)
                         prompt = retriever.generate_label_prompt(
                             idx,
```

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_ppl_only_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_ppl_only_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_sc_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_sc_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_inferencer/icl_tot_inferencer.py` & `opencompass-0.2.3/opencompass/openicl/icl_inferencer/icl_tot_inferencer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_prompt_template.py` & `opencompass-0.2.3/opencompass/openicl/icl_prompt_template.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_base_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_base_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_bm25_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_dpp_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_dpp_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_fix_k_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_fix_k_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_mdl_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_mdl_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_random_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_random_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_topk_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_topk_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_votek_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_votek_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/icl_retriever/icl_zero_retriever.py` & `opencompass-0.2.3/opencompass/openicl/icl_retriever/icl_zero_retriever.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/openicl/utils/logging.py` & `opencompass-0.2.3/opencompass/openicl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/partitioners/base.py` & `opencompass-0.2.3/opencompass/partitioners/base.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/partitioners/mm_naive.py` & `opencompass-0.2.3/opencompass/partitioners/mm_naive.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/partitioners/naive.py` & `opencompass-0.2.3/opencompass/partitioners/naive.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/partitioners/num_worker.py` & `opencompass-0.2.3/opencompass/partitioners/num_worker.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/partitioners/size.py` & `opencompass-0.2.3/opencompass/partitioners/size.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/partitioners/sub_naive.py` & `opencompass-0.2.3/opencompass/partitioners/sub_naive.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/partitioners/sub_size.py` & `opencompass-0.2.3/opencompass/partitioners/sub_size.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/registry.py` & `opencompass-0.2.3/opencompass/registry.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/runners/base.py` & `opencompass-0.2.3/opencompass/runners/base.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/runners/dlc.py` & `opencompass-0.2.3/opencompass/runners/slurm_sequential.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,229 +1,264 @@
-import datetime
 import os
 import os.path as osp
-import random
 import re
 import subprocess
-import sys
 import time
+import traceback
 from functools import partial
+from multiprocessing import Pipe, Pool
 from typing import Any, Dict, List, Optional, Tuple
 
 import mmengine
 from mmengine.config import ConfigDict
-from mmengine.utils import track_parallel_progress
+from tqdm import tqdm
 
 from opencompass.registry import RUNNERS, TASKS
-from opencompass.utils import get_logger
+from opencompass.utils import batched, get_logger
 
 from .base import BaseRunner
 
 
 @RUNNERS.register_module()
-class DLCRunner(BaseRunner):
-    """Distributed runner based on Alibaba Cloud Deep Learning Cluster (DLC).
-    It will launch multiple tasks in parallel with 'dlc' command. Please
-    install and configure DLC first before using this runner.
+class SlurmSequentialRunner(BaseRunner):
+    """Distributed runner based on Slurm. It will launch tasks in parallel
+    using `srun` command.
+
+    This runner launches tasks one by one for execution. A new task will only
+    be launched when and only when max_num_workers is not met, and the previous
+    task has been successfully allocated to a machine. Therefore, unlike the
+    `SlurmRunner`, at most only one task will be in the PENDING status at the
+    same time during a run, making the random_sleep strategy no longer
+    necessary. In addition, this runner also includes a feature to
+    automatically kill all jobs by the job_id on exit.
+
+    The runner will obtain the job_id by reading the srun output similar to
+    `srun: Job 123456 scheduled successfully!`. If the output of srun does not
+    match this pattern, the runner will not work properly.
 
     Args:
         task (ConfigDict): Task type config.
-        aliyun_cfg (ConfigDict): Alibaba Cloud config.
-        max_num_workers (int): Max number of workers. Default: 32.
-        retry (int): Number of retries when job failed. Default: 2.
-        debug (bool): Whether to run in debug mode. Default: False.
-        lark_bot_url (str): Lark bot url. Default: None.
+        max_num_workers (int): Max number of workers to run in parallel.
+            Defaults to 32.
+        retry (int): Number of retries if the job failed. Defaults to 2.
+        partition (str): Slurm partition name. Defaults to None.
+        quotatype (str): Slurm quota type. Defaults to None.
+        qos (str): Slurm quality of service. Defaults to None.
+        debug (bool): Whether to run in debug mode. Defaults to False.
+        lark_bot_url (str): Lark bot url. Defaults to None.
+        extra_command (List, optional): Extra slurm command.
+            For example ['-c 12', '-w node1']. Defaults to None.
     """
 
     def __init__(self,
                  task: ConfigDict,
-                 aliyun_cfg: ConfigDict,
+                 task_prefix: str = '',
                  max_num_workers: int = 32,
                  retry: int = 2,
+                 partition: str = None,
+                 quotatype: str = None,
+                 qos: str = None,
                  debug: bool = False,
-                 lark_bot_url: str = None):
+                 lark_bot_url: str = None,
+                 extra_command: Optional[List[str]] = None):
         super().__init__(task=task, debug=debug, lark_bot_url=lark_bot_url)
-        self.aliyun_cfg = aliyun_cfg
         self.max_num_workers = max_num_workers
         self.retry = retry
+        self.partition = partition
+        self.quotatype = quotatype
+        self.qos = qos
+        self.task_prefix = task_prefix
+        if not extra_command:
+            extra_command = []
+        assert isinstance(extra_command, list)
+        self.extra_command = extra_command
 
         logger = get_logger()
-        logger.warning(
-            'To ensure the integrity of the log results, the log displayed '
-            f'by {self.__class__.__name__} has a 10-second delay.')
+        if self.quotatype in ['spot', 'auto']:
+            logger.warning(
+                'Quotatype spot or auto may cause stability issues, '
+                'reserved is recommended.')
 
     def launch(self, tasks: List[Dict[str, Any]]) -> List[Tuple[str, int]]:
-        """Launch multiple tasks.
-
-        Args:
-            tasks (list[dict]): A list of task configs, usually generated by
-                Partitioner.
-
-        Returns:
-            list[tuple[str, int]]: A list of (task name, exit code).
-        """
-
         if not self.debug:
-            status = track_parallel_progress(self._launch,
-                                             tasks,
-                                             nproc=self.max_num_workers,
-                                             keep_order=False)
+            return self._launch_wo_debug(tasks)
         else:
-            status = [self._launch(task, random_sleep=False) for task in tasks]
-        return status
+            return [self._launch(task) for task in tasks]
+
+    def _launch_wo_debug(self,
+                         tasks: List[Dict[str, Any]]) -> List[Tuple[str, int]]:
+        launched_bar = tqdm(total=len(tasks), desc='Launched')
+        finished_bar = tqdm(total=len(tasks), desc='Finished')
+        job_ids = []
+        status = []
+
+        def _update(result):
+            finished_bar.update()
+            status.append(result)
+            return result
+
+        def _err_update(err):
+            finished_bar.update()
+            traceback.print_exc()
+            status.append(('', -1))
 
-    def _launch(self, cfg: ConfigDict, random_sleep: Optional[bool] = None):
-        """Launch a single task.
+        try:
+            parent_conns = []
+            num_workers = max(min(self.max_num_workers, len(tasks)), 1)
+            with Pool(processes=num_workers) as pool:
+                for task in tasks:
+                    parent_conn, child_conn = Pipe()
+                    _ = pool.apply_async(self._launch,
+                                         kwds={
+                                             'cfg': task,
+                                             'child_conn': child_conn
+                                         },
+                                         callback=_update,
+                                         error_callback=_err_update)
+                    time.sleep(0.5)
+
+                    job_id = parent_conn.recv()
+                    launched_bar.update()
+                    parent_conns.append(parent_conn)
+                    job_ids.append(job_id)
+
+                pool.close()
+                pool.join()
+            return status
+        except KeyboardInterrupt:
+            raise
+        finally:
+            launched_bar.close()
+            finished_bar.close()
+            for parent_conn in parent_conns:
+                while parent_conn.poll():
+                    try:
+                        job_id = parent_conn.recv()
+                        job_ids.append(job_id)
+                    except EOFError:
+                        break
+                parent_conn.close()
+
+            tbar = tqdm(total=len(job_ids), desc='clear sruns')
+            for batched_job_ids in batched(job_ids, 4):
+                while True:
+                    ps = []
+                    try:
+                        for job_id in batched_job_ids:
+                            tbar.update()
+                            if job_id is None:
+                                continue
+                            cmd = f'scancel {job_id}'
+                            p = subprocess.Popen(cmd,
+                                                 shell=True,
+                                                 stdout=subprocess.PIPE,
+                                                 stderr=subprocess.STDOUT)
+                            ps.append(p)
+                        break
+                    except KeyboardInterrupt:
+                        logger = get_logger()
+                        logger.error('Ignoring KeyboardInterrupt...')
+                for p in ps:
+                    p.wait()
+            tbar.close()
 
-        Args:
-            cfg (ConfigDict): Task config.
-            random_sleep (bool): Whether to sleep for a random time before
-                running the command. When Aliyun has many tasks to schedule,
-                its stability decreases. Therefore, when we need to submit a
-                large number of tasks at once, we adopt the "random_sleep"
-                strategy. Tasks that would have been submitted all at once are
-                now evenly spread out over a 10-second period. Default: None.
-
-        Returns:
-            tuple[str, int]: Task name and exit code.
-        """
-        if random_sleep is None:
-            random_sleep = (self.max_num_workers > 32)
+    def _launch(self, cfg: ConfigDict, child_conn: Pipe = None):
+        logger = get_logger()
 
         task = TASKS.build(dict(cfg=cfg, type=self.task_cfg['type']))
         num_gpus = task.num_gpus
         task_name = task.name
+        task_name = self.task_prefix + task_name
 
         # Dump task config to file
         mmengine.mkdir_or_exist('tmp/')
         param_file = f'tmp/{os.getpid()}_params.py'
+        process = None
         try:
             cfg.dump(param_file)
 
-            # Build up DLC command
-            pwd = os.getcwd()
-            shell_cmd = (
-                f'source {self.aliyun_cfg["bashrc_path"]}; '
-                f'conda activate {self.aliyun_cfg["conda_env_name"]}; '
-                f'cd {pwd}; '
-                '{task_cmd}')
-
-            tmpl = ('dlc create job'
-                    f" --command '{shell_cmd}'"
-                    f' --name {task_name[:512]}'
-                    ' --kind BatchJob'
-                    f" -c {self.aliyun_cfg['dlc_config_path']}"
-                    f" --workspace_id {self.aliyun_cfg['workspace_id']}"
-                    ' --worker_count 1'
-                    f' --worker_cpu {max(num_gpus * 6, 8)}'
-                    f' --worker_gpu {num_gpus}'
-                    f' --worker_memory {max(num_gpus * 64, 48)}'
-                    f" --worker_image {self.aliyun_cfg['worker_image']}"
-                    ' --interactive')
+            # Build up slurm command
+            tmpl = 'srun'
+            if self.partition:
+                tmpl += f' -p {self.partition}'
+            if self.quotatype:
+                tmpl += f' --quotatype={self.quotatype}'
+            if self.qos:
+                tmpl += f' --qos={self.qos}'
+            if num_gpus > 0:
+                tmpl += f' --gres=gpu:{num_gpus}'
+            for extra_cmd in self.extra_command:
+                tmpl += f' {extra_cmd}'
+            tmpl += f" -N1 -u -J '{task_name[:512]}'" + ' {task_cmd}'
             get_cmd = partial(task.get_command,
                               cfg_path=param_file,
                               template=tmpl)
             cmd = get_cmd()
 
-            logger = get_logger()
             logger.debug(f'Running command: {cmd}')
 
-            # Run command with retry
+            retry = self.retry
+            output_paths = task.get_output_paths()
+
             if self.debug:
-                stdout = sys.stdout
+                while True:
+                    process = subprocess.Popen(cmd, shell=True, text=True)
+                    process.communicate()
+                    process.wait()
+                    if self._job_failed(process.returncode, output_paths):
+                        if retry > 0:
+                            logger.warning(
+                                f'task {task_name} failed, retrying...')
+                            retry -= 1
+                            cmd = get_cmd()
+                        else:
+                            break
+                    else:
+                        break
             else:
                 out_path = task.get_log_path(file_extension='out')
                 mmengine.mkdir_or_exist(osp.split(out_path)[0])
                 stdout = open(out_path, 'w', encoding='utf-8')
-
-            if random_sleep:
-                time.sleep(random.randint(0, 10))
-
-            def _run_within_retry():
-                try:
+                stderr = subprocess.PIPE
+                while True:
                     process = subprocess.Popen(cmd,
                                                shell=True,
                                                text=True,
-                                               stdout=subprocess.PIPE,
-                                               stderr=subprocess.PIPE)
+                                               stdout=stdout,
+                                               stderr=stderr)
                     job_id = None
-                    job_allocated = False
-                    job_finished = False
-                    last_end_time = datetime.datetime.now().strftime(
-                        '%Y-%m-%dT%H:%M:%SZ')
                     while True:
-                        if not job_allocated:
-                            line = process.stdout.readline()
-                            if not line:
-                                break
-                            match = re.search(r'(dlc[0-9a-z]+)', line)
-                            if match and job_id is None:
-                                job_id = match.group(1)
-                            stdout.write(line)
-                            match = re.search(r'Job .* is \[Running\]', line)
-                            if match:
-                                job_allocated = True
-                        else:
-                            try:
-                                process.wait(10)
-                            except subprocess.TimeoutExpired:
-                                pass
-                            else:
-                                job_finished = True
-                            if job_finished:
-                                this_end_time = datetime.datetime.now(
-                                ).strftime('%Y-%m-%dT%H:%M:%SZ')
-                            else:
-                                this_end_time = (
-                                    datetime.datetime.now() -
-                                    datetime.timedelta(seconds=10)
-                                ).strftime('%Y-%m-%dT%H:%M:%SZ')
-                            logs_cmd = (
-                                'dlc logs'
-                                f' {job_id} {job_id}-worker-0'
-                                f' --start_time {last_end_time}'
-                                f' --end_time {this_end_time}'
-                                f" -c {self.aliyun_cfg['dlc_config_path']}")
-                            log_process = subprocess.Popen(
-                                logs_cmd,
-                                shell=True,
-                                text=True,
-                                stdout=subprocess.PIPE,
-                                stderr=subprocess.PIPE)
-                            log_output, log_err = log_process.communicate()
-                            log_output = '\n'.join(log_output.split('\n')[2:])
-                            stdout.write(log_output)
-                            last_end_time = this_end_time
-                        stdout.flush()
-                        if job_finished:
+                        line = process.stderr.readline()
+                        if not line:
                             break
+                        match = re.search(
+                            r'srun: Job (\d+) scheduled successfully!', line)
+                        if match and job_id is None:
+                            job_id = match.group(1)
+                            child_conn.send(job_id)
+                        stdout.write(line)
                     process.wait()
-                    return process.returncode
-                finally:
-                    if job_id is not None:
-                        cancel_cmd = (
-                            'dlc stop job'
-                            f' {job_id}'
-                            f" -c {self.aliyun_cfg['dlc_config_path']}"
-                            ' -f')
-                        subprocess.run(cancel_cmd,
-                                       shell=True,
-                                       text=True,
-                                       stdout=subprocess.PIPE,
-                                       stderr=subprocess.PIPE)
-
-            return_code = _run_within_retry()
-            retry = self.retry
-            output_paths = task.get_output_paths()
-            while self._job_failed(return_code, output_paths) and retry > 0:
-                retry -= 1
-                cmd = get_cmd()
-                return_code = _run_within_retry()
+                    if self._job_failed(process.returncode, output_paths):
+                        if retry > 0:
+                            retry -= 1
+                            cmd = get_cmd()
+                        else:
+                            logger.error(
+                                f'task {task_name} fail, see\n{out_path}')
+                            break
+                    else:
+                        break
+        except KeyboardInterrupt:
+            raise
         finally:
             # Clean up
+            if child_conn is not None:
+                child_conn.send(None)
+                child_conn.close()
+            if process is not None:
+                process.kill()
             os.remove(param_file)
-
-        return task_name, return_code
+        return task_name, process.returncode
 
     def _job_failed(self, return_code: int, output_paths: List[str]) -> bool:
         return return_code != 0 or not all(
             osp.exists(output_path) for output_path in output_paths)
```

### Comparing `opencompass-0.2.2/opencompass/runners/local.py` & `opencompass-0.2.3/opencompass/runners/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                     if len(all_gpu_ids) > num_gpus and num_gpus > 0:
                         get_logger().warning(f'Only use {num_gpus} GPUs for '
                                              f'total {len(all_gpu_ids)} '
                                              'available GPUs in debug mode.')
                     tmpl = get_command_template(all_gpu_ids[:num_gpus])
                     cmd = task.get_command(cfg_path=param_file, template=tmpl)
                     # run in subprocess if starts with torchrun etc.
-                    if cmd.startswith('python'):
+                    if 'python3 ' in cmd or 'python ' in cmd:
                         task.run()
                     else:
                         subprocess.run(cmd, shell=True, text=True)
                 finally:
                     os.remove(param_file)
                 status.append((task_name, 0))
         else:
@@ -185,12 +185,12 @@
             result = subprocess.run(cmd,
                                     shell=True,
                                     text=True,
                                     stdout=stdout,
                                     stderr=stdout)
 
             if result.returncode != 0:
-                logger.warning(f'task {task_name} fail, see\n{out_path}')
+                logger.error(f'task {task_name} fail, see\n{out_path}')
         finally:
             # Clean up
             os.remove(param_file)
         return task_name, result.returncode
```

### Comparing `opencompass-0.2.2/opencompass/runners/local_api.py` & `opencompass-0.2.3/opencompass/runners/local_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         end_time = time.time()
         logger.info(f'time elapsed: {end_time - start_time:.2f}s')
     except Exception:
         # print trace back in target file
         traceback.print_exc()
         # reset stdout and stderr
         reset_std()
-        logger.warning(f'task {task_name} fail, see\n{out_path}')
+        logger.error(f'task {task_name} fail, see\n{out_path}')
         returncode = 1
     else:
         # reset stdout and stderr
         reset_std()
     return task_name, returncode
```

### Comparing `opencompass-0.2.2/opencompass/runners/slurm.py` & `opencompass-0.2.3/opencompass/runners/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 result = subprocess.run(cmd,
                                         shell=True,
                                         text=True,
                                         stdout=stdout,
                                         stderr=stdout)
 
             if result.returncode != 0 and not self.debug:
-                logger.warning(f'task {task_name} fail, see\n{out_path}')
+                logger.error(f'task {task_name} fail, see\n{out_path}')
         finally:
             # Clean up
             os.remove(param_file)
         return task_name, result.returncode
 
     def _job_failed(self, return_code: int, output_paths: List[str]) -> bool:
         return return_code != 0 or not all(
```

### Comparing `opencompass-0.2.2/opencompass/runners/slurm_sequential.py` & `opencompass-0.2.3/opencompass/runners/dlc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,264 +1,262 @@
+import datetime
+import json
 import os
 import os.path as osp
+import random
 import re
 import subprocess
+import sys
 import time
-import traceback
 from functools import partial
-from multiprocessing import Pipe, Pool
 from typing import Any, Dict, List, Optional, Tuple
 
 import mmengine
 from mmengine.config import ConfigDict
-from tqdm import tqdm
+from mmengine.utils import track_parallel_progress
 
 from opencompass.registry import RUNNERS, TASKS
-from opencompass.utils import batched, get_logger
+from opencompass.utils import get_logger
 
 from .base import BaseRunner
 
 
 @RUNNERS.register_module()
-class SlurmSequentialRunner(BaseRunner):
-    """Distributed runner based on Slurm. It will launch tasks in parallel
-    using `srun` command.
-
-    This runner launches tasks one by one for execution. A new task will only
-    be launched when and only when max_num_workers is not met, and the previous
-    task has been successfully allocated to a machine. Therefore, unlike the
-    `SlurmRunner`, at most only one task will be in the PENDING status at the
-    same time during a run, making the random_sleep strategy no longer
-    necessary. In addition, this runner also includes a feature to
-    automatically kill all jobs by the job_id on exit.
-
-    The runner will obtain the job_id by reading the srun output similar to
-    `srun: Job 123456 scheduled successfully!`. If the output of srun does not
-    match this pattern, the runner will not work properly.
+class DLCRunner(BaseRunner):
+    """Distributed runner based on Alibaba Cloud Deep Learning Cluster (DLC).
+    It will launch multiple tasks in parallel with 'dlc' command. Please
+    install and configure DLC first before using this runner.
 
     Args:
         task (ConfigDict): Task type config.
-        max_num_workers (int): Max number of workers to run in parallel.
-            Defaults to 32.
-        retry (int): Number of retries if the job failed. Defaults to 2.
-        partition (str): Slurm partition name. Defaults to None.
-        quotatype (str): Slurm quota type. Defaults to None.
-        qos (str): Slurm quality of service. Defaults to None.
-        debug (bool): Whether to run in debug mode. Defaults to False.
-        lark_bot_url (str): Lark bot url. Defaults to None.
-        extra_command (List, optional): Extra slurm command.
-            For example ['-c 12', '-w node1']. Defaults to None.
+        aliyun_cfg (ConfigDict): Alibaba Cloud config.
+        max_num_workers (int): Max number of workers. Default: 32.
+        retry (int): Number of retries when job failed. Default: 2.
+        debug (bool): Whether to run in debug mode. Default: False.
+        lark_bot_url (str): Lark bot url. Default: None.
     """
 
     def __init__(self,
                  task: ConfigDict,
-                 task_prefix: str = '',
+                 aliyun_cfg: ConfigDict,
                  max_num_workers: int = 32,
+                 eval_with_gpu: list = ['plugin_eval'],
                  retry: int = 2,
-                 partition: str = None,
-                 quotatype: str = None,
-                 qos: str = None,
                  debug: bool = False,
-                 lark_bot_url: str = None,
-                 extra_command: Optional[List[str]] = None):
+                 lark_bot_url: str = None):
         super().__init__(task=task, debug=debug, lark_bot_url=lark_bot_url)
+        self.aliyun_cfg = aliyun_cfg
         self.max_num_workers = max_num_workers
         self.retry = retry
-        self.partition = partition
-        self.quotatype = quotatype
-        self.qos = qos
-        self.task_prefix = task_prefix
-        if not extra_command:
-            extra_command = []
-        assert isinstance(extra_command, list)
-        self.extra_command = extra_command
+
+        self.eval_with_gpu = eval_with_gpu
 
         logger = get_logger()
-        if self.quotatype in ['spot', 'auto']:
-            logger.warning(
-                'Quotatype spot or auto may cause stability issues, '
-                'reserved is recommended.')
+        logger.warning(
+            'To ensure the integrity of the log results, the log displayed '
+            f'by {self.__class__.__name__} has a 10-second delay.')
 
     def launch(self, tasks: List[Dict[str, Any]]) -> List[Tuple[str, int]]:
+        """Launch multiple tasks.
+
+        Args:
+            tasks (list[dict]): A list of task configs, usually generated by
+                Partitioner.
+
+        Returns:
+            list[tuple[str, int]]: A list of (task name, exit code).
+        """
+
         if not self.debug:
-            return self._launch_wo_debug(tasks)
+            status = track_parallel_progress(self._launch,
+                                             tasks,
+                                             nproc=self.max_num_workers,
+                                             keep_order=False)
         else:
-            return [self._launch(task) for task in tasks]
+            status = [self._launch(task, random_sleep=False) for task in tasks]
+        return status
 
-    def _launch_wo_debug(self,
-                         tasks: List[Dict[str, Any]]) -> List[Tuple[str, int]]:
-        launched_bar = tqdm(total=len(tasks), desc='Launched')
-        finished_bar = tqdm(total=len(tasks), desc='Finished')
-        job_ids = []
-        status = []
-
-        def _update(result):
-            finished_bar.update()
-            status.append(result)
-            return result
-
-        def _err_update(err):
-            finished_bar.update()
-            traceback.print_exc()
-            status.append(('', -1))
+    def _launch(self, cfg: ConfigDict, random_sleep: Optional[bool] = None):
+        """Launch a single task.
 
-        try:
-            parent_conns = []
-            num_workers = max(min(self.max_num_workers, len(tasks)), 1)
-            with Pool(processes=num_workers) as pool:
-                for task in tasks:
-                    parent_conn, child_conn = Pipe()
-                    _ = pool.apply_async(self._launch,
-                                         kwds={
-                                             'cfg': task,
-                                             'child_conn': child_conn
-                                         },
-                                         callback=_update,
-                                         error_callback=_err_update)
-                    time.sleep(0.5)
-
-                    job_id = parent_conn.recv()
-                    launched_bar.update()
-                    parent_conns.append(parent_conn)
-                    job_ids.append(job_id)
-
-                pool.close()
-                pool.join()
-            return status
-        except KeyboardInterrupt:
-            raise
-        finally:
-            launched_bar.close()
-            finished_bar.close()
-            for parent_conn in parent_conns:
-                while parent_conn.poll():
-                    try:
-                        job_id = parent_conn.recv()
-                        job_ids.append(job_id)
-                    except EOFError:
-                        break
-                parent_conn.close()
-
-            tbar = tqdm(total=len(job_ids), desc='clear sruns')
-            for batched_job_ids in batched(job_ids, 4):
-                while True:
-                    ps = []
-                    try:
-                        for job_id in batched_job_ids:
-                            tbar.update()
-                            if job_id is None:
-                                continue
-                            cmd = f'scancel {job_id}'
-                            p = subprocess.Popen(cmd,
-                                                 shell=True,
-                                                 stdout=subprocess.PIPE,
-                                                 stderr=subprocess.STDOUT)
-                            ps.append(p)
-                        break
-                    except KeyboardInterrupt:
-                        logger = get_logger()
-                        logger.error('Ignoring KeyboardInterrupt...')
-                for p in ps:
-                    p.wait()
-            tbar.close()
-
-    def _launch(self, cfg: ConfigDict, child_conn: Pipe = None):
-        logger = get_logger()
+        Args:
+            cfg (ConfigDict): Task config.
+            random_sleep (bool): Whether to sleep for a random time before
+                running the command. When Aliyun has many tasks to schedule,
+                its stability decreases. Therefore, when we need to submit a
+                large number of tasks at once, we adopt the "random_sleep"
+                strategy. Tasks that would have been submitted all at once are
+                now evenly spread out over a 10-second period. Default: None.
+
+        Returns:
+            tuple[str, int]: Task name and exit code.
+        """
+        if random_sleep is None:
+            random_sleep = (self.max_num_workers > 32)
 
         task = TASKS.build(dict(cfg=cfg, type=self.task_cfg['type']))
         num_gpus = task.num_gpus
         task_name = task.name
-        task_name = self.task_prefix + task_name
+
+        is_eval_task = 'OpenICLEval' in task_name
+        if is_eval_task and num_gpus == 0:
+            for check_name in self.eval_with_gpu:
+                if check_name in task_name:
+                    num_gpus = 1
+                    break
 
         # Dump task config to file
         mmengine.mkdir_or_exist('tmp/')
         param_file = f'tmp/{os.getpid()}_params.py'
-        process = None
+        pwd = os.getcwd()
         try:
             cfg.dump(param_file)
-
-            # Build up slurm command
-            tmpl = 'srun'
-            if self.partition:
-                tmpl += f' -p {self.partition}'
-            if self.quotatype:
-                tmpl += f' --quotatype={self.quotatype}'
-            if self.qos:
-                tmpl += f' --qos={self.qos}'
-            if num_gpus > 0:
-                tmpl += f' --gres=gpu:{num_gpus}'
-            for extra_cmd in self.extra_command:
-                tmpl += f' {extra_cmd}'
-            tmpl += f" -N1 -u -J '{task_name[:512]}'" + ' {task_cmd}'
+            if self.aliyun_cfg.get('bashrc_path') is not None:
+                # using user's conda env
+                bashrc_path = self.aliyun_cfg['bashrc_path']
+                assert osp.exists(bashrc_path)
+                assert self.aliyun_cfg.get('conda_env_name') is not None
+                conda_env_name = self.aliyun_cfg['conda_env_name']
+                shell_cmd = (f'source {bashrc_path}; '
+                             f'conda activate {conda_env_name}; ')
+            else:
+                # using public conda env
+                # users can also set `python_env_path` to their
+                # own env python path
+                assert self.aliyun_cfg.get('python_env_path') is not None
+                shell_cmd = (
+                    f'export PATH={self.aliyun_cfg["python_env_path"]}/bin:$PATH; '  # noqa: E501
+                    f'export PYTHONPATH={pwd}:$PYTHONPATH; ')
+
+            huggingface_cache = self.aliyun_cfg.get('huggingface_cache')
+            if huggingface_cache is not None:
+                # HUGGINGFACE_HUB_CACHE is a Legacy env variable, here we set
+                # `HF_HUB_CACHE` and `HUGGINGFACE_HUB_CACHE` for bc
+                shell_cmd += f'export HF_HUB_CACHE={huggingface_cache}; '
+                shell_cmd += f'export HUGGINGFACE_HUB_CACHE={huggingface_cache}; '  # noqa: E501
+
+            torch_cache = self.aliyun_cfg.get('torch_cache')
+            if torch_cache is not None:
+                shell_cmd += f'export TORCH_HOME={torch_cache}; '
+
+            hf_offline = self.aliyun_cfg.get('hf_offline', True)
+            if hf_offline:
+                shell_cmd += 'export HF_DATASETS_OFFLINE=1; export TRANSFORMERS_OFFLINE=1; export HF_EVALUATE_OFFLINE=1; '  # noqa: E501
+
+            http_proxy = self.aliyun_cfg.get('http_proxy')
+            if http_proxy is not None:
+                shell_cmd += f'export http_proxy={http_proxy}; export https_proxy={http_proxy}; '  # noqa: E501
+                shell_cmd += f'export HTTP_PROXY={http_proxy}; export HTTPS_PROXY={http_proxy}; '  # noqa: E501
+
+            hf_endpoint = self.aliyun_cfg.get('hf_endpoint')
+            if hf_endpoint is not None:
+                shell_cmd += f'export HF_ENDPOINT={hf_endpoint}; '
+
+            shell_cmd += f'cd {pwd}; '
+            shell_cmd += '{task_cmd}'
+
+            tmpl = ('dlc create job'
+                    f" --command '{shell_cmd}'"
+                    f' --name {task_name[:512]}'
+                    ' --kind BatchJob'
+                    f" -c {self.aliyun_cfg['dlc_config_path']}"
+                    f" --workspace_id {self.aliyun_cfg['workspace_id']}"
+                    ' --worker_count 1'
+                    f' --worker_cpu {max(num_gpus * 8, 32)}'
+                    f' --worker_gpu {num_gpus}'
+                    f' --worker_memory {max(num_gpus * 128, 256)}'
+                    f" --worker_image {self.aliyun_cfg['worker_image']}")
             get_cmd = partial(task.get_command,
                               cfg_path=param_file,
                               template=tmpl)
             cmd = get_cmd()
 
+            logger = get_logger()
             logger.debug(f'Running command: {cmd}')
 
-            retry = self.retry
-            output_paths = task.get_output_paths()
-
+            # Run command with retry
             if self.debug:
-                while True:
-                    process = subprocess.Popen(cmd, shell=True, text=True)
-                    process.communicate()
-                    process.wait()
-                    if self._job_failed(process.returncode, output_paths):
-                        if retry > 0:
-                            logger.warning(
-                                f'task {task_name} failed, retrying...')
-                            retry -= 1
-                            cmd = get_cmd()
-                        else:
-                            break
-                    else:
-                        break
+                stdout = sys.stdout
             else:
                 out_path = task.get_log_path(file_extension='out')
                 mmengine.mkdir_or_exist(osp.split(out_path)[0])
                 stdout = open(out_path, 'w', encoding='utf-8')
-                stderr = subprocess.PIPE
+
+            if random_sleep:
+                time.sleep(random.randint(0, 10))
+
+            def _run_within_retry():
+                output = subprocess.getoutput(cmd)
+                match = re.search(r'\|\s+(dlc[0-9a-z]+)\s+\|', output)
+                if match is None:
+                    raise RuntimeError(
+                        f'Failed to launch dlc job for {output}')
+                else:
+                    job_id = match.group(1)
+                stdout.write(output)
+
+                pod_create_time = None
+                pri_time = None
+                initial_time = datetime.datetime.now()
                 while True:
-                    process = subprocess.Popen(cmd,
-                                               shell=True,
-                                               text=True,
-                                               stdout=stdout,
-                                               stderr=stderr)
-                    job_id = None
-                    while True:
-                        line = process.stderr.readline()
-                        if not line:
-                            break
-                        match = re.search(
-                            r'srun: Job (\d+) scheduled successfully!', line)
-                        if match and job_id is None:
-                            job_id = match.group(1)
-                            child_conn.send(job_id)
-                        stdout.write(line)
-                    process.wait()
-                    if self._job_failed(process.returncode, output_paths):
-                        if retry > 0:
-                            retry -= 1
-                            cmd = get_cmd()
-                        else:
-                            logger.warning(
-                                f'task {task_name} fail, see\n{out_path}')
+                    # 1. Avoid to request dlc too frequently.
+                    # 2. DLC job may not be ready immediately after creation.
+                    for _ in range(5):
+                        time.sleep(2)
+                        try:
+                            job_info = json.loads(
+                                subprocess.getoutput(f'dlc get job {job_id}'))
                             break
+                        except:  # noqa: E722
+                            pass
                     else:
-                        break
-        except KeyboardInterrupt:
-            raise
+                        raise RuntimeError(
+                            f'Failed to get job info for {job_id}')
+
+                    status = job_info['Status']
+                    if status == 'Failed':
+                        return -1
+                    elif status == 'Succeeded':
+                        return 0
+                    elif status != 'Running':
+                        continue
+
+                    # The pod time could be different from the real time.
+                    # Therefore we need to extract the pod start time from
+                    # the `job_info` and calculate the `start_time` and
+                    # `end_time` in pod.
+                    if pod_create_time is None:
+                        pod_create_time = job_info['GmtCreateTime']
+                        pri_time = pod_create_time
+                        pod_create_time = datetime.datetime.strptime(
+                            pod_create_time, '%Y-%m-%dT%H:%M:%SZ')
+                    elasped_time = datetime.datetime.now() - initial_time
+                    cur_time = (pod_create_time +
+                                elasped_time).strftime('%Y-%m-%dT%H:%M:%SZ')
+                    logs_cmd = ('dlc logs'
+                                f' {job_id} {job_id}-worker-0'
+                                f" -c {self.aliyun_cfg['dlc_config_path']}"
+                                f' --start_time {pri_time}'
+                                f' --end_time {cur_time}')
+                    log_output = subprocess.getoutput(logs_cmd)
+
+                    if '[WARN] No logs found for the pod' not in log_output:
+                        pri_time = cur_time
+                        stdout.write(log_output)
+                        stdout.flush()
+
+            return_code = _run_within_retry()
+            retry = self.retry
+            output_paths = task.get_output_paths()
+            while self._job_failed(return_code, output_paths) and retry > 0:
+                retry -= 1
+                cmd = get_cmd()
+                return_code = _run_within_retry()
         finally:
             # Clean up
-            if child_conn is not None:
-                child_conn.send(None)
-                child_conn.close()
-            if process is not None:
-                process.kill()
             os.remove(param_file)
-        return task_name, process.returncode
+
+        return task_name, return_code
 
     def _job_failed(self, return_code: int, output_paths: List[str]) -> bool:
         return return_code != 0 or not all(
             osp.exists(output_path) for output_path in output_paths)
```

### Comparing `opencompass-0.2.2/opencompass/summarizers/circular.py` & `opencompass-0.2.3/opencompass/summarizers/circular.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/default.py` & `opencompass-0.2.3/opencompass/summarizers/default.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/multi_model.py` & `opencompass-0.2.3/opencompass/summarizers/multi_model.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/alignmentbench.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/alignmentbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/alpacaeval.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/alpacaeval.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/compass_arena.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/compass_arena.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/corev2.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/corev2.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/creationbench.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/creationbench.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/information_retrival.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/information_retrival.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/mtbench.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/mtbench.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,20 +123,24 @@
                 subdir = eval_model_abbr + '_judged-by--' + self.judge_abbr
                 subdir_path = os.path.join(results_folder, subdir)
                 if os.path.isdir(subdir_path):
                     model, judge_model = eval_model_abbr, self.judge_abbr
                     fout = osp.join(
                         output_dir,
                         'judged-by--' + judge_model + '-capability.csv')
+                    overall_judged_answers, overall_references = [], []
                     for dataset in dataset_cfgs:
                         judged_answers, references = get_judgeanswer_and_reference(
                             dataset, subdir_path, self.judge_function)
-                        get_capability_results(judged_answers, references,
-                                               fout, fout_flag, model)
-                        fout_flag += 1
+                        overall_judged_answers += judged_answers
+                        overall_references += references
+                    get_capability_results(overall_judged_answers,
+                                           overall_references, fout, fout_flag,
+                                           model)
+                    fout_flag += 1
                 else:
                     print(subdir_path + ' is not exist! please check!')
             with open(fout, 'r') as f:
                 x = from_csv(f)
             print(x)
         elif self.judge_type == 'pair':
             super().summarize()
```

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/multiround.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/multiround.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/subjective_post_process.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/subjective_post_process.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/subjective/utils.py` & `opencompass-0.2.3/opencompass/summarizers/subjective/utils.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/summarizers/summarizer_pretrain.py` & `opencompass-0.2.3/opencompass/summarizers/summarizer_pretrain.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/tasks/base.py` & `opencompass-0.2.3/opencompass/tasks/base.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/tasks/llm_eval.py` & `opencompass-0.2.3/opencompass/tasks/llm_eval.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/tasks/mm_infer.py` & `opencompass-0.2.3/opencompass/tasks/mm_infer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/tasks/openicl_attack.py` & `opencompass-0.2.3/opencompass/tasks/openicl_attack.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/tasks/openicl_eval.py` & `opencompass-0.2.3/opencompass/tasks/openicl_eval.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/tasks/openicl_infer.py` & `opencompass-0.2.3/opencompass/tasks/openicl_infer.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/tasks/subjective_eval.py` & `opencompass-0.2.3/opencompass/tasks/subjective_eval.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/abbr.py` & `opencompass-0.2.3/opencompass/utils/abbr.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/build.py` & `opencompass-0.2.3/opencompass/utils/build.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/dependency.py` & `opencompass-0.2.3/opencompass/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/file.py` & `opencompass-0.2.3/opencompass/utils/file.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/fileio.py` & `opencompass-0.2.3/opencompass/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/lark.py` & `opencompass-0.2.3/opencompass/utils/lark.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/logging.py` & `opencompass-0.2.3/opencompass/utils/logging.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/menu.py` & `opencompass-0.2.3/opencompass/utils/menu.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/prompt.py` & `opencompass-0.2.3/opencompass/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/run.py` & `opencompass-0.2.3/opencompass/utils/run.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/text_postprocessors.py` & `opencompass-0.2.3/opencompass/utils/text_postprocessors.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass/utils/types.py` & `opencompass-0.2.3/opencompass/utils/types.py`

 * *Files identical despite different names*

### Comparing `opencompass-0.2.2/opencompass.egg-info/PKG-INFO` & `opencompass-0.2.3/opencompass.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencompass
-Version: 0.2.2
+Version: 0.2.3
 Summary: A comprehensive toolkit for large model evaluation
 Home-page: https://github.com/open-compass/opencompass
 Author: OpenCompass Contributors
 Maintainer: OpenCompass Authors
 License: Apache License 2.0
 Description: <div align="center">
           <img src="docs/en/_static/image/logo.svg" width="500px"/>
@@ -13,39 +13,38 @@
         
         [![docs](https://readthedocs.org/projects/opencompass/badge)](https://opencompass.readthedocs.io/en)
         [![license](https://img.shields.io/github/license/InternLM/opencompass.svg)](https://github.com/open-compass/opencompass/blob/main/LICENSE)
         
         <!-- [![PyPI](https://badge.fury.io/py/opencompass.svg)](https://pypi.org/project/opencompass/) -->
         
         [🌐Website](https://opencompass.org.cn/) |
+        [📖CompassHub](https://hub.opencompass.org.cn/home) |
+        [📊CompassRank](https://rank.opencompass.org.cn/home) |
         [📘Documentation](https://opencompass.readthedocs.io/en/latest/) |
         [🛠️Installation](https://opencompass.readthedocs.io/en/latest/get_started/installation.html) |
         [🤔Reporting Issues](https://github.com/open-compass/opencompass/issues/new/choose)
         
         English | [简体中文](README_zh-CN.md)
         
         </div>
         
         <p align="center">
             👋 join us on <a href="https://discord.gg/KKwfEbFj7U" target="_blank">Discord</a> and <a href="https://r.vansin.top/?r=opencompass" target="_blank">WeChat</a>
         </p>
         
-        ## 📣 OpenCompass 2023 LLM Annual Leaderboard
+        ## 📣 OpenCompass 2.0
         
-        We are honored to have witnessed the tremendous progress of artificial general intelligence together with the community in the past year, and we are also very pleased that **OpenCompass** can help numerous developers and users.
+        We are thrilled to introduce OpenCompass 2.0, an advanced suite featuring three key components: [CompassKit](https://github.com/open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://rank.opencompass.org.cn/home).
+        ![oc20](https://github.com/tonysy/opencompass/assets/7881589/90dbe1c0-c323-470a-991e-2b37ab5350b2)
         
-        We announce the launch of the **OpenCompass 2023 LLM Annual Leaderboard** plan. We expect to release the annual leaderboard of the LLMs in January 2024, systematically evaluating the performance of LLMs in various capabilities such as language, knowledge, reasoning, creation, long-text, and agents.
+        **CompassRank** has been significantly enhanced into the leaderboards that now incorporates both open-source benchmarks and proprietary benchmarks. This upgrade allows for a more comprehensive evaluation of models across the industry.
         
-        At that time, we will release rankings for both open-source models and commercial API models, aiming to provide a comprehensive, objective, and neutral reference for the industry and research community.
+        **CompassHub** presents a pioneering benchmark browser interface, designed to simplify and expedite the exploration and utilization of an extensive array of benchmarks for researchers and practitioners alike. To enhance the visibility of your own benchmark within the community, we warmly invite you to contribute it to CompassHub. You may initiate the submission process by clicking [here](https://hub.opencompass.org.cn/dataset-submit).
         
-        We sincerely invite various large models to join the OpenCompass to showcase their performance advantages in different fields. At the same time, we also welcome researchers and developers to provide valuable suggestions and contributions to jointly promote the development of the LLMs. If you have any questions or needs, please feel free to [contact us](mailto:opencompass@pjlab.org.cn). In addition, relevant evaluation contents, performance statistics, and evaluation methods will be open-source along with the leaderboard release.
-        
-        We have provided the more details of the CompassBench 2023 in [Doc](docs/zh_cn/advanced_guides/compassbench_intro.md).
-        
-        Let's look forward to the release of the OpenCompass 2023 LLM Annual Leaderboard!
+        **CompassKit** is a powerful collection of evaluation toolkits specifically tailored for Large Language Models and Large Vision-language Models. It provides an extensive set of tools to assess and measure the performance of these complex models effectively. Welcome to try our toolkits for in your research and products.
         
         ## 🧭	Welcome
         
         to **OpenCompass**!
         
         Just like a compass guides us on our journey, OpenCompass will guide you through the complex landscape of evaluating large language models. With its powerful algorithms and intuitive interface, OpenCompass makes it easy to assess the quality and effectiveness of your NLP models.
         
@@ -56,20 +55,20 @@
         > **Attention**<br />
         > We launch the OpenCompass Collaboration project, welcome to support diverse evaluation benchmarks into OpenCompass!
         > Clike [Issue](https://github.com/open-compass/opencompass/issues/248) for more information.
         > Let's work together to build a more powerful OpenCompass toolkit!
         
         ## 🚀 What's New <a><img width="35" height="20" src="https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-4fe0-bbba-39ffb77730be.png"></a>
         
+        - **\[2024.02.29\]** We supported the MT-Bench, AlpacalEval and AlignBench, more information can be found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/subjective_evaluation.html) 🔥🔥🔥.
+        - **\[2024.01.30\]** We release OpenCompass 2.0. Click  [CompassKit](https://github.com/open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://rank.opencompass.org.cn/home) for more information ! 🔥🔥🔥.
         - **\[2024.01.17\]** We supported the evaluation of [InternLM2](https://github.com/open-compass/opencompass/blob/main/configs/eval_internlm2_keyset.py) and [InternLM2-Chat](https://github.com/open-compass/opencompass/blob/main/configs/eval_internlm2_chat_keyset.py), InternLM2 showed extremely strong performance in these tests, welcome to try! 🔥🔥🔥.
         - **\[2024.01.17\]** We supported the needle in a haystack test with multiple needles, more information can be found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/needleinahaystack_eval.html#id8) 🔥🔥🔥.
-        - **\[2023.12.28\]** We have enabled seamless evaluation of all models developed using [LLaMA2-Accessory](https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for comprehensive LLM development. 🔥🔥🔥.
-        - **\[2023.12.22\]** We have released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more details! 🔥🔥🔥.
-        - **\[2023.12.10\]** We have released [VLMEvalKit](https://github.com/open-compass/VLMEvalKit), a toolkit for evaluating vision-language models (VLMs), currently support 20+ VLMs and 7 multi-modal benchmarks (including MMBench series).
-        - **\[2023.12.10\]** We have supported Mistral AI's MoE LLM: **Mixtral-8x7B-32K**. Welcome to [MixtralKit](https://github.com/open-compass/MixtralKit) for more details about inference and evaluation.
+        - **\[2023.12.28\]** We have enabled seamless evaluation of all models developed using [LLaMA2-Accessory](https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for comprehensive LLM development.
+        - **\[2023.12.22\]** We have released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more details!
         
         > [More](docs/en/notes/news.md)
         
         ## ✨ Introduction
         
         ![image](https://github.com/open-compass/opencompass/assets/22607038/f45fe125-4aed-4f8c-8fe8-df4efb41a8ea)
         
@@ -83,15 +82,15 @@
         
         - **Modular design with high extensibility**: Want to add new models or datasets, customize an advanced task division strategy, or even support a new cluster management system? Everything about OpenCompass can be easily expanded!
         
         - **Experiment management and reporting mechanism**: Use config files to fully record each experiment, and support real-time reporting of results.
         
         ## 📊 Leaderboard
         
-        We provide [OpenCompass Leaderboard](https://opencompass.org.cn/rank) for the community to rank all public models and API models. If you would like to join the evaluation, please provide the model repository URL or a standard API interface to the email address `opencompass@pjlab.org.cn`.
+        We provide [OpenCompass Leaderboard](https://rank.opencompass.org.cn/home) for the community to rank all public models and API models. If you would like to join the evaluation, please provide the model repository URL or a standard API interface to the email address `opencompass@pjlab.org.cn`.
         
         <p align="right"><a href="#top">🔝Back to top</a></p>
         
         ## 🛠️ Installation
         
         Below are the steps for quick installation and datasets preparation.
         
@@ -118,16 +117,16 @@
         # also please install requiresments packages via `pip install -r requirements/api.txt` for API models if needed.
         ```
         
         ### 📂 Data Preparation
         
         ```bash
         # Download dataset to data/ folder
-        wget https://github.com/open-compass/opencompass/releases/download/0.1.8.rc1/OpenCompassData-core-20231110.zip
-        unzip OpenCompassData-core-20231110.zip
+        wget https://github.com/open-compass/opencompass/releases/download/0.2.2.rc1/OpenCompassData-core-20240207.zip
+        unzip OpenCompassData-core-20240207.zip
         ```
         
         Some third-party features, like Humaneval and Llama, may require additional steps to work properly, for detailed steps please refer to the [Installation Guide](https://opencompass.readthedocs.io/en/latest/get_started/installation.html).
         
         <p align="right"><a href="#top">🔝Back to top</a></p>
         
         ## 🏗️ ️Evaluation
@@ -424,18 +423,14 @@
               </td>
             </tr>
         </td>
             </tr>
           </tbody>
         </table>
         
-        ## OpenCompass Ecosystem
-        
-        <p align="right"><a href="#top">🔝Back to top</a></p>
-        
         ## 📖 Model Support
         
         <table align="center">
           <tbody>
             <tr align="center" valign="bottom">
               <td>
                 <b>Open-source Models</b>
@@ -457,20 +452,22 @@
         - [Baichuan](https://github.com/baichuan-inc)
         - [WizardLM](https://github.com/nlpxucan/WizardLM)
         - [ChatGLM2](https://github.com/THUDM/ChatGLM2-6B)
         - [ChatGLM3](https://github.com/THUDM/ChatGLM3-6B)
         - [TigerBot](https://github.com/TigerResearch/TigerBot)
         - [Qwen](https://github.com/QwenLM/Qwen)
         - [BlueLM](https://github.com/vivo-ai-lab/BlueLM)
+        - [Gemma](https://huggingface.co/google/gemma-7b)
         - ...
         
         </td>
         <td>
         
         - OpenAI
+        - Gemini
         - Claude
         - ZhipuAI(ChatGLM)
         - Baichuan
         - ByteDance(YunQue)
         - Huawei(PanGu)
         - 360
         - Baidu(ERNIEBot)
@@ -485,26 +482,26 @@
           </tbody>
         </table>
         
         <p align="right"><a href="#top">🔝Back to top</a></p>
         
         ## 🔜 Roadmap
         
-        - [ ] Subjective Evaluation
+        - [x] Subjective Evaluation
           - [ ] Release CompassAreana
-          - [ ] Subjective evaluation dataset.
+          - [x] Subjective evaluation.
         - [x] Long-context
-          - [ ] Long-context evaluation with extensive datasets.
+          - [x] Long-context evaluation with extensive datasets.
           - [ ] Long-context leaderboard.
-        - [ ] Coding
+        - [x] Coding
           - [ ] Coding evaluation leaderboard.
           - [x] Non-python language evaluation service.
-        - [ ] Agent
+        - [x] Agent
           - [ ] Support various agenet framework.
-          - [ ] Evaluation of tool use of the LLMs.
+          - [x] Evaluation of tool use of the LLMs.
         - [x] Robustness
           - [x] Support various attack method
         
         ## 👷‍♂️ Contributing
         
         We appreciate all contributions to improving OpenCompass. Please refer to the [contributing guideline](https://opencompass.readthedocs.io/en/latest/notes/contribution_guide.html) for the best practice.
```

#### html2text {}

```diff
@@ -1,79 +1,79 @@
-Metadata-Version: 2.1 Name: opencompass Version: 0.2.2 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opencompass Version: 0.2.3 Summary: A comprehensive
 toolkit for large model evaluation Home-page: https://github.com/open-compass/
 opencompass Author: OpenCompass Contributors Maintainer: OpenCompass Authors
 License: Apache License 2.0 Description:
                        [docs/en/_static/image/logo.svg]
 
     [![docs](https://readthedocs.org/projects/opencompass/badge)](https://
    opencompass.readthedocs.io/en) [![license](https://img.shields.io/github/
 license/InternLM/opencompass.svg)](https://github.com/open-compass/opencompass/
        blob/main/LICENSE) [ðWebsite](https://opencompass.org.cn/) |
-     [ðDocumentation](https://opencompass.readthedocs.io/en/latest/) |
-[ð ï¸Installation](https://opencompass.readthedocs.io/en/latest/get_started/
- installation.html) | [ð¤Reporting Issues](https://github.com/open-compass/
-   opencompass/issues/new/choose) English | [ç®ä½ä¸­æ](README_zh-CN.md)
+   [ðCompassHub](https://hub.opencompass.org.cn/home) | [ðCompassRank]
+     (https://rank.opencompass.org.cn/home) | [ðDocumentation](https://
+    opencompass.readthedocs.io/en/latest/) | [ð ï¸Installation](https://
+    opencompass.readthedocs.io/en/latest/get_started/installation.html) |
+[ð¤Reporting Issues](https://github.com/open-compass/opencompass/issues/new/
+               choose) English | [ç®ä½ä¸­æ](README_zh-CN.md)
                       ð join us on _D_i_s_c_o_r_d and _W_e_C_h_a_t
-## ð£ OpenCompass 2023 LLM Annual Leaderboard We are honored to have
-witnessed the tremendous progress of artificial general intelligence together
-with the community in the past year, and we are also very pleased that
-**OpenCompass** can help numerous developers and users. We announce the launch
-of the **OpenCompass 2023 LLM Annual Leaderboard** plan. We expect to release
-the annual leaderboard of the LLMs in January 2024, systematically evaluating
-the performance of LLMs in various capabilities such as language, knowledge,
-reasoning, creation, long-text, and agents. At that time, we will release
-rankings for both open-source models and commercial API models, aiming to
-provide a comprehensive, objective, and neutral reference for the industry and
-research community. We sincerely invite various large models to join the
-OpenCompass to showcase their performance advantages in different fields. At
-the same time, we also welcome researchers and developers to provide valuable
-suggestions and contributions to jointly promote the development of the LLMs.
-If you have any questions or needs, please feel free to [contact us](mailto:
-opencompass@pjlab.org.cn). In addition, relevant evaluation contents,
-performance statistics, and evaluation methods will be open-source along with
-the leaderboard release. We have provided the more details of the CompassBench
-2023 in [Doc](docs/zh_cn/advanced_guides/compassbench_intro.md). Let's look
-forward to the release of the OpenCompass 2023 LLM Annual Leaderboard! ## ð§­
-Welcome to **OpenCompass**! Just like a compass guides us on our journey,
-OpenCompass will guide you through the complex landscape of evaluating large
-language models. With its powerful algorithms and intuitive interface,
-OpenCompass makes it easy to assess the quality and effectiveness of your NLP
-models. ð©ð©ð© Explore opportunities at OpenCompass! We're currently
-**hiring full-time researchers/engineers and interns**. If you're passionate
-about LLM and OpenCompass, don't hesitate to reach out to us via [email]
-(mailto:zhangsongyang@pjlab.org.cn). We'd love to hear from you! ð¥ð¥ð¥
-We are delighted to announce that **the OpenCompass has been recommended by the
-Meta AI**, click [Get Started](https://ai.meta.com/llama/get-started/
-#validation) of Llama for more information. > **Attention**
+## ð£ OpenCompass 2.0 We are thrilled to introduce OpenCompass 2.0, an
+advanced suite featuring three key components: [CompassKit](https://github.com/
+open-compass), [CompassHub](https://hub.opencompass.org.cn/home), and
+[CompassRank](https://rank.opencompass.org.cn/home). ![oc20](https://
+github.com/tonysy/opencompass/assets/7881589/90dbe1c0-c323-470a-991e-
+2b37ab5350b2) **CompassRank** has been significantly enhanced into the
+leaderboards that now incorporates both open-source benchmarks and proprietary
+benchmarks. This upgrade allows for a more comprehensive evaluation of models
+across the industry. **CompassHub** presents a pioneering benchmark browser
+interface, designed to simplify and expedite the exploration and utilization of
+an extensive array of benchmarks for researchers and practitioners alike. To
+enhance the visibility of your own benchmark within the community, we warmly
+invite you to contribute it to CompassHub. You may initiate the submission
+process by clicking [here](https://hub.opencompass.org.cn/dataset-submit).
+**CompassKit** is a powerful collection of evaluation toolkits specifically
+tailored for Large Language Models and Large Vision-language Models. It
+provides an extensive set of tools to assess and measure the performance of
+these complex models effectively. Welcome to try our toolkits for in your
+research and products. ## ð§­ Welcome to **OpenCompass**! Just like a compass
+guides us on our journey, OpenCompass will guide you through the complex
+landscape of evaluating large language models. With its powerful algorithms and
+intuitive interface, OpenCompass makes it easy to assess the quality and
+effectiveness of your NLP models. ð©ð©ð© Explore opportunities at
+OpenCompass! We're currently **hiring full-time researchers/engineers and
+interns**. If you're passionate about LLM and OpenCompass, don't hesitate to
+reach out to us via [email](mailto:zhangsongyang@pjlab.org.cn). We'd love to
+hear from you! ð¥ð¥ð¥ We are delighted to announce that **the OpenCompass
+has been recommended by the Meta AI**, click [Get Started](https://ai.meta.com/
+llama/get-started/#validation) of Llama for more information. > **Attention**
 > We launch the OpenCompass Collaboration project, welcome to support diverse
 evaluation benchmarks into OpenCompass! > Clike [Issue](https://github.com/
 open-compass/opencompass/issues/248) for more information. > Let's work
 together to build a more powerful OpenCompass toolkit! ## ð What's New
 [https://user-images.githubusercontent.com/12782558/212848161-5e783dd6-11e8-
-4fe0-bbba-39ffb77730be.png]- **\[2024.01.17\]** We supported the evaluation of
-[InternLM2](https://github.com/open-compass/opencompass/blob/main/configs/
-eval_internlm2_keyset.py) and [InternLM2-Chat](https://github.com/open-compass/
-opencompass/blob/main/configs/eval_internlm2_chat_keyset.py), InternLM2 showed
-extremely strong performance in these tests, welcome to try! ð¥ð¥ð¥. -
-**\[2024.01.17\]** We supported the needle in a haystack test with multiple
-needles, more information can be found [here](https://
+4fe0-bbba-39ffb77730be.png]- **\[2024.02.29\]** We supported the MT-Bench,
+AlpacalEval and AlignBench, more information can be found [here](https://
 opencompass.readthedocs.io/en/latest/advanced_guides/
+subjective_evaluation.html) ð¥ð¥ð¥. - **\[2024.01.30\]** We release
+OpenCompass 2.0. Click [CompassKit](https://github.com/open-compass),
+[CompassHub](https://hub.opencompass.org.cn/home), and [CompassRank](https://
+rank.opencompass.org.cn/home) for more information ! ð¥ð¥ð¥. - **\
+[2024.01.17\]** We supported the evaluation of [InternLM2](https://github.com/
+open-compass/opencompass/blob/main/configs/eval_internlm2_keyset.py) and
+[InternLM2-Chat](https://github.com/open-compass/opencompass/blob/main/configs/
+eval_internlm2_chat_keyset.py), InternLM2 showed extremely strong performance
+in these tests, welcome to try! ð¥ð¥ð¥. - **\[2024.01.17\]** We supported
+the needle in a haystack test with multiple needles, more information can be
+found [here](https://opencompass.readthedocs.io/en/latest/advanced_guides/
 needleinahaystack_eval.html#id8) ð¥ð¥ð¥. - **\[2023.12.28\]** We have
 enabled seamless evaluation of all models developed using [LLaMA2-Accessory]
 (https://github.com/Alpha-VLLM/LLaMA2-Accessory), a powerful toolkit for
-comprehensive LLM development. ð¥ð¥ð¥. - **\[2023.12.22\]** We have
-released [T-Eval](https://github.com/open-compass/T-Eval), a step-by-step
-evaluation benchmark to gauge your LLMs on tool utilization. Welcome to our
-[Leaderboard](https://open-compass.github.io/T-Eval/leaderboard.html) for more
-details! ð¥ð¥ð¥. - **\[2023.12.10\]** We have released [VLMEvalKit]
-(https://github.com/open-compass/VLMEvalKit), a toolkit for evaluating vision-
-language models (VLMs), currently support 20+ VLMs and 7 multi-modal benchmarks
-(including MMBench series). - **\[2023.12.10\]** We have supported Mistral AI's
-MoE LLM: **Mixtral-8x7B-32K**. Welcome to [MixtralKit](https://github.com/open-
-compass/MixtralKit) for more details about inference and evaluation. > [More]
+comprehensive LLM development. - **\[2023.12.22\]** We have released [T-Eval]
+(https://github.com/open-compass/T-Eval), a step-by-step evaluation benchmark
+to gauge your LLMs on tool utilization. Welcome to our [Leaderboard](https://
+open-compass.github.io/T-Eval/leaderboard.html) for more details! > [More]
 (docs/en/notes/news.md) ## â¨ Introduction ![image](https://github.com/open-
 compass/opencompass/assets/22607038/f45fe125-4aed-4f8c-8fe8-df4efb41a8ea)
 OpenCompass is a one-stop platform for large model evaluation, aiming to
 provide a fair, open, and reproducible benchmark for large model evaluation.
 Its main features include: - **Comprehensive support for models and datasets**:
 Pre-support for 20+ HuggingFace and API models, a model evaluation scheme of
 70+ datasets with about 400,000 questions, comprehensively evaluating the
@@ -84,33 +84,34 @@
 shot, and chain-of-thought evaluations, combined with standard or dialogue-type
 prompt templates, to easily stimulate the maximum performance of various
 models. - **Modular design with high extensibility**: Want to add new models or
 datasets, customize an advanced task division strategy, or even support a new
 cluster management system? Everything about OpenCompass can be easily expanded!
 - **Experiment management and reporting mechanism**: Use config files to fully
 record each experiment, and support real-time reporting of results. ## ð
-Leaderboard We provide [OpenCompass Leaderboard](https://opencompass.org.cn/
-rank) for the community to rank all public models and API models. If you would
-like to join the evaluation, please provide the model repository URL or a
-standard API interface to the email address `opencompass@pjlab.org.cn`.
+Leaderboard We provide [OpenCompass Leaderboard](https://
+rank.opencompass.org.cn/home) for the community to rank all public models and
+API models. If you would like to join the evaluation, please provide the model
+repository URL or a standard API interface to the email address
+`opencompass@pjlab.org.cn`.
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ð ï¸ Installation Below are the steps for quick installation and datasets
 preparation. ### ð» Environment Setup #### Open-source Models with GPU
 ```bash conda create --name opencompass python=3.10 pytorch torchvision
 pytorch-cuda -c nvidia -c pytorch -y conda activate opencompass git clone
 https://github.com/open-compass/opencompass opencompass cd opencompass pip
 install -e . ``` #### API Models with CPU-only ```bash conda create -
 n opencompass python=3.10 pytorch torchvision torchaudio cpuonly -c pytorch -
 y conda activate opencompass git clone https://github.com/open-compass/
 opencompass opencompass cd opencompass pip install -e . # also please install
 requiresments packages via `pip install -r requirements/api.txt` for API models
 if needed. ``` ### ð Data Preparation ```bash # Download dataset to data/
 folder wget https://github.com/open-compass/opencompass/releases/download/
-0.1.8.rc1/OpenCompassData-core-20231110.zip unzip OpenCompassData-core-
-20231110.zip ``` Some third-party features, like Humaneval and Llama, may
+0.2.2.rc1/OpenCompassData-core-20240207.zip unzip OpenCompassData-core-
+20240207.zip ``` Some third-party features, like Humaneval and Llama, may
 require additional steps to work properly, for detailed steps please refer to
 the [Installation Guide](https://opencompass.readthedocs.io/en/latest/
 get_started/installation.html).
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ðï¸ ï¸Evaluation After ensuring that OpenCompass is installed correctly
 according to the above steps and the datasets are prepared, you can evaluate
 the performance of the LLaMA-7b model on the MMLU and C-Eval datasets using the
@@ -165,52 +166,51 @@
 DROP - OpenBookQA - NarrativeQA -       JigsawMultilingual
 SQuAD2.0 CCoonntteenntt    Qasper              - TruthfulQA
 SSuummmmaarryy - CSL -                         RRoobbuussttnneessss -
 LCSTS - XSum -                          AdvGLUE
 SummScreen CCoonntteenntt
 AAnnaallyyssiiss - EPRSTMT
 - LAMBADA - TNEWS
-## OpenCompass Ecosystem
-                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
 ## ð Model Support
-                OOppeenn--ssoouurrccee MMooddeellss                            AAPPII MMooddeellss
-- [InternLM](https://github.com/         - OpenAI - Claude - ZhipuAI(ChatGLM) -
-InternLM/InternLM) - [LLaMA](https://    Baichuan - ByteDance(YunQue) - Huawei
-github.com/facebookresearch/llama) -     (PanGu) - 360 - Baidu(ERNIEBot) -
-[Vicuna](https://github.com/lm-sys/      MiniMax(ABAB-Chat) - SenseTime(nova) -
-FastChat) - [Alpaca](https://github.com/ Xunfei(Spark) - â¦â¦
-tatsu-lab/stanford_alpaca) - [Baichuan]
-(https://github.com/baichuan-inc) -
-[WizardLM](https://github.com/nlpxucan/
-WizardLM) - [ChatGLM2](https://
-github.com/THUDM/ChatGLM2-6B) -
+               OOppeenn--ssoouurrccee MMooddeellss                            AAPPII MMooddeellss
+- [InternLM](https://github.com/        - OpenAI - Gemini - Claude - ZhipuAI
+InternLM/InternLM) - [LLaMA](https://   (ChatGLM) - Baichuan - ByteDance
+github.com/facebookresearch/llama) -    (YunQue) - Huawei(PanGu) - 360 - Baidu
+[Vicuna](https://github.com/lm-sys/     (ERNIEBot) - MiniMax(ABAB-Chat) -
+FastChat) - [Alpaca](https://           SenseTime(nova) - Xunfei(Spark) -
+github.com/tatsu-lab/stanford_alpaca) - â¦â¦
+[Baichuan](https://github.com/baichuan-
+inc) - [WizardLM](https://github.com/
+nlpxucan/WizardLM) - [ChatGLM2](https:/
+/github.com/THUDM/ChatGLM2-6B) -
 [ChatGLM3](https://github.com/THUDM/
 ChatGLM3-6B) - [TigerBot](https://
 github.com/TigerResearch/TigerBot) -
-[Qwen](https://github.com/QwenLM/Qwen) -
-[BlueLM](https://github.com/vivo-ai-lab/
-BlueLM) - ...
-                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
-## ð Roadmap - [ ] Subjective Evaluation - [ ] Release CompassAreana - [ ]
-Subjective evaluation dataset. - [x] Long-context - [ ] Long-context evaluation
-with extensive datasets. - [ ] Long-context leaderboard. - [ ] Coding - [ ]
-Coding evaluation leaderboard. - [x] Non-python language evaluation service. -
-[ ] Agent - [ ] Support various agenet framework. - [ ] Evaluation of tool use
-of the LLMs. - [x] Robustness - [x] Support various attack method ##
-ð·ââï¸ Contributing We appreciate all contributions to improving
-OpenCompass. Please refer to the [contributing guideline](https://
-opencompass.readthedocs.io/en/latest/notes/contribution_guide.html) for the
-best practice. ## ð¤ Acknowledgements Some code in this project is cited and
-modified from [OpenICL](https://github.com/Shark-NLP/OpenICL). Some datasets
-and prompt implementations are modified from [chain-of-thought-hub](https://
-github.com/FranxYao/chain-of-thought-hub) and [instruct-eval](https://
-github.com/declare-lab/instruct-eval). ## ðï¸ Citation ```bibtex @misc
-{2023opencompass, title={OpenCompass: A Universal Evaluation Platform for
-Foundation Models}, author={OpenCompass Contributors}, howpublished = {\url
-{https://github.com/open-compass/opencompass}}, year={2023} } ```
+[Qwen](https://github.com/QwenLM/Qwen)
+- [BlueLM](https://github.com/vivo-ai-
+lab/BlueLM) - [Gemma](https://
+huggingface.co/google/gemma-7b) - ...
+                                                                _ð____B_a_c_k_ _t_o_ _t_o_p
+## ð Roadmap - [x] Subjective Evaluation - [ ] Release CompassAreana - [x]
+Subjective evaluation. - [x] Long-context - [x] Long-context evaluation with
+extensive datasets. - [ ] Long-context leaderboard. - [x] Coding - [ ] Coding
+evaluation leaderboard. - [x] Non-python language evaluation service. - [x]
+Agent - [ ] Support various agenet framework. - [x] Evaluation of tool use of
+the LLMs. - [x] Robustness - [x] Support various attack method ## ð·ââï¸
+Contributing We appreciate all contributions to improving OpenCompass. Please
+refer to the [contributing guideline](https://opencompass.readthedocs.io/en/
+latest/notes/contribution_guide.html) for the best practice. ## ð¤
+Acknowledgements Some code in this project is cited and modified from [OpenICL]
+(https://github.com/Shark-NLP/OpenICL). Some datasets and prompt
+implementations are modified from [chain-of-thought-hub](https://github.com/
+FranxYao/chain-of-thought-hub) and [instruct-eval](https://github.com/declare-
+lab/instruct-eval). ## ðï¸ Citation ```bibtex @misc{2023opencompass, title=
+{OpenCompass: A Universal Evaluation Platform for Foundation Models}, author=
+{OpenCompass Contributors}, howpublished = {\url{https://github.com/open-
+compass/opencompass}}, year={2023} } ```
                                                                 _ð____B_a_c_k_ _t_o_ _t_o_p
 Keywords: AI,NLP,in-context learning,large language
 model,evaluation,benchmark,llm Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Requires-Python: >=3.8.0 Description-
```

### Comparing `opencompass-0.2.2/opencompass.egg-info/SOURCES.txt` & `opencompass-0.2.3/opencompass.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 opencompass.egg-info/PKG-INFO
 opencompass.egg-info/SOURCES.txt
 opencompass.egg-info/dependency_links.txt
 opencompass.egg-info/requires.txt
 opencompass.egg-info/top_level.txt
 opencompass/datasets/FinanceIQ.py
 opencompass/datasets/GaokaoBench.py
+opencompass/datasets/OpenFinData.py
 opencompass/datasets/TheoremQA.py
 opencompass/datasets/__init__.py
 opencompass/datasets/advglue.py
 opencompass/datasets/afqmcd.py
 opencompass/datasets/anli.py
 opencompass/datasets/anthropics_evals.py
 opencompass/datasets/arc.py
@@ -186,14 +187,27 @@
 opencompass/datasets/longbench/longbench_qasper.py
 opencompass/datasets/longbench/longbench_qmsum.py
 opencompass/datasets/longbench/longbench_repobench.py
 opencompass/datasets/longbench/longbench_samsum.py
 opencompass/datasets/longbench/longbench_trec.py
 opencompass/datasets/longbench/longbench_trivia_qa.py
 opencompass/datasets/longbench/longbench_vcsum.py
+opencompass/datasets/lveval/__init__.py
+opencompass/datasets/lveval/evaluators.py
+opencompass/datasets/lveval/lveval_cmrc_mixup.py
+opencompass/datasets/lveval/lveval_dureader_mixup.py
+opencompass/datasets/lveval/lveval_factrecall_en.py
+opencompass/datasets/lveval/lveval_factrecall_zh.py
+opencompass/datasets/lveval/lveval_hotpotwikiqa_mixup.py
+opencompass/datasets/lveval/lveval_lic_mixup.py
+opencompass/datasets/lveval/lveval_loogle_CR_mixup.py
+opencompass/datasets/lveval/lveval_loogle_MIR_mixup.py
+opencompass/datasets/lveval/lveval_loogle_SD_mixup.py
+opencompass/datasets/lveval/lveval_multifieldqa_en_mixup.py
+opencompass/datasets/lveval/lveval_multifieldqa_zh_mixup.py
 opencompass/datasets/medbench/__init__.py
 opencompass/datasets/medbench/constructions.py
 opencompass/datasets/medbench/dataset_loader.py
 opencompass/datasets/medbench/evaluation.py
 opencompass/datasets/medbench/math_equivalence.py
 opencompass/datasets/medbench/medbench.py
 opencompass/datasets/medbench/post_process.py
@@ -230,21 +244,24 @@
 opencompass/models/ai360_api.py
 opencompass/models/alaya.py
 opencompass/models/baichuan_api.py
 opencompass/models/baidu_api.py
 opencompass/models/base.py
 opencompass/models/base_api.py
 opencompass/models/bytedance_api.py
+opencompass/models/gemini_api.py
 opencompass/models/glm.py
 opencompass/models/huggingface.py
 opencompass/models/intern_model.py
+opencompass/models/krgpt_api.py
 opencompass/models/lagent.py
 opencompass/models/langchain.py
 opencompass/models/lightllm_api.py
 opencompass/models/llama2.py
+opencompass/models/lmdeploy_pytorch.py
 opencompass/models/minimax_api.py
 opencompass/models/mixtral.py
 opencompass/models/modelscope.py
 opencompass/models/moonshot_api.py
 opencompass/models/nanbeige_api.py
 opencompass/models/openai_api.py
 opencompass/models/pangu_api.py
@@ -268,14 +285,15 @@
 opencompass/openicl/icl_evaluator/icl_aucroc_evaluator.py
 opencompass/openicl/icl_evaluator/icl_base_evaluator.py
 opencompass/openicl/icl_evaluator/icl_circular_evaluator.py
 opencompass/openicl/icl_evaluator/icl_em_evaluator.py
 opencompass/openicl/icl_evaluator/icl_hf_evaluator.py
 opencompass/openicl/icl_evaluator/icl_jieba_rouge_evaluator.py
 opencompass/openicl/icl_evaluator/icl_misc_evaluator.py
+opencompass/openicl/icl_evaluator/icl_plugin_evaluator.py
 opencompass/openicl/icl_evaluator/icl_toxic_evaluator.py
 opencompass/openicl/icl_evaluator/lm_evaluator.py
 opencompass/openicl/icl_inferencer/__init__.py
 opencompass/openicl/icl_inferencer/icl_agent_inferencer.py
 opencompass/openicl/icl_inferencer/icl_attack_inferencer.py
 opencompass/openicl/icl_inferencer/icl_base_inferencer.py
 opencompass/openicl/icl_inferencer/icl_chat_inferencer.py
@@ -314,14 +332,15 @@
 opencompass/runners/local_api.py
 opencompass/runners/slurm.py
 opencompass/runners/slurm_sequential.py
 opencompass/summarizers/__init__.py
 opencompass/summarizers/circular.py
 opencompass/summarizers/default.py
 opencompass/summarizers/multi_model.py
+opencompass/summarizers/needlebench.py
 opencompass/summarizers/summarizer_pretrain.py
 opencompass/summarizers/subjective/__init__.py
 opencompass/summarizers/subjective/alignmentbench.py
 opencompass/summarizers/subjective/alpacaeval.py
 opencompass/summarizers/subjective/compass_arena.py
 opencompass/summarizers/subjective/corev2.py
 opencompass/summarizers/subjective/creationbench.py
```

### Comparing `opencompass-0.2.2/opencompass.egg-info/requires.txt` & `opencompass-0.2.3/opencompass.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 cpm_kernels
 datasets>=2.12.0
 einops==0.5.0
 evaluate>=0.3.0
 fairscale
 func_timeout
 fuzzywuzzy
+immutabledict
 jieba
+langdetect
 ltp
 mmengine-lite
 nltk==3.8
 numpy==1.23.4
 openai
 OpenCC
 opencv-python-headless
```

### Comparing `opencompass-0.2.2/setup.py` & `opencompass-0.2.3/setup.py`

 * *Files identical despite different names*

