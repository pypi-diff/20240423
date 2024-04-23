# Comparing `tmp/seqnado-0.5.0.tar.gz` & `tmp/seqnado-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqnado-0.5.0.tar", last modified: Mon Apr  1 16:05:03 2024, max compression
+gzip compressed data, was "seqnado-0.5.1.tar", last modified: Tue Apr 23 14:24:55 2024, max compression
```

## Comparing `seqnado-0.5.0.tar` & `seqnado-0.5.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.113903 seqnado-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.101903 seqnado-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 16:04:53.000000 seqnado-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.101903 seqnado-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 16:04:53.000000 seqnado-0.5.0/.github/workflows/build_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-01 16:04:53.000000 seqnado-0.5.0/.github/workflows/publish_pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-01 16:04:53.000000 seqnado-0.5.0/.github/workflows/test_pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-01 16:04:53.000000 seqnado-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-01 16:04:53.000000 seqnado-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-01 16:04:53.000000 seqnado-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-01 16:04:53.000000 seqnado-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-01 16:05:03.109902 seqnado-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 16:04:53.000000 seqnado-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 16:04:53.000000 seqnado-0.5.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.101903 seqnado-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-01 16:04:53.000000 seqnado-0.5.0/docs/cluster_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-01 16:04:53.000000 seqnado-0.5.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-01 16:04:53.000000 seqnado-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-01 16:04:53.000000 seqnado-0.5.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-01 16:04:53.000000 seqnado-0.5.0/docs/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 16:04:53.000000 seqnado-0.5.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-01 16:04:53.000000 seqnado-0.5.0/environment_minimal.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-04-01 16:04:53.000000 seqnado-0.5.0/install_seqnado.sh
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-01 16:04:53.000000 seqnado-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 16:04:53.000000 seqnado-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 16:05:02.000000 seqnado-0.5.0/seqnado/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/data/logo.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33825 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/design.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/workflow/config/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1528 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/config/config.yaml.jinja
--rwxr-xr-x   0 runner    (1001) docker     (127)    16268 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/config/deseq2.qmd.jinja
--rwxr-xr-x   0 runner    (1001) docker     (127)     4282 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/config/preset_genomes.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/envs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.097903 seqnado-0.5.0/seqnado/workflow/envs/profiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/workflow/envs/profiles/profile_singularity/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/envs/profiles/profile_singularity/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/workflow/envs/profiles/profile_slurm_singularity/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/envs/profiles/profile_slurm_singularity/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.105903 seqnado-0.5.0/seqnado/workflow/envs/profiles/profile_test/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/envs/profiles/profile_test/config.v8+.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.109902 seqnado-0.5.0/seqnado/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/align.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/align_rna.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/alignment_counts.smk
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/alignment_post_processing.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/custom_genome.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/deseq2_rna.smk
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/exogenous_norm.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/fastq_screen.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/fastq_trim.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/heatmap.smk
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/hub.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/motif.smk
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/peak_call_chip.smk
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/peak_call_grouped.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/peak_call_other.smk
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/pileup_default.smk
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/pileup_grouped.smk
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/pileup_norm.smk
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/qc.smk
--rwxr-xr-x   0 runner    (1001) docker     (127)     2880 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/rules/variant.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.109902 seqnado-0.5.0/seqnado/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/calculate_scaling_norm_factors.r
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/calculate_spikein_norm_factors.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/calculate_spikein_norm_factors.r
--rwxr-xr-x   0 runner    (1001) docker     (127)     1330 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/calculate_spikein_norm_orlando.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/create_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/get_salmon_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/remove_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/remove_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/scripts/shift_alignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/snakefile_atac
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/snakefile_build_index
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/snakefile_chip
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/snakefile_rna
--rwxr-xr-x   0 runner    (1001) docker     (127)     2216 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado/workflow/snakefile_snp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.109902 seqnado-0.5.0/seqnado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-01 16:05:03.000000 seqnado-0.5.0/seqnado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-01 16:05:03.000000 seqnado-0.5.0/seqnado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:05:03.000000 seqnado-0.5.0/seqnado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-01 16:05:03.000000 seqnado-0.5.0/seqnado.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 16:05:03.000000 seqnado-0.5.0/seqnado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 16:05:03.000000 seqnado-0.5.0/seqnado.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado_dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)   254229 2024-04-01 16:04:53.000000 seqnado-0.5.0/seqnado_logo.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:05:03.113903 seqnado-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:04:53.000000 seqnado-0.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 16:04:53.000000 seqnado-0.5.0/testing.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:05:03.109902 seqnado-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-04-01 16:04:53.000000 seqnado-0.5.0/tests/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.595202 seqnado-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.583202 seqnado-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-23 14:24:46.000000 seqnado-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.583202 seqnado-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-23 14:24:46.000000 seqnado-0.5.1/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 14:24:46.000000 seqnado-0.5.1/.github/workflows/publish_pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-23 14:24:46.000000 seqnado-0.5.1/.github/workflows/test_pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 14:24:46.000000 seqnado-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-23 14:24:46.000000 seqnado-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-23 14:24:46.000000 seqnado-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-23 14:24:46.000000 seqnado-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-23 14:24:55.595202 seqnado-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-23 14:24:46.000000 seqnado-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-23 14:24:46.000000 seqnado-0.5.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.583202 seqnado-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-23 14:24:46.000000 seqnado-0.5.1/docs/cluster_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-23 14:24:46.000000 seqnado-0.5.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-23 14:24:46.000000 seqnado-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-23 14:24:46.000000 seqnado-0.5.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-23 14:24:46.000000 seqnado-0.5.1/docs/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-23 14:24:46.000000 seqnado-0.5.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 14:24:46.000000 seqnado-0.5.1/environment_minimal.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-04-23 14:24:46.000000 seqnado-0.5.1/install_seqnado.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-23 14:24:46.000000 seqnado-0.5.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-23 14:24:46.000000 seqnado-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 14:24:55.000000 seqnado-0.5.1/seqnado/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/data/logo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    37326 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/workflow/config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1528 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/config/config.yaml.jinja
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16307 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/config/deseq2.qmd.jinja
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4282 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/config/preset_genomes.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/envs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.579202 seqnado-0.5.1/seqnado/workflow/envs/profiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/workflow/envs/profiles/profile_singularity/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/envs/profiles/profile_singularity/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/workflow/envs/profiles/profile_slurm_singularity/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/envs/profiles/profile_slurm_singularity/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.587201 seqnado-0.5.1/seqnado/workflow/envs/profiles/profile_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/envs/profiles/profile_test/config.v8+.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.591202 seqnado-0.5.1/seqnado/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/align.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/align_rna.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/alignment_counts.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/alignment_post_processing.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/custom_genome.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/deseq2_rna.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/exogenous_norm.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/fastq_screen.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/fastq_trim.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/heatmap.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/hub.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/motif.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/peak_call_chip.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/peak_call_grouped.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/peak_call_other.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/pileup_default.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/pileup_grouped.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/pileup_norm.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/qc.smk
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2880 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/rules/variant.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.595202 seqnado-0.5.1/seqnado/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/calculate_scaling_factors.R
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/calculate_spikein_norm_factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/calculate_spikein_norm_factors_rna.R
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1330 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/calculate_spikein_norm_orlando.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/create_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/get_salmon_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/remove_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/remove_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/scripts/shift_alignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/snakefile_atac
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/snakefile_build_index
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/snakefile_chip
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/snakefile_rna
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2216 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado/workflow/snakefile_snp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.595202 seqnado-0.5.1/seqnado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-23 14:24:55.000000 seqnado-0.5.1/seqnado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-23 14:24:55.000000 seqnado-0.5.1/seqnado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:24:55.000000 seqnado-0.5.1/seqnado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 14:24:55.000000 seqnado-0.5.1/seqnado.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-23 14:24:55.000000 seqnado-0.5.1/seqnado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 14:24:55.000000 seqnado-0.5.1/seqnado.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   254229 2024-04-23 14:24:46.000000 seqnado-0.5.1/seqnado_logo.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:24:55.595202 seqnado-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:24:46.000000 seqnado-0.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 14:24:46.000000 seqnado-0.5.1/testing.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:24:55.595202 seqnado-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-04-23 14:24:46.000000 seqnado-0.5.1/tests/test_pipelines.py
```

### Comparing `seqnado-0.5.0/.github/workflows/build_docs.yml` & `seqnado-0.5.1/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/.github/workflows/publish_pypi_release.yml` & `seqnado-0.5.1/.github/workflows/publish_pypi_release.yml`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/.github/workflows/test_pipelines.yml` & `seqnado-0.5.1/.github/workflows/test_pipelines.yml`

 * *Files 8% similar despite different names*

```diff
@@ -49,8 +49,14 @@
     - name: Test design works
       shell: pwsh
       run: |
         seqnado-design chip tests/data/fastq/CTCF*.fastq.gz
     - name: Test with pytest
       shell: pwsh
       run: |
-        pytest -s --cores 4
+        pytest -vv -s --cov=./ --cov-report=xml --cores 4
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v4.0.1
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
+        slug: alsmith151/SeqNado
+
```

### Comparing `seqnado-0.5.0/.pre-commit-config.yaml` & `seqnado-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/LICENSE` & `seqnado-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/PKG-INFO` & `seqnado-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: seqnado
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pipelines for genomics analysis
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>, Catherine Chahrour <catherine.chahrour@msdtc.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Homepage, https://github.com/alsmith151/seqnado
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: cookiecutter
 Requires-Dist: drmaa
 Requires-Dist: pandas
+Requires-Dist: pandera
 Requires-Dist: pulp<=2.7.0
 Requires-Dist: pydantic
 Requires-Dist: pyranges
 Requires-Dist: pyyaml
 Requires-Dist: seaborn
 Requires-Dist: setuptools_scm
 Requires-Dist: snakemake-wrapper-utils
```

### Comparing `seqnado-0.5.0/docs/cluster_config.md` & `seqnado-0.5.1/docs/cluster_config.md`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/docs/index.md` & `seqnado-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/docs/installation.md` & `seqnado-0.5.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/docs/pipeline.md` & `seqnado-0.5.1/docs/pipeline.md`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/install_seqnado.sh` & `seqnado-0.5.1/install_seqnado.sh`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/mkdocs.yml` & `seqnado-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/pyproject.toml` & `seqnado-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 license = {text = "GNU GENERAL PUBLIC LICENSE Version 3"}
 dynamic = ["version"]
 dependencies = [
     "click",
     "cookiecutter",
     "drmaa",
     "pandas",
+    "pandera",
     "pulp<=2.7.0",
     "pydantic",
     "pyranges",
     "pyyaml",
     "seaborn",
     "setuptools_scm",
     "snakemake-wrapper-utils",
```

### Comparing `seqnado-0.5.0/seqnado/cli.py` & `seqnado-0.5.1/seqnado/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -49,33 +49,49 @@
 @click.option("-o", "--output", default="design.csv", help="Output file name")
 def cli_design(method, files, output="design.csv"):
     """
     Generates a SeqNado design file from a list of files.
     """
     import pathlib
     from seqnado.design import Design, DesignIP, FastqFile, FastqFileIP
-
+    
     if not files:
-        files = list(pathlib.Path(".").glob("*.fastq.gz"))
+        potential_file_locations = [
+            ".",
+            "fastqs",
+            "fastq",
+            "data",
+            "data/fastqs",
+        ]
+
+        for location in potential_file_locations:
+            files = list(pathlib.Path(location).glob("*.fastq.gz"))
+            if files:
+                break
 
         if not files:
-            raise ValueError("No fastq files provided or found in current directory.")
+            logger.error("No fastq files provided or found in current directory")
+            logger.error(f"""
+                         Fastq files can be provided as arguments or found in the following directories:
+                         {potential_file_locations}
+                         """)
+            raise ValueError("No fastq files provided or found in current directory" )
+
+
 
     if not method == "chip":
-        design = Design.from_fastq_files([FastqFile(path=fq) for fq in files])
+        design = Design.from_fastq_files(files)
     else:
 
-        design = DesignIP.from_fastq_files([FastqFileIP(path=fq) for fq in files])
+        design = DesignIP.from_fastq_files(files)
 
     (
         design.to_dataframe()
         .assign(scale_group="all")
-        .reset_index()
-        .rename(columns={"index": "sample"})
-        .sort_values("sample")
+        .sort_values("sample_name")
         .to_csv(output, index=False)
     )
 
 
 @click.command(context_settings=dict(ignore_unknown_options=True))
 @click.argument(
     "method",
@@ -88,38 +104,65 @@
     help="""Pre-set snakemake job profile to use for pipeline run:
             lc: local conda environment
             ls: local singularity environment
             ss: slurm singularity environment (runs jobs on cluster)
             """,
     type=click.Choice(choices=["lc", "ls", "ss"]),
 )
+@click.option(
+    "--clean-symlinks",
+    is_flag=True,
+    help="Remove symlinks created by previous runs. Useful for re-running pipeline after misconfiguration.",
+)
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    help="Increase logging verbosity",
+)
 @click.argument("pipeline_options", nargs=-1, type=click.UNPROCESSED)
 def cli_pipeline(
     method,
     pipeline_options,
     help=False,
     preset="local",
     version=False,
-    apptainer_args="",
+    verbose=False,
+    clean_symlinks=False,
 ):
     """Runs the data processing pipeline"""
 
     from seqnado.helpers import extract_cores_from_options
 
     if version:
         from importlib.metadata import version
 
         _version = version("seqnado")
 
         _version = version("seqnado")
         print(f"SeqNado version {_version}")
         sys.exit(0)
+    
+    if verbose:
+        logger.remove()
+        logger.add(sys.stderr, level="DEBUG")
+    else:
+        logger.remove()
+        logger.add(sys.stderr, level="INFO")
 
     pipeline_options, cores = extract_cores_from_options(pipeline_options)
 
+    # Removes old symlinks if requested
+    if clean_symlinks:
+        logger.info("Cleaning symlinks")
+        links = pathlib.Path("seqnado_output/fastqs").glob("*")
+        for link in links:
+            if link.is_symlink():
+                link.unlink()
+    
     cmd = [
         "snakemake",
         "-c",
         str(cores),
         "--snakefile",
         os.path.join(PACKAGE_DIR, "workflow", f"snakefile_{method.replace('-', '_')}"),
     ]
```

### Comparing `seqnado-0.5.0/seqnado/config.py` & `seqnado-0.5.1/seqnado/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 homer:
     use_input: true
     maketagdirectory:
     makebigwig:
     findpeaks:
 
 deeptools:
-    threads: 16
+    threads: 8
     alignmentsieve: --minMappingQuality 30 
     bamcoverage: --extendReads -bs 1 --normalizeUsing RPKM
 
 macs:
     version: 2
     callpeak: -f BAMPE
```

### Comparing `seqnado-0.5.0/seqnado/data/logo.txt` & `seqnado-0.5.1/seqnado/data/logo.txt`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/design.py` & `seqnado-0.5.1/seqnado/design.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import os
 import pathlib
 import re
-from typing import Any, Dict, List, Optional, Union, Literal, LiteralString
 import sys
+from typing import Any, Dict, List, Literal, LiteralString, Optional, Union
 
+import numpy as np
 import pandas as pd
 from loguru import logger
-from pydantic import BaseModel, Field, computed_field
+from pydantic import BaseModel, Field, computed_field, field_validator
 from snakemake.io import expand
-
-
-logger.add(sink=sys.stderr, level="WARNING")
+import pandera
+from pandera.typing import Index, DataFrame, Series
 
 
 def is_path(path: Optional[Union[str, pathlib.Path]]) -> Optional[pathlib.Path]:
     if isinstance(path, str):
         p = pathlib.Path(path)
     elif isinstance(path, pathlib.Path):
         p = path
@@ -28,17 +29,21 @@
 
 class FastqFile(BaseModel):
     path: pathlib.Path
 
     def model_post_init(self, *args):
         self.path = pathlib.Path(self.path).resolve()
 
-        if not self.path.exists():
+        if not self.path.exists() or str(self.path) in ["-", ".", "", None]:
             raise FileNotFoundError(f"{self.path} does not exist.")
 
+    @property
+    def stem(self):
+        return pathlib.Path(str(self.path).removesuffix(".gz")).stem
+
     @computed_field
     @property
     def sample_name(self) -> str:
         name = pathlib.Path(str(self.path).removesuffix(".gz")).stem
         if name.endswith("_001"):
             name = name.removesuffix("_001")
         return name
@@ -155,19 +160,43 @@
             "",
             self.sample_name,
         )
 
         return base
 
 
-class AssayNonIP(BaseModel):
+class Metadata(BaseModel):
+    deseq2: Optional[str] = None
+    merge: Optional[str] = None
+    scale_group: Union[str, int] = "all"
+
+    @field_validator("deseq2", "merge")
+    @classmethod
+    def prevent_none(cls, v):
+        none_vals = [
+            None,
+            "None",
+            "none",
+            "null",
+            "Null",
+            "NULL",
+            ".",
+            "",
+            "NA",
+            np.nan,
+        ]
+        if any([v == n for n in none_vals]):
+            assert v is not None, "None is not allowed when setting metadata"
+        return v
+
+
+class FastqSet(BaseModel):
     name: str = Field(default=None, description="Name of the assay")
     r1: FastqFile
     r2: Optional[FastqFile] = None
-    metadata: Optional[dict] = None
 
     @property
     def fastq_paths(self):
         return [self.r1.path, self.r2.path] if self.is_paired else [self.r1.path]
 
     @property
     def is_paired(self):
@@ -191,426 +220,488 @@
             return cls(name=sample_name, r1=fq[0], **kwargs)
         elif len(fq) == 2:
             return cls(name=sample_name, r1=fq[0], r2=fq[1], **kwargs)
         else:
             raise ValueError(f"Invalid number of fastq files for {sample_name}.")
 
 
-class AssayIP(AssayNonIP):
-    name: str = Field(default=None, description="Name of the assay")
+class FastqSetIP(FastqSet):
+    name: str = Field(default=None, description="Name of the sample set")
     r1: FastqFileIP
     r2: Optional[FastqFileIP] = None
-    metadata: Optional[dict] = None
+
+    @property
+    def ip_or_control_name(self) -> str:
+        return self.r1.ip
+
+    @property
+    def sample_name(self) -> str:
+        return f"{self.name}_{self.ip_or_control_name}"
+
+    @property
+    def sample_name_base(self) -> str:
+        return self.r1.sample_base_without_ip
 
     @property
     def is_control(self) -> bool:
         return self.r1.is_control
 
 
-class ExperimentIP(BaseModel):
-    ip_files: AssayIP
-    control_files: AssayIP = None
-    name: str = Field(default=None, description="Name of the assay")
-    ip: str = Field(default=None, description="IP performed on the sample")
-    control: Optional[str] = Field(
-        default=None, description="IP performed on the control"
-    )
-    metadata: Optional[dict] = None
+class IPExperiment(BaseModel):
+    ip: FastqSetIP
+    control: Optional[FastqSetIP] = None
 
-    def model_post_init(self, *args):
-        if self.name is None:
-            self.name = (
-                f"{self.ip_files.r1.sample_base_without_ip}_{self.ip_files.r1.ip}"
-            )
+    @property
+    def has_control(self) -> bool:
+        return self.control is not None
 
-        if self.ip is None:
-            self.ip = self.ip_files.r1.ip
+    @property
+    def ip_set_fullname(self) -> str:
+        return self.ip.sample_name
 
-        if self.control is None and self.control_files is not None:
-            self.control = self.control_files.r1.ip
+    @property
+    def control_fullname(self) -> str:
+        return self.control.sample_name
 
-    @computed_field
     @property
-    def is_paired(self) -> bool:
-        return self.ip_files.is_paired
+    def ip_performed(self) -> str:
+        return self.ip.ip_or_control_name
 
-    @classmethod
-    def from_fastq_files(cls, fq: List[FastqFileIP], **kwargs):
-        """
-        Create a Experiment object from a list of FastqFiles.
+    @property
+    def control_performed(self) -> str:
+        return self.control.ip_or_control_name
 
-        """
+    @property
+    def fastqs_are_paired(self) -> bool:
 
-        fq_ip = [f for f in fq if not f.is_control]
-        fq_control = [f for f in fq if f.is_control]
+        ip = self.ip.is_paired
+        control = self.control.is_paired if self.control else True
+        return ip and control
 
-        assert len(fq_ip) > 0, "No IP files found"
-        assert len(fq_ip) < 3, "Too many IP files found"
-        assert len(fq_control) < 3, "Too many control files found"
 
-        if len(fq_control) == 0:
-            return cls(ip_files=AssayIP.from_fastq_files(fq_ip, **kwargs), **kwargs)
-        else:
-            return cls(
-                ip_files=AssayIP.from_fastq_files(fq_ip, **kwargs),
-                control_files=AssayIP.from_fastq_files(fq_control, **kwargs),
-                **kwargs,
-            )
+class DataFrameDesign(pandera.DataFrameModel):
+    sample_name: Series[str]
+    r1: Series[str] = pandera.Field(coerce=True)
+    r2: Series[str] = pandera.Field(coerce=True, nullable=True)
+    scale_group: Series[str]
+    deseq2: Optional[Series[str]] = pandera.Field()
+    merge: Optional[Series[str]] = pandera.Field()
+
+
+class DataFrameDesignIP(pandera.DataFrameModel):
+    sample_name: Series[str]
+    ip: Series[str] = pandera.Field(coerce=True)
+    control: Optional[Series[str]] = pandera.Field(coerce=True, nullable=True)
+    ip_r1: Series[str] = pandera.Field(coerce=True)
+    ip_r2: Series[str] = pandera.Field(coerce=True, nullable=True)
+    control_r1: Optional[Series[str]] = pandera.Field(coerce=True, nullable=True)
+    control_r2: Optional[Series[str]] = pandera.Field(coerce=True, nullable=True)
+    scale_group: Series[str]
 
 
 class Design(BaseModel):
-    assays: Dict[str, AssayNonIP] = Field(
-        default_factory=dict,
-        description="Dictionary of assay classes keyed by sample name",
-    )
+    fastq_sets: List[FastqSet]
+    metadata: List[Metadata]
 
-    @computed_field
     @property
     def sample_names(self) -> List[str]:
-        return list(self.assays.keys())
+        return [f.name for f in self.fastq_sets]
 
-    @computed_field
     @property
     def fastq_paths(self) -> List[pathlib.Path]:
         paths = []
-        for assay in self.assays.values():
-            paths.append(assay.r1.path)
-            if assay.r2 is not None:
-                paths.append(assay.r2.path)
-
+        for fastq_set in self.fastq_sets:
+            paths.append(fastq_set.r1.path)
+            if fastq_set.r2 is not None:
+                paths.append(fastq_set.r2.path)
         return paths
 
-    def query(self, sample_name: str) -> AssayNonIP:
-        return self.assays[sample_name]
-
-    @classmethod
-    def from_fastq_files(cls, fq: List[FastqFile], **kwargs):
+    def query(self, sample_name: str) -> FastqSet:
         """
-        Create a SampleInfo object from a list of FastqFiles.
-
+        Extract a sample pair of fastq files from the design.
         """
 
-        sample_names = set([f.sample_base for f in fq])
-        assays = {}
-        for sample_name in sample_names:
-            assays[sample_name] = AssayNonIP.from_fastq_files(
-                [f for f in fq if f.sample_base == sample_name], **kwargs
-            )
+        for fastq_set in self.fastq_sets:
+            if fastq_set.name == sample_name:
+                return fastq_set
 
-        return cls(assays=assays, **kwargs)
+        raise ValueError(f"Could not find sample with name {sample_name}")
 
     @classmethod
-    def from_directory(
-        cls, path: pathlib.Path, metadata: Dict[str, Any] = None, **kwargs
-    ):
+    def from_fastq_files(cls, fq: List[Union[str, pathlib.Path]], **kwargs):
         """
-        Create a SampleInfo object from a directory of fastq files.
-
+        Generate a Design object from a list of FastqFiles.
         """
+        import pandas as pd
 
-        fq = list(pathlib.Path(path).glob("*.fastq.gz"))
-        fq = sorted([FastqFile(path=f) for f in fq])
-        return cls.from_fastq_files(fq, metadata=metadata, **kwargs)
+        fq = sorted([pathlib.Path(f) for f in fq])
 
-    @classmethod
-    def from_dataframe(cls, df: pd.DataFrame, simplified: bool = True, **kwargs):
-        assays = {}
-        for assay_name, row in df.iterrows():
-            if simplified:
-                metadata = {}
-                for k, v in row.items():
-                    if k not in ["r1", "r2"]:
-                        metadata[k] = v
-                assays[assay_name] = AssayNonIP(
-                    name=assay_name,
-                    r1=FastqFile(path=row["r1"]),
-                    r2=FastqFile(path=row["r2"]) if row["r2"] else None,
-                    metadata=metadata,
+        # Collate the fastq files by sample name
+        df = pd.DataFrame(fq, columns=["path"])
+        df = df.assign(
+            fastq_files=lambda x: x["path"].apply(lambda y: FastqFile(path=y)),
+            read_number=lambda x: x["fastq_files"].apply(lambda y: y.read_number),
+            sample_stem=lambda x: x["fastq_files"].apply(lambda y: y.stem),
+            sample_base=lambda x: x["fastq_files"].apply(lambda y: y.sample_base),
+        )
+
+        # Create the fastq sets
+        fastq_sets = []
+        for sample_name, group in df.groupby("sample_base"):
+
+            if group.shape[0] == 1:
+                fq_set = FastqSet(
+                    name=sample_name, r1=group["fastq_files"].iloc[0], **kwargs
+                )
+            elif group.shape[0] == 2:
+                fq_set = FastqSet(
+                    name=sample_name,
+                    r1=group["fastq_files"].iloc[0],
+                    r2=group["fastq_files"].iloc[1],
+                    **kwargs,
                 )
             else:
-                raise NotImplementedError("Not implemented")
-        return cls(assays=assays, **kwargs)
+                raise ValueError(
+                    f"Invalid number of fastq files ({group.shape[0]}) for {sample_name}"
+                )
+
+            fastq_sets.append(fq_set)
 
-    def to_dataframe(self, simplify: bool = True) -> pd.DataFrame:
+        return cls(
+            fastq_sets=fastq_sets,
+            metadata=[Metadata(scale_group="all") for _ in fastq_sets],
+        )
+
+    def to_dataframe(self) -> pd.DataFrame:
+        """
+        Return the Design object as a pandas DataFrame.
         """
-        Return the SampleInfo object as a pandas DataFrame.
 
+        data = []
+        for fastq_set, metadata in zip(self.fastq_sets, self.metadata):
+            row = {
+                "sample_name": fastq_set.name,
+                "r1": fastq_set.r1.path,
+                "r2": fastq_set.r2.path if fastq_set.r2 is not None else None,
+            }
+
+            for k, v in metadata.model_dump(exclude_none=True).items():
+                row[k] = v
+
+            data.append(row)
+
+        df = pd.DataFrame(data).sort_values("sample_name")
+
+        return DataFrameDesign.validate(df)
+
+    @classmethod
+    def from_dataframe(cls, df: pd.DataFrame, **kwargs):
         """
+        Create a Design object from a pandas DataFrame.
+        """
+        df = DataFrameDesign.validate(df)
+
+        fastq_sets = []
+        metadata = []
 
-        if not simplify:
-            df = pd.DataFrame.from_dict(
-                {k: v.model_dump() for k, v in self.assays.items()}, orient="index"
+        non_metadata_keys = ["sample_name", "r1", "r2"]
+
+        for _, row in df.iterrows():
+            if row["r2"] is not None:
+                fastq_sets.append(
+                    FastqSet(
+                        name=row["sample_name"],
+                        r1=FastqFile(path=row["r1"]),
+                        r2=FastqFile(path=row["r2"]),
+                        **kwargs,
+                    )
+                )
+            else:
+                fastq_sets.append(
+                    FastqSet(
+                        name=row["sample_name"], r1=FastqFile(path=row["r1"]), **kwargs
+                    )
+                )
+
+            metadata.append(
+                Metadata(**{k: v for k, v in row.items() if k not in non_metadata_keys})
             )
-        else:
-            data = {}
-            for assay_name, assay in self.assays.items():
-                data[assay_name] = {}
-                data[assay_name]["r1"] = assay.r1.path
-                if assay.r2 is not None:
-                    data[assay_name]["r2"] = assay.r2.path
-
-                if assay.metadata is not None:
-                    for k, v in assay.metadata.items():
-                        data[assay_name][k] = v
 
-            df = pd.DataFrame.from_dict(data, orient="index")
+        return cls(fastq_sets=fastq_sets, metadata=metadata, **kwargs)
+
+    @classmethod
+    def from_directory(cls, directory: Union[pathlib.Path, str], **kwargs):
+        """
+        Create a Design object from a directory of fastq files.
+        """
+        directory = pathlib.Path(directory)
+        file_patterns = ["*.fq", "*.fq.gz", "*.fastq", "*.fastq.gz"]
+        fastq_files = sorted(
+            [f for pattern in file_patterns for f in directory.glob(pattern)]
+        )
+
+        if len(fastq_files) == 0:
+            raise FileNotFoundError(f"No fastq files found in {directory}")
 
-        return df
+        return cls.from_fastq_files(fastq_files, **kwargs)
 
 
 class DesignIP(BaseModel):
-    assays: Dict[str, ExperimentIP] = Field(
-        default_factory=dict,
-        description="Dictionary of experiment classes keyed by sample name",
-    )
+    experiments: List[IPExperiment]
+    metadata: List[Metadata]
 
-    @computed_field
     @property
     def sample_names_ip(self) -> List[str]:
-        sample_names = set()
-        for experiment in self.assays.values():
-            sample_names.add(experiment.ip_files.name)
-
-        return list(sample_names)
+        return [f.ip_set_fullname for f in self.experiments]
 
     @property
     def sample_names_control(self) -> List[str]:
-        sample_names = set()
-        for experiment in self.assays.values():
-            if experiment.control is not None:
-                sample_names.add(experiment.control_files.name)
-
-        if all([s is None for s in sample_names]):
-            return []
-        else:
-            return list(sample_names)
+        names = set()
+        for f in self.experiments:
+            if f.has_control:
+                names.add(f.control_fullname)
+        return list(names)
 
     @property
     def sample_names(self) -> List[str]:
-        return self.sample_names_ip + self.sample_names_control
+        return sorted([*self.sample_names_ip, *self.sample_names_control])
 
     @property
-    def ip_names(self) -> List[str]:
-        return list(set([experiment.ip for experiment in self.assays.values()]))
+    def ips_performed(self) -> List[str]:
+        ip = set()
+        for f in self.experiments:
+            ip.add(f.ip_performed)
+        return list(ip)
 
     @property
-    def control_names(self) -> List[str]:
-        names = list(set([experiment.control for experiment in self.assays.values()]))
-        if all([s is None for s in names]):
-            return []
-        else:
-            return [n for n in names if n is not None]
+    def controls_performed(self) -> List[str]:
+        control = set()
+        for f in self.experiments:
+            if f.has_control:
+                control.add(f.control_performed)
+        return list(control)
 
-    @computed_field
-    @property
-    def fastq_paths(self) -> List[pathlib.Path]:
-        paths = []
-        for experiment in self.assays.values():
-            paths.extend(experiment.ip_files.fastq_paths)
-
-            if experiment.control_files is not None:
-                paths.extend(experiment.control_files.fastq_paths)
-
-        return paths
-
-    def query(
-        self, sample_name: str, ip: str = None, control: str = None
-    ) -> ExperimentIP:
+    def query(self, sample_name: str) -> FastqSetIP:
         """
-        Extract an experiment from the design.
+        Extracts a pair of fastq files from the design.
         """
-
-        name_to_query = sample_name + (f"_{ip}" if ip is not None else "")
-
-        for experiment in self.assays.values():
-
-            name_ip = experiment.name
-            name_control = f"{experiment.control_files.r1.sample_base_without_ip}_{experiment.control_files.r1.ip}"
-
-            if name_to_query == name_ip or name_to_query == name_control:
-                if control is not None:
-                    if experiment.control == control:
-                        return experiment
-                else:
-                    return experiment
-
-        raise ValueError(
-            f"Could not find experiment with sample name {sample_name} and ip {ip} and control {control}"
+        ip_names = set(f.ip_set_fullname for f in self.experiments)
+        control_names = set(
+            f.control_fullname for f in self.experiments if f.has_control
         )
 
+        if sample_name in ip_names or sample_name in control_names:
+            for experiment in self.experiments:
+                if experiment.ip_set_fullname == sample_name:
+                    return experiment.ip
+                elif (
+                    experiment.has_control
+                    and experiment.control_fullname == sample_name
+                ):
+                    return experiment.control
+        else:
+            raise ValueError(f"Could not find sample with name {sample_name}")
+
     @classmethod
-    def from_fastq_files(cls, fq: List[FastqFileIP], **kwargs):
+    def from_fastq_files(cls, fq: List[Union[str, pathlib.Path]], **kwargs):
         """
-        Create a SampleInfo object from a list of FastqFiles.
-
+        Generate a Design object from a list of FastqFiles.
         """
+        import pandas as pd
 
-        ## Run through the list and pair upt the read1 and read2 files
-        ## If there is only one file, then it is the read1 file
-        import itertools
+        fq = sorted([pathlib.Path(f) for f in fq])
 
         # Collate the fastq files by sample name
-        fq = sorted(fq)
-        fastq_collated = dict()
-        for f in fq:
-            if f.sample_base not in fastq_collated:
-                fastq_collated[f.sample_base] = dict()
-                fastq_collated[f.sample_base][f.read_number or 1] = f
-            else:
-                fastq_collated[f.sample_base][f.read_number] = f
+        df = pd.DataFrame(fq, columns=["path"])
+        df = df.assign(
+            fastq_files=lambda x: x["path"].apply(lambda y: FastqFileIP(path=y)),
+            read_number=lambda x: x["fastq_files"].apply(lambda y: y.read_number),
+            sample_stem=lambda x: x["fastq_files"].apply(lambda y: y.stem),
+            sample_base=lambda x: x["fastq_files"].apply(lambda y: y.sample_base),
+            sample_base_without_ip=lambda x: x["fastq_files"].apply(
+                lambda y: y.sample_base_without_ip
+            ),
+            is_control=lambda x: x["fastq_files"].apply(lambda y: y.is_control),
+        )
+
+        # Break the dataframe into IP and control files
+        ip_files = df.query("is_control == False")
+        control_files = df.query("is_control == True")[
+            ["path", "sample_base_without_ip"]
+        ]
 
-        # Create the assays
-        assays = {}
-        for sample_name, fastq_files in fastq_collated.items():
-            assays[sample_name] = AssayIP(
-                name=sample_name, r1=fastq_files[1], r2=fastq_files.get(2), **kwargs
+        # Merge the IP and control files using the sample base without the IP
+        df = (
+            ip_files.merge(
+                control_files,
+                on=["sample_base_without_ip"],
+                suffixes=("_ip", "_control"),
+                how="left",
             )
+            .assign(
+                has_control=lambda x: x["path_control"].notnull(),
+            )
+            .drop_duplicates(["sample_base", "read_number"])
+        )
 
-        # Create the experiments
-        experiments = {}
+        # Group the files by the sample base
+        experiments = []
+        for base, group in df.groupby("sample_base"):
+
+            name_without_ip = group["sample_base_without_ip"].iloc[0]
+            if group.shape[0] == 1:
+                # Single end experiment
+                ip = FastqSetIP(
+                    name=name_without_ip, r1=FastqFileIP(path=group["path_ip"].iloc[0])
+                )
 
-        for base, assay in itertools.groupby(
-            assays.values(), lambda x: x.r1.sample_base_without_ip
-        ):
-            assay = list(assay)
+                if pathlib.Path(str(group["path_control"].iloc[0])).exists():
+                    control = FastqSetIP(
+                        name=name_without_ip,
+                        r1=FastqFileIP(path=group["path_control"].iloc[0]),
+                    )
+                else:
+                    control = None
+
+                experiments.append(IPExperiment(ip=ip, control=control, **kwargs))
 
-            if len(assay) == 1:
-                experiments[assay[0].name] = ExperimentIP(ip_files=assay[0], **kwargs)
-            elif len(assay) == 2 and any([a.is_control for a in assay]):
-                ip = [a for a in assay if not a.is_control][0]
-                control = [a for a in assay if a.is_control][0]
-                experiments[ip.name] = ExperimentIP(
-                    ip_files=ip, control_files=control, **kwargs
+            elif group.shape[0] == 2:
+                # Paired end experiment
+                ip = FastqSetIP(
+                    name=name_without_ip,
+                    r1=FastqFileIP(path=group["path_ip"].iloc[0]),
+                    r2=FastqFileIP(path=group["path_ip"].iloc[1]),
                 )
-            elif len(assay) >= 2 and not any([a.is_control for a in assay]):
-                for a in assay:
-                    experiments[a.name] = ExperimentIP(ip_files=a, **kwargs)
-
-            elif len(assay) >= 2 and any([a.is_control for a in assay]):
-                logger.warning(f"Multiple controls for {assay[0].name}")
-                logger.warning("Will generate all possible combinations")
-                ip = [a for a in assay if not a.is_control]
-                control = [a for a in assay if a.is_control]
-
-                for combination in itertools.product(ip, control):
-                    experiments[combination[0].name] = ExperimentIP(
-                        ip_files=combination[0], control_files=combination[1], **kwargs
+
+                if group["has_control"].iloc[0]:
+                    control = FastqSetIP(
+                        name=name_without_ip,
+                        r1=FastqFileIP(path=group["path_control"].iloc[0]),
+                        r2=FastqFileIP(path=group["path_control"].iloc[1]),
                     )
+                else:
+                    control = None
 
-        return cls(assays=experiments, **kwargs)
+                experiments.append(IPExperiment(ip=ip, control=control, **kwargs))
 
-    @classmethod
-    def from_directory(
-        cls, path: pathlib.Path, metadata: Dict[str, Any] = None, **kwargs
-    ):
-        """
-        Create a SampleInfo object from a directory of fastq files.
+            else:
+                raise ValueError(
+                    f"Invalid number of fastq files ({group.shape[0]}) for {name_without_ip}"
+                )
+
+        return cls(
+            experiments=experiments,
+            metadata=[Metadata(scale_group="all") for _ in experiments],
+        )
 
+    def to_dataframe(self) -> pd.DataFrame:
+        """
+        Return the Design object as a pandas DataFrame.
         """
 
-        fq = list(pathlib.Path(path).glob("*.fastq.gz"))
-        fq = sorted([FastqFileIP(path=f) for f in fq])
-        return cls.from_fastq_files(fq, metadata=metadata, **kwargs)
+        data = []
+        for experiment, metadata in zip(self.experiments, self.metadata):
+            row = {
+                "sample_name": experiment.ip.name,
+                "ip": experiment.ip.ip_or_control_name,
+                "control": (
+                    experiment.control.ip_or_control_name
+                    if experiment.control
+                    else None
+                ),
+                "ip_r1": experiment.ip.r1.path,
+                "ip_r2": experiment.ip.r2.path if experiment.ip.r2 else None,
+                "control_r1": (
+                    experiment.control.r1.path if experiment.control else None
+                ),
+                "control_r2": (
+                    experiment.control.r2.path if experiment.control else None
+                ),
+            }
 
-    def to_dataframe(self, simplify: bool = True):
-        """
-        Return the SampleInfo object as a pandas DataFrame.
+            for k, v in metadata.model_dump(exclude_none=True).items():
+                row[k] = v
 
-        """
+            data.append(row)
 
-        data = {}
-        for experiment_name, experiment in self.assays.items():
-            data[experiment_name] = {}
-            data[experiment_name]["ip_r1"] = experiment.ip_files.r1.path
-            if experiment.ip_files.r2 is not None:
-                data[experiment_name]["ip_r2"] = experiment.ip_files.r2.path
+        df = pd.DataFrame(data).sort_values("sample_name")
 
-            if experiment.control_files is not None:
-                data[experiment_name]["control_r1"] = experiment.control_files.r1.path
-                if experiment.control_files.r2 is not None:
-                    data[experiment_name][
-                        "control_r2"
-                    ] = experiment.control_files.r2.path
+        return DataFrameDesignIP.validate(df)
 
-            if experiment.metadata is not None:
-                for k, v in experiment.metadata.items():
-                    data[experiment_name][k] = v
+    @classmethod
+    def from_dataframe(cls, df: pd.DataFrame, **kwargs):
+        """
+        Create a Design object from a pandas DataFrame.
+        """
+        df = DataFrameDesignIP.validate(df)
 
-            data[experiment_name]["ip"] = experiment.ip
-            data[experiment_name]["control"] = experiment.control
+        experiments = []
+        metadata = []
 
-        df = pd.DataFrame.from_dict(data, orient="index")
+        non_metadata_keys = [
+            "sample_name",
+            "ip",
+            "control",
+            "ip_r1",
+            "ip_r2",
+            "control_r1",
+            "control_r2",
+        ]
 
-        return df
+        for _, row in df.iterrows():
+            ip = FastqSetIP(
+                name=row["sample_name"],
+                r1=FastqFileIP(path=row["ip_r1"]),
+                r2=FastqFileIP(path=row["ip_r2"]) if row["ip_r2"] else None,
+            )
+            control = (
+                FastqSetIP(
+                    name=row["sample_name"],
+                    r1=FastqFileIP(path=row["control_r1"]),
+                    r2=(
+                        FastqFileIP(path=row["control_r2"])
+                        if row["control_r2"]
+                        else None
+                    ),
+                )
+                if row["control_r1"]
+                else None
+            )
+
+            experiments.append(IPExperiment(ip=ip, control=control, **kwargs))
+            metadata.append(
+                Metadata(**{k: v for k, v in row.items() if k not in non_metadata_keys})
+            )
+
+        return cls(experiments=experiments, metadata=metadata, **kwargs)
 
     @classmethod
-    def from_dataframe(cls, df: pd.DataFrame, simplified: bool = True, **kwargs):
-        experiments = {}
-        for experiment_name, row in df.iterrows():
-            if simplified:
-                # Add the metadata
-                metadata = {}
-                for k, v in row.items():
-                    if k not in [
-                        "ip_r1",
-                        "ip_r2",
-                        "control_r1",
-                        "control_r2",
-                        "ip",
-                        "control",
-                    ]:
-                        metadata[k] = v
-
-                # Add the experiment
-                ip = row["ip"]
-                control = row["control"]
-
-                if "control_r1" not in row or not is_path(row["control_r1"]):
-                    experiments[experiment_name] = ExperimentIP(
-                        ip_files=AssayIP(
-                            name=experiment_name,
-                            r1=FastqFileIP(path=row["ip_r1"]),
-                            r2=(
-                                FastqFileIP(path=row["ip_r2"])
-                                if "ip_r2" in row and is_path(row["ip_r2"])
-                                else None
-                            ),
-                        ),
-                        ip=ip,
-                        control=None,
-                        metadata=metadata,
-                    )
-                else:
-                    experiments[experiment_name] = ExperimentIP(
-                        ip_files=AssayIP(
-                            name=experiment_name,
-                            r1=FastqFileIP(path=row["ip_r1"]),
-                            r2=(
-                                FastqFileIP(path=row["ip_r2"])
-                                if "ip_r2" in row and is_path(row["ip_r2"])
-                                else None
-                            ),
-                        ),
-                        control_files=AssayIP(
-                            name=experiment_name,
-                            r1=FastqFileIP(path=row["control_r1"]),
-                            r2=(
-                                FastqFileIP(path=row["control_r2"])
-                                if "control_r2" in row and is_path(row["control_r2"])
-                                else None
-                            ),
-                        ),
-                        ip=ip,
-                        control=control,
-                        metadata=metadata,
-                    )
-            else:
-                raise NotImplementedError("Not implemented")
+    def from_directory(cls, directory: Union[pathlib.Path, str], **kwargs):
+        """
+        Create a Design object from a directory of fastq files.
+        """
+        directory = pathlib.Path(directory)
+        file_patterns = ["*.fq", "*.fq.gz", "*.fastq", "*.fastq.gz"]
+        fastq_files = sorted(
+            [f for pattern in file_patterns for f in directory.glob(pattern)]
+        )
 
-        return cls(assays=experiments, **kwargs)
+        if len(fastq_files) == 0:
+            raise FileNotFoundError(f"No fastq files found in {directory}")
+
+        return cls.from_fastq_files(fastq_files, **kwargs)
+
+    @property
+    def fastq_paths(self) -> List[pathlib.Path]:
+        paths = []
+        for experiment in self.experiments:
+            paths.extend(experiment.ip.fastq_paths)
+            if experiment.control:
+                paths.extend(experiment.control.fastq_paths)
+        return paths
 
 
 class NormGroup(BaseModel):
     """
     Class to handle normalisation groups.
     """
 
@@ -621,22 +712,52 @@
     @classmethod
     def from_design(
         cls,
         design: Union[Design, DesignIP],
         reference_sample: Optional[str] = None,
         subset_column: Optional[str] = "scale_group",
         subset_value: Optional[List[str]] = None,
+        include_controls: bool = False,
     ):
-        df = design.to_dataframe()
+        
+        if isinstance(design, Design):
+            df = (
+                design.to_dataframe()
+                .assign(sample_fullname=lambda df: df.sample_name)
+                .set_index("sample_fullname")
+            )
+        elif isinstance(design, DesignIP) and not include_controls:
+            df = (
+                design.to_dataframe()
+                .assign(sample_fullname=lambda df: df.sample_name + "_" + df.ip)
+                .set_index("sample_fullname")
+            )
+        elif isinstance(design, DesignIP) and include_controls:
+            df_ip = (
+                design.to_dataframe()
+                .assign(sample_fullname=lambda df: df.sample_name + "_" + df.ip)
+                .set_index("sample_fullname")
+            )
+            df_control = (
+                design.to_dataframe()
+                .query("control.notnull()")
+                .assign(sample_fullname=lambda df: df.sample_name + "_" + df.control)
+                .set_index("sample_fullname")
+            )
+            df = pd.concat([df_ip, df_control])
+
 
         if subset_value:
             df = df.query(f"{subset_column} in {subset_value}")
 
         samples = df.index.tolist()
+
+
         reference_sample = reference_sample or df.index[0]
+
         return cls(
             samples=samples,
             reference_sample=reference_sample,
             group=subset_value[0] or "all",
         )
 
 
@@ -649,14 +770,15 @@
 
     @classmethod
     def from_design(
         cls,
         design: Union[Design, DesignIP],
         reference_sample: Optional[str] = None,
         subset_column: Optional[str] = "scale_group",
+        include_controls: bool = False,
     ):
         df = design.to_dataframe()
 
         # If the subset column is in the design
         # make the groups based on the subset column
         if subset_column in df.columns:
             subset_values = df[subset_column].drop_duplicates()
@@ -666,14 +788,15 @@
                     NormGroup.from_design(
                         design,
                         reference_sample,
                         subset_column,
                         [
                             subset_value,
                         ],
+                        include_controls,
                     )
                     for subset_value in subset_values
                 ]
             )
 
         else:  # If not then just make one group with all the samples
             return cls(
@@ -739,45 +862,44 @@
 class BigWigFiles(BaseModel):
     assay: Literal["ChIP", "ATAC", "RNA", "SNP"]
     names: List[str]
     pileup_method: Union[
         Literal["deeptools", "homer"], List[Literal["deeptools", "homer"]]
     ] = None
     make_bigwigs: bool = False
-    scale_method: Optional[Literal["cpm", "rpkm", "spikein", "csaw", "grouped"]] = None
+    scale_method: Optional[Literal["cpm", "rpkm", "spikein", "csaw", "merged"]] = None
+    include_unscaled: bool = True
     prefix: Optional[str] = "seqnado_output/bigwigs/"
 
     def model_post_init(self, __context: Any) -> None:
         if isinstance(self.pileup_method, str):
             self.pileup_method = [self.pileup_method]
 
+        if self.include_unscaled and not self.scale_method:
+            self.scale_method = ["unscaled",]
+        elif self.include_unscaled and self.scale_method:
+            self.scale_method = ["unscaled", self.scale_method]
+        else:
+            self.scale_method = [self.scale_method]
+
     @property
     def bigwigs_non_rna(self):
-        scale_methods = (
-            ["unscaled", self.scale_method] if self.scale_method else ["unscaled"]
-        )
-
         return expand(
             self.prefix + "{method}/{scale}/{sample}.bigWig",
             sample=self.names,
-            scale=scale_methods,
+            scale=self.scale_method,
             method=self.pileup_method,
         )
 
     @property
     def bigwigs_rna(self):
-
-        scale_methods = (
-            ["unscaled", self.scale_method] if self.scale_method else ["unscaled"]
-        )
-
         return expand(
             self.prefix + "{method}/{scale}/{sample}_{strand}.bigWig",
             sample=self.names,
-            scale=scale_methods,
+            scale=self.scale_method,
             method=self.pileup_method,
             strand=["plus", "minus"],
         )
 
     @computed_field
     @property
     def files(self) -> List[str]:
@@ -794,19 +916,20 @@
     assay: Literal["ChIP", "ATAC", "RNA", "SNP"]
     names: List[str]
     peak_calling_method: Union[
         Literal["macs", "homer", "lanceotron", "seacr", False],
         List[Literal["macs", "homer", "lanceotron", "seacr"]],
     ] = None
     call_peaks: bool = False
+    prefix: Optional[str] = "seqnado_output/peaks/"
 
     @property
     def peak_files(self) -> List[str]:
         return expand(
-            "seqnado_output/peaks/{method}/{sample}.bed",
+            self.prefix + "{method}/{sample}.bed",
             sample=self.names,
             method=self.peak_calling_method,
         )
 
     @computed_field
     @property
     def files(self) -> List[str]:
@@ -879,16 +1002,16 @@
 
 class Output(BaseModel):
     assay: Literal["ChIP", "ATAC", "RNA", "SNP"]
     run_design: Union[Design, DesignIP]
     sample_names: List[str]
 
     make_bigwigs: bool = False
-    pileup_method: Union[
-        Literal["deeptools", "homer"], List[Literal["deeptools", "homer"]]
+    pileup_method: Optional[
+        Union[Literal["deeptools", "homer"], List[Literal["deeptools", "homer"]]]
     ] = None
     scale_method: Optional[Literal["cpm", "rpkm", "spikein", "csaw"]] = None
 
     make_heatmaps: bool = False
     make_ucsc_hub: bool = False
 
     ucsc_hub_details: Optional[Dict[str, Any]] = None
@@ -918,16 +1041,17 @@
             scale_method=self.scale_method,
         )
         if self.merge_bigwigs:
             bwf_merged = BigWigFiles(
                 assay=self.assay,
                 names=self.design_dataframe["merge"].unique().tolist(),
                 make_bigwigs=self.make_bigwigs,
-                pileup_method=self.pileup_method,
-                scale_method="rpkm",
+                pileup_method="deeptools",
+                scale_method="merged",
+                include_unscaled=False,
             )
 
             files = bwf_samples.files + bwf_merged.files
         else:
             files = bwf_samples.files
 
         return files or []
@@ -1005,30 +1129,33 @@
 
         return files
 
 
 class NonRNAOutput(Output):
     assay: Union[Literal["ChIP"], Literal["ATAC"]]
     call_peaks: bool = False
-    peak_calling_method: Union[
-        Literal["macs", "homer", "lanceotron", False],
-        List[Literal["macs", "homer", "lanceotron"]],
+    peak_calling_method: Optional[
+        Union[
+            Literal["macs", "homer", "lanceotron", False],
+            List[Literal["macs", "homer", "lanceotron"]],
+        ]
     ] = None
 
     @property
     def merge_peaks(self):
         return "merge" in self.design_dataframe.columns
 
     @property
     def merged_peaks(self):
         return PeakCallingFiles(
             assay=self.assay,
             names=self.design_dataframe["merge"].unique().tolist(),
             call_peaks=self.call_peaks,
-            peak_calling_method=self.peak_calling_method,
+            peak_calling_method="lanceotron",
+            prefix="seqnado_output/peaks/merged/",
         )
 
     @computed_field
     @property
     def peaks(self) -> List[str]:
         pcf_samples = PeakCallingFiles(
             assay=self.assay,
@@ -1076,17 +1203,19 @@
 
 
 class ChIPOutput(NonRNAOutput):
     assay: Literal["ChIP"]
     ip_names: List[str]
     control_names: List[str]
     call_peaks: bool = False
-    peak_calling_method: Union[
-        Literal["macs", "homer", "lanceotron", "seacr", False],
-        List[Literal["macs", "homer", "lanceotron", "seacr"]],
+    peak_calling_method: Optional[
+        Union[
+            Literal["macs", "homer", "lanceotron", "seacr", False],
+            List[Literal["macs", "homer", "lanceotron", "seacr"]],
+        ]
     ] = None
     chip_spikein_normalisation: bool = False
     scale_method: Optional[Literal["cpm", "rpkm", "spikein", "csaw"]] = None
 
     @property
     def peaks(self):
         ip_sample_names = [
```

### Comparing `seqnado-0.5.0/seqnado/helpers.py` & `seqnado-0.5.1/seqnado/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import Dict, Union, Optional, List, Tuple
 import pathlib
 import numpy as np
 import shlex
 
+from loguru import logger
+
+
 from seqnado.design import Design, DesignIP
 
 
 FILETYPE_TO_DIR_MAPPING = {
     "tag": "tag_dirs",
     "bigwig": "bigwigs/deeptools",
     "bam": "aligned",
@@ -15,15 +18,14 @@
 FILETYPE_TO_EXTENSION_MAPPING = {"tag": "/", "bigwig": ".bigWig", "bam": ".bam"}
 
 
 def extract_cores_from_options(options: List[str]) -> Tuple[List[str], int]:
     """
     Extract the number of cores from the snakemake options.
     """
-    from loguru import logger
 
     try:
         cores_flag = options.index("-c")
         cores = int(options[cores_flag + 1])
         options = [o for i, o in enumerate(options) if i not in [cores_flag, cores_flag + 1]]
     except ValueError:
         try:
@@ -58,77 +60,74 @@
 
 def symlink_file(
     output_dir: pathlib.Path, source_path: pathlib.Path, new_file_name: str
 ):
     """
     Create a symlink in the output directory with the new file name.
     """
+
     new_path = output_dir / new_file_name
     if not new_path.exists() and source_path.is_file():
-        try:
+        # logger.debug(f"Symlinking {source_path} to {output_dir / new_file_name}")
+        if str(source_path) in [".", "..", "", None, "None"]:
+            logger.warning(f"Source path is empty for {new_file_name}. Will not symlink.")
+
+        else:
             new_path.symlink_to(source_path.resolve())
-        except FileExistsError:
-            print(f"Symlink for {new_path} already exists.")
+            # logger.debug(f"Symlinked {source_path} to {output_dir / new_file_name} successfully.")
 
 
 def symlink_fastq_files(
     design: Union[Design, DesignIP], output_dir: str = "seqnado_output/fastqs/"
 ):
     """
     Symlink the fastq files to the output directory.
     """
     output_dir = pathlib.Path(output_dir)
     output_dir.mkdir(parents=True, exist_ok=True)
 
     if isinstance(design, Design):
-        for assay_name, assay in design.assays.items():
-            if assay.is_paired:
-                symlink_file(output_dir, assay.r1.path, f"{assay_name}_1.fastq.gz")
-                symlink_file(output_dir, assay.r2.path, f"{assay_name}_2.fastq.gz")
+        for fastq_set in design.fastq_sets:
+            if fastq_set.is_paired:
+                symlink_file(output_dir, fastq_set.r1.path, f"{fastq_set.name}_1.fastq.gz")
+                symlink_file(output_dir, fastq_set.r2.path, f"{fastq_set.name}_2.fastq.gz")
             else:
-                symlink_file(output_dir, assay.r1.path, f"{assay_name}.fastq.gz")
+                symlink_file(output_dir, fastq_set.r1.path, f"{fastq_set.name}.fastq.gz")
 
     elif isinstance(design, DesignIP):
-        for experiment_name, experiment in design.assays.items():
+        for experiment in design.experiments:
 
-            # IP files
-            ip_assay = experiment.ip_files
-            is_paired = ip_assay.is_paired
-            has_control = experiment.control_files
-
-            if is_paired:
+            if experiment.fastqs_are_paired:
                 symlink_file(
-                    output_dir, ip_assay.r1.path, f"{ip_assay.name}_1.fastq.gz"
+                    output_dir, experiment.ip.r1.path, f"{experiment.ip.name}_{experiment.ip_performed}_1.fastq.gz"
                 )
                 symlink_file(
-                    output_dir, ip_assay.r2.path, f"{ip_assay.name}_2.fastq.gz"
+                    output_dir, experiment.ip.r2.path, f"{experiment.ip.name}_{experiment.ip_performed}_2.fastq.gz"
                 )
             else:
-                symlink_file(output_dir, ip_assay.r1.path, f"{ip_assay.name}.fastq.gz")
+                symlink_file(output_dir, experiment.ip.r1.path, f"{experiment.ip.name}_{experiment.ip_performed}.fastq.gz")
 
             # Control files
-            if has_control:
-                control_assay = experiment.control_files
-
-                if control_assay.is_paired:
+            if experiment.has_control:
+                if experiment.control.is_paired:
                     symlink_file(
                         output_dir,
-                        control_assay.r1.path,
-                        f"{control_assay.r1.sample_base_without_ip}_{control_assay.r1.ip}_1.fastq.gz",
+                        experiment.control.r1.path,
+                        f"{experiment.control.r1.sample_base_without_ip}_{experiment.control_performed}_1.fastq.gz",
                     )
                     symlink_file(
                         output_dir,
-                        control_assay.r2.path,
-                        f"{control_assay.r1.sample_base_without_ip}_{control_assay.r1.ip}_2.fastq.gz",
+                        experiment.control.r2.path,
+                        f"{experiment.control.r1.sample_base_without_ip}_{experiment.control_performed}_2.fastq.gz",
                     )
                 else:
                     symlink_file(
                         output_dir,
-                        control_assay.r1.path,
-                        f"{control_assay.r1.sample_base_without_ip}_{control_assay.r1.ip}.fastq.gz",
+                        experiment.control.r1.path,
+                        f"{experiment.control.r1.sample_base_without_ip}_{experiment.control_performed}.fastq.gz",
                     )
 
 
 def is_on(param: str) -> bool:
     """
     Returns True if parameter in "on" values
     On values:
@@ -224,27 +223,52 @@
     print("PEPE SILVIA")
     _pepe_silvia = (
         "https://relix.com/wp-content/uploads/2017/03/tumblr_o16n2kBlpX1ta3qyvo1_1280.jpg"
     )
     return _pepe_silvia
 
 
-def get_group_for_sample(wildcards, design: Union[Design, DesignIP]):
+def get_group_for_sample(wildcards, design: Union[Design, DesignIP], strip: str = ""):
     from seqnado.design import NormGroups
 
-    norm_groups = NormGroups.from_design(design)
-    group = norm_groups.get_sample_group(wildcards.sample)
-    return group
+    norm_groups = NormGroups.from_design(design, include_controls=True)
+
+    try:
+        group = norm_groups.get_sample_group(wildcards.sample.strip(strip))
+        return group
+    except KeyError:
+        # logger.error(f"Sample {wildcards.sample} not found in normalisation groups.")
+        raise KeyError(f"Sample {wildcards.sample} not found in normalisation groups.")
 
 def get_scale_method(config: Dict) -> Optional[str]:
     """
     Returns the scale method based on the config.
     """
 
     if config["spikein"]:
        method = "spikein"
     elif config["scale"]:
         method = "csaw"
     else:
         method = None
     
     return method
+
+
+def remove_unwanted_run_files():
+    import glob
+    import os
+    import shutil
+
+    slurm_files = glob.glob("slurm-*.out")
+    sps_files = glob.glob("sps-*")
+    simg_files = glob.glob("*.simg")
+
+    for fn in [*slurm_files, *sps_files, *simg_files]:
+        try:
+            if not os.path.isdir(fn):
+                os.remove(fn)
+            else:
+                shutil.rmtree(fn)
+
+        except Exception as e:
+            print(e)
```

### Comparing `seqnado-0.5.0/seqnado/workflow/config/config.yaml.jinja` & `seqnado-0.5.1/seqnado/workflow/config/config.yaml.jinja`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/config/deseq2.qmd.jinja` & `seqnado-0.5.1/seqnado/workflow/config/deseq2.qmd.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
 ## Counts
 
 ```{r counts}
 counts <- read.delim(params$counts, comment.char = "#") %>%
   rename_with(~ gsub("(seqnado_output.aligned.)(.+)(.bam)", "\\2", .), everything()) %>%
   column_to_rownames(var = "Geneid") %>%
-  dplyr::select(one_of(make.names(sample_info$sample))) %>%
-  setNames(sample_info$sample) %>%
+  dplyr::select(one_of(make.names(sample_info$sample_name))) %>%
+  setNames(sample_info$sample_name) %>%
   filter(rowSums(.) > 0)
 
 total_counts <- data.frame(
   sample = colnames(counts), 
   total_counts = colSums(counts), 
   mean_counts = colMeans(counts))
 
@@ -112,15 +112,15 @@
   dds <- estimateSizeFactors(dds, controlGenes=spikein_genes)
   kable(colData(dds), row.names = F)
   counts(dds) <- counts(dds)[!rownames(counts(dds)) %in% spikein_genes, ]
   dds <- DESeq(dds, quiet = T)
   
   # Output size factors
   size_factors <- colData(dds)[, "sizeFactor"]
-  names(size_factors) <- colData(dds)[, "sample"]
+  names(size_factors) <- colData(dds)[, "sample_name"]
   sf <- toJSON(size_factors)
   writeLines(sf, params$size_factors_out)
 
 } else {
 
 dds <- DESeqDataSetFromMatrix(countData = counts,
                               colData = sample_info,
@@ -477,19 +477,19 @@
 ## Top 12 DE genes
 
 ```{r top_DEgenes}
 top_DE_genes <- normCounts %>%
   as.data.frame() %>%
   filter(gene %in% DE_results$gene[1:12]) %>%
   pivot_longer(
-    cols = sample_info$sample, 
+    cols = sample_info$sample_name, 
     values_to = "count", 
     names_to = "sample"
   ) %>%
-  left_join(sample_info, by = "sample") %>%
+  left_join(sample_info, by = c("sample" = "sample_name")) %>%
   mutate(gene = factor(gene, levels = unique(gene)))
 
 p <- ggplot(data = top_DE_genes, aes(x = deseq2, y = count, color = deseq2)) +
     geom_boxplot() +
     geom_point(position = position_jitter(width = 0.1, height = 0)) +
     theme_light() +
     ylab("Normalized Count") +
```

### Comparing `seqnado-0.5.0/seqnado/workflow/config/preset_genomes.json` & `seqnado-0.5.1/seqnado/workflow/config/preset_genomes.json`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/envs/environment.yml` & `seqnado-0.5.1/seqnado/workflow/envs/environment.yml`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/align.smk` & `seqnado-0.5.1/seqnado/workflow/rules/align.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/align_rna.smk` & `seqnado-0.5.1/seqnado/workflow/rules/align_rna.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/alignment_counts.smk` & `seqnado-0.5.1/seqnado/workflow/rules/alignment_counts.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/alignment_post_processing.smk` & `seqnado-0.5.1/seqnado/workflow/rules/alignment_post_processing.smk`

 * *Files 2% similar despite different names*

```diff
@@ -199,36 +199,41 @@
         samtools view -f 2 -c {output.bam} >> {log} 2>&1
         """
 
 
 def get_bam_files_for_merge(wildcards):
     from seqnado.design import NormGroups
     norm_groups = NormGroups.from_design(DESIGN, subset_column="merge")
-    return norm_groups.get_sample_group(wildcards.group)
+
+    sample_names = norm_groups.get_grouped_samples(wildcards.group)
+    bam_files = [
+        f"seqnado_output/aligned/{sample}.bam" for sample in sample_names
+    ]
+    return bam_files
 
 
 rule merge_bams:
     input:
         bams=get_bam_files_for_merge,
     output:
-        temp("seqnado_output/aligned/grouped/{group}.bam"),
+        temp("seqnado_output/aligned/merged/{group}.bam"),
     threads: 8
     log:
         "seqnado_output/logs/merge_bam/{group}.log",
     shell:
         """
         samtools merge {output} {input} -@ {threads}
         """
 
 
 use rule index_bam as index_consensus_bam with:
     input:
-        bam="seqnado_output/aligned/grouped/{group}.bam",
+        bam="seqnado_output/aligned/merged/{group}.bam",
     output:
-        bai="seqnado_output/aligned/grouped/{group}.bam.bai",
+        bai="seqnado_output/aligned/merged/{group}.bam.bai",
     threads: 8
 
 
 
 
 
 localrules:
```

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/custom_genome.smk` & `seqnado-0.5.1/seqnado/workflow/rules/custom_genome.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/deseq2_rna.smk` & `seqnado-0.5.1/seqnado/workflow/rules/deseq2_rna.smk`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 rule deseq2_report_rnaseq:
     input:
         counts="seqnado_output/readcounts/feature_counts/read_counts.tsv",
         qmd=f"deseq2_{PROJECT_NAME}.qmd".replace(" ", ""),
         yml="seqnado_output/resources/deseq2_params.yml"
     output:
         deseq2=f"deseq2_{PROJECT_NAME}.html".replace(" ", ""),
-        size_factors="seqnado_output/resources/all_normalisation_factors.json"
     log:
         "seqnado_output/logs/deseq2/deseq2.log",
     container:
         "library://asmith151/seqnado/seqnado_report:latest"
     shell:
         """
         input_file=$(realpath "{input.qmd}")
```

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/exogenous_norm.smk` & `seqnado-0.5.1/seqnado/workflow/rules/exogenous_norm.smk`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from seqnado.design import NormGroups
-
-NORM_GROUPS = NormGroups.from_design(DESIGN)
-
 use rule align_paired as align_paired_spikein with:
     params:
         options="--no-mixed --no-discordant",
         index=config["genome"]["indices"],
     output:
         bam=temp("seqnado_output/aligned/spikein/raw/{sample}.bam"),
     resources:
@@ -96,28 +92,28 @@
     """
 
 
 if config["spikein_options"]["normalisation_method"] == "orlando":
 
     rule calculate_normalisation_factors:
         input:
-            lambda wc: expand(rules.split_bam.output.stats, sample=[sample for sample in NORM_GROUPS.get_grouped_samples(wc.group)]),
+            lambda wc: expand(rules.split_bam.output.stats, sample=SAMPLE_NAMES_IP + SAMPLE_NAMES_CONTROL),
         output:
             normalisation_table="seqnado_output/resources/{group}_normalisation_factors.tsv",
             normalisation_factors="seqnado_output/resources/{group}_normalisation_factors.json",
         log:
             "seqnado_output/logs/normalisation_factors_{group}.log",
         script:
             "../scripts/calculate_spikein_norm_orlando.py"
 
 elif config["spikein_options"]["normalisation_method"] == "with_input":
 
     rule calculate_normalisation_factors:
         input:
-            lambda wc: expand(rules.split_bam.output.stats, sample=[sample for sample in NORM_GROUPS.get_grouped_samples(wc.group)]),
+            lambda wc: expand(rules.split_bam.output.stats, sample=SAMPLE_NAMES_IP + SAMPLE_NAMES_CONTROL),
         output:
             normalisation_table="seqnado_output/resources/{group}_normalisation_factors.tsv",
             normalisation_factors="seqnado_output/resources/{group}_normalisation_factors.json",
         log:
             "seqnado_output/logs/normalisation_factors_{group}.log",
         script:
             "../scripts/calculate_spikein_norm_factors.py"
```

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/fastq_screen.smk` & `seqnado-0.5.1/seqnado/workflow/rules/fastq_screen.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/fastq_trim.smk` & `seqnado-0.5.1/seqnado/workflow/rules/fastq_trim.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/heatmap.smk` & `seqnado-0.5.1/seqnado/workflow/rules/heatmap.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/hub.smk` & `seqnado-0.5.1/seqnado/workflow/rules/hub.smk`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,24 @@
                 "samplename",
             ],
         ),
         "overlay_by": config["ucsc_hub_details"].get("overlay_by", None),
         "subgroup_by": config["ucsc_hub_details"].get(
             "subgroup_by",
             [
-                "pileup_method",
+                "method",
                 "norm"
             ],
         ),
         "supergroup_by": config["ucsc_hub_details"].get("supergroup_by", None),
     }
 
     if ASSAY == "RNA":
-        hub_params["overlay_by"] = ["samplename", "pileup_method", "norm"]
-        hub_params["subgroup_by"] = ["samplename", "pileup_method", "norm", "strand"]
+        hub_params["overlay_by"] = ["samplename", "method", "norm"]
+        hub_params["subgroup_by"] = ["method", "norm", "strand"]
 
     return hub_params
 
 
 rule save_design:
     output:
         "seqnado_output/design.csv",
@@ -60,15 +60,16 @@
     run:
         from loguru import logger
 
         with logger.catch():
             for peak_file in input.peaks:
                 with open(peak_file, "r+") as p:
                     peak_entries = p.readlines()
-                    if len(peak_entries) < 1:
+                    n_peak_lines = sum(1 for line in peak_entries if not line.startswith("#"))
+                    if n_peak_lines == 0: # empty peak file, write a dummy peak
                         p.write("chr21\t1\t2\n")
 
         with open(output.sentinel, "w") as s:
             s.write("validated")
 
 
 rule bed_to_bigbed:
@@ -82,15 +83,15 @@
     resources:
         mem="1GB",
     log:
         "seqnado_output/logs/bed_to_bigbed/{directory}/{sample}.log",
     shell:
         """
         sort -k1,1 -k2,2n {input.bed} | grep '#' -v > {input.bed}.tmp &&
-        bedToBigBed {input.bed}.tmp {params.chrom_sizes} {output.bigbed} &&
+        bedToBigBed {input.bed}.tmp {params.chrom_sizes} {output.bigbed} 2> {log} &&
         rm {input.bed}.tmp
         """
 
 
 rule generate_hub:
     input:
         data=[
```

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/motif.smk` & `seqnado-0.5.1/seqnado/workflow/rules/motif.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/peak_call_chip.smk` & `seqnado-0.5.1/seqnado/workflow/rules/peak_call_chip.smk`

 * *Files 7% similar despite different names*

```diff
@@ -6,50 +6,64 @@
 
 def get_lanceotron_threshold(wildcards):
     options = config["lanceotron"]["callpeak"]
     threshold_pattern = re.compile(r"\-c\s+(\d+.?\d*)")
     threshold = threshold_pattern.search(options).group(1)
     return threshold
 
+def format_macs_options(wildcards, options):
+
+    query_name = f"{wildcards.sample}_{wildcards.treatment}"
+    
+    is_paired = DESIGN.query(query_name).is_paired
+    options = check_options(options)
+
+    if not is_paired:
+        options = re.sub(r"-f BAMPE", "", options)
+    if not options:
+        return ""
+    else:
+        return options
+
 
 def get_control_bam(wildcards):
-    exp = DESIGN.query(sample_name=wildcards.sample, ip=wildcards.treatment)
-    if exp.control:
-        control = f"seqnado_output/aligned/{wildcards.sample}_{exp.control}.bam"
+    exp = DESIGN.query(sample_name=f"{wildcards.sample}_{wildcards.treatment}")
+    if exp:
+        control = f"seqnado_output/aligned/{wildcards.sample}_{exp.ip_or_control_name}.bam"
     else:
         control = "UNDEFINED"
     return control
 
 
 def get_control_tag(wildcards):
-    exp = DESIGN.query(sample_name=wildcards.sample, ip=wildcards.treatment)
-    if not exp.control:
+    exp = DESIGN.query(sample_name=f"{wildcards.sample}_{wildcards.treatment}")
+    if not exp:
         control = "UNDEFINED"
     else:
-        control = f"seqnado_output/tag_dirs/{wildcards.sample}_{exp.control}"
+        control = f"seqnado_output/tag_dirs/{wildcards.sample}_{exp.ip_or_control_name}"
     return control
 
 
 def get_control_bigwig(wildcards):
-    exp = DESIGN.query(sample_name=wildcards.sample, ip=wildcards.treatment)
-    if not exp.control:
+    exp = DESIGN.query(sample_name=f"{wildcards.sample}_{wildcards.treatment}")
+    if not exp:
         control = "UNDEFINED"
     else:
-        control = f"seqnado_output/bigwigs/deeptools/unscaled/{wildcards.sample}_{exp.control}.bigWig"
+        control = f"seqnado_output/bigwigs/deeptools/unscaled/{wildcards.sample}_{exp.ip_or_control_name}.bigWig"
     return control
 
 
 rule macs2_with_input:
     input:
         treatment="seqnado_output/aligned/{sample}_{treatment}.bam",
         control=get_control_bam,
     output:
         peaks="seqnado_output/peaks/macs/{sample}_{treatment}.bed",
     params:
-        options=check_options(config["macs"]["callpeak"]),
+        options=lambda wc: format_macs_options(wc, config["macs"]["callpeak"]),
         narrow=lambda wc, output: output.peaks.replace(".bed", "_peaks.narrowPeak"),
         basename=lambda wc, output: output.peaks.replace(".bed", ""),
     threads: 1
     resources:
         mem="2GB",
         runtime="2h",
     log:
@@ -64,15 +78,15 @@
 rule macs2_no_input:
     input:
         treatment="seqnado_output/aligned/{sample}_{treatment}.bam",
         control=lambda wc: [] if get_control_bam(wc) == "UNDEFINED" else get_control_bam(wc), 
     output:
         peaks="seqnado_output/peaks/macs/{sample}_{treatment}.bed",
     params:
-        options=check_options(config["macs"]["callpeak"]),
+        options=lambda wc: format_macs_options(wc, config["macs"]["callpeak"]),
         narrow=lambda wc, output: output.peaks.replace(".bed", "_peaks.narrowPeak"),
         basename=lambda wc, output: output.peaks.replace(".bed", ""),
     threads: 1
     resources:
         mem="2GB",
         runtime="2h",
     log:
@@ -191,15 +205,15 @@
         prefix=lambda wc, output: pathlib.Path(output.peaks).parent / pathlib.Path(output.peaks).name,
     threads: 1
     resources:
         mem="5GB",
         runtime="2h",
     shell:
         """
-        SEACR_1.3.sh {input.treatment} {params.threshold} {params.norm} {params.stringency} {output.peaks} > {log} 2>&1
+        SEACR_1.3.sh {input.treatment} {params.threshold} {params.norm} {params.stringency} {output.peaks} > {log} 2>&1 || touch {params.prefix}.{params.stringency}.bed
         mv {params.prefix}.{params.stringency}.bed {params.prefix}_seacr.txt
         cut -f 1-3 {params.prefix}_seacr.txt > {output.peaks}
         """
     
 
 ruleorder: lanceotron_with_input > lanceotron_no_input
 ruleorder: homer_with_input > homer_no_input
```

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/peak_call_other.smk` & `seqnado-0.5.1/seqnado/workflow/rules/peak_call_other.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/pileup_default.smk` & `seqnado-0.5.1/seqnado/workflow/rules/pileup_default.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/pileup_norm.smk` & `seqnado-0.5.1/seqnado/workflow/rules/pileup_norm.smk`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 from seqnado.helpers import check_options, get_group_for_sample
-from seqnado.design import NormGroups
-
-NORM_GROUPS = NormGroups.from_design(DESIGN)
-
 
 def format_feature_counts(counts: str) -> pd.DataFrame:
     counts = pd.read_csv(input.counts, sep="\t", comment="#")
     counts = counts.set_index("Geneid")
     counts = counts.drop(
         columns=["Chr", "Start", "End", "Strand", "Length"], errors="ignore"
     )
@@ -21,15 +17,15 @@
     df = pd.read_csv(scale_path, sep="\t", header=None, index_col=0)
     return df.loc[wildcards.sample, "norm.factors"]
 
 
 def get_norm_factor_spikein(wildcards, negative=False):
     import json
 
-    group = NORM_GROUPS.get_sample_group(wildcards.sample)
+    group = NORMALISATION_SCALING.get_sample_group(wildcards.sample)
     with open(f"seqnado_output/resources/{group}_normalisation_factors.json") as f:
         norm_factors = json.load(f)
 
     if not negative:
         return norm_factors[wildcards.sample]
     else:
         return -norm_factors[wildcards.sample]
@@ -41,14 +37,18 @@
     options = check_options(config["deeptools"]["bamcoverage"])
 
     if "--normalizeUsing" in options:
         options = re.sub("--normalizeUsing [a-zA-Z]+", "", options)
 
     if "--scaleFactor" in options:
         options = re.sub("--scaleFactor [0-9.]+", "", options)
+         
+    if not DESIGN.query(wildcards.sample).is_paired:
+        options = re.sub(r"--extendReads", "", options)
+        options = re.sub(r"-e", "", options)
 
     return options
 
 
 def format_homer_make_bigwigs_options(wildcards):
     import re
 
@@ -72,23 +72,22 @@
         genome_tiled="seqnado_output/resources/genome_tiled.gtf",
     params:
         tile_size=config["genome"].get("tile_size", 10_000),
     run:
         import pyranges as pr
 
         chromsizes = (
-            pd.read_csv(chromsizes, sep="\t", header=None).set_index(0)[1].to_dict()
+            pd.read_csv(input.chromsizes, sep="\t", header=None).set_index(0)[1].to_dict()
         )
-        genome_tiled = pr.gf.tile_genome(chromsizes, tile_size=tile_size)
+        genome_tiled = pr.gf.tile_genome(chromsizes, tile_size=params.tile_size)
         genome_tiled = genome_tiled.df.assign(
             feature="tile", gene_id=lambda df: df.index.astype(str)
         ).pipe(pr.PyRanges)
         genome_tiled.to_gtf(output.genome_tiled)
 
-
 rule count_bam:
     input:
         bam=expand("seqnado_output/aligned/{sample}.bam", sample=DESIGN.sample_names),
         tiles="seqnado_output/resources/genome_tiled.gtf",
     output:
         counts="seqnado_output/counts/counts.tsv",
     threads: 8
@@ -112,18 +111,37 @@
 
 rule calculate_scaling_factors:
     input:
         formatted_counts="seqnado_output/counts/{group}_formatted_counts.tsv",
         metadata="seqnado_output/counts/{group}_metadata.tsv",
     output:
         scaling_factors="seqnado_output/resources/{group}_scaling_factors.tsv",
+    container:
+        "library://asmith151/seqnado/seqnado_report:latest"
     script:
         "../scripts/calculate_scaling_factors.R"
 
 
+rule calculate_scaling_factors_spikein:
+    input:
+        counts="seqnado_output/readcounts/feature_counts/read_counts.tsv",
+        metadata="seqnado_output/design.csv",
+    output:
+        size_factors="seqnado_output/resources/all_normalisation_factors.json"
+    container:
+        "library://asmith151/seqnado/seqnado_report:latest"
+    params:
+        spikein_genes=["AmpR_seq", "Cas9_5p_seq", "Cas9_3p_seq"],
+    log:
+        "seqnado_output/logs/normalisation_factors.log"
+    script:
+        "../scripts/calculate_spikein_norm_factors_rna.R"
+
+
+
 rule deeptools_make_bigwigs_scale:
     input:
         bam="seqnado_output/aligned/{sample}.bam",
         bai="seqnado_output/aligned/{sample}.bam.bai",
         scaling_factors=lambda wc: f"seqnado_output/resources/{get_group_for_sample(wc , DESIGN)}_scaling_factors.tsv",
     output:
         bigwig="seqnado_output/bigwigs/deeptools/csaw/{sample}.bigWig",
```

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/qc.smk` & `seqnado-0.5.1/seqnado/workflow/rules/qc.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/rules/variant.smk` & `seqnado-0.5.1/seqnado/workflow/rules/variant.smk`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/scripts/calculate_spikein_norm_factors.py` & `seqnado-0.5.1/seqnado/workflow/scripts/calculate_spikein_norm_factors.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/scripts/calculate_spikein_norm_orlando.py` & `seqnado-0.5.1/seqnado/workflow/scripts/calculate_spikein_norm_orlando.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/scripts/create_hub.py` & `seqnado-0.5.1/seqnado/workflow/scripts/create_hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,30 +19,29 @@
     columns=["fn"],
 )
 
 
 # Use the TrackFiles class to deduplicate files and add metadata
 df = tracknado.TrackFiles(files=df, deduplicate=True).files
 
-
 if snakemake.params.assay == "ChIP":
     df[["samplename", "antibody"]] = df["fn"].str.extract(
         r".*/(.*)_(.*)\.(?:bigBed|bigWig)"
     )
-    df["pileup_method"] = df["fn"].apply(lambda x: x.split("/")[-3])
+    df["method"] = df["fn"].apply(lambda x: x.split("/")[-3])
     df['norm'] = df['fn'].apply(lambda x: x.split("/")[-2])
 
 elif snakemake.params.assay == "ATAC":
     df["samplename"] = df["fn"].str.extract(r".*/(.*)\.(?:bigBed|bigWig)")
-    df["pileup_method"] = df["fn"].apply(lambda x: x.split("/")[-3])
+    df["method"] = df["fn"].apply(lambda x: x.split("/")[-3])
     df["norm"] = df["fn"].apply(lambda x: x.split("/")[-2])
 
 elif snakemake.params.assay == "RNA":
     df["samplename"] = df["fn"].apply(get_rna_samplename)
-    df["pileup_method"] = df["fn"].apply(lambda x: x.split("/")[-3])
+    df["method"] = df["fn"].apply(lambda x: x.split("/")[-3])
     df["strand"] = np.where(df["fn"].str.contains("_plus.bigWig"), "plus", "minus")
     df["norm"] = df["fn"].apply(lambda x: x.split("/")[-2])
 
 # Create hub design
 design = tracknado.TrackDesign.from_design(
     df,
     color_by=snakemake.params.color_by,
```

### Comparing `seqnado-0.5.0/seqnado/workflow/scripts/get_salmon_counts.py` & `seqnado-0.5.1/seqnado/workflow/scripts/get_salmon_counts.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/scripts/remove_blacklist.py` & `seqnado-0.5.1/seqnado/workflow/scripts/remove_blacklist.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/scripts/remove_duplicates.py` & `seqnado-0.5.1/seqnado/workflow/scripts/remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/scripts/shift_alignments.py` & `seqnado-0.5.1/seqnado/workflow/scripts/shift_alignments.py`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado/workflow/snakefile_atac` & `seqnado-0.5.1/seqnado/workflow/snakefile_rna`

 * *Files 16% similar despite different names*

```diff
@@ -4,90 +4,105 @@
 import shutil
 import sys
 
 import pandas as pd
 from snakemake.utils import min_version
 
 
-from seqnado.design import Design, ATACOutput
-from seqnado.helpers import format_config_dict, symlink_fastq_files
-
+from seqnado.design import Design, RNAOutput, NormGroups
+from seqnado.helpers import format_config_dict, symlink_fastq_files, remove_unwanted_run_files
 
 ####################
 # Hardcoded config #
 ####################
+ASSAY = "RNA"
+
+
+configfile: "config_rna.yml"
+
 
-ASSAY = "ATAC"
-configfile: "config_atac.yml"
 container: "library://asmith151/seqnado/seqnado_pipeline:latest"
 
 
 ####################
 # Experiment config #
 ####################
 
 # Load config
 format_config_dict(config)
 
 # Generate design
 if os.path.exists(config["design"]):
-    df = pd.read_csv(config["design"], sep=r"\s+|,|\t", engine="python", index_col=0).fillna("")
+    df = pd.read_csv(config["design"], sep=r"\s+|,|\t", engine="python").fillna("")
     DESIGN = Design.from_dataframe(df)
 else:
     DESIGN = Design.from_directory(".")
 
 # Attempt to symlink the fastq files
-assert len(DESIGN.fastq_paths) > 0, "No fastq files found in the working directory or no design file provided."
+assert (
+    len(DESIGN.fastq_paths) > 0
+), "No fastq files found in the working directory or no design file provided."
 symlink_fastq_files(DESIGN, output_dir="seqnado_output/fastqs")
 
-
 # Define global variables
 SAMPLE_NAMES = DESIGN.sample_names
-OUTPUT = ATACOutput(
+
+# DESeq2 parameters
+RUN_DESEQ2 = True if (DESIGN.to_dataframe().columns.str.contains("deseq2").any() and config["run_deseq2"]) else False
+del config["run_deseq2"]
+
+PROJECT_NAME = config['project_name'].replace(" ", "_").strip()
+config["project_name"] = PROJECT_NAME
+
+
+# Define output files
+OUTPUT = RNAOutput(
     assay=ASSAY,
     run_design=DESIGN,
     sample_names=SAMPLE_NAMES,
+    run_deseq2=RUN_DESEQ2,
+    scale_method="spikein" if config["spikein"] else None,
     **config
 )
 
-###################
-# Pipeline config #
-###################
+NORMALISATION_SCALING = NormGroups.from_design(DESIGN, subset_column="scale_group", include_controls=True)
+NORMALISATION_MERGING = NormGroups.from_design(DESIGN, subset_column="merge", include_controls=True)
 
-include: "rules/align.smk"
+# Rules to include
+include: "rules/align_rna.smk"
+include: "rules/alignment_counts.smk"
 include: "rules/alignment_post_processing.smk"
+include: "rules/deseq2_rna.smk"
 include: "rules/fastq_screen.smk"
 include: "rules/fastq_trim.smk"
-include: "rules/pileup_default.smk"
-include: "rules/pileup_norm.smk"
-include: "rules/pileup_grouped.smk"
-include: "rules/peak_call_other.smk"
-include: "rules/peak_call_grouped.smk"
-include: "rules/qc.smk"
 include: "rules/heatmap.smk"
 include: "rules/hub.smk"
+include: "rules/pileup_norm.smk"
+include: "rules/pileup_default.smk"
+include: "rules/qc.smk"
+
 
 rule all:
     input:
         OUTPUT.files
 
-onsuccess:
-    slurm_files = glob.glob("slurm-*.out")
-    sps_files = glob.glob("sps-*")
-    simg_files = glob.glob("*.simg")
-
-    for fn in [*slurm_files, *sps_files, *simg_files]:
-        try:
-            if not os.path.isdir(fn):
-                os.remove(fn)
-            else:
-                shutil.rmtree(fn)
 
-        except Exception as e:
-            print(e)
+
+
+
+
+
+
+
+onsuccess:
+    remove_unwanted_run_files()
+    
 
 onerror:
     log_out = "seqnado_error.log"
     shutil.copyfile(log, log_out)
     print(
         f"An error occurred. Please check the log file {log_out} for more information."
     )
+    remove_unwanted_run_files()
+
+
```

### Comparing `seqnado-0.5.0/seqnado/workflow/snakefile_chip` & `seqnado-0.5.1/seqnado/workflow/snakefile_chip`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import shutil
 import sys
 
 import pandas as pd
 from snakemake.utils import min_version
 
 
-from seqnado.design import DesignIP, ChIPOutput 
-from seqnado.helpers import format_config_dict, symlink_fastq_files, get_scale_method
+from seqnado.design import DesignIP, ChIPOutput, NormGroups
+from seqnado.helpers import format_config_dict, symlink_fastq_files, get_scale_method, remove_unwanted_run_files
 
 ####################
 # Hardcoded config #
 ####################
 
 ASSAY = "ChIP"
 configfile: "config_chip.yml"
@@ -24,43 +24,45 @@
 ####################
 
 # Load config
 format_config_dict(config)
 
 # Generate design
 if os.path.exists(config["design"]):
-    df = pd.read_csv(config["design"], sep=r"\s+|,|\t", engine="python", index_col=0).fillna("")
+    df = pd.read_csv(config["design"], sep=r"\s+|,|\t", engine="python").fillna("")
     DESIGN = DesignIP.from_dataframe(df)
 else:
     DESIGN = DesignIP.from_directory(".")
 
 # Attempt to symlink the fastq files
 assert len(DESIGN.fastq_paths) > 0, "No fastq files found in the working directory or no design file provided."
 symlink_fastq_files(DESIGN, output_dir="seqnado_output/fastqs")
 
 
 # Define global variables
 SAMPLE_NAMES = DESIGN.sample_names
 SAMPLE_NAMES_IP = DESIGN.sample_names_ip
 SAMPLE_NAMES_CONTROL = DESIGN.sample_names_control
-IP = DESIGN.ip_names
-CONTROL = DESIGN.control_names
-
+IP = DESIGN.ips_performed
+CONTROL = DESIGN.controls_performed
 
 # Define output files
 OUTPUT = ChIPOutput(
     assay=ASSAY,
     run_design=DESIGN,
     sample_names=SAMPLE_NAMES,
     ip_names=IP,
     control_names=CONTROL,
     scale_method=get_scale_method(config),
     **config    
 )
 
+NORMALISATION_SCALING = NormGroups.from_design(DESIGN, subset_column="scale_group", include_controls=True)
+NORMALISATION_MERGING = NormGroups.from_design(DESIGN, subset_column="merge", include_controls=True)
+
 
 # Load required rules
 include: "rules/align.smk"
 include: "rules/alignment_post_processing.smk"
 include: "rules/fastq_screen.smk"
 include: "rules/fastq_trim.smk"
 include: "rules/exogenous_norm.smk"
@@ -76,39 +78,28 @@
 
 if config["spikein"]:
     ruleorder: move_ref_bam > align_paired > align_single
     ruleorder: deeptools_make_bigwigs_spikein > deeptools_make_bigwigs
 else:
     ruleorder: align_paired > align_single > move_ref_bam
 
-# Define wildcard constraints
-wildcard_constraints:
-    treatment= "|".join(IP),
+# # Define wildcard constraints
+# wildcard_constraints:
+#     treatment= "|".join(IP),
 
 
 
 rule all:
     input:
         OUTPUT.files
 
 
 onsuccess:
-    slurm_files = glob.glob("slurm-*.out")
-    sps_files = glob.glob("sps-*")
-    simg_files = glob.glob("*.simg")
-
-    for fn in [*slurm_files, *sps_files, *simg_files]:
-        try:
-            if not os.path.isdir(fn):
-                os.remove(fn)
-            else:
-                shutil.rmtree(fn)
-
-        except Exception as e:
-            print(e)
+   remove_unwanted_run_files()
 
 onerror:
     log_out = "seqnado_error.log"
     shutil.copyfile(log, log_out)
     print(
         f"An error occurred. Please check the log file {log_out} for more information."
     )
+    remove_unwanted_run_files()
```

### Comparing `seqnado-0.5.0/seqnado/workflow/snakefile_rna` & `seqnado-0.5.1/seqnado/workflow/snakefile_snp`

 * *Files 19% similar despite different names*

```diff
@@ -1,95 +1,59 @@
-from datetime import datetime
-import glob
 import os
-import shutil
 import sys
-
-import pandas as pd
+import shutil
+from datetime import datetime
+import glob
 from snakemake.utils import min_version
+from seqnado.helpers import check_options
+import pandas as pd
 
-
-from seqnado.design import Design, RNAOutput 
-from seqnado.helpers import format_config_dict, symlink_fastq_files
-
-####################
-# Hardcoded config #
-####################
-ASSAY = "RNA"
-
-
-configfile: "config_rna.yml"
-
-
+ASSAY = "snp"
+configfile: "config_snp.yml"
 container: "library://asmith151/seqnado/seqnado_pipeline:latest"
 
+utils.format_config_dict(config)
 
-####################
-# Experiment config #
-####################
-
-# Load config
-format_config_dict(config)
-
-# Generate design
+# Get experiment design
 if os.path.exists(config["design"]):
-    df = pd.read_csv(config["design"], sep=r"\s+|,|\t", engine="python", index_col=0).fillna("")
-    DESIGN = Design.from_dataframe(df)
+    # Expect columns - sample fq1 fq2
+    FASTQ_SAMPLES = utils.GenericFastqSamples(
+        pd.read_csv(config["design"], sep="[\s+,\t]", engine="python")
+    )
+    assert FASTQ_SAMPLES.design.shape[0] > 0, "No samples found in design file"
+    for col in ["sample", "fq1", "fq2"]:
+        assert col in FASTQ_SAMPLES.design.columns, f"Design file must contain columns sample, fq1, fq2. Columns found: {FASTQ_SAMPLES.design.columns}"
+
 else:
-    DESIGN = Design.from_directory(".")
+    # Use pattern matching to get samples
+    fq_files = list(utils.get_fastq_files("."))
+    if fq_files:
+        FASTQ_SAMPLES = utils.GenericFastqSamples.from_files(fq_files)
+    else:
+        raise ValueError("No FASTQ files found in the working directory")
 
-# Attempt to symlink the fastq files
-assert (
-    len(DESIGN.fastq_paths) > 0
-), "No fastq files found in the working directory or no design file provided."
-symlink_fastq_files(DESIGN, output_dir="seqnado_output/fastqs")
-
-# Define global variables
-SAMPLE_NAMES = DESIGN.sample_names
-
-# DESeq2 parameters
-RUN_DESEQ2 = True if (DESIGN.to_dataframe().columns.str.contains("deseq2").any() and config["run_deseq2"]) else False
-del config["run_deseq2"]
-
-if config["spikein"] and not RUN_DESEQ2:
-    sys.exit("Spike-in normalization requires DESeq2 to be run and is not enabled.")
-
-
-PROJECT_NAME = config['project_name'].replace(" ", "_").strip()
-config["project_name"] = PROJECT_NAME
-
-
-# Define output files
-OUTPUT = RNAOutput(
-    assay=ASSAY,
-    run_design=DESIGN,
-    sample_names=SAMPLE_NAMES,
-    run_deseq2=RUN_DESEQ2,
-    scale_method="spikein" if config["spikein"] else None,
-    **config
-)
-
-# Rules to include
-include: "rules/align_rna.smk"
-include: "rules/alignment_counts.smk"
-include: "rules/alignment_post_processing.smk"
-include: "rules/deseq2_rna.smk"
-include: "rules/fastq_screen.smk"
+
+DESIGN = FASTQ_SAMPLES.design
+SAMPLE_NAMES = FASTQ_SAMPLES.sample_names_all
 include: "rules/fastq_trim.smk"
-include: "rules/heatmap.smk"
+include: "rules/fastq_screen.smk"
+include: "rules/align.smk"
+include: "rules/alignment_post_processing.smk"
 include: "rules/hub.smk"
-include: "rules/pileup_norm.smk"
-include: "rules/pileup_default.smk"
 include: "rules/qc.smk"
+include: "rules/variant.smk"
 
+OUTPUT = utils.define_output_files(snakemake_design=DESIGN,
+                                            sample_names=SAMPLE_NAMES,
+                                            assay=ASSAY,
+                                            **config)
 
 rule all:
     input:
-        OUTPUT.files
-
+        OUTPUT
 
 onsuccess:
     slurm_files = glob.glob("slurm-*.out")
     sps_files = glob.glob("sps-*")
     simg_files = glob.glob("*.simg")
 
     for fn in [*slurm_files, *sps_files, *simg_files]:
@@ -98,14 +62,13 @@
                 os.remove(fn)
             else:
                 shutil.rmtree(fn)
 
         except Exception as e:
             print(e)
 
-
 onerror:
     log_out = "seqnado_error.log"
     shutil.copyfile(log, log_out)
     print(
         f"An error occurred. Please check the log file {log_out} for more information."
     )
```

### Comparing `seqnado-0.5.0/seqnado.egg-info/PKG-INFO` & `seqnado-0.5.1/seqnado.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: seqnado
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pipelines for genomics analysis
 Author-email: Alastair Smith <alastair.smith@ndcls.ox.ac.uk>, Catherine Chahrour <catherine.chahrour@msdtc.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Homepage, https://github.com/alsmith151/seqnado
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: cookiecutter
 Requires-Dist: drmaa
 Requires-Dist: pandas
+Requires-Dist: pandera
 Requires-Dist: pulp<=2.7.0
 Requires-Dist: pydantic
 Requires-Dist: pyranges
 Requires-Dist: pyyaml
 Requires-Dist: seaborn
 Requires-Dist: setuptools_scm
 Requires-Dist: snakemake-wrapper-utils
```

### Comparing `seqnado-0.5.0/seqnado.egg-info/SOURCES.txt` & `seqnado-0.5.1/seqnado.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,17 @@
 seqnado/workflow/rules/peak_call_grouped.smk
 seqnado/workflow/rules/peak_call_other.smk
 seqnado/workflow/rules/pileup_default.smk
 seqnado/workflow/rules/pileup_grouped.smk
 seqnado/workflow/rules/pileup_norm.smk
 seqnado/workflow/rules/qc.smk
 seqnado/workflow/rules/variant.smk
-seqnado/workflow/scripts/calculate_scaling_norm_factors.r
+seqnado/workflow/scripts/calculate_scaling_factors.R
 seqnado/workflow/scripts/calculate_spikein_norm_factors.py
-seqnado/workflow/scripts/calculate_spikein_norm_factors.r
+seqnado/workflow/scripts/calculate_spikein_norm_factors_rna.R
 seqnado/workflow/scripts/calculate_spikein_norm_orlando.py
 seqnado/workflow/scripts/create_hub.py
 seqnado/workflow/scripts/get_salmon_counts.py
 seqnado/workflow/scripts/remove_blacklist.py
 seqnado/workflow/scripts/remove_duplicates.py
 seqnado/workflow/scripts/shift_alignments.py
 tests/test_pipelines.py
```

### Comparing `seqnado-0.5.0/seqnado_dev.yml` & `seqnado-0.5.1/seqnado_dev.yml`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/seqnado_logo.jpeg` & `seqnado-0.5.1/seqnado_logo.jpeg`

 * *Files identical despite different names*

### Comparing `seqnado-0.5.0/tests/test_pipelines.py` & `seqnado-0.5.1/tests/test_pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,16 +172,16 @@
         with tarfile.open(tar_path) as tar:
             tar.extractall(path=path.parent, filter="data")
 
     match assay:
         case "atac":
             files = list(path.glob("atac*.fastq.gz"))
         case "chip":
-            files = list(path.glob("CTCF*.fastq.gz"))
-            files.append(path / "SINGLE-CTCF_CTCF.fastq.gz")
+            files = list(path.glob("chip-rx*.fastq.gz"))
+            files.append(path / "chip-rx-single_MLL.fastq.gz")
         case "chip-rx":
             files = list(path.glob("chip-rx*.fastq.gz"))
         case "rna":
             files = list(path.glob("rna_*.fastq.gz"))
         case "rna-rx":
             files = list(path.glob("rna-spikein*.fastq.gz"))
 
@@ -323,14 +323,15 @@
     with open(config_yaml, "r") as f:
         config = yaml.safe_load(f)
 
     if assay == "chip":
         config["pileup_method"] = ["deeptools", "homer"]
         config['peak_calling_method'] = ["lanceotron", "macs", "homer"]
         config["library_complexity"] = False
+        config["bowtie2"]["options"] = "--no-mixed --no-discordant"
     elif assay == "chip-rx":
         config["call_peaks"] = True
         config["peak_calling_method"] = ["seacr"]
 
     with open(config_yaml, "w") as f:
         yaml.dump(config, f)
 
@@ -344,15 +345,22 @@
 
 @pytest.fixture(scope="function")
 def design(seqnado_run_dir, assay_type, assay):
     cmd = ["seqnado-design", assay_type]
     completed = subprocess.run(" ".join(cmd), shell=True, cwd=seqnado_run_dir)
     assert completed.returncode == 0
 
-    if assay == "rna-rx":
+    if assay == "chip":
+        # Add merge column to design file
+        import pandas as pd
+        df = pd.read_csv(seqnado_run_dir / "design.csv", index_col=0)
+        df["merge"] = "MLL-MERGED-TOGETHER"
+        df.to_csv(seqnado_run_dir / "design.csv")
+
+    elif assay == "rna-rx":
         # Add deseq2 column to design file
         import pandas as pd
 
         df = pd.read_csv(seqnado_run_dir / "design.csv", index_col=0)
         df["deseq2"] = df.index.str.split("-").str[-2]
         df.to_csv(seqnado_run_dir / "design.csv")
```

