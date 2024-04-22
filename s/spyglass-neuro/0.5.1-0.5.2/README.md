# Comparing `tmp/spyglass_neuro-0.5.1.tar.gz` & `tmp/spyglass_neuro-0.5.2.tar.gz`

## Comparing `spyglass_neuro-0.5.1.tar` & `spyglass_neuro-0.5.2.tar`

### file list

```diff
@@ -1,283 +1,289 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.gitattributes
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.markdownlint.yaml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/CITATION.cff
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/MANIFEST.in
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/dj_local_conf_example.json
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/environment.yml
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/environment_dlc.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/setup.cfg
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.github/pull_request_template.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.github/workflows/test-conda.yml
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.github/workflows/test-package-build.yml
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.vscode/extensions.json
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.vscode/settings.json
--rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/config/add_dj_collaborator.py
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/config/add_dj_guest.py
--rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/config/add_dj_module.py
--rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/config/add_dj_user.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/config/datajoint_user_config.yml
--rwxr-xr-x   0        0        0      678 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/config/dj_config.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/README.md
--rwxr-xr-x   0        0        0     2161 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/build-docs.sh
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/overrides/nav.html
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/contribute.md
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/index.md
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/installation.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/api/index.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/api/make_pages.py
--rw-r--r--   0        0        0   297397 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/images/FrankLab.png
--rw-r--r--   0        0        0    75394 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/images/Spyglass.png
--rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/images/Spyglass.svg
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/images/fig1.png
--rw-r--r--   0        0        0    98482 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/images/merge_diagram.png
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/misc/database_management.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/misc/figurl_views.md
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/misc/index.md
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/misc/insert_data.md
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/misc/merge_tables.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/misc/session_groups.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/docs/src/stylesheets/extra.css
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/artifactdetectionparameters_default.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/artifactdetectionparameters_none.yaml
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/create_session_group.py
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/create_spike_sorting_recording.sh
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/create_spike_sorting_recording_view.sh
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/create_spike_sorting_view.sh
--rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/create_spyglass_view.sh
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_artifact_detection_parameters.sh
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_lab_member.sh
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_lab_team.sh
--rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_lab_team_member.sh
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_session.sh
--rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_sort_interval.py
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_spike_sorter_parameters.sh
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/insert_spike_sorting_preprocessing_parameters.sh
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/labmember.yaml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/labteammember.yaml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/parameters.yaml
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/readme.md
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/run_spike_sorting.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/set_sort_groups_by_shank.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/spikesorterparameters_default.yaml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/spikesortingpreprocessingparameters.yaml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/team.yaml
--rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/cli_examples/update_lab_team_description.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/config_yaml/entries.yaml
--rw-r--r--   0        0        0    53048 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/franklab_scripts/alter_tables.py
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/franklab_scripts/nightly_cleanup.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/franklab_scripts/sort.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/00_Setup.ipynb
--rw-r--r--   0        0        0   128150 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/01_Insert_Data.ipynb
--rw-r--r--   0        0        0    47991 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/02_Data_Sync.ipynb
--rw-r--r--   0        0        0  2174443 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/03_Merge_Tables.ipynb
--rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/04_PopulateConfigFile.ipynb
--rw-r--r--   0        0        0   103897 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/10_Spike_SortingV0.ipynb
--rw-r--r--   0        0        0    25027 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/10_Spike_SortingV1.ipynb
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/11_CurationV0.ipynb
--rw-r--r--   0        0        0   699515 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/20_Position_Trodes.ipynb
--rw-r--r--   0        0        0    84430 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/21_DLC.ipynb
--rw-r--r--   0        0        0    31324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/22_DLC_Loop.ipynb
--rw-r--r--   0        0        0   877085 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/24_Linearization.ipynb
--rw-r--r--   0        0        0   232187 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/30_LFP.ipynb
--rw-r--r--   0        0        0   520960 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/31_Theta.ipynb
--rw-r--r--   0        0        0   124350 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/32_Ripple_Detection.ipynb
--rw-r--r--   0        0        0   131467 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb
--rw-r--r--   0        0        0   178925 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/41_Decoding_Clusterless.ipynb
--rw-r--r--   0        0        0    79021 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/42_Decoding_SortedSpikes.ipynb
--rw-r--r--   0        0        0   129019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/50_MUA_Detection.ipynb
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/README.md
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/00_Setup.py
--rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/01_Insert_Data.py
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/02_Data_Sync.py
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/03_Merge_Tables.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/04_PopulateConfigFile.py
--rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/10_Spike_SortingV0.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/10_Spike_SortingV1.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/11_CurationV0.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/20_Position_Trodes.py
--rw-r--r--   0        0        0    26539 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/21_DLC.py
--rw-r--r--   0        0        0    19409 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/22_DLC_Loop.py
--rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/24_Linearization.py
--rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/30_LFP.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/31_Theta.py
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/32_Ripple_Detection.py
--rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py
--rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/42_Decoding_Clusterless.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/43_Decoding_SortedSpikes.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/notebooks/py_scripts/51_MUA_Detection.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/_version.py
--rw-r--r--   0        0        0    19703 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/settings.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/cli/__init__.py
--rw-r--r--   0        0        0    14650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/cli/cli.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/__init__.py
--rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_behav.py
--rw-r--r--   0        0        0    26420 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_device.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_dio.py
--rw-r--r--   0        0        0    34946 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_ephys.py
--rw-r--r--   0        0        0    19143 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_filter.py
--rw-r--r--   0        0        0    17240 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_interval.py
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_lab.py
--rw-r--r--   0        0        0    24995 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_nwbfile.py
--rw-r--r--   0        0        0    27319 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_position.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_region.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_ripple.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_sensors.py
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_session.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_subject.py
--rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_task.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/common_usage.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/errors.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/populate_all_common.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/signal_processing.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/prepopulate/__init__.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/common/prepopulate/prepopulate.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/data_import/__init__.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/data_import/insert_sessions.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/__init__.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/decoding_merge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/__init__.py
--rw-r--r--   0        0        0    26847 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/clusterless.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/core.py
--rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/dj_decoder_conversion.py
--rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/sorted_spikes.py
--rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/visualization.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/visualization_1D_view.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v0/visualization_2D_view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v1/__init__.py
--rw-r--r--   0        0        0    17992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v1/clusterless.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v1/core.py
--rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v1/dj_decoder_conversion.py
--rw-r--r--   0        0        0    16294 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v1/sorted_spikes.py
--rw-r--r--   0        0        0    12224 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/decoding/v1/waveform_features.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/lfp_electrode.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/lfp_imported.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/lfp_merge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/analysis/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/analysis/v1/__init__.py
--rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/analysis/v1/lfp_band.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/v1/__init__.py
--rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp_artifact.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/linearization/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/linearization/merge.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/linearization/v0/__init__.py
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/linearization/v0/main.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/linearization/v1/__init__.py
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/linearization/v1/main.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lock/__init__.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/lock/file_lock.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/mua/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/mua/v1/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/mua/v1/mua.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/__init__.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/position_merge.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/__init__.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/dlc_decorators.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/dlc_reader.py
--rw-r--r--   0        0        0    45570 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/dlc_utils.py
--rw-r--r--   0        0        0    28632 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_centroid.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_cohort.py
--rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_model.py
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_orient.py
--rw-r--r--   0        0        0    16278 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_pose_estimation.py
--rw-r--r--   0        0        0    17212 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_position.py
--rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_project.py
--rw-r--r--   0        0        0    15728 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_selection.py
--rw-r--r--   0        0        0     9551 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_training.py
--rw-r--r--   0        0        0    14388 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/position/v1/position_trodes_position.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/ripple/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/ripple/v1/__init__.py
--rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/ripple/v1/ripple.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/sharing/__init__.py
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/sharing/sharing_kachery.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/__init__.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/imported.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/spikesorting_merge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/analysis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/analysis/v1/__init__.py
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/analysis/v1/group.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/__init__.py
--rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/curation_figurl.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/merged_sorting_extractor.py
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/sortingview.py
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/sortingview_helper_fn.py
--rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_artifact.py
--rw-r--r--   0        0        0    39520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_curation.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_populator.py
--rw-r--r--   0        0        0    23579 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_recording.py
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_sorting.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/figurl_views/__init__.py
--rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/__init__.py
--rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/artifact.py
--rw-r--r--   0        0        0    14918 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/curation.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/figurl_curation.py
--rw-r--r--   0        0        0    19276 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/metric_curation.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/metric_utils.py
--rw-r--r--   0        0        0    32996 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/recording.py
--rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/sorting.py
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/utils.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/__init__.py
--rwxr-xr-x   0        0        0     7345 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/database_settings.py
--rw-r--r--   0        0        0    13345 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/dj_chains.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/dj_helper_fn.py
--rw-r--r--   0        0        0    29253 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/dj_merge_tables.py
--rw-r--r--   0        0        0    19047 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/dj_mixin.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/logging.py
--rw-r--r--   0        0        0    17753 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/src/spyglass/utils/nwb_helper_fn.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/container.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/conftest.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_behav.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_device.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_dio.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_ephys.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_filter.py
--rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_insert.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_interval.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_interval_helpers.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_lab.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_nwbfile.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_position.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_region.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_ripple.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_sensors.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/common/test_session.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/data_import/__init__.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/data_import/test_insert_sessions.py
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/lfp/conftest.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/lfp/test_lfp.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/linearization/conftest.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/linearization/test_lin.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/position/test_trodes.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/conftest.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/test_chains.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/test_db_settings.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/test_dj_helper_fn.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/test_logging.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/test_merge.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/test_mixin.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/tests/utils/test_nwb_helper_fn.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/LICENSE
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/README.md
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.gitattributes
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.markdownlint.yaml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9432 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/CITATION.cff
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/MANIFEST.in
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/dj_local_conf_example.json
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/environment.yml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/environment_dlc.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/setup.cfg
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/test-conda.yml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.github/workflows/test-package-build.yml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.vscode/extensions.json
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.vscode/settings.json
+-rwxr-xr-x   0        0        0      336 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_collaborator.py
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_guest.py
+-rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_module.py
+-rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/add_dj_user.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/datajoint_user_config.yml
+-rwxr-xr-x   0        0        0      678 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/config/dj_config.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/README.md
+-rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/build-docs.sh
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/overrides/nav.html
+-rw-r--r--   0        0        0     9683 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/contribute.md
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/index.md
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/installation.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/api/index.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/api/make_pages.py
+-rw-r--r--   0        0        0   297397 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/FrankLab.png
+-rw-r--r--   0        0        0    75394 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/Spyglass.png
+-rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/Spyglass.svg
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/fig1.png
+-rw-r--r--   0        0        0    98482 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/images/merge_diagram.png
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/database_management.md
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/export.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/figurl_views.md
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/index.md
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/insert_data.md
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/merge_tables.md
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/mixin.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/misc/session_groups.md
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/docs/src/stylesheets/extra.css
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/artifactdetectionparameters_default.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/artifactdetectionparameters_none.yaml
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_session_group.py
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spike_sorting_recording.sh
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spike_sorting_recording_view.sh
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spike_sorting_view.sh
+-rwxr-xr-x   0        0        0       73 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/create_spyglass_view.sh
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_artifact_detection_parameters.sh
+-rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_lab_member.sh
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_lab_team.sh
+-rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_lab_team_member.sh
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_session.sh
+-rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_sort_interval.py
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_spike_sorter_parameters.sh
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/insert_spike_sorting_preprocessing_parameters.sh
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/labmember.yaml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/labteammember.yaml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/parameters.yaml
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/readme.md
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/run_spike_sorting.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/set_sort_groups_by_shank.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/spikesorterparameters_default.yaml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/spikesortingpreprocessingparameters.yaml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/team.yaml
+-rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/cli_examples/update_lab_team_description.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/config_yaml/entries.yaml
+-rw-r--r--   0        0        0    53048 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/franklab_scripts/alter_tables.py
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/franklab_scripts/nightly_cleanup.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/franklab_scripts/sort.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/00_Setup.ipynb
+-rw-r--r--   0        0        0   128150 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/01_Insert_Data.ipynb
+-rw-r--r--   0        0        0    47991 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/02_Data_Sync.ipynb
+-rw-r--r--   0        0        0  2174485 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/03_Merge_Tables.ipynb
+-rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/04_PopulateConfigFile.ipynb
+-rw-r--r--   0        0        0    27301 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/05_Export.ipynb
+-rw-r--r--   0        0        0   137862 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/10_Spike_SortingV0.ipynb
+-rw-r--r--   0        0        0    99395 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/10_Spike_SortingV1.ipynb
+-rw-r--r--   0        0        0   699515 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/20_Position_Trodes.ipynb
+-rw-r--r--   0        0        0    84430 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/21_DLC.ipynb
+-rw-r--r--   0        0        0    31324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/22_DLC_Loop.ipynb
+-rw-r--r--   0        0        0   877085 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/24_Linearization.ipynb
+-rw-r--r--   0        0        0   232187 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/30_LFP.ipynb
+-rw-r--r--   0        0        0   520960 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/31_Theta.ipynb
+-rw-r--r--   0        0        0   404028 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/32_Ripple_Detection.ipynb
+-rw-r--r--   0        0        0    92888 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb
+-rw-r--r--   0        0        0   178894 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/41_Decoding_Clusterless.ipynb
+-rw-r--r--   0        0        0    75214 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/42_Decoding_SortedSpikes.ipynb
+-rw-r--r--   0        0        0   129019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/50_MUA_Detection.ipynb
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/README.md
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/00_Setup.py
+-rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/01_Insert_Data.py
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/02_Data_Sync.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/03_Merge_Tables.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/04_PopulateConfigFile.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/05_Export.py
+-rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/10_Spike_SortingV0.py
+-rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/10_Spike_SortingV1.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/20_Position_Trodes.py
+-rw-r--r--   0        0        0    26539 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/21_DLC.py
+-rw-r--r--   0        0        0    19409 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/22_DLC_Loop.py
+-rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/24_Linearization.py
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/30_LFP.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/31_Theta.py
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/32_Ripple_Detection.py
+-rw-r--r--   0        0        0    11057 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/40_Extracting_Clusterless_Waveform_Features.py
+-rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/41_Decoding_Clusterless.py
+-rw-r--r--   0        0        0    10272 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py
+-rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/42_Decoding_Clusterless.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/42_Decoding_SortedSpikes.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/43_Decoding_SortedSpikes.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/notebooks/py_scripts/51_MUA_Detection.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/_version.py
+-rw-r--r--   0        0        0    20126 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/settings.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/cli/__init__.py
+-rw-r--r--   0        0        0    14650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/cli/cli.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/__init__.py
+-rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_behav.py
+-rw-r--r--   0        0        0    26420 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_device.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_dio.py
+-rw-r--r--   0        0        0    35128 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_ephys.py
+-rw-r--r--   0        0        0    19143 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_filter.py
+-rw-r--r--   0        0        0    17246 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_interval.py
+-rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_lab.py
+-rw-r--r--   0        0        0    28397 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_nwbfile.py
+-rw-r--r--   0        0        0    27415 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_position.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_region.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_ripple.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_sensors.py
+-rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_session.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_subject.py
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_task.py
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/common_usage.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/errors.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/populate_all_common.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/signal_processing.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/prepopulate/__init__.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/common/prepopulate/prepopulate.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/data_import/__init__.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/data_import/insert_sessions.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/__init__.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/decoding_merge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/__init__.py
+-rw-r--r--   0        0        0    26920 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/clusterless.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/core.py
+-rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/dj_decoder_conversion.py
+-rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/sorted_spikes.py
+-rw-r--r--   0        0        0    20617 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_1D_view.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_2D_view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/__init__.py
+-rw-r--r--   0        0        0    18008 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/clusterless.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/core.py
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/dj_decoder_conversion.py
+-rw-r--r--   0        0        0    16300 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/sorted_spikes.py
+-rw-r--r--   0        0        0    12380 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/decoding/v1/waveform_features.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_electrode.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_imported.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_merge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/v1/__init__.py
+-rw-r--r--   0        0        0    18049 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/v1/lfp_band.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/__init__.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py
+-rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/merge.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v0/__init__.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v0/main.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v1/__init__.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/linearization/v1/main.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lock/__init__.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/lock/file_lock.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/mua/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/mua/v1/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/mua/v1/mua.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/__init__.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/position_merge.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/__init__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_decorators.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_reader.py
+-rw-r--r--   0        0        0    45570 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_utils.py
+-rw-r--r--   0        0        0    28739 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_centroid.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_cohort.py
+-rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_model.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_orient.py
+-rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_pose_estimation.py
+-rw-r--r--   0        0        0    17289 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_position.py
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_project.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_selection.py
+-rw-r--r--   0        0        0     9551 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_training.py
+-rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/position/v1/position_trodes_position.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/ripple/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/ripple/v1/__init__.py
+-rw-r--r--   0        0        0    17519 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/ripple/v1/ripple.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/sharing/__init__.py
+-rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/sharing/sharing_kachery.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/__init__.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/imported.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/spikesorting_merge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/v1/__init__.py
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/v1/group.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/__init__.py
+-rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/curation_figurl.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/merged_sorting_extractor.py
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview.py
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview_helper_fn.py
+-rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_artifact.py
+-rw-r--r--   0        0        0    41121 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_curation.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_populator.py
+-rw-r--r--   0        0        0    23579 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_recording.py
+-rw-r--r--   0        0        0    10095 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_sorting.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/__init__.py
+-rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/__init__.py
+-rw-r--r--   0        0        0    14842 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/artifact.py
+-rw-r--r--   0        0        0    16347 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/curation.py
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/figurl_curation.py
+-rw-r--r--   0        0        0    19431 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_curation.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_utils.py
+-rw-r--r--   0        0        0    33193 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/recording.py
+-rw-r--r--   0        0        0    13943 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/sorting.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/utils.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/__init__.py
+-rwxr-xr-x   0        0        0     7345 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/database_settings.py
+-rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_chains.py
+-rw-r--r--   0        0        0    12976 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_graph.py
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_helper_fn.py
+-rw-r--r--   0        0        0    30084 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_merge_tables.py
+-rw-r--r--   0        0        0    27533 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/dj_mixin.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/logging.py
+-rw-r--r--   0        0        0    17753 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/src/spyglass/utils/nwb_helper_fn.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0    12154 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/container.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/conftest.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_behav.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_device.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_dio.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_ephys.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_filter.py
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_insert.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_interval.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_interval_helpers.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_lab.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_nwbfile.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_position.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_region.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_ripple.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_sensors.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/common/test_session.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/data_import/__init__.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/data_import/test_insert_sessions.py
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/lfp/conftest.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/lfp/test_lfp.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/linearization/conftest.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/linearization/test_lin.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/position/test_trodes.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/conftest.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_chains.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_db_settings.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_dj_helper_fn.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_logging.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_merge.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_mixin.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/tests/utils/test_nwb_helper_fn.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/LICENSE
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/README.md
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 spyglass_neuro-0.5.2/PKG-INFO
```

### Comparing `spyglass_neuro-0.5.1/.pre-commit-config.yaml` & `spyglass_neuro-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/CHANGELOG.md` & `spyglass_neuro-0.5.2/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,40 @@
 # Change Log
 
+## [0.5.2] (April 22, 2024)
+
+### Infrastructure
+
+- Refactor `TableChain` to include `_searched` attribute. #867
+- Fix errors in config import #882
+- Save current spyglass version in analysis nwb files to aid diagnosis #897
+- Add functionality to export vertical slice of database. #875
+- Add pynapple support #898
+- Update PR template checklist to include db changes. #903
+- Avoid permission check on personnel tables. #903
+- Add documentation for `SpyglassMixin`. #903
+- Add helper to identify merge table by definition. #903
+- Prioritize datajoint filepath entry for defining abs_path of analysis nwbfile
+    #918
+- Fix potential duplicate entries in Merge part tables #922
+- Add logging of AnalysisNwbfile creation time and size #937
+- Fix error on empty delete call in merge table. #940
+- Add log of AnalysisNwbfile creation time, size, and access count #937, #941
+
+### Pipelines
+
+- Spikesorting
+    - Update calls in v0 pipeline for spikeinterface>=0.99 #893
+    - Fix method type of `get_spike_times` #904
+    - Add helper functions for restricting spikesorting results and linking to
+        probe info #910
+- Decoding
+    - Handle dimensions of clusterless `get_ahead_behind_distance` #904
+    - Fix improper handling of nwb file names with .strip #929
+
 ## [0.5.1] (March 7, 2024)
 
 ### Infrastructure
 
 - Add user roles to `database_settings.py`. #832
 - Fix redundancy in `waveforms_dir` #857
 - Revise `dj_chains` to permit undirected paths for paths with multiple Merge
@@ -13,16 +44,17 @@
 
 - Position:
     - Fixes to `environment-dlc.yml` restricting tensortflow #834
     - Video restriction for multicamera epochs #834
     - Fixes to `_convert_mp4` #834
     - Replace deprecated calls to `yaml.safe_load()` #834
 - Spikesorting:
-    - Increase`spikeinterface` version to >=0.99.1, <0.100 #852
+    - Increase`spikeinterface` version to >=0.99.1, \<0.100 #852
     - Bug fix in single artifact interval edge case #859
+    - Bug fix in FigURL #871
 - LFP
     - In LFPArtifactDetection, only apply referencing if explicitly selected #863
 
 ## [0.5.0] (February 9, 2024)
 
 ### Infrastructure
 
@@ -189,7 +221,9 @@
 [0.3.3]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.3.3
 [0.3.4]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.3.4
 [0.4.0]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.0
 [0.4.1]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.1
 [0.4.2]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.2
 [0.4.3]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.4.3
 [0.5.0]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.5.0
+[0.5.1]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.5.1
+[0.5.2]: https://github.com/LorenFrankLab/spyglass/releases/tag/0.5.2
```

### Comparing `spyglass_neuro-0.5.1/CITATION.cff` & `spyglass_neuro-0.5.2/CITATION.cff`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,34 @@
     orcid: 'https://orcid.org/0000-0003-0357-351X'
     affiliation: 'University of California, San Francisco'
   - given-names: Xulu
     family-names: Sun
     email: xulu.sun@ucsf.edu
     affiliation: 'University of California, San Francisco'
     orcid: 'https://orcid.org/0000-0003-3076-0994'
+  - given-names: Broyles
+    family-names: Emrey
+    email: emrey.broyles@ucsf.edu
+    affiliation: 'University of California, San Francisco'
+    orcid: 'https://orcid.org/0000-0001-5559-2910'
+  - given-names: Shin
+    family-names: Donghoon
+    email: donghoon.shin@ucsf.edu
+    affiliation: 'University of California, San Francisco'
+    orcid: 'https://orcid.org/0009-0000-8916-7314'
+  - given-names: Chiang
+    family-names: Sharon
+    email: sharon.chiang@ucsf.edu
+    affiliation: 'University of California, San Francisco'
+    orcid: 'https://orcid.org/0000-0002-4548-4550'
+  - given-names: Holobetz
+    family-names: Cristofer
+    email: cristofer.holobetz.23@ucl.ac.uk
+    affiliation: 'University College London'
+    orcid: 'https://orcid.org/0009-0009-8567-3290'
   - given-names: Andrew
     family-names: Tritt
     email: ajtritt@lbl.gov
     affiliation: Lawrence Berkeley National Laboratory
     orcid: 'https://orcid.org/0000-0002-1617-449X'
   - given-names: Oliver
     family-names: Rübel
@@ -142,9 +162,9 @@
   - interactive data visualization
   - Neurodata Without Borders
   - Spike interface
   - Datajoint
   - spike sorting
   - kachery
 license: MIT
-version: 0.5.1
-date-released: '2024-03-07'
+version: 0.5.2
+date-released: '2024-04-22'
```

### Comparing `spyglass_neuro-0.5.1/CODE_OF_CONDUCT.md` & `spyglass_neuro-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/dj_local_conf_example.json` & `spyglass_neuro-0.5.2/dj_local_conf_example.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996141975308643%*

 * *Differences: {"'custom'": "{'kachery_dirs': {'cloud': '/your/base/path/.kachery-cloud'}}"}*

```diff
@@ -6,15 +6,15 @@
         "dlc_dirs": {
             "base": "/your/base/path/deeplabcut",
             "output": "/your/base/path/deeplabcut/output",
             "project": "/your/base/path/deeplabcut/projects",
             "video": "/your/base/path/deeplabcut/video"
         },
         "kachery_dirs": {
-            "cloud": "/your/base/path/kachery_storage",
+            "cloud": "/your/base/path/.kachery-cloud",
             "storage": "/your/base/path/kachery_storage",
             "temp": "/your/base/path/tmp"
         },
         "kachery_zone": "franklab.default",
         "spyglass_dirs": {
             "analysis": "/your/base/path/analysis",
             "base": "/your/base/path",
```

### Comparing `spyglass_neuro-0.5.1/environment.yml` & `spyglass_neuro-0.5.2/environment.yml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/environment_dlc.yml` & `spyglass_neuro-0.5.2/environment_dlc.yml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,29 @@
 ---
 
 **Describe the bug**
 A clear and concise description of what the bug is.
 
 **To Reproduce**
 Steps to reproduce the behavior:
+
 1. This error is on file '....' at file path '....'
 2. Click on '....'
 3. Scroll down to '....'
 4. See error
 
+</details><summary>Error Stack</summary>
+
+```python
+# Paste the error stack trace here
+```
+
+</details>
+
 **Expected behavior**
 A clear and concise description of what you expected to happen.
 
 **Screenshots**
 If applicable, add screenshots to help explain your problem.
 
 **Additional context**
 Add any other context about the problem here.
-
```

### Comparing `spyglass_neuro-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `spyglass_neuro-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 title: ''
 labels: ''
 assignees: ''
 
 ---
 
 **Is your feature request related to a problem? Please describe.**
-A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
+A clear and concise description of what the problem is.
+For example, I'm always frustrated when [...]
 
 **Describe the solution you'd like**
 A clear and concise description of what you want to happen.
 
 **Describe alternatives you've considered**
-A clear and concise description of any alternative solutions or features you've considered.
+A clear and concise description of any alternative solutions or features you've
+considered.
 
 **Additional context**
 Add any other context or screenshots about the feature request here.
```

### Comparing `spyglass_neuro-0.5.1/.github/workflows/publish-docs.yml` & `spyglass_neuro-0.5.2/.github/workflows/publish-docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,14 @@
       - name: Setup - pip & config
         run: |
           pip install .[docs]
           git config user.name 'github-actions[bot]' && git config user.email 'github-actions[bot]@users.noreply.github.com'
 
       - name: Deploy
         run: |
-          FULL_VERSION=${{ github.ref }}
+          FULL_VERSION=${{ github.ref_name }}
           export MAJOR_VERSION=${FULL_VERSION:0:3}
           echo "OWNER: ${REPO_OWNER}. BUILD: ${MAJOR_VERSION}"
           bash ./docs/build-docs.sh push $REPO_OWNER
         env:
           USERNAME: github-actions[bot]
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `spyglass_neuro-0.5.1/.github/workflows/test-conda.yml` & `spyglass_neuro-0.5.2/.github/workflows/test-conda.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 name: Test conda env and run tests
 
 on:
   push:
     branches: 
       - '!test_branch'
+      - '!documentation'
   schedule:  # once a day at midnight UTC
     - cron: '0 0 * * *'
 
 jobs:
   run-tests:
     runs-on: ${{ matrix.os }}
     defaults:
```

### Comparing `spyglass_neuro-0.5.1/.github/workflows/test-package-build.yml` & `spyglass_neuro-0.5.2/.github/workflows/test-package-build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 on:
   push:
     branches:
       - master
       - maint/*
       - '!test_branch'
+      - '!documentation'
     tags:
       - "*"
   pull_request:
     branches:
       - master
       - maint/*
 defaults:
@@ -85,15 +86,15 @@
     runs-on: ubuntu-latest
     needs: [test-package]
     environment:
       name: pypi
       url: https://pypi.org/p/spyglass-neuro
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/') && github.ref == 'refs/heads/master'
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: dist
           path: dist/
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `spyglass_neuro-0.5.1/.vscode/extensions.json` & `spyglass_neuro-0.5.2/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/.vscode/settings.json` & `spyglass_neuro-0.5.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/config/dj_config.py` & `spyglass_neuro-0.5.2/config/dj_config.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/README.md` & `spyglass_neuro-0.5.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/build-docs.sh` & `spyglass_neuro-0.5.2/docs/build-docs.sh`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Then, navigate to localhost:8000/ to inspect site, then ctrl+c to exit
 # For auto-reload during dev, use `mkdocs serve -f ./docs/mkdocs.yaml`
 
 # Copy top-level repo files for docs display
 cp ./CHANGELOG.md ./docs/src/
 cp ./LICENSE ./docs/src/LICENSE.md
 mkdir -p ./docs/src/notebooks
+rm -r ./docs/src/notebooks/*
 cp ./notebooks/*ipynb ./docs/src/notebooks/
 cp ./notebooks/*md ./docs/src/notebooks/
 mv ./docs/src/notebooks/README.md ./docs/src/notebooks/index.md
 cp -r ./notebook-images ./docs/src/notebooks/
 cp -r ./notebook-images ./docs/src/
 
 if [ -z "$MAJOR_VERSION" ]; then # Get version from file
```

### Comparing `spyglass_neuro-0.5.1/docs/mkdocs.yml` & `spyglass_neuro-0.5.2/docs/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -47,18 +47,18 @@
       - Overview: notebooks/index.md
       - Intro:
           - Setup: notebooks/00_Setup.ipynb
           - Insert Data: notebooks/01_Insert_Data.ipynb
           - Data Sync: notebooks/02_Data_Sync.ipynb
           - Merge Tables: notebooks/03_Merge_Tables.ipynb
           - Config Populate: notebooks/04_PopulateConfigFile.ipynb
+          - Export: notebooks/05_Export.ipynb
       - Spikes:
           - Spike Sorting V0: notebooks/10_Spike_SortingV0.ipynb
           - Spike Sorting V1: notebooks/10_Spike_SortingV1.ipynb
-          - Curation: notebooks/11_CurationV0.ipynb
       - Position:
           - Position Trodes: notebooks/20_Position_Trodes.ipynb
           - DLC Models: notebooks/21_DLC.ipynb
           - Looping DLC: notebooks/22_DLC_Loop.ipynb
           - Linearization: notebooks/24_Linearization.ipynb
       - LFP:
           - LFP: notebooks/30_LFP.ipynb
@@ -72,14 +72,15 @@
   - Miscellaneous:
       - Overview: misc/index.md
       - FigURL: misc/figurl_views.md
       - Session Groups: misc/session_groups.md
       - Insert Data: misc/insert_data.md
       - Merge Tables: misc/merge_tables.md
       - Database Management: misc/database_management.md
+      - Export: misc/export.md
   - API Reference: api/ # defer to gen-files + literate-nav
   - How to Contribute: contribute.md
   - Change Log: CHANGELOG.md
   - Copyright: LICENSE.md
 
 extra_css:
   - stylesheets/extra.css
```

### Comparing `spyglass_neuro-0.5.1/docs/src/contribute.md` & `spyglass_neuro-0.5.2/docs/src/contribute.md`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 By convention, an individual pipeline has one or more the following table types:
 
 - Common/Multi-pipeline table
 - NWB ingestion table
 - Parameters table
 - Selection table
 - Data table
-- Merge Table (see also [doc](./misc/merge_tables.md)
+- Merge Table (see also [doc](./misc/merge_tables.md))
 
 ### Common/Multi-pipeline
 
 Tables shared across multiple pipelines for shared data types.
 
 - Naming convention: None
 - Data tier: `dj.Manual`
@@ -222,24 +222,16 @@
     associated with each sample. Some older recordings are missing PTP times,
     and times must be inferred from the TTL pulses from the camera.
 
 ## Misc
 
 - During development, we suggest using a Docker container. See
     [example](./notebooks/00_Setup.ipynb).
-- DataJoint is unable to set delete permissions on a per-table basis. If a user
-    is able to delete entries in a given table, she can delete entries in any
-    table in the schema. The `SpikeSorting` table extends the built-in `delete`
-    method to check if the username matches a list of allowed users when
-    `delete` is called. Issues #226 and #586 track the progress of generalizing
-    this feature.
 - `numpy` style docstrings will be interpreted by API docs. To check for
     compliance, monitor the std out when building docs (see `docs/README.md`)
-- `fetch_nwb` is currently reperated across many tables. For progress on a fix,
-    follow issue #530
 
 ## Making a release
 
 Spyglass follows [Semantic Versioning](https://semver.org/) with versioning of
 the form `X.Y.Z` (e.g., `0.4.2`).
 
 1. In `CITATION.cff`, update the `version` key.
```

### Comparing `spyglass_neuro-0.5.1/docs/src/index.md` & `spyglass_neuro-0.5.2/docs/src/index.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/installation.md` & `spyglass_neuro-0.5.2/docs/src/installation.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/api/index.md` & `spyglass_neuro-0.5.2/docs/src/api/index.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/api/make_pages.py` & `spyglass_neuro-0.5.2/docs/src/api/make_pages.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/images/FrankLab.png` & `spyglass_neuro-0.5.2/docs/src/images/FrankLab.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/images/Spyglass.png` & `spyglass_neuro-0.5.2/docs/src/images/Spyglass.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/images/Spyglass.svg` & `spyglass_neuro-0.5.2/docs/src/images/Spyglass.svg`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/images/fig1.png` & `spyglass_neuro-0.5.2/docs/src/images/fig1.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/images/merge_diagram.png` & `spyglass_neuro-0.5.2/docs/src/images/merge_diagram.png`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/misc/database_management.md` & `spyglass_neuro-0.5.2/docs/src/misc/database_management.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/misc/figurl_views.md` & `spyglass_neuro-0.5.2/docs/src/misc/figurl_views.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/misc/insert_data.md` & `spyglass_neuro-0.5.2/docs/src/misc/insert_data.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/misc/merge_tables.md` & `spyglass_neuro-0.5.2/docs/src/misc/merge_tables.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,31 +6,14 @@
 Merge Tables allow us to join divergent pipelines together, and unify downstream
 processing steps. For a more in depth discussion, please refer to
 [this notebook](https://github.com/ttngu207/db-programming-with-datajoint/blob/master/notebooks/pipelines_merging_design_master_part.ipynb)
 and related discussions
 [here](https://github.com/datajoint/datajoint-python/issues/151) and
 [here](https://github.com/LorenFrankLab/spyglass/issues/469).
 
-**Note:** Deleting entries upstream of Merge Tables will throw errors related to
-deleting a part entry before the master. To circumvent this, you can add
-`force_parts=True` to the
-[`delete` function](https://datajoint.com/docs/core/datajoint-python/0.14/api/datajoint/__init__/#datajoint.table.Table.delete)
-call, but this will leave and orphaned primary key in the master. Instead, use
-`(YourTable & restriction).delete_downstream_merge()` to delete master/part
-pairs. If errors persist, identify and import the offending part table and rerun
-`delete_downstream_merge` with `reload_cache=True`. This process will be faster
-for subsequent calls if you reassign the your table after importing.
-
-```python
-from spyglass.common import Nwbfile
-
-nwbfile = Nwbfile()
-(nwbfile & "nwb_file_name LIKE 'Name%'").delete_downstream_merge()
-```
-
 ## What
 
 A Merge Table is fundamentally a master table with one part for each divergent
 pipeline. By convention...
 
 1. The master table has one primary key, `merge_id`, a
     [UUID](https://en.wikipedia.org/wiki/Universally_unique_identifier), and
```

### Comparing `spyglass_neuro-0.5.1/docs/src/misc/session_groups.md` & `spyglass_neuro-0.5.2/docs/src/misc/session_groups.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/docs/src/stylesheets/extra.css` & `spyglass_neuro-0.5.2/docs/src/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/examples/cli_examples/insert_sort_interval.py` & `spyglass_neuro-0.5.2/examples/cli_examples/insert_sort_interval.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/examples/cli_examples/readme.md` & `spyglass_neuro-0.5.2/examples/cli_examples/readme.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/examples/config_yaml/entries.yaml` & `spyglass_neuro-0.5.2/examples/config_yaml/entries.yaml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml` & `spyglass_neuro-0.5.2/examples/config_yaml/sub-AppleBottom_ses-AppleBottom-DY20-g3_behavior+ecephys_spyglass_config.yaml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/franklab_scripts/alter_tables.py` & `spyglass_neuro-0.5.2/franklab_scripts/alter_tables.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/franklab_scripts/nightly_cleanup.py` & `spyglass_neuro-0.5.2/franklab_scripts/nightly_cleanup.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/franklab_scripts/sort.py` & `spyglass_neuro-0.5.2/franklab_scripts/sort.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/00_Setup.ipynb` & `spyglass_neuro-0.5.2/notebooks/00_Setup.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/01_Insert_Data.ipynb` & `spyglass_neuro-0.5.2/notebooks/01_Insert_Data.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/02_Data_Sync.ipynb` & `spyglass_neuro-0.5.2/notebooks/02_Data_Sync.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/03_Merge_Tables.ipynb` & `spyglass_neuro-0.5.2/notebooks/03_Merge_Tables.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991567460317461%*

 * *Differences: {"'cells'": "{19: {'execution_count': None, 'source': {insert: [(0, 'uuid_key = (LFPOutput & "*

 * *            "nwb_file_dict).fetch(limit=1, as_dict=True)[-1]\\n')], delete: [0]}}, 20: {'source': "*

 * *            '{insert: [(0, \'result1 = restrict.fetch_nwb(restrict.fetch1("KEY"))\\n\')], delete: '*

 * *            "[0]}}, 22: {'source': {insert: [(0, 'result2 = LFPOutput().fetch_nwb(nwb_key)\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -411,15 +411,15 @@
             "source": [
                 "UUIDs help retain unique entries across all part tables. We can fetch NWB file\n",
                 "by referencing this or other features.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -499,15 +499,15 @@
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "uuid_key = LFPOutput.fetch(limit=1, as_dict=True)[-1]\n",
+                "uuid_key = (LFPOutput & nwb_file_dict).fetch(limit=1, as_dict=True)[-1]\n",
                 "restrict = LFPOutput & uuid_key\n",
                 "restrict"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
@@ -542,15 +542,15 @@
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "result1 = restrict.fetch_nwb()\n",
+                "result1 = restrict.fetch_nwb(restrict.fetch1(\"KEY\"))\n",
                 "result1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
@@ -590,15 +590,15 @@
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "result2 = (LFPOutput & nwb_key).fetch_nwb()\n",
+                "result2 = LFPOutput().fetch_nwb(nwb_key)\n",
                 "result2 == result1"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `spyglass_neuro-0.5.1/notebooks/04_PopulateConfigFile.ipynb` & `spyglass_neuro-0.5.2/notebooks/04_PopulateConfigFile.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/10_Spike_SortingV0.ipynb` & `spyglass_neuro-0.5.2/notebooks/10_Spike_SortingV1.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7662689647707015%*

 * *Differences: {"'cells'": "{0: {'source': ['# Spike Sorting: pipeline version 1'], 'id': '0cb86657'}, 1: "*

 * *            "{'source': {insert: [(0, 'This is a tutorial for Spyglass spike sorting pipeline "*

 * *            'version 1 (V1). This pipeline coexists with [version 0](./10_Spike_SortingV0.ipynb) '*

 * *            "but differs in that:\\n'), (1, '- it stores more of the intermediate results (e.g. "*

 * *            "filtered and referenced recording) in the NWB format\\n'), (2, '- it has more "*

 * *            "streamlined curation […]*

```diff
@@ -1,122 +1,118 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "0cb86657",
             "metadata": {},
             "source": [
-                "# Spike Sorting\n"
+                "# Spike Sorting: pipeline version 1"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "5fce5c22-caab-473b-a103-5009a2798d12",
             "metadata": {},
             "source": [
-                "## Overview\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "_Developer Note:_ if you may make a PR in the future, be sure to copy this\n",
-                "notebook, and use the `gitignore` prefix `temp` to avoid future conflicts.\n",
-                "\n",
-                "This is one notebook in a multi-part series on Spyglass.\n",
+                "This is a tutorial for Spyglass spike sorting pipeline version 1 (V1). This pipeline coexists with [version 0](./10_Spike_SortingV0.ipynb) but differs in that:\n",
+                "- it stores more of the intermediate results (e.g. filtered and referenced recording) in the NWB format\n",
+                "- it has more streamlined curation pipelines\n",
+                "- it uses UUIDs as the primary key for important tables (e.g. `SpikeSorting`) to reduce the number of keys that make up the composite primary key\n",
                 "\n",
-                "- To set up your Spyglass environment and database, see\n",
-                "  [the Setup notebook](./00_Setup.ipynb)\n",
-                "- For additional info on DataJoint syntax, including table definitions and\n",
-                "  inserts, see\n",
-                "  [the Insert Data notebook](./01_Insert_Data.ipynb)\n"
+                "The output of both versions of the pipeline are saved in a [merge table](./03_Merge_Tables.ipynb) called `SpikeSortingOutput`. "
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "71c80e78",
             "metadata": {},
             "source": [
-                "### [Extract the recording](#section1)<br>\n",
-                "\n",
-                "1. Specifying your [NWB](#Specifying-your-NWB-filename) file.<br>\n",
-                "2. Specifying which electrodes involved in the recording to sort data from. - [`SortGroup`](#SortGroup)<br>\n",
-                "3. Specifying the time segment of the recording we want to sort. - [`IntervalList`](#IntervalList), [`SortInterval`](#SortInterval)<br>\n",
-                "4. Specifying the parameters to use for filtering the recording. - [`SpikeSortingPreprocessingParameters`](#SpikeSortingPreprocessingParameters)<br>\n",
-                "5. Combining these parameters. - [`SpikeSortingRecordingSelection`](#SpikeSortingRecordingSelection)<br>\n",
-                "6. Extracting the recording. - [`SpikeSortingRecording`](#SpikeSortingRecording)<br>\n",
-                "7. Specifying the parameters to apply for artifact detection/removal. -[`ArtifactDetectionParameters`](#ArtifactDetectionParameters)<br>\n",
-                "\n",
-                "### [Spike sorting the recording](#section2)<br>\n",
-                "\n",
-                "1. Specify the spike sorter and parameters to use. - [`SpikeSorterParameters`](#SpikeSorterParameters)<br>\n",
-                "2. Combine these parameters. - [`SpikeSortingSelection`](#SpikeSortingSelection)<br>\n",
-                "3. Spike sort the extracted recording according to chose parameter set. - [`SpikeSorting`](#SpikeSorting)<br>\n",
-                "\n",
-                "<a href='#section1'></a>\n",
-                "<a href='#section2'></a>\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Imports\n",
-                "\n",
-                "Let's start by importing tables from Spyglass and quieting warnings caused by\n",
-                "some dependencies.\n",
-                "\n",
-                "_Note:_ It the imports below throw a `FileNotFoundError`, make a cell with `!env | grep X` where X is part of the problematic directory. This will show the variable causing issues. Make another cell that sets this variable elsewhere with `%env VAR=\"/your/path/\"`\n"
+                "To start, connect to the database. See instructions in [Setup](./00_Setup.ipynb)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 1,
+            "id": "5778bf96-740c-4e4b-a695-ed4385fc9b58",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import datajoint as dj\n",
                 "import numpy as np\n",
                 "\n",
                 "# change to the upper level folder to detect dj_local_conf.json\n",
                 "if os.path.basename(os.getcwd()) == \"notebooks\":\n",
                 "    os.chdir(\"..\")\n",
-                "dj.config.load(\"dj_local_conf.json\")  # load config for database connection info\n",
-                "\n",
-                "import spyglass.common as sgc\n",
-                "import spyglass.spikesorting.v0 as sgs\n",
-                "\n",
-                "# ignore datajoint+jupyter async warnings\n",
-                "import warnings\n",
-                "\n",
-                "warnings.simplefilter(\"ignore\", category=DeprecationWarning)\n",
-                "warnings.simplefilter(\"ignore\", category=ResourceWarning)"
+                "dj.config[\"enable_python_native_blobs\"] = True\n",
+                "dj.config.load(\"dj_local_conf.json\")  # load config for database connection info"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "344e01b4",
             "metadata": {},
             "source": [
-                "## Fetch Exercise\n"
+                "## Insert Data and populate pre-requisite tables"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "84e7c0b5-f660-4304-9b87-08f5bbf4dbac",
             "metadata": {},
             "source": [
-                "If you haven't already done so, add yourself to `LabTeam`\n"
+                "First, import the pipeline and other necessary modules."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
+            "id": "16345184-c012-486c-b0b6-c914168f2449",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[2024-04-19 10:57:17,965][INFO]: Connecting sambray@lmf-db.cin.ucsf.edu:3306\n",
+                        "[2024-04-19 10:57:17,985][INFO]: Connected sambray@lmf-db.cin.ucsf.edu:3306\n"
+                    ]
+                }
+            ],
+            "source": [
+                "import spyglass.common as sgc\n",
+                "import spyglass.spikesorting.v1 as sgs\n",
+                "import spyglass.data_import as sgi"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "48d2c06a-feb6-438c-94b3-4028127e2101",
+            "metadata": {},
+            "source": [
+                "We will be using `minirec20230622.nwb` as our example. As usual, first insert the NWB file into `Session` (can skip if you have already done so)."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "id": "a3a0ecdf-8dad-41d5-9ee2-fa60f80c746d",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/sambray/Documents/spyglass/src/spyglass/data_import/insert_sessions.py:58: UserWarning: Cannot insert data from minirec20230622.nwb: minirec20230622_.nwb is already in Nwbfile table.\n",
+                        "  warnings.warn(\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
                             "    <style type=\"text/css\">\n",
                             "        .Table{\n",
                             "            border-collapse:collapse;\n",
@@ -163,223 +159,198 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b>Information about lab member in the context of Frank lab network</b>\n",
+                            "    <b>Table for holding experimental sessions.</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">lab_member_name</p>\n",
+                            "                            <p id=\"primary\">nwb_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">subject_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">google_user_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">For permission to curate</span>\n",
+                            "                            <p id=\"nonprimary\">institution_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">datajoint_user_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">For permission to delete</span>\n",
+                            "                            <p id=\"nonprimary\">lab_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">session_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">session_description</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">session_start_time</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">admin</p>\n",
-                            "                            <span class=\"djtooltiptext\">Ignore permission checks</span>\n",
+                            "                            <p id=\"nonprimary\">timestamps_reference_time</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">experiment_description</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>Firstname Lastname</td>\n",
-                            "<td>example@gmail.com</td>\n",
-                            "<td>user</td>\n",
-                            "<td>0</td> </tr> </tbody>\n",
+                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
+                            "<td>54321</td>\n",
+                            "<td>UCSF</td>\n",
+                            "<td>Loren Frank Lab</td>\n",
+                            "<td>12345</td>\n",
+                            "<td>test yaml insertion</td>\n",
+                            "<td>2023-06-22 15:59:58</td>\n",
+                            "<td>1970-01-01 00:00:00</td>\n",
+                            "<td>Test Conversion</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
                             "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*lab_member_na google_user_na datajoint_user admin    \n",
-                            "+------------+ +------------+ +------------+ +-------+\n",
-                            "Firstname Last example@gmail. user           0        \n",
+                            "*nwb_file_name subject_id     institution_na lab_name       session_id     session_descri session_start_ timestamps_ref experiment_des\n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "minirec2023062 54321          UCSF           Loren Frank La 12345          test yaml inse 2023-06-22 15: 1970-01-01 00: Test Conversio\n",
                             " (Total: 1)"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# Full name, Google email address, DataJoint username, admin\n",
-                "name, email, dj_user, admin = (\n",
-                "    \"Firstname Lastname\",\n",
-                "    \"example@gmail.com\",\n",
-                "    \"user\",\n",
-                "    0,\n",
-                ")\n",
-                "sgc.LabMember.insert_from_name(name)\n",
-                "sgc.LabMember.LabMemberInfo.insert1(\n",
-                "    [\n",
-                "        name,\n",
-                "        email,\n",
-                "        dj_user,\n",
-                "        admin,\n",
-                "    ],\n",
-                "    skip_duplicates=True,\n",
-                ")\n",
-                "sgc.LabMember.LabMemberInfo()"
+                "nwb_file_name = \"minirec20230622.nwb\"\n",
+                "nwb_file_name2 = \"minirec20230622_.nwb\"\n",
+                "sgi.insert_sessions(nwb_file_name)\n",
+                "sgc.Session() & {\"nwb_file_name\": nwb_file_name2}"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "49ea5ac0",
             "metadata": {},
             "source": [
-                "We can try `fetch` to confirm.\n",
-                "\n",
-                "_Exercise:_ Try to write a fer lines to generate a dictionary with team names as\n",
-                "keys and lists of members as values. It may be helpful to add more data with the\n",
-                "code above and use `fetch(as_dict=True)`.\n"
+                "All spikesorting results are linked to a team name from the `LabTeam` table. If you haven't already inserted a team for your project do so here. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
+            "id": "8d659323",
             "metadata": {},
             "outputs": [],
             "source": [
-                "my_team_members = (\n",
-                "    (sgc.LabTeam.LabTeamMember & {\"team_name\": \"My Team\"})\n",
-                "    .fetch(\"lab_member_name\")\n",
-                "    .tolist()\n",
-                ")\n",
-                "if name in my_team_members:\n",
-                "    print(\"You made it in!\")"
+                "# Make a lab team if doesn't already exist, otherwise insert yourself into team\n",
+                "team_name = \"My Team\"\n",
+                "if not sgc.LabTeam() & {\"team_name\": team_name}:\n",
+                "    sgc.LabTeam().create_new_team(\n",
+                "        team_name=team_name,  # Should be unique\n",
+                "        team_members=[],\n",
+                "        team_description=\"test\",  # Optional\n",
+                "    )"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "4e390a71",
             "metadata": {},
             "source": [
-                "<details>\n",
-                "<summary>Code hidden here</summary>\n",
-                "\n",
-                "```python\n",
-                "members = sgc.LabTeam.LabTeamMember.fetch(as_dict=True)\n",
-                "teams_dict = {member[\"team_name\"]: [] for member in members}\n",
-                "for member in members:\n",
-                "    teams_dict[member[\"team_name\"]].append(member[\"lab_member_name\"])\n",
-                "print(teams_dict)\n",
-                "```\n",
-                "</details>"
+                "## Define sort groups and extract recordings"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "5f3dfe2d-4645-44f9-b169-479292215afe",
             "metadata": {},
             "source": [
-                "## Adding an NWB file\n"
+                "Each NWB file will have multiple electrodes we can use for spike sorting. We\n",
+                "commonly use multiple electrodes in a `SortGroup` selected by what tetrode or\n",
+                "shank of a probe they were on. Electrodes in the same sort group will then be\n",
+                "sorted together."
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "a269f6af-eb16-4551-b511-a264368c9490",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Import Data\n"
+                "sgs.SortGroup.set_group_by_shank(nwb_file_name=nwb_file_name2)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "1c55792e-f9ba-4e0d-a4d2-8c60bf0e8f34",
             "metadata": {},
             "source": [
-                "If you haven't already, load an NWB file. For more details on downloading and\n",
-                "importing data, see [this notebook](./01_Insert_Data.ipynb).\n"
+                "The next step is to filter and reference the recording so that we isolate the spike band data. This is done by combining the data with the parameters in `SpikeSortingRecordingSelection`. For inserting into this table, use `insert_selection` method. This automatically generates a UUID for a recording.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 6,
+            "id": "5b307631-3cc5-4859-9e95-aeedf6a3de56",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": []
+                    "data": {
+                        "text/plain": [
+                            "{'nwb_file_name': 'minirec20230622_.nwb',\n",
+                            " 'sort_group_id': 0,\n",
+                            " 'preproc_param_name': 'default',\n",
+                            " 'interval_list_name': '01_s1',\n",
+                            " 'team_name': 'My Team',\n",
+                            " 'recording_id': UUID('3450db49-28d5-4942-aa37-7c19126d16db')}"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "import spyglass.data_import as sdi\n",
-                "\n",
-                "sdi.insert_sessions(\"minirec20230622.nwb\")\n",
-                "nwb_file_name = \"minirec20230622_.nwb\""
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Extracting the recording\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "#### `SortGroup`\n"
+                "# define and insert a key for each sort group and interval you want to sort\n",
+                "key = {\n",
+                "    \"nwb_file_name\": nwb_file_name2,\n",
+                "    \"sort_group_id\": 0,\n",
+                "    \"preproc_param_name\": \"default\",\n",
+                "    \"interval_list_name\": \"01_s1\",\n",
+                "    \"team_name\": \"My Team\",\n",
+                "}\n",
+                "sgs.SpikeSortingRecordingSelection.insert_selection(key)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "01948666",
             "metadata": {},
             "source": [
-                "Each NWB file will have multiple electrodes we can use for spike sorting. We\n",
-                "commonly use multiple electrodes in a `SortGroup` selected by what tetrode or\n",
-                "shank of a probe they were on.\n",
-                "\n",
-                "_Note:_ This will delete any existing entries. Answer 'yes' when prompted.\n"
+                "Next we will call `populate` method of `SpikeSortingRecording`. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 7,
+            "id": "3840f86a-8769-423e-8aeb-4d9ab694f1ef",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[2023-07-21 13:56:24,232][INFO]: Deleting 128 rows from `spikesorting_recording`.`sort_group__sort_group_electrode`\n",
-                        "[2023-07-21 13:56:24,234][INFO]: Deleting 4 rows from `spikesorting_recording`.`sort_group`\n"
+                        "[10:57:43][INFO] Spyglass: Writing new NWB file minirec20230622_PTCFX77XOI.nwb\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/build/objectmapper.py:668: MissingRequiredBuildWarning: NWBFile 'root' is missing required value for attribute 'source_script_file_name'.\n",
+                        "  warnings.warn(msg, MissingRequiredBuildWarning)\n"
                     ]
                 },
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2023-07-21 13:56:27,358][INFO]: Deletes committed.\n"
-                    ]
-                }
-            ],
-            "source": [
-                "sgs.SortGroup().set_group_by_shank(nwb_file_name)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Each electrode has an `electrode_id` and is associated with an\n",
-                "`electrode_group_name`, which corresponds with a `sort_group_id`.\n",
-                "\n",
-                "For example, data recorded from a 32 tetrode (128 channel) drive results in 128\n",
-                "unique `electrode_id`. This could result in 32 unique `electrode_group_name` and\n",
-                "32 unique `sort_group_id`.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 18,
-            "metadata": {},
-            "outputs": [
-                {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
                             "    <style type=\"text/css\">\n",
                             "        .Table{\n",
                             "            border-collapse:collapse;\n",
@@ -426,118 +397,133 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b></b>\n",
+                            "    <b>Processed recording.</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_group_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">identifier for a group of electrodes</span>\n",
+                            "                            <p id=\"primary\">recording_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">electrode_group_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">electrode group name from NWBFile</span>\n",
+                            "                            <p id=\"nonprimary\">analysis_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the file</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">electrode_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">the unique number for this electrode</span>\n",
+                            "                            <p id=\"nonprimary\">object_id</p>\n",
+                            "                            <span class=\"djtooltiptext\">Object ID for the processed recording in NWB file</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>1</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>2</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>3</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>4</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>5</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>6</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>7</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>8</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>9</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>10</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>11</td> </tr> </tbody>\n",
+                            "            <tbody> <tr> <td>3450db49-28d5-4942-aa37-7c19126d16db</td>\n",
+                            "<td>minirec20230622_PTCFX77XOI.nwb</td>\n",
+                            "<td>15592178-c317-4112-bfa6-b0943542e507</td> </tr> </tbody>\n",
                             "        </table>\n",
-                            "        <p>...</p>\n",
-                            "        <p>Total: 128</p></div>\n",
+                            "        \n",
+                            "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*nwb_file_name *sort_group_id *electrode_gro *electrode_id \n",
-                            "+------------+ +------------+ +------------+ +------------+\n",
-                            "minirec2023062 0              0              0             \n",
-                            "minirec2023062 0              0              1             \n",
-                            "minirec2023062 0              0              2             \n",
-                            "minirec2023062 0              0              3             \n",
-                            "minirec2023062 0              0              4             \n",
-                            "minirec2023062 0              0              5             \n",
-                            "minirec2023062 0              0              6             \n",
-                            "minirec2023062 0              0              7             \n",
-                            "minirec2023062 0              0              8             \n",
-                            "minirec2023062 0              0              9             \n",
-                            "minirec2023062 0              0              10            \n",
-                            "minirec2023062 0              0              11            \n",
-                            "   ...\n",
-                            " (Total: 128)"
+                            "*recording_id  analysis_file_ object_id     \n",
+                            "+------------+ +------------+ +------------+\n",
+                            "3450db49-28d5- minirec2023062 15592178-c317-\n",
+                            " (Total: 1)"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.SortGroup.SortGroupElectrode & {\"nwb_file_name\": nwb_file_name}"
+                "# Assuming 'key' is a dictionary with fields that you want to include in 'ssr_key'\n",
+                "ssr_key = {\n",
+                "    \"recording_id\": (sgs.SpikeSortingRecordingSelection() & key).fetch1(\n",
+                "        \"recording_id\"\n",
+                "    ),\n",
+                "} | key\n",
+                "\n",
+                "ssr_pk = (sgs.SpikeSortingRecordingSelection & key).proj()\n",
+                "sgs.SpikeSortingRecording.populate(ssr_pk)\n",
+                "sgs.SpikeSortingRecording() & ssr_key"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "1c6c7ea3-9538-4fa9-890b-ee16cc18af31",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "key = (sgs.SpikeSortingRecordingSelection & key).fetch1()"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "tags": []
-            },
+            "id": "348334fa",
+            "metadata": {},
             "source": [
-                "#### `IntervalList`\n",
-                "\n",
-                "Next, we make a decision about the time interval for our spike sorting using\n",
-                "`IntervalList`.\n"
+                "## Artifact Detection"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "1955ed06-d754-470a-b5b3-94df6c3e03eb",
+            "metadata": {},
+            "source": [
+                "Sometimes the recording may contain artifacts that can confound spike sorting. For example, we often have artifacts when the animal licks the reward well for milk during behavior. These appear as sharp transients across all channels, and sometimes they are not adequately removed by filtering and referencing. We will identify the periods during which this type of artifact appears and set them to zero so that they won't interfere with spike sorting. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
-            "metadata": {
-                "tags": []
-            },
+            "execution_count": 9,
+            "id": "74415172-f2da-4fd3-ab43-01857d682b0d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[10:57:52][INFO] Spyglass: Using 4 jobs...\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "461383a7fb194d79b603244c4e371a98",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "detect_artifact_frames:   0%|          | 0/2 [00:00<?, ?it/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[10:57:53][WARNING] Spyglass: No artifacts detected.\n"
+                    ]
+                }
+            ],
+            "source": [
+                "sgs.ArtifactDetectionSelection.insert_selection(\n",
+                "    {\"recording_id\": key[\"recording_id\"], \"artifact_param_name\": \"default\"}\n",
+                ")\n",
+                "sgs.ArtifactDetection.populate()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "ca9a9f64-0afc-4c83-b22c-0ed120cb87f6",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
                             "    <style type=\"text/css\">\n",
@@ -586,199 +572,126 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b>Time intervals used for analysis</b>\n",
+                            "    <b>Detected artifacts (e.g. large transients from movement).</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">interval_list_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">valid_times</p>\n",
-                            "                            <span class=\"djtooltiptext\">numpy array with start and end times for each interval</span>\n",
+                            "                            <p id=\"primary\">artifact_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
-                            "<td>01_s1</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>02_s2</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>pos 0 valid times</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>pos 1 valid times</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>pos 2 valid times</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>pos 3 valid times</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>minirec20230622_.nwb</td>\n",
-                            "<td>raw data valid times</td>\n",
-                            "<td>=BLOB=</td> </tr> </tbody>\n",
+                            "            <tbody> <tr> <td>0058dab4-41c1-42b1-91f4-5773f2ad36cc</td></tr><tr><td>01b39d37-3ff8-4907-9da6-9fec9baf87b5</td></tr><tr><td>035f0bae-80b3-4ce9-a767-94d336f36283</td></tr><tr><td>038ee778-6cf1-4e99-ab80-e354db5170c9</td></tr><tr><td>03e9768d-d101-4f56-abf9-5b0e3e1803b7</td></tr><tr><td>0490c820-c381-43b6-857e-f463147723ff</td></tr><tr><td>04a289c6-9e19-486a-a4cb-7e9638af225a</td></tr><tr><td>06dd7922-7042-4023-bebf-da1dacb0b6c7</td></tr><tr><td>07036486-e9f5-4dba-8662-7fb5ff2a6711</td></tr><tr><td>070ed448-a52d-478e-9102-0d04a6ed0b96</td></tr><tr><td>07a65788-bb89-48f3-90ea-4ab1add06eae</td></tr><tr><td>0a6611b3-c593-4900-a715-66bb1396940e</td> </tr> </tbody>\n",
                             "        </table>\n",
-                            "        \n",
-                            "        <p>Total: 7</p></div>\n",
+                            "        <p>...</p>\n",
+                            "        <p>Total: 151</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*nwb_file_name *interval_list valid_time\n",
-                            "+------------+ +------------+ +--------+\n",
-                            "minirec2023062 01_s1          =BLOB=    \n",
-                            "minirec2023062 02_s2          =BLOB=    \n",
-                            "minirec2023062 pos 0 valid ti =BLOB=    \n",
-                            "minirec2023062 pos 1 valid ti =BLOB=    \n",
-                            "minirec2023062 pos 2 valid ti =BLOB=    \n",
-                            "minirec2023062 pos 3 valid ti =BLOB=    \n",
-                            "minirec2023062 raw data valid =BLOB=    \n",
-                            " (Total: 7)"
+                            "*artifact_id  \n",
+                            "+------------+\n",
+                            "0058dab4-41c1-\n",
+                            "01b39d37-3ff8-\n",
+                            "035f0bae-80b3-\n",
+                            "038ee778-6cf1-\n",
+                            "03e9768d-d101-\n",
+                            "0490c820-c381-\n",
+                            "04a289c6-9e19-\n",
+                            "06dd7922-7042-\n",
+                            "07036486-e9f5-\n",
+                            "070ed448-a52d-\n",
+                            "07a65788-bb89-\n",
+                            "0a6611b3-c593-\n",
+                            "   ...\n",
+                            " (Total: 151)"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgc.IntervalList & {\"nwb_file_name\": nwb_file_name}"
+                "sgs.ArtifactDetection()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "da2ac6b4",
             "metadata": {},
             "source": [
-                "Let's start with the first run interval (`01_s1`) and fetch corresponding `valid_times`. For the `minirec` example, this is relatively short.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 20,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "This interval list is 10 seconds long\n"
-                    ]
-                }
-            ],
-            "source": [
-                "interval_list_name = \"01_s1\"\n",
-                "interval_list = (\n",
-                "    sgc.IntervalList\n",
-                "    & {\"nwb_file_name\": nwb_file_name, \"interval_list_name\": interval_list_name}\n",
-                ").fetch1(\"valid_times\")[0]\n",
-                "\n",
-                "\n",
-                "def print_interval_duration(interval_list: np.ndarray):\n",
-                "    duration = np.round((interval_list[1] - interval_list[0]))\n",
-                "    print(f\"This interval list is {duration:g} seconds long\")\n",
-                "\n",
-                "\n",
-                "print_interval_duration(interval_list)"
+                "The output of `ArtifactDetection` is actually stored in `IntervalList` because it is another type of interval. The UUID however can be found in both. "
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "0ee9ca19",
             "metadata": {},
             "source": [
-                "#### `SortInterval`\n",
-                "\n",
-                "For longer recordings, Spyglass subsets this interval with `SortInterval`.\n",
-                "Below, we select the first `n` seconds of this interval.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 21,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "n = 9\n",
-                "sort_interval_name = interval_list_name + f\"_first{n}\"\n",
-                "sort_interval = np.array([interval_list[0], interval_list[0] + n])"
+                "## Run Spike Sorting"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "65ae0f70-2d8d-40d4-86c9-2ab206b28ca9",
             "metadata": {},
             "source": [
-                "With the above, we can insert into `SortInterval`\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 22,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "sgs.SortInterval.insert1(\n",
-                "    {\n",
-                "        \"nwb_file_name\": nwb_file_name,\n",
-                "        \"sort_interval_name\": sort_interval_name,\n",
-                "        \"sort_interval\": sort_interval,\n",
-                "    },\n",
-                "    skip_duplicates=True,\n",
-                ")"
+                "Now that we have prepared the recording, we will pair this with a spike sorting algorithm and associated parameters. This will be inserted to `SpikeSortingSelection`, again via `insert_selection` method. "
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "50fdadbb",
             "metadata": {},
             "source": [
-                "And verify the entry\n"
+                "The spike sorting pipeline is powered by `spikeinterface`, a community-developed Python package that enables one to easily apply multiple spike sorters to a single recording. Some spike sorters have special requirements, such as GPU. Others need to be installed separately from spyglass. In the Frank lab, we have been using `mountainsort4`, though the pipeline have been tested with `mountainsort5`, `kilosort2_5`, `kilosort3`, and `ironclust` as well.\n",
+                "\n",
+                "When using `mountainsort5`, make sure to run `pip install mountainsort5`. `kilosort2_5`, `kilosort3`, and `ironclust` are MATLAB-based, but we can run these without having to install MATLAB thanks to `spikeinterface`. It does require downloading additional files (as singularity containers) so make sure to do `pip install spython`. These sorters also require GPU access, so also do ` pip install cuda-python` (and make sure your computer does have a GPU). "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "This interval list is 9 seconds long\n"
-                    ]
-                }
-            ],
-            "source": [
-                "print_interval_duration(\n",
-                "    (\n",
-                "        sgs.SortInterval\n",
-                "        & {\n",
-                "            \"nwb_file_name\": nwb_file_name,\n",
-                "            \"sort_interval_name\": sort_interval_name,\n",
-                "        }\n",
-                "    ).fetch1(\"sort_interval\")\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Preprocessing Parameters\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
+            "execution_count": 11,
+            "id": "34246883-9dc4-43c5-a438-009215a3a35e",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "`SpikeSortingPreprocessingParameters` contains the parameters used to filter the\n",
-                "recorded data in the spike band prior to sorting.\n"
+                "sorter = \"mountainsort4\"\n",
+                "\n",
+                "common_key = {\n",
+                "    \"recording_id\": key[\"recording_id\"],\n",
+                "    \"sorter\": sorter,\n",
+                "    \"nwb_file_name\": nwb_file_name2,\n",
+                "    \"interval_list_name\": str(\n",
+                "        (\n",
+                "            sgs.ArtifactDetectionSelection\n",
+                "            & {\"recording_id\": key[\"recording_id\"]}\n",
+                "        ).fetch1(\"artifact_id\")\n",
+                "    ),\n",
+                "}\n",
+                "\n",
+                "if sorter == \"mountainsort4\":\n",
+                "    key = {\n",
+                "        **common_key,\n",
+                "        \"sorter_param_name\": \"franklab_tetrode_hippocampus_30KHz\",\n",
+                "    }\n",
+                "else:\n",
+                "    key = {\n",
+                "        **common_key,\n",
+                "        \"sorter_param_name\": \"default\",\n",
+                "    }"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 12,
+            "id": "68856fb6-b5c2-4ee4-b300-43a117e453a1",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -828,160 +741,215 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b></b>\n",
+                            "    <b>Processed recording and spike sorting parameters. Use `insert_selection` method to insert rows.</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">preproc_params_name</p>\n",
+                            "                            <p id=\"primary\">sorting_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">preproc_params</p>\n",
+                            "                            <p id=\"nonprimary\">recording_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">sorter</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">sorter_param_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">nwb_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">interval_list_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>default</td>\n",
-                            "<td>=BLOB=</td> </tr> </tbody>\n",
+                            "            <tbody> <tr> <td>16cbb873-052f-44f3-9f4d-89af3544915e</td>\n",
+                            "<td>3450db49-28d5-4942-aa37-7c19126d16db</td>\n",
+                            "<td>mountainsort4</td>\n",
+                            "<td>franklab_tetrode_hippocampus_30KHz</td>\n",
+                            "<td>minirec20230622_.nwb</td>\n",
+                            "<td>f03513af-bff8-4732-a6ab-e53f0550e7b0</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
                             "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*preproc_param preproc_pa\n",
-                            "+------------+ +--------+\n",
-                            "default        =BLOB=    \n",
+                            "*sorting_id    recording_id   sorter         sorter_param_n nwb_file_name  interval_list_\n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "16cbb873-052f- 3450db49-28d5- mountainsort4  franklab_tetro minirec2023062 f03513af-bff8-\n",
                             " (Total: 1)"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.SpikeSortingPreprocessingParameters()"
+                "sgs.SpikeSortingSelection.insert_selection(key)\n",
+                "sgs.SpikeSortingSelection() & key"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "bb343fb7-04d6-48fc-bf67-9919769a7a52",
             "metadata": {},
             "source": [
-                "Here, we insert the default parameters and then fetch them.\n"
+                "Once `SpikeSortingSelection` is populated, let's run `SpikeSorting.populate`. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 13,
+            "id": "54ccf059-b1ae-42e8-aede-4af30a61fd2b",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'frequency_min': 300, 'frequency_max': 6000, 'margin_ms': 5, 'seed': 0}\n"
+                        "Mountainsort4 use the OLD spikeextractors mapped with NewToOldRecording\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[10:58:17][INFO] Spyglass: Writing new NWB file minirec20230622_PP6Y10VW0V.nwb\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/build/objectmapper.py:668: MissingRequiredBuildWarning: NWBFile 'root' is missing required value for attribute 'source_script_file_name'.\n",
+                        "  warnings.warn(msg, MissingRequiredBuildWarning)\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/datajoint/hash.py:39: ResourceWarning: unclosed file <_io.BufferedReader name='/stelmo/nwb/analysis/minirec20230622/minirec20230622_PP6Y10VW0V.nwb'>\n",
+                        "  return uuid_from_stream(Path(filepath).open(\"rb\"), init_string=init_string)\n",
+                        "ResourceWarning: Enable tracemalloc to get the object allocation traceback\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/datajoint/external.py:276: DeprecationWarning: The truth value of an empty array is ambiguous. Returning False, but in future this will result in an error. Use `array.size > 0` to check that an array is not empty.\n",
+                        "  if check_hash:\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/tempfile.py:821: ResourceWarning: Implicitly cleaning up <TemporaryDirectory '/stelmo/nwb/tmp/tmpa7_uli3g'>\n",
+                        "  _warnings.warn(warn_message, ResourceWarning)\n"
                     ]
                 }
             ],
             "source": [
-                "sgs.SpikeSortingPreprocessingParameters().insert_default()\n",
-                "preproc_params = (\n",
-                "    sgs.SpikeSortingPreprocessingParameters()\n",
-                "    & {\"preproc_params_name\": \"default\"}\n",
-                ").fetch1(\"preproc_params\")\n",
-                "print(preproc_params)"
+                "sss_pk = (sgs.SpikeSortingSelection & key).proj()\n",
+                "\n",
+                "sgs.SpikeSorting.populate(sss_pk)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "f3d1e621",
             "metadata": {},
             "source": [
-                "Let's adjust the `frequency_min` to 600, the preference for hippocampal data,\n",
-                "and insert that into the table as a new set of parameters for hippocampal data.\n"
+                "The spike sorting results (spike times of detected units) are saved in an NWB file. We can access this in two ways. First, we can access it via the `fetch_nwb` method, which allows us to directly access the spike times saved in the `units` table of the NWB file. Second, we can access it as a `spikeinterface.NWBSorting` object. This allows us to take advantage of the rich APIs of `spikeinterface` to further analyze the sorting. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 14,
+            "id": "3d41d3ab",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/datajoint/hash.py:39: ResourceWarning: unclosed file <_io.BufferedReader name='/stelmo/nwb/analysis/minirec20230622/minirec20230622_PP6Y10VW0V.nwb'>\n",
+                        "  return uuid_from_stream(Path(filepath).open(\"rb\"), init_string=init_string)\n",
+                        "ResourceWarning: Enable tracemalloc to get the object allocation traceback\n"
+                    ]
+                }
+            ],
             "source": [
-                "preproc_params[\"frequency_min\"] = 600\n",
-                "sgs.SpikeSortingPreprocessingParameters().insert1(\n",
-                "    {\n",
-                "        \"preproc_params_name\": \"default_hippocampus\",\n",
-                "        \"preproc_params\": preproc_params,\n",
-                "    },\n",
-                "    skip_duplicates=True,\n",
-                ")"
+                "sorting_nwb = (sgs.SpikeSorting & key).fetch_nwb()\n",
+                "sorting_si = sgs.SpikeSorting.get_sorting(key)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "db328eb1",
             "metadata": {},
             "source": [
-                "## Processing a key\n",
-                "\n",
-                "_key_ is often used to describe an entry we want to move through the pipeline,\n",
-                "and keys are often managed as dictionaries. Here, we'll manage the spike sort\n",
-                "recording key, `ssr_key`.\n"
+                "Note that the spike times of `fetch_nwb` is in units of seconds aligned with the timestamps of the recording. The spike times of the `spikeinterface.NWBSorting` object is in units of samples (as is generally true for sorting objects in `spikeinterface`)."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "55d6c183",
+            "metadata": {},
+            "source": [
+                "## Automatic Curation"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "ea8fcaa0-9dd7-4870-9f5b-be039e3579cc",
+            "metadata": {},
+            "source": [
+                "Next step is to curate the results of spike sorting. This is often necessary because spike sorting algorithms are not perfect;\n",
+                "they often return clusters that are clearly not biological in origin, and sometimes oversplit clusters that should have been merged.\n",
+                "We have two main ways of curating spike sorting: by computing quality metrics followed by thresholding, and manually applying curation labels.\n",
+                "To do either, we first insert the spike sorting to `CurationV1` using `insert_curation` method.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 15,
+            "id": "6245eec9-3fba-4071-b58b-eec6d9345532",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[10:58:32][INFO] Spyglass: Writing new NWB file minirec20230622_SYPH1SYT75.nwb\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/build/objectmapper.py:668: MissingRequiredBuildWarning: NWBFile 'root' is missing required value for attribute 'source_script_file_name'.\n",
+                        "  warnings.warn(msg, MissingRequiredBuildWarning)\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/datajoint/hash.py:39: ResourceWarning: unclosed file <_io.BufferedReader name='/stelmo/nwb/analysis/minirec20230622/minirec20230622_SYPH1SYT75.nwb'>\n",
+                        "  return uuid_from_stream(Path(filepath).open(\"rb\"), init_string=init_string)\n",
+                        "ResourceWarning: Enable tracemalloc to get the object allocation traceback\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/datajoint/external.py:276: DeprecationWarning: The truth value of an empty array is ambiguous. Returning False, but in future this will result in an error. Use `array.size > 0` to check that an array is not empty.\n",
+                        "  if check_hash:\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/plain": [
-                            "'01_s1'"
+                            "{'sorting_id': UUID('16cbb873-052f-44f3-9f4d-89af3544915e'),\n",
+                            " 'curation_id': 0,\n",
+                            " 'parent_curation_id': -1,\n",
+                            " 'analysis_file_name': 'minirec20230622_SYPH1SYT75.nwb',\n",
+                            " 'object_id': '3e4f927b-716f-4dd8-9c98-acd132d758fb',\n",
+                            " 'merges_applied': False,\n",
+                            " 'description': 'testing sort'}"
                         ]
                     },
-                    "execution_count": 33,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "interval_list_name"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 34,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ssr_key = dict(\n",
-                "    nwb_file_name=nwb_file_name,\n",
-                "    sort_group_id=0,  # See SortGroup\n",
-                "    sort_interval_name=sort_interval_name,  # First N seconds above\n",
-                "    preproc_params_name=\"default_hippocampus\",  # See preproc_params\n",
-                "    interval_list_name=interval_list_name,\n",
-                "    team_name=\"My Team\",\n",
+                "sgs.SpikeSortingRecording & key\n",
+                "sgs.CurationV1.insert_curation(\n",
+                "    sorting_id=(\n",
+                "        sgs.SpikeSortingSelection & {\"recording_id\": key[\"recording_id\"]}\n",
+                "    ).fetch1(\"sorting_id\"),\n",
+                "    description=\"testing sort\",\n",
                 ")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Recording Selection\n",
-                "\n",
-                "We now insert this key `SpikeSortingRecordingSelection` table to specify what\n",
-                "time/tetrode/etc. of the recording we want to extract.\n"
-            ]
-        },
-        {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 16,
+            "id": "5bec5b97-4e9f-4ee9-a6b5-4f05f4726744",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -1031,122 +999,175 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b>Defines recordings to be sorted</b>\n",
+                            "    <b>Curation of a SpikeSorting. Use `insert_curation` to insert rows.</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
+                            "                            <p id=\"primary\">sorting_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_group_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">identifier for a group of electrodes</span>\n",
+                            "                            <p id=\"primary\">curation_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_interval_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name for this interval</span>\n",
+                            "                            <p id=\"nonprimary\">parent_curation_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">preproc_params_name</p>\n",
+                            "                            <p id=\"nonprimary\">analysis_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">object_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">team_name</p>\n",
+                            "                            <p id=\"nonprimary\">merges_applied</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">interval_list_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
+                            "                            <p id=\"nonprimary\">description</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
+                            "            <tbody> <tr> <td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
                             "<td>0</td>\n",
-                            "<td>01_s1_first9</td>\n",
-                            "<td>default_hippocampus</td>\n",
-                            "<td>My Team</td>\n",
-                            "<td>01_s1</td> </tr> </tbody>\n",
+                            "<td>-1</td>\n",
+                            "<td>BS2820231107_8Z8CLG184Z.nwb</td>\n",
+                            "<td>37ee7365-028f-46e1-8351-1cd402a7b36c</td>\n",
+                            "<td>0</td>\n",
+                            "<td>testing sort</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>1</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_HPIQR9LZWU.nwb</td>\n",
+                            "<td>538032a5-5d29-4cb8-b0a2-7224fee6d8ce</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>2</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_SVW8YK84IP.nwb</td>\n",
+                            "<td>ed440315-7302-4217-be15-087c7efeda7e</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>3</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_7CWR2JR68B.nwb</td>\n",
+                            "<td>0d8be667-2831-4e99-8c9b-54102de48e85</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>4</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_1PCRTB2UZ2.nwb</td>\n",
+                            "<td>9f9e9a1e-9be3-405c-9c66-4bf6dc54d4d9</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>5</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_4NPZ4YTASV.nwb</td>\n",
+                            "<td>89170a28-487a-4787-83dd-18009c446700</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>6</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_MMSIJ8YQ54.nwb</td>\n",
+                            "<td>c9fb8c88-6449-4d9a-a40a-cd10dcdc193f</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>7</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_LZJWQPP1YW.nwb</td>\n",
+                            "<td>f078e3bb-92fc-4e7f-b3a8-32936a90e057</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>8</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_RJ7DLUKOIG.nwb</td>\n",
+                            "<td>c311fbfb-cd3d-4d92-b535-b5da3d4a6ec3</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>9</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_6ZJP5NRCX9.nwb</td>\n",
+                            "<td>a54ee3f8-851a-4dca-bb46-7673e2807462</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>03dc29a5-febe-4a59-ab61-21a25dea3625</td>\n",
+                            "<td>0</td>\n",
+                            "<td>-1</td>\n",
+                            "<td>j1620210710_EOE1VZ4YAX.nwb</td>\n",
+                            "<td>52889e86-c249-4916-9576-a9ccf7f48dbe</td>\n",
+                            "<td>0</td>\n",
+                            "<td></td></tr><tr><td>061ba57b-d2cb-4052-b375-42ba13684e41</td>\n",
+                            "<td>0</td>\n",
+                            "<td>-1</td>\n",
+                            "<td>BS2820231107_S21IIVRCZA.nwb</td>\n",
+                            "<td>5d71500d-1065-4610-b3a6-746821d0f438</td>\n",
+                            "<td>0</td>\n",
+                            "<td>testing sort</td> </tr> </tbody>\n",
                             "        </table>\n",
-                            "        \n",
-                            "        <p>Total: 1</p></div>\n",
+                            "        <p>...</p>\n",
+                            "        <p>Total: 626</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*nwb_file_name *sort_group_id *sort_interval *preproc_param *team_name    interval_list_\n",
-                            "+------------+ +------------+ +------------+ +------------+ +-----------+ +------------+\n",
-                            "minirec2023062 0              01_s1_first9   default_hippoc My Team       01_s1         \n",
-                            " (Total: 1)"
+                            "*sorting_id    *curation_id   parent_curatio analysis_file_ object_id      merges_applied description   \n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "021fb85a-992f- 0              -1             BS2820231107_8 37ee7365-028f- 0              testing sort  \n",
+                            "021fb85a-992f- 1              0              BS2820231107_H 538032a5-5d29- 0              after metric c\n",
+                            "021fb85a-992f- 2              0              BS2820231107_S ed440315-7302- 0              after metric c\n",
+                            "021fb85a-992f- 3              0              BS2820231107_7 0d8be667-2831- 0              after metric c\n",
+                            "021fb85a-992f- 4              0              BS2820231107_1 9f9e9a1e-9be3- 0              after metric c\n",
+                            "021fb85a-992f- 5              0              BS2820231107_4 89170a28-487a- 0              after metric c\n",
+                            "021fb85a-992f- 6              0              BS2820231107_M c9fb8c88-6449- 0              after metric c\n",
+                            "021fb85a-992f- 7              0              BS2820231107_L f078e3bb-92fc- 0              after metric c\n",
+                            "021fb85a-992f- 8              0              BS2820231107_R c311fbfb-cd3d- 0              after metric c\n",
+                            "021fb85a-992f- 9              0              BS2820231107_6 a54ee3f8-851a- 0              after metric c\n",
+                            "03dc29a5-febe- 0              -1             j1620210710_EO 52889e86-c249- 0                            \n",
+                            "061ba57b-d2cb- 0              -1             BS2820231107_S 5d71500d-1065- 0              testing sort  \n",
+                            "   ...\n",
+                            " (Total: 626)"
                         ]
                     },
-                    "execution_count": 35,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.SpikeSortingRecordingSelection.insert1(ssr_key, skip_duplicates=True)\n",
-                "sgs.SpikeSortingRecordingSelection() & ssr_key"
+                "sgs.CurationV1()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "97317b6f-a40a-4f84-8042-4361064f010a",
             "metadata": {},
             "source": [
-                "### `SpikeSortingRecording`\n",
-                "\n",
-                "And now we're ready to extract the recording! The\n",
-                "[`populate` command](https://datajoint.com/docs/core/datajoint-python/0.14/compute/populate/)\n",
-                "will automatically process data in Computed or Imported\n",
-                "[table tiers](https://datajoint.com/docs/core/datajoint-python/0.14/design/tables/tiers/).\n",
-                "\n",
-                "If we only want to process certain entries, we can grab their primary key with\n",
-                "the [`.proj()` command](https://datajoint.com/docs/core/datajoint-python/0.14/query/project/)\n",
-                "and use a list of primary keys when calling `populate`.\n"
+                "We will first do an automatic curation based on quality metrics. Under the hood, this part again makes use of `spikeinterface`. Some of the quality metrics that we often compute are the nearest neighbor isolation and noise overlap metrics, as well as SNR and ISI violation rate. For computing some of these metrics, the waveforms must be extracted and projected onto a feature space. Thus here we set the parameters for waveform extraction as well as how to curate the units based on these metrics (e.g. if `nn_noise_overlap` is greater than 0.1, mark as `noise`)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "write_binary_recording with n_jobs = 8 and chunk_size = 299593\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "0b6d4bd70bba4a92bdf77c88d07d4b08",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "write_binary_recording:   0%|          | 0/1 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "ssr_pk = (sgs.SpikeSortingRecordingSelection & ssr_key).proj()\n",
-                "sgs.SpikeSortingRecording.populate([ssr_pk])"
-            ]
-        },
-        {
-            "cell_type": "markdown",
+            "execution_count": 17,
+            "id": "7207abda-ea84-43af-97d4-e5be3464d28d",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Now we can see our recording in the table. _E x c i t i n g !_\n"
+                "key = {\n",
+                "    \"sorting_id\": (\n",
+                "        sgs.SpikeSortingSelection & {\"recording_id\": key[\"recording_id\"]}\n",
+                "    ).fetch1(\"sorting_id\"),\n",
+                "    \"curation_id\": 0,\n",
+                "    \"waveform_param_name\": \"default_not_whitened\",\n",
+                "    \"metric_param_name\": \"franklab_default\",\n",
+                "    \"metric_curation_param_name\": \"default\",\n",
+                "}"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 18,
+            "id": "14c2eacc-cc45-4e61-9919-04785a721079",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -1196,104 +1217,68 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b></b>\n",
+                            "    <b>Spike sorting and parameters for metric curation. Use `insert_selection` to insert a row into this table.</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_group_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">identifier for a group of electrodes</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_interval_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name for this interval</span>\n",
+                            "                            <p id=\"primary\">metric_curation_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">preproc_params_name</p>\n",
+                            "                            <p id=\"nonprimary\">sorting_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">team_name</p>\n",
+                            "                            <p id=\"nonprimary\">curation_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">recording_path</p>\n",
+                            "                            <p id=\"nonprimary\">waveform_param_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of waveform extraction parameters</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">metric_param_name</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">sort_interval_list_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
+                            "                            <p id=\"nonprimary\">metric_curation_param_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
+                            "            <tbody> <tr> <td>5bd75cd5-cc2e-41dd-9056-5d62fa46021a</td>\n",
+                            "<td>16cbb873-052f-44f3-9f4d-89af3544915e</td>\n",
                             "<td>0</td>\n",
-                            "<td>01_s1_first9</td>\n",
-                            "<td>default_hippocampus</td>\n",
-                            "<td>My Team</td>\n",
-                            "<td>/home/cb/wrk/zOther/data/recording/minirec20230622_.nwb_01_s1_first9_0_default_hippocampus</td>\n",
-                            "<td>minirec20230622_.nwb_01_s1_first9_0_default_hippocampus</td> </tr> </tbody>\n",
+                            "<td>default_not_whitened</td>\n",
+                            "<td>franklab_default</td>\n",
+                            "<td>default</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
                             "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*nwb_file_name *sort_group_id *sort_interval *preproc_param *team_name    recording_path sort_interval_\n",
-                            "+------------+ +------------+ +------------+ +------------+ +-----------+ +------------+ +------------+\n",
-                            "minirec2023062 0              01_s1_first9   default_hippoc My Team       /home/cb/wrk/z minirec2023062\n",
+                            "*metric_curati sorting_id     curation_id    waveform_param metric_param_n metric_curatio\n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "5bd75cd5-cc2e- 16cbb873-052f- 0              default_not_wh franklab_defau default       \n",
                             " (Total: 1)"
                         ]
                     },
-                    "execution_count": 39,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.SpikeSortingRecording() & ssr_key"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Artifact Detection\n",
-                "\n",
-                "`ArtifactDetectionParameters` establishes the parameters for removing artifacts\n",
-                "from the data. We may want to target artifact signal that is within the\n",
-                "frequency band of our filter (600Hz-6KHz), and thus will not get removed by\n",
-                "filtering.\n",
-                "\n",
-                "For this demo, we'll use a parameter set to skip this step.\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 41,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "sgs.ArtifactDetectionParameters().insert_default()\n",
-                "artifact_key = (sgs.SpikeSortingRecording() & ssr_key).fetch1(\"KEY\")\n",
-                "artifact_key[\"artifact_params_name\"] = \"none\""
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "We then pair artifact detection parameters in `ArtifactParameters` with a\n",
-                "recording extracted through population of `SpikeSortingRecording` and insert\n",
-                "into `ArtifactDetectionSelection`.\n"
+                "sgs.MetricCurationSelection.insert_selection(key)\n",
+                "sgs.MetricCurationSelection() & key"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": 27,
+            "id": "d22f5725-4fd1-42ea-a1d4-590bd1353d46",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -1343,103 +1328,123 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b>Specifies artifact detection parameters to apply to a sort group's recording.</b>\n",
+                            "    <b>Results of applying curation based on quality metrics. To do additional curation, insert another row in `CurationV1`</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_group_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">identifier for a group of electrodes</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_interval_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name for this interval</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">preproc_params_name</p>\n",
+                            "                            <p id=\"primary\">metric_curation_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">team_name</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                            <p id=\"nonprimary\">analysis_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the file</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">artifact_params_name</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">custom_artifact_detection</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                            <p id=\"nonprimary\">object_id</p>\n",
+                            "                            <span class=\"djtooltiptext\">Object ID for the metrics in NWB file</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>01_s1_first9</td>\n",
-                            "<td>default_hippocampus</td>\n",
-                            "<td>My Team</td>\n",
-                            "<td>none</td>\n",
-                            "<td>0</td> </tr> </tbody>\n",
+                            "            <tbody> <tr> <td>5bd75cd5-cc2e-41dd-9056-5d62fa46021a</td>\n",
+                            "<td>minirec20230622_PVSMM7XHHJ.nwb</td>\n",
+                            "<td>01b58a59-1b49-4bd1-a204-16fb09d67b2a</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
                             "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*nwb_file_name *sort_group_id *sort_interval *preproc_param *team_name    *artifact_para custom_artifac\n",
-                            "+------------+ +------------+ +------------+ +------------+ +-----------+ +------------+ +------------+\n",
-                            "minirec2023062 0              01_s1_first9   default_hippoc My Team       none           0             \n",
+                            "*metric_curati analysis_file_ object_id     \n",
+                            "+------------+ +------------+ +------------+\n",
+                            "5bd75cd5-cc2e- minirec2023062 01b58a59-1b49-\n",
                             " (Total: 1)"
                         ]
                     },
-                    "execution_count": 42,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.ArtifactDetectionSelection().insert1(artifact_key)\n",
-                "sgs.ArtifactDetectionSelection() & artifact_key"
+                "sgs.MetricCuration.populate(key)\n",
+                "sgs.MetricCuration() & key"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "54f354bf-0bfa-4148-9c5d-c5593f3f3915",
             "metadata": {},
             "source": [
-                "Then, we can populate `ArtifactDetection`, which will find periods where there\n",
-                "are artifacts, as specified by the parameters.\n"
+                "to do another round of curation, fetch the relevant info and insert back into CurationV1 using `insert_curation`\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 28,
+            "id": "544ba8c0-560e-471b-9eaf-5924f6051faa",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
+                    "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Amplitude and zscore thresholds are both None, skipping artifact detection\n"
+                        "[11:08:29][INFO] Spyglass: Writing new NWB file minirec20230622_ZCMODPF1NM.nwb\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/build/objectmapper.py:668: MissingRequiredBuildWarning: NWBFile 'root' is missing required value for attribute 'source_script_file_name'.\n",
+                        "  warnings.warn(msg, MissingRequiredBuildWarning)\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/datajoint/hash.py:39: ResourceWarning: unclosed file <_io.BufferedReader name='/stelmo/nwb/analysis/minirec20230622/minirec20230622_ZCMODPF1NM.nwb'>\n",
+                        "  return uuid_from_stream(Path(filepath).open(\"rb\"), init_string=init_string)\n",
+                        "ResourceWarning: Enable tracemalloc to get the object allocation traceback\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/datajoint/external.py:276: DeprecationWarning: The truth value of an empty array is ambiguous. Returning False, but in future this will result in an error. Use `array.size > 0` to check that an array is not empty.\n",
+                        "  if check_hash:\n"
                     ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "{'sorting_id': UUID('16cbb873-052f-44f3-9f4d-89af3544915e'),\n",
+                            " 'curation_id': 1,\n",
+                            " 'parent_curation_id': 0,\n",
+                            " 'analysis_file_name': 'minirec20230622_ZCMODPF1NM.nwb',\n",
+                            " 'object_id': 'c43cd7ab-e5bd-4528-a0e5-0ca7c337a72d',\n",
+                            " 'merges_applied': False,\n",
+                            " 'description': 'after metric curation'}"
+                        ]
+                    },
+                    "execution_count": 28,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.ArtifactDetection.populate(artifact_key)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Populating `ArtifactDetection` also inserts an entry into `ArtifactRemovedIntervalList`, which stores the interval without detected artifacts.\n"
+                "key = {\n",
+                "    \"metric_curation_id\": (\n",
+                "        sgs.MetricCurationSelection & {\"sorting_id\": key[\"sorting_id\"]}\n",
+                "    ).fetch1(\"metric_curation_id\")\n",
+                "}\n",
+                "labels = sgs.MetricCuration.get_labels(key)\n",
+                "merge_groups = sgs.MetricCuration.get_merge_groups(key)\n",
+                "metrics = sgs.MetricCuration.get_metrics(key)\n",
+                "sgs.CurationV1.insert_curation(\n",
+                "    sorting_id=(\n",
+                "        sgs.MetricCurationSelection\n",
+                "        & {\"metric_curation_id\": key[\"metric_curation_id\"]}\n",
+                "    ).fetch1(\"sorting_id\"),\n",
+                "    parent_curation_id=0,\n",
+                "    labels=labels,\n",
+                "    merge_groups=merge_groups,\n",
+                "    metrics=metrics,\n",
+                "    description=\"after metric curation\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 29,
+            "id": "f7c6bfd9-5985-41e1-bf37-8c8874b59191",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -1489,275 +1494,304 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b>Stores intervals without detected artifacts.</b>\n",
+                            "    <b>Curation of a SpikeSorting. Use `insert_curation` to insert rows.</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">artifact_removed_interval_list_name</p>\n",
+                            "                            <p id=\"primary\">sorting_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">sort_group_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">identifier for a group of electrodes</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">sort_interval_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name for this interval</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">preproc_params_name</p>\n",
+                            "                            <p id=\"primary\">curation_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">team_name</p>\n",
+                            "                            <p id=\"nonprimary\">parent_curation_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">artifact_params_name</p>\n",
+                            "                            <p id=\"nonprimary\">analysis_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">object_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">artifact_removed_valid_times</p>\n",
+                            "                            <p id=\"nonprimary\">merges_applied</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">artifact_times</p>\n",
-                            "                            <span class=\"djtooltiptext\">np array of artifact intervals</span>\n",
+                            "                            <p id=\"nonprimary\">description</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb_01_s1_first9_0_default_hippocampus_none_artifact_removed_valid_times</td>\n",
-                            "<td>minirec20230622_.nwb</td>\n",
+                            "            <tbody> <tr> <td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
                             "<td>0</td>\n",
-                            "<td>01_s1_first9</td>\n",
-                            "<td>default_hippocampus</td>\n",
-                            "<td>My Team</td>\n",
-                            "<td>none</td>\n",
-                            "<td>=BLOB=</td>\n",
-                            "<td>=BLOB=</td> </tr> </tbody>\n",
+                            "<td>-1</td>\n",
+                            "<td>BS2820231107_8Z8CLG184Z.nwb</td>\n",
+                            "<td>37ee7365-028f-46e1-8351-1cd402a7b36c</td>\n",
+                            "<td>0</td>\n",
+                            "<td>testing sort</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>1</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_HPIQR9LZWU.nwb</td>\n",
+                            "<td>538032a5-5d29-4cb8-b0a2-7224fee6d8ce</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>2</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_SVW8YK84IP.nwb</td>\n",
+                            "<td>ed440315-7302-4217-be15-087c7efeda7e</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>3</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_7CWR2JR68B.nwb</td>\n",
+                            "<td>0d8be667-2831-4e99-8c9b-54102de48e85</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>4</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_1PCRTB2UZ2.nwb</td>\n",
+                            "<td>9f9e9a1e-9be3-405c-9c66-4bf6dc54d4d9</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>5</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_4NPZ4YTASV.nwb</td>\n",
+                            "<td>89170a28-487a-4787-83dd-18009c446700</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>6</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_MMSIJ8YQ54.nwb</td>\n",
+                            "<td>c9fb8c88-6449-4d9a-a40a-cd10dcdc193f</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>7</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_LZJWQPP1YW.nwb</td>\n",
+                            "<td>f078e3bb-92fc-4e7f-b3a8-32936a90e057</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>8</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_RJ7DLUKOIG.nwb</td>\n",
+                            "<td>c311fbfb-cd3d-4d92-b535-b5da3d4a6ec3</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>021fb85a-992f-4360-99c7-e2da32c5b9cb</td>\n",
+                            "<td>9</td>\n",
+                            "<td>0</td>\n",
+                            "<td>BS2820231107_6ZJP5NRCX9.nwb</td>\n",
+                            "<td>a54ee3f8-851a-4dca-bb46-7673e2807462</td>\n",
+                            "<td>0</td>\n",
+                            "<td>after metric curation</td></tr><tr><td>03dc29a5-febe-4a59-ab61-21a25dea3625</td>\n",
+                            "<td>0</td>\n",
+                            "<td>-1</td>\n",
+                            "<td>j1620210710_EOE1VZ4YAX.nwb</td>\n",
+                            "<td>52889e86-c249-4916-9576-a9ccf7f48dbe</td>\n",
+                            "<td>0</td>\n",
+                            "<td></td></tr><tr><td>061ba57b-d2cb-4052-b375-42ba13684e41</td>\n",
+                            "<td>0</td>\n",
+                            "<td>-1</td>\n",
+                            "<td>BS2820231107_S21IIVRCZA.nwb</td>\n",
+                            "<td>5d71500d-1065-4610-b3a6-746821d0f438</td>\n",
+                            "<td>0</td>\n",
+                            "<td>testing sort</td> </tr> </tbody>\n",
                             "        </table>\n",
-                            "        \n",
-                            "        <p>Total: 1</p></div>\n",
+                            "        <p>...</p>\n",
+                            "        <p>Total: 627</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*artifact_remo nwb_file_name  sort_group_id  sort_interval_ preproc_params team_name     artifact_param artifact_r artifact_t\n",
-                            "+------------+ +------------+ +------------+ +------------+ +------------+ +-----------+ +------------+ +--------+ +--------+\n",
-                            "minirec2023062 minirec2023062 0              01_s1_first9   default_hippoc My Team       none           =BLOB=     =BLOB=    \n",
-                            " (Total: 1)"
+                            "*sorting_id    *curation_id   parent_curatio analysis_file_ object_id      merges_applied description   \n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "021fb85a-992f- 0              -1             BS2820231107_8 37ee7365-028f- 0              testing sort  \n",
+                            "021fb85a-992f- 1              0              BS2820231107_H 538032a5-5d29- 0              after metric c\n",
+                            "021fb85a-992f- 2              0              BS2820231107_S ed440315-7302- 0              after metric c\n",
+                            "021fb85a-992f- 3              0              BS2820231107_7 0d8be667-2831- 0              after metric c\n",
+                            "021fb85a-992f- 4              0              BS2820231107_1 9f9e9a1e-9be3- 0              after metric c\n",
+                            "021fb85a-992f- 5              0              BS2820231107_4 89170a28-487a- 0              after metric c\n",
+                            "021fb85a-992f- 6              0              BS2820231107_M c9fb8c88-6449- 0              after metric c\n",
+                            "021fb85a-992f- 7              0              BS2820231107_L f078e3bb-92fc- 0              after metric c\n",
+                            "021fb85a-992f- 8              0              BS2820231107_R c311fbfb-cd3d- 0              after metric c\n",
+                            "021fb85a-992f- 9              0              BS2820231107_6 a54ee3f8-851a- 0              after metric c\n",
+                            "03dc29a5-febe- 0              -1             j1620210710_EO 52889e86-c249- 0                            \n",
+                            "061ba57b-d2cb- 0              -1             BS2820231107_S 5d71500d-1065- 0              testing sort  \n",
+                            "   ...\n",
+                            " (Total: 627)"
                         ]
                     },
-                    "execution_count": 44,
+                    "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.ArtifactRemovedIntervalList() & artifact_key"
+                "sgs.CurationV1()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "a627274b",
             "metadata": {},
             "source": [
-                "## Spike sorting\n"
+                "## Manual Curation (Optional)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "cf8708a4-0a55-4309-b3c4-dbf47d61ad31",
             "metadata": {},
             "source": [
-                "### `SpikeSorterParameters`\n",
+                "Next we will do manual curation. this is done with figurl. to incorporate info from other stages of processing (e.g. metrics) we have to store that with kachery cloud and get curation uri referring to it. it can be done with `generate_curation_uri`.\n",
                 "\n",
-                "For our example, we will be using `mountainsort4`. There are already some default parameters in the `SpikeSorterParameters` table we'll `fetch`.\n"
+                "_Note_: This step is dependent on setting up a kachery sharing system as described in [02_Data_Sync.ipynb](02_Data_Sync.ipynb)\n",
+                "and will likely not work correctly on the spyglass-demo server.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": null,
+            "id": "924cdfce-e287-41d7-abf9-872797637777",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'sorter': 'mountainsort4', 'sorter_params_name': 'default', 'sorter_params': {'detect_sign': -1, 'adjacency_radius': -1, 'freq_min': 300, 'freq_max': 6000, 'filter': True, 'whiten': True, 'num_workers': 1, 'clip_size': 50, 'detect_threshold': 3, 'detect_interval': 10, 'tempdir': None}}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "sgs.SpikeSorterParameters().insert_default()\n",
-                "\n",
-                "# Let's look at the default params\n",
-                "sorter_name = \"mountainsort4\"\n",
-                "ms4_default_params = (\n",
-                "    sgs.SpikeSorterParameters\n",
-                "    & {\"sorter\": sorter_name, \"sorter_params_name\": \"default\"}\n",
-                ").fetch1()\n",
-                "print(ms4_default_params)"
+                "curation_uri = sgs.FigURLCurationSelection.generate_curation_uri(\n",
+                "    {\n",
+                "        \"sorting_id\": (\n",
+                "            sgs.MetricCurationSelection\n",
+                "            & {\"metric_curation_id\": key[\"metric_curation_id\"]}\n",
+                "        ).fetch1(\"sorting_id\"),\n",
+                "        \"curation_id\": 1,\n",
+                "    }\n",
+                ")\n",
+                "key = {\n",
+                "    \"sorting_id\": (\n",
+                "        sgs.MetricCurationSelection\n",
+                "        & {\"metric_curation_id\": key[\"metric_curation_id\"]}\n",
+                "    ).fetch1(\"sorting_id\"),\n",
+                "    \"curation_id\": 1,\n",
+                "    \"curation_uri\": curation_uri,\n",
+                "    \"metrics_figurl\": list(metrics.keys()),\n",
+                "}\n",
+                "sgs.FigURLCurationSelection()"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ecb9106b-8f92-4725-a68c-d5233453b3a4",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Now we can change these default parameters to line up more closely with our preferences.\n"
+                "sgs.FigURLCurationSelection.insert_selection(key)\n",
+                "sgs.FigURLCurationSelection()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 52,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'adjacency_radius': 100,\n",
-                        " 'clip_size': 39,\n",
-                        " 'detect_interval': 10,\n",
-                        " 'detect_sign': -1,\n",
-                        " 'detect_threshold': 3,\n",
-                        " 'filter': False,\n",
-                        " 'freq_max': 0,\n",
-                        " 'freq_min': 0,\n",
-                        " 'num_workers': 4,\n",
-                        " 'tempdir': None,\n",
-                        " 'verbose': True,\n",
-                        " 'whiten': False}\n"
-                    ]
-                }
-            ],
+            "execution_count": null,
+            "id": "c3b029c6-8dc8-4af3-ad42-8a9443e70023",
+            "metadata": {},
+            "outputs": [],
             "source": [
-                "sorter_params = {\n",
-                "    **ms4_default_params[\"sorter_params\"],  # start with defaults\n",
-                "    \"detect_sign\": -1,  # downward going spikes (1 for upward, 0 for both)\n",
-                "    \"adjacency_radius\": 100,  # Sort electrodes together within 100 microns\n",
-                "    \"filter\": False,  # No filter, since we filter prior to starting sort\n",
-                "    \"freq_min\": 0,\n",
-                "    \"freq_max\": 0,\n",
-                "    \"whiten\": False,  # Turn whiten, since we whiten it prior to starting sort\n",
-                "    \"num_workers\": 4,  #  same number as number of electrodes\n",
-                "    \"verbose\": True,\n",
-                "    \"clip_size\": np.int64(\n",
-                "        1.33e-3  # same as # of samples for 1.33 ms based on the sampling rate\n",
-                "        * (sgc.Raw & {\"nwb_file_name\": nwb_file_name}).fetch1(\"sampling_rate\")\n",
-                "    ),\n",
-                "}\n",
-                "from pprint import pprint\n",
-                "\n",
-                "pprint(sorter_params)"
+                "sgs.FigURLCuration.populate()\n",
+                "sgs.FigURLCuration()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "9ca0d48c-900b-4985-a27a-be1ff82616a4",
             "metadata": {},
             "source": [
-                "We can give these `sorter_params` a `sorter_params_name` and insert into `SpikeSorterParameters`.\n"
+                "or you can manually specify it if you already have a `curation.json`\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 53,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "{'sorter': 'mountainsort4',\n",
-                            " 'sorter_params_name': 'hippocampus_tutorial',\n",
-                            " 'sorter_params': {'detect_sign': -1,\n",
-                            "  'adjacency_radius': 100,\n",
-                            "  'freq_min': 0,\n",
-                            "  'freq_max': 0,\n",
-                            "  'filter': False,\n",
-                            "  'whiten': False,\n",
-                            "  'num_workers': 4,\n",
-                            "  'clip_size': 39,\n",
-                            "  'detect_threshold': 3,\n",
-                            "  'detect_interval': 10,\n",
-                            "  'tempdir': None,\n",
-                            "  'verbose': True}}"
-                        ]
-                    },
-                    "execution_count": 53,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "execution_count": null,
+            "id": "b2e9b018-9a8b-4344-9b8e-9e2141324bfa",
+            "metadata": {},
+            "outputs": [],
             "source": [
-                "sorter_params_name = \"hippocampus_tutorial\"\n",
-                "sgs.SpikeSorterParameters.insert1(\n",
-                "    {\n",
-                "        \"sorter\": sorter_name,\n",
-                "        \"sorter_params_name\": sorter_params_name,\n",
-                "        \"sorter_params\": sorter_params,\n",
-                "    },\n",
-                "    skip_duplicates=True,\n",
+                "gh_curation_uri = (\n",
+                "    \"gh://LorenFrankLab/sorting-curations/main/khl02007/test/curation.json\"\n",
                 ")\n",
-                "(\n",
-                "    sgs.SpikeSorterParameters\n",
-                "    & {\"sorter\": sorter_name, \"sorter_params_name\": sorter_params_name}\n",
-                ").fetch1()"
+                "\n",
+                "key = {\n",
+                "    \"sorting_id\": key[\"sorting_id\"],\n",
+                "    \"curation_id\": 1,\n",
+                "    \"curation_uri\": gh_curation_uri,\n",
+                "    \"metrics_figurl\": [],\n",
+                "}\n",
+                "sgs.FigURLCurationSelection.insert_selection(key)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ad86c81e-1424-4fa2-a022-7cc0a3425fc0",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sgs.FigURLCuration.populate()\n",
+                "sgs.FigURLCuration()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "6d68f93e-1586-4d3b-b680-0fe2115c0ab4",
             "metadata": {},
             "source": [
-                "### `SpikeSortingSelection`\n",
-                "\n",
-                "**Gearing up to Spike Sort!**\n",
-                "\n",
-                "We now collect our various keys to insert into `SpikeSortingSelection`, which is specific to this recording and eventual sorting segment.\n",
-                "\n",
-                "_Note:_ the spike _sorter_ parameters defined above are specific to\n",
-                "`mountainsort4` and may not work for other sorters.\n"
+                "once you apply manual curation (curation labels and merge groups) you can store them as nwb by inserting another row in CurationV1. And then you can do more rounds of curation if you want.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 59,
+            "execution_count": null,
+            "id": "15694ca0-3ec1-49a8-9ac4-66cf6d6f49ee",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "{'nwb_file_name': 'minirec20230622_.nwb',\n",
-                            " 'sort_group_id': 0,\n",
-                            " 'sort_interval_name': '01_s1_first9',\n",
-                            " 'preproc_params_name': 'default_hippocampus',\n",
-                            " 'team_name': 'My Team',\n",
-                            " 'artifact_removed_interval_list_name': 'minirec20230622_.nwb_01_s1_first9_0_default_hippocampus_none_artifact_removed_valid_times',\n",
-                            " 'sorter': 'mountainsort4',\n",
-                            " 'sorter_params_name': 'hippocampus_tutorial'}"
-                        ]
-                    },
-                    "execution_count": 59,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "ss_key = dict(\n",
-                "    **(sgs.ArtifactDetection & ssr_key).fetch1(\"KEY\"),\n",
-                "    **(sgs.ArtifactRemovedIntervalList() & ssr_key).fetch1(\"KEY\"),\n",
-                "    sorter=sorter_name,\n",
-                "    sorter_params_name=sorter_params_name,\n",
-                ")\n",
-                "ss_key.pop(\"artifact_params_name\")\n",
-                "ss_key"
+                "labels = sgs.FigURLCuration.get_labels(gh_curation_uri)\n",
+                "merge_groups = sgs.FigURLCuration.get_merge_groups(gh_curation_uri)\n",
+                "sgs.CurationV1.insert_curation(\n",
+                "    sorting_id=key[\"sorting_id\"],\n",
+                "    parent_curation_id=1,\n",
+                "    labels=labels,\n",
+                "    merge_groups=merge_groups,\n",
+                "    metrics=metrics,\n",
+                "    description=\"after figurl curation\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 60,
+            "execution_count": null,
+            "id": "1d40eb3a-34c5-4771-8fc0-730fafb5cb8a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sgs.CurationV1()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "9ff6aff5-7020-40d6-832f-006d66d54a7e",
+            "metadata": {},
+            "source": [
+                "## Downstream usage (Merge table)\n",
+                "\n",
+                "Regardless of Curation method used, to make use of spikeorting results in downstream pipelines like Decoding, we will need to insert it into the `SpikeSortingOutput` merge table. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 30,
+            "id": "511ecb19-7d8d-4db6-be71-c0ed66e2b0f2",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -1807,573 +1841,168 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b>Table for holding selection of recording and parameters for each spike sorting run</b>\n",
+                            "    <b>Output of spike sorting pipelines.</b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_group_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">identifier for a group of electrodes</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sort_interval_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name for this interval</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">preproc_params_name</p>\n",
+                            "                            <p id=\"primary\">merge_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">team_name</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sorter</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sorter_params_name</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">artifact_removed_interval_list_name</p>\n",
+                            "                            <p id=\"nonprimary\">source</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">import_path</p>\n",
-                            "                            <span class=\"djtooltiptext\">optional path to previous curated sorting output</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
-                            "<td>0</td>\n",
-                            "<td>01_s1_first9</td>\n",
-                            "<td>default_hippocampus</td>\n",
-                            "<td>My Team</td>\n",
-                            "<td>mountainsort4</td>\n",
-                            "<td>hippocampus_tutorial</td>\n",
-                            "<td>minirec20230622_.nwb_01_s1_first9_0_default_hippocampus_none_artifact_removed_valid_times</td>\n",
-                            "<td></td> </tr> </tbody>\n",
+                            "            <tbody> <tr> <td>0001a1ab-7c2b-1085-2062-53c0338ffe22</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>000c5d0b-1c4c-55d1-ccf6-5808f57152d3</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>0015e01d-0dc0-ca2c-1f5c-2178fa2c7f1e</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>001628b1-0af1-7c74-a211-0e5c158ba10f</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>001783f0-c5da-98c2-5b2a-63f1334c0a43</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>0020b039-6a2d-1d68-6585-4866fb7ea266</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>002be77b-38a6-fff8-cb48-a81e20ccb51b</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>002da11c-2d16-a6dc-0468-980674ca12b0</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>003bf29a-fa09-05be-5cac-b7ea70a48c0c</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>003cabf2-c471-972a-4b18-63d4ab7e1b8b</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>004d99c6-1b2e-1696-fc85-e78ac5cc7e6b</td>\n",
+                            "<td>CuratedSpikeSorting</td></tr><tr><td>004faf9a-72cb-4416-ae13-3f85d538604f</td>\n",
+                            "<td>CuratedSpikeSorting</td> </tr> </tbody>\n",
                             "        </table>\n",
-                            "        \n",
-                            "        <p>Total: 1</p></div>\n",
+                            "        <p>...</p>\n",
+                            "        <p>Total: 8684</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*nwb_file_name *sort_group_id *sort_interval *preproc_param *team_name    *sorter        *sorter_params *artifact_remo import_path   \n",
-                            "+------------+ +------------+ +------------+ +------------+ +-----------+ +------------+ +------------+ +------------+ +------------+\n",
-                            "minirec2023062 0              01_s1_first9   default_hippoc My Team       mountainsort4  hippocampus_tu minirec2023062               \n",
-                            " (Total: 1)"
+                            "*merge_id      source        \n",
+                            "+------------+ +------------+\n",
+                            "0001a1ab-7c2b- CuratedSpikeSo\n",
+                            "000c5d0b-1c4c- CuratedSpikeSo\n",
+                            "0015e01d-0dc0- CuratedSpikeSo\n",
+                            "001628b1-0af1- CuratedSpikeSo\n",
+                            "001783f0-c5da- CuratedSpikeSo\n",
+                            "0020b039-6a2d- CuratedSpikeSo\n",
+                            "002be77b-38a6- CuratedSpikeSo\n",
+                            "002da11c-2d16- CuratedSpikeSo\n",
+                            "003bf29a-fa09- CuratedSpikeSo\n",
+                            "003cabf2-c471- CuratedSpikeSo\n",
+                            "004d99c6-1b2e- CuratedSpikeSo\n",
+                            "004faf9a-72cb- CuratedSpikeSo\n",
+                            "   ...\n",
+                            " (Total: 8684)"
                         ]
                     },
-                    "execution_count": 60,
+                    "execution_count": 30,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.SpikeSortingSelection.insert1(ss_key, skip_duplicates=True)\n",
-                "(sgs.SpikeSortingSelection & ss_key)"
+                "from spyglass.spikesorting.spikesorting_merge import SpikeSortingOutput\n",
+                "\n",
+                "SpikeSortingOutput()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 52,
+            "id": "b20c2c9e-0c97-4669-b45d-4b1c50fd2fcc",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "*merge_id      *source        *sorting_id    *curation_id   *nwb_file_name *sort_group_id *sort_interval *preproc_param *team_name    *sorter    *sorter_params *artifact_remo\n",
+                        "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +-----------+ +--------+ +------------+ +------------+\n",
+                        "d76584f8-0969- CurationV1     03dc29a5-febe- 0              None           0              None           None           None          None       None           None          \n",
+                        "33d71671-63e5- CurationV1     090377fb-72b7- 0              None           0              None           None           None          None       None           None          \n",
+                        "dfa87e8e-c5cf- CurationV1     0cf93833-6a14- 0              None           0              None           None           None          None       None           None          \n",
+                        "a6cc0a23-7e29- CurationV1     110e27f6-5ffa- 0              None           0              None           None           None          None       None           None          \n",
+                        "7f8841a6-5e27- CurationV1     16cbb873-052f- 1              None           0              None           None           None          None       None           None          \n",
+                        "91e8e8d8-1568- CurationV1     21bea0ea-3084- 0              None           0              None           None           None          None       None           None          \n",
+                        "218c17c7-8a4c- CurationV1     21bea0ea-3084- 1              None           0              None           None           None          None       None           None          \n",
+                        "25823222-85ed- CurationV1     2484ee5d-0819- 0              None           0              None           None           None          None       None           None          \n",
+                        "5ae79d97-6a99- CurationV1     3046a016-1613- 0              None           0              None           None           None          None       None           None          \n",
+                        "869072e1-76d6- CurationV1     41a13836-e128- 0              None           0              None           None           None          None       None           None          \n",
+                        "a0771d6c-fc9d- CurationV1     4bc61e94-5bf9- 0              None           0              None           None           None          None       None           None          \n",
+                        "ed70dacb-a637- CurationV1     5d15f94e-d53d- 0              None           0              None           None           None          None       None           None          \n",
+                        "   ...\n",
+                        " (Total: 0)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# insert the automatic curation spikesorting results\n",
+                "curation_key = sss_pk.fetch1(\"KEY\")\n",
+                "curation_key[\"curation_id\"] = 1\n",
+                "merge_insert_key = (sgs.CurationV1 & curation_key).fetch(\"KEY\", as_dict=True)\n",
+                "SpikeSortingOutput.insert(merge_insert_key, part_name=\"CurationV1\")\n",
+                "SpikeSortingOutput.merge_view()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "a8ab3ed2",
             "metadata": {},
             "source": [
-                "### `SpikeSorting`\n",
-                "\n",
-                "After adding to `SpikeSortingSelection`, we can simply populate `SpikeSorting`.\n",
-                "\n",
-                "_Note:_ This may take time with longer data sets. Be sure to `pip install mountainsort4` if this is your first time spike sorting.\n"
+                "Finding the merge id's corresponding to an interpretable restriction such as `merge_id` or `interval_list` can require several join steps with upstream tables.  To simplify this process we can use the included helper function `SpikeSortingOutput().get_restricted_merge_ids()` to perform the necessary joins and return the matching merge id's"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 62,
-            "metadata": {
-                "tags": []
-            },
+            "execution_count": 6,
+            "id": "3925b5de",
+            "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
+                    "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Running spike sorting on {'nwb_file_name': 'minirec20230622_.nwb', 'sort_group_id': 0, 'sort_interval_name': '01_s1_first9', 'preproc_params_name': 'default_hippocampus', 'team_name': 'My Team', 'sorter': 'mountainsort4', 'sorter_params_name': 'hippocampus_tutorial', 'artifact_removed_interval_list_name': 'minirec20230622_.nwb_01_s1_first9_0_default_hippocampus_none_artifact_removed_valid_times'}...\n",
-                        "Mountainsort4 use the OLD spikeextractors mapped with NewToOldRecording\n",
-                        "Using temporary directory /home/cb/wrk/zOther/data/tmp/tmpr9_xzjwk\n",
-                        "Using 4 workers.\n",
-                        "Using tempdir: /home/cb/wrk/zOther/data/tmp/tmpr9_xzjwk/tmpo_xved1i\n",
-                        "Num. workers = 4\n",
-                        "Preparing /home/cb/wrk/zOther/data/tmp/tmpr9_xzjwk/tmpo_xved1i/timeseries.hdf5...\n",
-                        "Preparing neighborhood sorters (M=31, N=269997)...\n",
-                        "Neighboorhood of channel 29 has 5 channels.Neighboorhood of channel 28 has 6 channels.\n",
-                        "\n",
-                        "Detecting events on channel 29 (phase1)...\n",
-                        "Detecting events on channel 30 (phase1)...\n",
-                        "Neighboorhood of channel 23 has 7 channels.\n",
-                        "Detecting events on channel 24 (phase1)...\n",
-                        "Neighboorhood of channel 7 has 7 channels.\n",
-                        "Detecting events on channel 8 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.022525\n",
-                        "Num events detected on channel 30 (phase1): 1\n",
-                        "Computing PCA features for channel 30 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.025604\n",
-                        "Num events detected on channel 29 (phase1): 6\n",
-                        "Computing PCA features for channel 29 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.028793\n",
-                        "Num events detected on channel 24 (phase1): 5\n",
-                        "Computing PCA features for channel 24 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.029814\n",
-                        "Num events detected on channel 8 (phase1): 5\n",
-                        "Computing PCA features for channel 8 (phase1)...\n",
-                        "Clustering for channel 30 (phase1)...\n",
-                        "Found 1 clusters for channel 30 (phase1)...\n",
-                        "Computing templates for channel 30 (phase1)...\n",
-                        "Re-assigning events for channel 30 (phase1)...\n",
-                        "Neighboorhood of channel 17 has 7 channels.\n",
-                        "Detecting events on channel 18 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.096352\n",
-                        "Num events detected on channel 18 (phase1): 5\n",
-                        "Computing PCA features for channel 18 (phase1)...\n",
-                        "Clustering for channel 24 (phase1)...\n",
-                        "Found 1 clusters for channel 24 (phase1)...Clustering for channel 29 (phase1)...\n",
-                        "\n",
-                        "Computing templates for channel 24 (phase1)...\n",
-                        "Found 1 clusters for channel 29 (phase1)...\n",
-                        "Computing templates for channel 29 (phase1)...\n",
-                        "Clustering for channel 8 (phase1)...\n",
-                        "Found 1 clusters for channel 8 (phase1)...\n",
-                        "Computing templates for channel 8 (phase1)...\n",
-                        "Re-assigning events for channel 29 (phase1)...Re-assigning events for channel 24 (phase1)...\n",
-                        "Neighboorhood of channel 20 has 7 channels.\n",
-                        "Detecting events on channel 21 (phase1)...\n",
-                        "\n",
-                        "Neighboorhood of channel 25 has 7 channels.\n",
-                        "Detecting events on channel 26 (phase1)...\n",
-                        "Clustering for channel 18 (phase1)...\n",
-                        "Found 1 clusters for channel 18 (phase1)...\n",
-                        "Computing templates for channel 18 (phase1)...\n",
-                        "Re-assigning events for channel 8 (phase1)...\n",
-                        "Neighboorhood of channel 26 has 7 channels.\n",
-                        "Detecting events on channel 27 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.039213\n",
-                        "Num events detected on channel 26 (phase1): 4\n",
-                        "Computing PCA features for channel 26 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood:Re-assigning events for channel 18 (phase1)...\n",
-                        " 0:00:00.055824\n",
-                        "Num events detected on channel 21 (phase1): 14\n",
-                        "Neighboorhood of channel 14 has 7 channels.Computing PCA features for channel 21 (phase1)...\n",
-                        "\n",
-                        "Detecting events on channel 15 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.029223\n",
-                        "Num events detected on channel 27 (phase1): 8\n",
-                        "Computing PCA features for channel 27 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood:Clustering for channel 27 (phase1)...\n",
-                        "Found 1 clusters for channel 27 (phase1)... 0:00:00.086340\n",
-                        "Num events detected on channel 15 (phase1): 2\n",
-                        "Computing PCA features for channel 15 (phase1)...\n",
-                        "\n",
-                        "Computing templates for channel 27 (phase1)...\n",
-                        "Clustering for channel 26 (phase1)...\n",
-                        "Found 1 clusters for channel 26 (phase1)...\n",
-                        "Computing templates for channel 26 (phase1)...\n",
-                        "Clustering for channel 21 (phase1)...\n",
-                        "Found 1 clusters for channel 21 (phase1)...\n",
-                        "Computing templates for channel 21 (phase1)...\n",
-                        "Re-assigning events for channel 26 (phase1)...Re-assigning events for channel 27 (phase1)...\n",
-                        "Neighboorhood of channel 4 has 7 channels.\n",
-                        "Detecting events on channel 5 (phase1)...\n",
-                        "Re-assigning events for channel 21 (phase1)...\n",
-                        "\n",
-                        "Neighboorhood of channel 15 has 7 channels.Neighboorhood of channel 16 has 7 channels.\n",
-                        "Detecting events on channel 16 (phase1)...\n",
-                        "\n",
-                        "Detecting events on channel 17 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.027093\n",
-                        "Num events detected on channel 5 (phase1): 18\n",
-                        "Computing PCA features for channel 5 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.035564\n",
-                        "Num events detected on channel 16 (phase1): 6\n",
-                        "Computing PCA features for channel 16 (phase1)...\n",
-                        "Clustering for channel 5 (phase1)...\n",
-                        "Found 1 clusters for channel 5 (phase1)...\n",
-                        "Computing templates for channel 5 (phase1)...\n",
-                        "Clustering for channel 16 (phase1)...\n",
-                        "Found 1 clusters for channel 16 (phase1)...\n",
-                        "Computing templates for channel 16 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.091005\n",
-                        "Num events detected on channel 17 (phase1): 17\n",
-                        "Computing PCA features for channel 17 (phase1)...\n",
-                        "Clustering for channel 15 (phase1)...Re-assigning events for channel 5 (phase1)...\n",
-                        "Found 1 clusters for channel 15 (phase1)...\n",
-                        "Computing templates for channel 15 (phase1)...\n",
-                        "\n",
-                        "Neighboorhood of channel 11 has 7 channels.\n",
-                        "Detecting events on channel 12 (phase1)...\n",
-                        "Re-assigning events for channel 16 (phase1)...\n",
-                        "Neighboorhood of channel 12 has 7 channels.\n",
-                        "Detecting events on channel 13 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood:Re-assigning events for channel 15 (phase1)... 0:00:00.040278\n",
-                        "Num events detected on channel 12 (phase1): 7\n",
-                        "Computing PCA features for channel 12 (phase1)...\n",
-                        "\n",
-                        "Neighboorhood of channel 6 has 7 channels.\n",
-                        "Detecting events on channel 7 (phase1)...\n",
-                        "Clustering for channel 17 (phase1)...\n",
-                        "Found 1 clusters for channel 17 (phase1)...\n",
-                        "Computing templates for channel 17 (phase1)...\n",
-                        "Re-assigning events for channel 17 (phase1)...\n",
-                        "Neighboorhood of channel 21 has 7 channels.\n",
-                        "Detecting events on channel 22 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.033808\n",
-                        "Num events detected on channel 7 (phase1): 10\n",
-                        "Computing PCA features for channel 7 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.076235\n",
-                        "Num events detected on channel 13 (phase1): 1\n",
-                        "Computing PCA features for channel 13 (phase1)...\n",
-                        "Clustering for channel 12 (phase1)...\n",
-                        "Found 1 clusters for channel 12 (phase1)...\n",
-                        "Computing templates for channel 12 (phase1)...\n",
-                        "Clustering for channel 13 (phase1)...Re-assigning events for channel 12 (phase1)...\n",
-                        "Neighboorhood of channel 0 has 4 channels.\n",
-                        "Detecting events on channel 1 (phase1)...\n",
-                        "\n",
-                        "Found 1 clusters for channel 13 (phase1)...\n",
-                        "Computing templates for channel 13 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood:Re-assigning events for channel 13 (phase1)...\n",
-                        "Neighboorhood of channel 5 has 7 channels.\n",
-                        "Detecting events on channel 6 (phase1)...\n",
-                        " 0:00:00.026181\n",
-                        "Num events detected on channel 1 (phase1): 3\n",
-                        "Computing PCA features for channel 1 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.133353\n",
-                        "Num events detected on channel 22 (phase1): 3\n",
-                        "Computing PCA features for channel 22 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.025383\n",
-                        "Num events detected on channel 6 (phase1): 2\n",
-                        "Computing PCA features for channel 6 (phase1)...\n",
-                        "Clustering for channel 1 (phase1)...Clustering for channel 7 (phase1)...\n",
-                        "Found 1 clusters for channel 1 (phase1)...\n",
-                        "Computing templates for channel 1 (phase1)...\n",
-                        "\n",
-                        "Found 1 clusters for channel 7 (phase1)...\n",
-                        "Computing templates for channel 7 (phase1)...\n",
-                        "Re-assigning events for channel 1 (phase1)...\n",
-                        "Neighboorhood of channel 13 has 7 channels.Re-assigning events for channel 7 (phase1)...\n",
-                        "Detecting events on channel 14 (phase1)...\n",
-                        "\n",
-                        "Neighboorhood of channel 8 has 7 channels.\n",
-                        "Detecting events on channel 9 (phase1)...\n",
-                        "Clustering for channel 6 (phase1)...\n",
-                        "Found 1 clusters for channel 6 (phase1)...\n",
-                        "Computing templates for channel 6 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.033709\n",
-                        "Num events detected on channel 9 (phase1): 6\n",
-                        "Computing PCA features for channel 9 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood:Re-assigning events for channel 6 (phase1)... 0:00:00.055517\n",
-                        "Num events detected on channel 14 (phase1): 4\n",
-                        "Computing PCA features for channel 14 (phase1)...\n",
-                        "\n",
-                        "Neighboorhood of channel 22 has 7 channels.\n",
-                        "Detecting events on channel 23 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.020576\n",
-                        "Num events detected on channel 23 (phase1): 17\n",
-                        "Computing PCA features for channel 23 (phase1)...\n",
-                        "Clustering for channel 23 (phase1)...Clustering for channel 14 (phase1)...\n",
-                        "Found 1 clusters for channel 14 (phase1)...\n",
-                        "Computing templates for channel 14 (phase1)...\n",
-                        "Clustering for channel 22 (phase1)...\n",
-                        "Found 1 clusters for channel 22 (phase1)...\n",
-                        "Computing templates for channel 22 (phase1)...\n",
-                        "Clustering for channel 9 (phase1)...\n",
-                        "Found 1 clusters for channel 9 (phase1)...\n",
-                        "Computing templates for channel 9 (phase1)...\n",
-                        "\n",
-                        "Found 1 clusters for channel 23 (phase1)...\n",
-                        "Computing templates for channel 23 (phase1)...\n",
-                        "Re-assigning events for channel 14 (phase1)...\n",
-                        "Re-assigning events for channel 9 (phase1)...Neighboorhood of channel 18 has 7 channels.\n",
-                        "Detecting events on channel 19 (phase1)...\n",
-                        "\n",
-                        "Neighboorhood of channel 9 has 7 channels.\n",
-                        "Detecting events on channel 10 (phase1)...\n",
-                        "Re-assigning events for channel 23 (phase1)...\n",
-                        "Neighboorhood of channel 27 has 7 channels.\n",
-                        "Detecting events on channel 28 (phase1)...\n",
-                        "Re-assigning events for channel 22 (phase1)...\n",
-                        "Neighboorhood of channel 3 has 7 channels.\n",
-                        "Detecting events on channel 4 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.035256\n",
-                        "Num events detected on channel 19 (phase1): 11\n",
-                        "Computing PCA features for channel 19 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.040792\n",
-                        "Num events detected on channel 10 (phase1): 5\n",
-                        "Computing PCA features for channel 10 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.033487\n",
-                        "Num events detected on channel 28 (phase1): 4\n",
-                        "Computing PCA features for channel 28 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.029246\n",
-                        "Num events detected on channel 4 (phase1): 10\n",
-                        "Computing PCA features for channel 4 (phase1)...\n",
-                        "Clustering for channel 28 (phase1)...\n",
-                        "Found 1 clusters for channel 28 (phase1)...\n",
-                        "Computing templates for channel 28 (phase1)...\n",
-                        "Re-assigning events for channel 28 (phase1)...\n",
-                        "Clustering for channel 10 (phase1)...\n",
-                        "Found 1 clusters for channel 10 (phase1)...\n",
-                        "Computing templates for channel 10 (phase1)...\n",
-                        "Re-assigning events for channel 10 (phase1)...\n",
-                        "Clustering for channel 19 (phase1)...\n",
-                        "Found 1 clusters for channel 19 (phase1)...\n",
-                        "Computing templates for channel 19 (phase1)...\n",
-                        "Re-assigning events for channel 19 (phase1)...\n",
-                        "Neighboorhood of channel 1 has 5 channels.\n",
-                        "Detecting events on channel 2 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.019415\n",
-                        "Num events detected on channel 2 (phase1): 3\n",
-                        "Computing PCA features for channel 2 (phase1)...\n",
-                        "Clustering for channel 4 (phase1)...\n",
-                        "Found 1 clusters for channel 4 (phase1)...\n",
-                        "Computing templates for channel 4 (phase1)...\n",
-                        "Clustering for channel 2 (phase1)...\n",
-                        "Found 1 clusters for channel 2 (phase1)...\n",
-                        "Computing templates for channel 2 (phase1)...\n",
-                        "Re-assigning events for channel 2 (phase1)...\n",
-                        "Neighboorhood of channel 30 has 4 channels.\n",
-                        "Detecting events on channel 31 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.012684\n",
-                        "Num events detected on channel 31 (phase1): 0\n",
-                        "Computing PCA features for channel 31 (phase1)...\n",
-                        "Clustering for channel 31 (phase1)...\n",
-                        "Found 0 clusters for channel 31 (phase1)...\n",
-                        "Computing templates for channel 31 (phase1)...\n",
-                        "Re-assigning events for channel 31 (phase1)...\n",
-                        "Neighboorhood of channel 24 has 7 channels.\n",
-                        "Detecting events on channel 25 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.017826\n",
-                        "Num events detected on channel 25 (phase1): 14\n",
-                        "Computing PCA features for channel 25 (phase1)...\n",
-                        "Re-assigning events for channel 4 (phase1)...\n",
-                        "Neighboorhood of channel 19 has 7 channels.\n",
-                        "Detecting events on channel 20 (phase1)...\n",
-                        "Clustering for channel 25 (phase1)...\n",
-                        "Found 1 clusters for channel 25 (phase1)...\n",
-                        "Computing templates for channel 25 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.022288\n",
-                        "Num events detected on channel 20 (phase1): 14\n",
-                        "Computing PCA features for channel 20 (phase1)...\n",
-                        "Re-assigning events for channel 25 (phase1)...\n",
-                        "Neighboorhood of channel 2 has 6 channels.\n",
-                        "Detecting events on channel 3 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.018741\n",
-                        "Num events detected on channel 3 (phase1): 11\n",
-                        "Computing PCA features for channel 3 (phase1)...\n",
-                        "Clustering for channel 3 (phase1)...\n",
-                        "Found 1 clusters for channel 3 (phase1)...\n",
-                        "Computing templates for channel 3 (phase1)...\n",
-                        "Re-assigning events for channel 3 (phase1)...\n",
-                        "Neighboorhood of channel 10 has 7 channels.\n",
-                        "Detecting events on channel 11 (phase1)...\n",
-                        "Clustering for channel 20 (phase1)...\n",
-                        "Found 1 clusters for channel 20 (phase1)...\n",
-                        "Computing templates for channel 20 (phase1)...\n",
-                        "Re-assigning events for channel 20 (phase1)...\n",
-                        "Elapsed time for detect on neighborhood: 0:00:00.035092\n",
-                        "Num events detected on channel 11 (phase1): 6\n",
-                        "Computing PCA features for channel 11 (phase1)...\n",
-                        "Clustering for channel 11 (phase1)...\n",
-                        "Found 1 clusters for channel 11 (phase1)...\n",
-                        "Computing templates for channel 11 (phase1)...\n",
-                        "Re-assigning events for channel 11 (phase1)...\n",
-                        "Neighboorhood of channel 17 has 7 channels.\n",
-                        "Computing PCA features for channel 18 (phase2)...\n",
-                        "No duplicate events found for channel 17 in phase2\n",
-                        "Neighboorhood of channel 25 has 7 channels.\n",
-                        "Computing PCA features for channel 26 (phase2)...\n",
-                        "No duplicate events found for channel 25 in phase2\n",
-                        "Neighboorhood of channel 4 has 7 channels.\n",
-                        "Computing PCA features for channel 5 (phase2)...\n",
-                        "No duplicate events found for channel 4 in phase2\n",
-                        "Neighboorhood of channel 29 has 5 channels.\n",
-                        "Computing PCA features for channel 30 (phase2)...\n",
-                        "No duplicate events found for channel 29 in phase2\n",
-                        "Clustering for channel 30 (phase2)...\n",
-                        "Found 1 clusters for channel 30 (phase2)...\n",
-                        "Neighboorhood of channel 8 has 7 channels.\n",
-                        "Computing PCA features for channel 9 (phase2)...\n",
-                        "No duplicate events found for channel 8 in phase2\n",
-                        "Clustering for channel 18 (phase2)...\n",
-                        "Found 1 clusters for channel 18 (phase2)...\n",
-                        "Neighboorhood of channel 24 has 7 channels.\n",
-                        "Computing PCA features for channel 25 (phase2)...\n",
-                        "No duplicate events found for channel 24 in phase2\n",
-                        "Clustering for channel 5 (phase2)...\n",
-                        "Found 1 clusters for channel 5 (phase2)...\n",
-                        "Neighboorhood of channel 1 has 5 channels.\n",
-                        "Computing PCA features for channel 2 (phase2)...\n",
-                        "No duplicate events found for channel 1 in phase2\n",
-                        "Clustering for channel 9 (phase2)...\n",
-                        "Found 1 clusters for channel 9 (phase2)...\n",
-                        "Neighboorhood of channel 14 has 7 channels.\n",
-                        "Computing PCA features for channel 15 (phase2)...\n",
-                        "No duplicate events found for channel 14 in phase2\n",
-                        "Clustering for channel 2 (phase2)...\n",
-                        "Found 1 clusters for channel 2 (phase2)...\n",
-                        "Neighboorhood of channel 12 has 7 channels.\n",
-                        "Computing PCA features for channel 13 (phase2)...\n",
-                        "No duplicate events found for channel 12 in phase2\n",
-                        "Clustering for channel 26 (phase2)...\n",
-                        "Found 1 clusters for channel 26 (phase2)...\n",
-                        "Neighboorhood of channel 27 has 7 channels.\n",
-                        "Computing PCA features for channel 28 (phase2)...\n",
-                        "No duplicate events found for channel 27 in phase2\n",
-                        "Clustering for channel 15 (phase2)...\n",
-                        "Found 1 clusters for channel 15 (phase2)...\n",
-                        "Neighboorhood of channel 28 has 6 channels.\n",
-                        "Computing PCA features for channel 29 (phase2)...\n",
-                        "No duplicate events found for channel 28 in phase2\n",
-                        "Clustering for channel 13 (phase2)...\n",
-                        "Found 1 clusters for channel 13 (phase2)...\n",
-                        "Clustering for channel 29 (phase2)...\n",
-                        "Found 1 clusters for channel 29 (phase2)...\n",
-                        "Neighboorhood of channel 16 has 7 channels.\n",
-                        "Computing PCA features for channel 17 (phase2)...\n",
-                        "No duplicate events found for channel 16 in phase2\n",
-                        "Neighboorhood of channel 13 has 7 channels.\n",
-                        "Computing PCA features for channel 14 (phase2)...\n",
-                        "No duplicate events found for channel 13 in phase2\n",
-                        "Clustering for channel 17 (phase2)...\n",
-                        "Found 1 clusters for channel 17 (phase2)...\n",
-                        "Neighboorhood of channel 26 has 7 channels.\n",
-                        "Computing PCA features for channel 27 (phase2)...\n",
-                        "No duplicate events found for channel 26 in phase2\n",
-                        "Clustering for channel 27 (phase2)...Clustering for channel 14 (phase2)...\n",
-                        "\n",
-                        "Found 1 clusters for channel 14 (phase2)...\n",
-                        "Found 1 clusters for channel 27 (phase2)...\n",
-                        "Neighboorhood of channel 18 has 7 channels.\n",
-                        "Computing PCA features for channel 19 (phase2)...\n",
-                        "No duplicate events found for channel 18 in phase2\n",
-                        "Neighboorhood of channel 11 has 7 channels.\n",
-                        "Computing PCA features for channel 12 (phase2)...Clustering for channel 28 (phase2)...\n",
-                        "\n",
-                        "No duplicate events found for channel 11 in phase2\n",
-                        "Found 1 clusters for channel 28 (phase2)...\n",
-                        "Neighboorhood of channel 15 has 7 channels.\n",
-                        "Computing PCA features for channel 16 (phase2)...\n",
-                        "No duplicate events found for channel 15 in phase2\n",
-                        "Clustering for channel 25 (phase2)...\n",
-                        "Found 1 clusters for channel 25 (phase2)...\n",
-                        "Neighboorhood of channel 9 has 7 channels.\n",
-                        "Computing PCA features for channel 10 (phase2)...\n",
-                        "No duplicate events found for channel 9 in phase2\n",
-                        "Clustering for channel 12 (phase2)...\n",
-                        "Found 1 clusters for channel 12 (phase2)...\n",
-                        "Neighboorhood of channel 10 has 7 channels.\n",
-                        "Computing PCA features for channel 11 (phase2)...\n",
-                        "No duplicate events found for channel 10 in phase2\n",
-                        "Clustering for channel 19 (phase2)...\n",
-                        "Found 1 clusters for channel 19 (phase2)...\n",
-                        "Neighboorhood of channel 3 has 7 channels.\n",
-                        "Computing PCA features for channel 4 (phase2)...\n",
-                        "No duplicate events found for channel 3 in phase2\n",
-                        "Clustering for channel 11 (phase2)...\n",
-                        "Found 1 clusters for channel 11 (phase2)...\n",
-                        "Neighboorhood of channel 6 has 7 channels.\n",
-                        "Computing PCA features for channel 7 (phase2)...\n",
-                        "No duplicate events found for channel 6 in phase2\n",
-                        "Clustering for channel 4 (phase2)...\n",
-                        "Found 1 clusters for channel 4 (phase2)...\n",
-                        "Neighboorhood of channel 23 has 7 channels.\n",
-                        "Computing PCA features for channel 24 (phase2)...\n",
-                        "No duplicate events found for channel 23 in phase2\n",
-                        "Clustering for channel 7 (phase2)...\n",
-                        "Found 1 clusters for channel 7 (phase2)...\n",
-                        "Neighboorhood of channel 22 has 7 channels.\n",
-                        "Computing PCA features for channel 23 (phase2)...\n",
-                        "No duplicate events found for channel 22 in phase2\n",
-                        "Clustering for channel 23 (phase2)...Clustering for channel 16 (phase2)...\n",
-                        "\n",
-                        "Found 1 clusters for channel 16 (phase2)...\n",
-                        "Found 1 clusters for channel 23 (phase2)...\n",
-                        "Neighboorhood of channel 5 has 7 channels.\n",
-                        "Computing PCA features for channel 6 (phase2)...\n",
-                        "No duplicate events found for channel 5 in phase2\n",
-                        "Neighboorhood of channel 20 has 7 channels.\n",
-                        "Computing PCA features for channel 21 (phase2)...\n",
-                        "No duplicate events found for channel 20 in phase2\n",
-                        "Clustering for channel 10 (phase2)...\n",
-                        "Found 1 clusters for channel 10 (phase2)...\n",
-                        "Neighboorhood of channel 2 has 6 channels.\n",
-                        "Computing PCA features for channel 3 (phase2)...\n",
-                        "No duplicate events found for channel 2 in phase2\n",
-                        "Clustering for channel 24 (phase2)...\n",
-                        "Found 1 clusters for channel 24 (phase2)...\n",
-                        "Clustering for channel 21 (phase2)...\n",
-                        "Found 1 clusters for channel 21 (phase2)...\n",
-                        "Neighboorhood of channel 21 has 7 channels.\n",
-                        "Computing PCA features for channel 22 (phase2)...\n",
-                        "No duplicate events found for channel 21 in phase2\n",
-                        "Clustering for channel 6 (phase2)...\n",
-                        "Found 1 clusters for channel 6 (phase2)...\n",
-                        "Neighboorhood of channel 7 has 7 channels.\n",
-                        "Clustering for channel 22 (phase2)...\n",
-                        "Found 1 clusters for channel 22 (phase2)...\n",
-                        "Computing PCA features for channel 8 (phase2)...\n",
-                        "No duplicate events found for channel 7 in phase2\n",
-                        "Clustering for channel 3 (phase2)...\n",
-                        "Found 1 clusters for channel 3 (phase2)...\n",
-                        "Neighboorhood of channel 0 has 4 channels.\n",
-                        "Computing PCA features for channel 1 (phase2)...\n",
-                        "No duplicate events found for channel 0 in phase2\n",
-                        "Clustering for channel 1 (phase2)...\n",
-                        "Found 1 clusters for channel 1 (phase2)...\n",
-                        "Neighboorhood of channel 30 has 4 channels.\n",
-                        "Computing PCA features for channel 31 (phase2)...\n",
-                        "No duplicate events found for channel 30 in phase2\n",
-                        "Clustering for channel 31 (phase2)...\n",
-                        "Found 0 clusters for channel 31 (phase2)...\n",
-                        "Clustering for channel 8 (phase2)...\n",
-                        "Found 1 clusters for channel 8 (phase2)...\n",
-                        "Neighboorhood of channel 19 has 7 channels.\n",
-                        "Computing PCA features for channel 20 (phase2)...\n",
-                        "No duplicate events found for channel 19 in phase2\n",
-                        "Clustering for channel 20 (phase2)...\n",
-                        "Found 1 clusters for channel 20 (phase2)...\n",
-                        "Preparing output...\n",
-                        "Done with ms4alg.\n",
-                        "Cleaning tempdir::::: /home/cb/wrk/zOther/data/tmp/tmpr9_xzjwk/tmpo_xved1i\n",
-                        "mountainsort4 run time 5.69s\n",
-                        "Saving sorting results...\n"
+                        "[13:34:12][WARNING] Spyglass: V0 requires artifact restrict. Ignoring \"restrict_by_artifact\" flag.\n"
                     ]
                 },
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/cb/miniconda3/envs/spy/lib/python3.9/site-packages/spikeinterface/core/basesorting.py:212: UserWarning: The registered recording will not be persistent on disk, but only available in memory\n",
-                        "  warnings.warn(\"The registered recording will not be persistent on disk, but only available in memory\")\n",
-                        "/home/cb/miniconda3/envs/spy/lib/python3.9/tempfile.py:821: ResourceWarning: Implicitly cleaning up <TemporaryDirectory '/home/cb/wrk/zOther/data/tmp/tmpr9_xzjwk'>\n",
-                        "  _warnings.warn(warn_message, ResourceWarning)\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "[{'merge_id': UUID('74c006e8-dcfe-e994-7b40-73f8d9f75b85')}]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# [(sgs.SpikeSortingSelection & ss_key).proj()]\n",
-                "sgs.SpikeSorting.populate()"
+                "selection_key = {\n",
+                "    \"nwb_file_name\": nwb_file_name2,\n",
+                "    \"sorter\": \"mountainsort4\",\n",
+                "    \"interval_list_name\": \"01_s1\",\n",
+                "    \"curation_id\": 0,\n",
+                "}  # this function can use restrictions from throughout the spikesorting pipeline\n",
+                "spikesorting_merge_ids = SpikeSortingOutput().get_restricted_merge_ids(\n",
+                "    selection_key, as_dict=True\n",
+                ")\n",
+                "spikesorting_merge_ids"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "007fbb60",
             "metadata": {},
             "source": [
-                "#### Check to make sure the table populated\n"
+                "With the spikesorting merge_ids we want we can also use the method `get_sort_group_info` to get a table linking the merge id to the electrode group it is sourced from.  This can be helpful for restricting to just electrodes from a brain area of interest"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 63,
+            "execution_count": 60,
+            "id": "696345db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -2423,21 +2052,33 @@
                             "\n",
                             "        /* Show the tooltip text when you mouse over the tooltip container */\n",
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
-                            "    <b></b>\n",
+                            "    \n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">merge_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">nwb_file_name</p>\n",
                             "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">electrode_group_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">electrode group name from NWBFile</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">electrode_id</p>\n",
+                            "                            <span class=\"djtooltiptext\">the unique number for this electrode</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">curation_id</p>\n",
+                            "                            <span class=\"djtooltiptext\">a number correponding to the index of this curation</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">sort_group_id</p>\n",
                             "                            <span class=\"djtooltiptext\">identifier for a group of electrodes</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">sort_interval_name</p>\n",
                             "                            <span class=\"djtooltiptext\">name for this interval</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">preproc_params_name</p>\n",
@@ -2451,82 +2092,148 @@
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">sorter_params_name</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">artifact_removed_interval_list_name</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">sorting_path</p>\n",
+                            "                            <p id=\"primary\">region_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">probe_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">time_of_sort</p>\n",
-                            "                            <span class=\"djtooltiptext\">in Unix time, to the nearest second</span>\n",
+                            "                            <p id=\"nonprimary\">probe_shank</p>\n",
+                            "                            <span class=\"djtooltiptext\">shank number within probe</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">probe_electrode</p>\n",
+                            "                            <span class=\"djtooltiptext\">electrode</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">name</p>\n",
+                            "                            <span class=\"djtooltiptext\">unique label for each contact</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">original_reference_electrode</p>\n",
+                            "                            <span class=\"djtooltiptext\">the configured reference electrode for this electrode</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">x</p>\n",
+                            "                            <span class=\"djtooltiptext\">the x coordinate of the electrode position in the brain</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">y</p>\n",
+                            "                            <span class=\"djtooltiptext\">the y coordinate of the electrode position in the brain</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">z</p>\n",
+                            "                            <span class=\"djtooltiptext\">the z coordinate of the electrode position in the brain</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">filtering</p>\n",
+                            "                            <span class=\"djtooltiptext\">description of the signal filtering</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">impedance</p>\n",
+                            "                            <span class=\"djtooltiptext\">electrode impedance</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">bad_channel</p>\n",
+                            "                            <span class=\"djtooltiptext\">if electrode is \"good\" or \"bad\" as observed during recording</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">x_warped</p>\n",
+                            "                            <span class=\"djtooltiptext\">x coordinate of electrode position warped to common template brain</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">y_warped</p>\n",
+                            "                            <span class=\"djtooltiptext\">y coordinate of electrode position warped to common template brain</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">z_warped</p>\n",
+                            "                            <span class=\"djtooltiptext\">z coordinate of electrode position warped to common template brain</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">contacts</p>\n",
+                            "                            <span class=\"djtooltiptext\">label of electrode contacts used for a bipolar signal - current workaround</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">analysis_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">units_object_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">region_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">the name of the brain region</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">subregion_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">subregion name</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">subsubregion_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">subregion within subregion</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>minirec20230622_.nwb</td>\n",
+                            "            <tbody> <tr> <td>662f3e35-c81e-546c-69c3-b3a2f5ed2776</td>\n",
+                            "<td>minirec20230622_.nwb</td>\n",
+                            "<td>0</td>\n",
+                            "<td>0</td>\n",
+                            "<td>1</td>\n",
                             "<td>0</td>\n",
                             "<td>01_s1_first9</td>\n",
                             "<td>default_hippocampus</td>\n",
                             "<td>My Team</td>\n",
                             "<td>mountainsort4</td>\n",
                             "<td>hippocampus_tutorial</td>\n",
                             "<td>minirec20230622_.nwb_01_s1_first9_0_default_hippocampus_none_artifact_removed_valid_times</td>\n",
-                            "<td>/home/cb/wrk/zOther/data/\"sorting\"/minirec20230622_.nwb_01_s1_first9_0_default_hippocampus_3335c236_spikesorting</td>\n",
-                            "<td>1689971050</td> </tr> </tbody>\n",
+                            "<td>35</td>\n",
+                            "<td>tetrode_12.5</td>\n",
+                            "<td>0</td>\n",
+                            "<td>0</td>\n",
+                            "<td>0</td>\n",
+                            "<td>0</td>\n",
+                            "<td>0.0</td>\n",
+                            "<td>0.0</td>\n",
+                            "<td>0.0</td>\n",
+                            "<td>None</td>\n",
+                            "<td>0.0</td>\n",
+                            "<td>False</td>\n",
+                            "<td>0.0</td>\n",
+                            "<td>0.0</td>\n",
+                            "<td>0.0</td>\n",
+                            "<td></td>\n",
+                            "<td>minirec20230622_RXRSAFCGVJ.nwb</td>\n",
+                            "<td></td>\n",
+                            "<td>corpus callosum and associated subcortical white matter (cc-ec-cing-dwm)</td>\n",
+                            "<td>None</td>\n",
+                            "<td>None</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
                             "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*nwb_file_name *sort_group_id *sort_interval *preproc_param *team_name    *sorter        *sorter_params *artifact_remo sorting_path   time_of_sort  \n",
-                            "+------------+ +------------+ +------------+ +------------+ +-----------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
-                            "minirec2023062 0              01_s1_first9   default_hippoc My Team       mountainsort4  hippocampus_tu minirec2023062 /home/cb/wrk/z 1689971050    \n",
+                            "*merge_id      *nwb_file_name *electrode_gro *electrode_id  *curation_id   *sort_group_id *sort_interval *preproc_param *team_name    *sorter        *sorter_params *artifact_remo *region_id    probe_id       probe_shank    probe_electrod name     original_refer x       y       z       filtering     impedance     bad_channel    x_warped     y_warped     z_warped     contacts     analysis_file_ units_object_i region_name    subregion_name subsubregion_n\n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +-----------+ +------------+ +------------+ +------------+ +-----------+ +------------+ +------------+ +------------+ +------+ +------------+ +-----+ +-----+ +-----+ +-----------+ +-----------+ +------------+ +----------+ +----------+ +----------+ +----------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "662f3e35-c81e- minirec2023062 0              0              1              0              01_s1_first9   default_hippoc My Team       mountainsort4  hippocampus_tu minirec2023062 35            tetrode_12.5   0              0              0        0              0.0     0.0     0.0     None          0.0           False          0.0          0.0          0.0                       minirec2023062                corpus callosu None           None          \n",
                             " (Total: 1)"
                         ]
                     },
-                    "execution_count": 63,
+                    "execution_count": 60,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgs.SpikeSorting() & ss_key"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Next Steps\n",
-                "\n",
-                "Congratulations, you've spike sorted! See our\n",
-                "[next notebook](./03_Curation.ipynb) for curation steps.\n"
+                "merge_keys = [{\"merge_id\": str(id)} for id in spikesorting_merge_ids]\n",
+                "SpikeSortingOutput().get_sort_group_info(merge_keys)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.10.5 64-bit",
+            "display_name": "spyglass",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.18"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "8a94588eda9d64d9e9a351ab8144e55b1fabf5113b54e67dd26a8c27df0381b3"
-            }
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `spyglass_neuro-0.5.1/notebooks/20_Position_Trodes.ipynb` & `spyglass_neuro-0.5.2/notebooks/20_Position_Trodes.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/21_DLC.ipynb` & `spyglass_neuro-0.5.2/notebooks/21_DLC.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/22_DLC_Loop.ipynb` & `spyglass_neuro-0.5.2/notebooks/22_DLC_Loop.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/24_Linearization.ipynb` & `spyglass_neuro-0.5.2/notebooks/24_Linearization.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/30_LFP.ipynb` & `spyglass_neuro-0.5.2/notebooks/30_LFP.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/31_Theta.ipynb` & `spyglass_neuro-0.5.2/notebooks/31_Theta.ipynb`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/32_Ripple_Detection.ipynb` & `spyglass_neuro-0.5.2/notebooks/50_MUA_Detection.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7305244033686711%*

 * *Differences: {"'cells'": "{0: {'outputs': {0: {'text': ['[2024-02-07 14:44:16,324][INFO]: Connecting "*

 * *            "edeno@lmf-db.cin.ucsf.edu:3306\\n', '[2024-02-07 14:44:16,357][INFO]: Connected "*

 * *            "edeno@lmf-db.cin.ucsf.edu:3306\\n']}}, 'source': {insert: [(1, 'from pathlib import "*

 * *            "Path\\n'), (3, 'dj.config.load(\\n'), (4, '    "*

 * *            'Path("../dj_local_conf.json").absolute()\\n\'), (5, \')  # load config for database '*

 * *            "connection info\\n'), (7, 'from spyglass.mua.v1.mua im […]*

```diff
@@ -1,995 +1,297 @@
 {
     "cells": [
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "3c61f507-3175-4fb7-ae20-bc6174c83fe4",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "# Ripple Detection\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "50d9b693",
-            "metadata": {},
-            "source": [
-                "## Overview\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "0f36c4dd",
-            "metadata": {},
-            "source": [
-                "_Developer Note:_ if you may make a PR in the future, be sure to copy this\n",
-                "notebook, and use the `gitignore` prefix `temp` to avoid future conflicts.\n",
-                "\n",
-                "This is one notebook in a multi-part series on Spyglass.\n",
-                "\n",
-                "- To set up your Spyglass environment and database, see\n",
-                "  [the Setup notebook](./00_Setup.ipynb)\n",
-                "- For additional info on DataJoint syntax, including table definitions and\n",
-                "  inserts, see\n",
-                "  [the Insert Data notebook](./01_Insert_Data.ipynb)\n",
-                "\n",
-                "Ripple detection depends on a set of LFPs, the parameters used for detection and the speed of the animal. You will need `RippleLFPSelection`, `RippleParameters`, and `PositionOutput` to be populated accordingly.\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "53eb4779",
-            "metadata": {},
-            "source": [
-                "## Imports\n"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "fc5e9860",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[2024-01-24 09:56:01,323][INFO]: Connecting sambray@lmf-db.cin.ucsf.edu:3306\n",
-                        "[2024-01-24 09:56:01,355][INFO]: Connected sambray@lmf-db.cin.ucsf.edu:3306\n",
-                        "[09:56:02][WARNING] Spyglass: Please update position_tools to >= 0.1.0\n"
+                        "[2024-02-07 14:44:16,324][INFO]: Connecting edeno@lmf-db.cin.ucsf.edu:3306\n",
+                        "[2024-02-07 14:44:16,357][INFO]: Connected edeno@lmf-db.cin.ucsf.edu:3306\n"
                     ]
                 }
             ],
             "source": [
-                "import os\n",
                 "import datajoint as dj\n",
-                "import numpy as np\n",
-                "\n",
-                "# change to the upper level folder to detect dj_local_conf.json\n",
-                "if os.path.basename(os.getcwd()) == \"notebooks\":\n",
-                "    os.chdir(\"..\")\n",
-                "dj.config.load(\"dj_local_conf.json\")  # load config for database connection info\n",
-                "\n",
-                "import spyglass.common as sgc\n",
-                "import spyglass.position as sgp\n",
-                "import spyglass.lfp as lfp\n",
-                "import spyglass.lfp.analysis.v1 as lfp_analysis\n",
-                "from spyglass.lfp import LFPOutput\n",
-                "import spyglass.lfp.v1 as sglfp\n",
-                "from spyglass.position import PositionOutput\n",
-                "import spyglass.ripple.v1 as sgrip\n",
-                "import spyglass.ripple.v1 as sgr\n",
+                "from pathlib import Path\n",
                 "\n",
-                "# ignore datajoint+jupyter async warnings\n",
-                "import warnings\n",
+                "dj.config.load(\n",
+                "    Path(\"../dj_local_conf.json\").absolute()\n",
+                ")  # load config for database connection info\n",
                 "\n",
-                "warnings.simplefilter(\"ignore\", category=DeprecationWarning)\n",
-                "warnings.simplefilter(\"ignore\", category=ResourceWarning)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "d741727d-6609-465a-add8-b5c4c9ab844c",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "## Selecting Electrodes\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "c571fe1a",
-            "metadata": {},
-            "source": [
-                "First, we'll pick the electrodes on which we'll run ripple detection on, using\n",
-                "`RippleLFPSelection.set_lfp_electrodes`\n"
+                "from spyglass.mua.v1.mua import MuaEventsV1, MuaEventsParameters"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "902494c3-37ec-4550-b14c-4b17df7d0ec7",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[0;31mSignature:\u001b[0m\n",
-                        "\u001b[0msgr\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mRippleLFPSelection\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mset_lfp_electrodes\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;34m\u001b[0m\n",
-                        "\u001b[0;34m\u001b[0m    \u001b[0mkey\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
-                        "\u001b[0;34m\u001b[0m    \u001b[0melectrode_list\u001b[0m\u001b[0;34m=\u001b[0m\u001b[0;32mNone\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
-                        "\u001b[0;34m\u001b[0m    \u001b[0mgroup_name\u001b[0m\u001b[0;34m=\u001b[0m\u001b[0;34m'CA1'\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
-                        "\u001b[0;34m\u001b[0m    \u001b[0;34m**\u001b[0m\u001b[0mkwargs\u001b[0m\u001b[0;34m,\u001b[0m\u001b[0;34m\u001b[0m\n",
-                        "\u001b[0;34m\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
-                        "\u001b[0;31mDocstring:\u001b[0m\n",
-                        "Removes all electrodes for the specified nwb file and then\n",
-                        "adds back the electrodes in the list\n",
-                        "\n",
-                        "Parameters\n",
-                        "----------\n",
-                        "key : dict\n",
-                        "    dictionary corresponding to the LFPBand entry to use for\n",
-                        "    ripple detection\n",
-                        "electrode_list : list\n",
-                        "    list of electrodes from LFPBandSelection.LFPBandElectrode\n",
-                        "    to be used as the ripple LFP during detection\n",
-                        "group_name : str, optional\n",
-                        "    description of the electrode group, by default \"CA1\"\n",
-                        "\u001b[0;31mFile:\u001b[0m      ~/Documents/spyglass/src/spyglass/ripple/v1/ripple.py\n",
-                        "\u001b[0;31mType:\u001b[0m      function"
-                    ]
+                    "data": {
+                        "text/html": [
+                            "\n",
+                            "    \n",
+                            "    <style type=\"text/css\">\n",
+                            "        .Relation{\n",
+                            "            border-collapse:collapse;\n",
+                            "        }\n",
+                            "        .Relation th{\n",
+                            "            background: #A0A0A0; color: #ffffff; padding:4px; border:#f0e0e0 1px solid;\n",
+                            "            font-weight: normal; font-family: monospace; font-size: 100%;\n",
+                            "        }\n",
+                            "        .Relation td{\n",
+                            "            padding:4px; border:#f0e0e0 1px solid; font-size:100%;\n",
+                            "        }\n",
+                            "        .Relation tr:nth-child(odd){\n",
+                            "            background: #ffffff;\n",
+                            "        }\n",
+                            "        .Relation tr:nth-child(even){\n",
+                            "            background: #f3f1ff;\n",
+                            "        }\n",
+                            "        /* Tooltip container */\n",
+                            "        .djtooltip {\n",
+                            "        }\n",
+                            "        /* Tooltip text */\n",
+                            "        .djtooltip .djtooltiptext {\n",
+                            "            visibility: hidden;\n",
+                            "            width: 120px;\n",
+                            "            background-color: black;\n",
+                            "            color: #fff;\n",
+                            "            text-align: center;\n",
+                            "            padding: 5px 0;\n",
+                            "            border-radius: 6px;\n",
+                            "            /* Position the tooltip text - see examples below! */\n",
+                            "            position: absolute;\n",
+                            "            z-index: 1;\n",
+                            "        }\n",
+                            "        #primary {\n",
+                            "            font-weight: bold;\n",
+                            "            color: black;\n",
+                            "        }\n",
+                            "        #nonprimary {\n",
+                            "            font-weight: normal;\n",
+                            "            color: white;\n",
+                            "        }\n",
+                            "\n",
+                            "        /* Show the tooltip text when you mouse over the tooltip container */\n",
+                            "        .djtooltip:hover .djtooltiptext {\n",
+                            "            visibility: visible;\n",
+                            "        }\n",
+                            "    </style>\n",
+                            "    \n",
+                            "    <b></b>\n",
+                            "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
+                            "        <table border=\"1\" class=\"Relation\">\n",
+                            "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">mua_param_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">a name for this set of parameters</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">mua_param_dict</p>\n",
+                            "                            <span class=\"djtooltiptext\">dictionary of parameters</span>\n",
+                            "                        </div> </th> </tr> </thead>\n",
+                            "            <tbody> <tr> <td>default</td>\n",
+                            "<td>=BLOB=</td> </tr> </tbody>\n",
+                            "        </table>\n",
+                            "        \n",
+                            "        <p>Total: 1</p></div>\n",
+                            "        "
+                        ],
+                        "text/plain": [
+                            "*mua_param_nam mua_param_\n",
+                            "+------------+ +--------+\n",
+                            "default        =BLOB=    \n",
+                            " (Total: 1)"
+                        ]
+                    },
+                    "execution_count": 2,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "?sgr.RippleLFPSelection.set_lfp_electrodes"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "355190ce-a553-44d6-8260-7eda67f9407f",
-            "metadata": {},
-            "source": [
-                "We'll need the `nwb_file_name`, an `electrode_list`, and to a `group_name`.\n",
-                "\n",
-                "- By default, `group_name` is set to CA1 for ripple detection, but we could\n",
-                "  alternatively use PFC.\n",
-                "- We use `nwb_file_name` to explore which electrodes are available for the\n",
-                "  `electrode_list`.\n"
+                "MuaEventsParameters()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "5e29339b-3d2b-4fb4-a966-6166c6a40ab8",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "nwb_file_name = \"tonks20211103_.nwb\"\n",
-                "interval_list_name = \"test interval\"\n",
-                "filter_name = \"Ripple 150-250 Hz\"\n",
-                "if not sgc.Session & {\"nwb_file_name\": nwb_file_name}:\n",
-                "    # This error will be raised when notebooks auto-run with 'minirec'\n",
-                "    raise ValueError(f\"Session with nwb_file_name={nwb_file_name} not found\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "ac9c694f-06dd-47e8-9379-ec37397758f8",
-            "metadata": {},
-            "source": [
-                "Now we can look at `electrode_id` in the `Electrode` table:\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 10,
-            "id": "7c9f301d-7199-4c20-b008-38a1c16f1d04",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
                             "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
+                            "    \n",
+                            "    <style type=\"text/css\">\n",
+                            "        .Relation{\n",
+                            "            border-collapse:collapse;\n",
+                            "        }\n",
+                            "        .Relation th{\n",
+                            "            background: #A0A0A0; color: #ffffff; padding:4px; border:#f0e0e0 1px solid;\n",
+                            "            font-weight: normal; font-family: monospace; font-size: 100%;\n",
+                            "        }\n",
+                            "        .Relation td{\n",
+                            "            padding:4px; border:#f0e0e0 1px solid; font-size:100%;\n",
+                            "        }\n",
+                            "        .Relation tr:nth-child(odd){\n",
+                            "            background: #ffffff;\n",
+                            "        }\n",
+                            "        .Relation tr:nth-child(even){\n",
+                            "            background: #f3f1ff;\n",
+                            "        }\n",
+                            "        /* Tooltip container */\n",
+                            "        .djtooltip {\n",
+                            "        }\n",
+                            "        /* Tooltip text */\n",
+                            "        .djtooltip .djtooltiptext {\n",
+                            "            visibility: hidden;\n",
+                            "            width: 120px;\n",
+                            "            background-color: black;\n",
+                            "            color: #fff;\n",
+                            "            text-align: center;\n",
+                            "            padding: 5px 0;\n",
+                            "            border-radius: 6px;\n",
+                            "            /* Position the tooltip text - see examples below! */\n",
+                            "            position: absolute;\n",
+                            "            z-index: 1;\n",
+                            "        }\n",
+                            "        #primary {\n",
+                            "            font-weight: bold;\n",
+                            "            color: black;\n",
+                            "        }\n",
+                            "        #nonprimary {\n",
+                            "            font-weight: normal;\n",
+                            "            color: white;\n",
+                            "        }\n",
                             "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th>probe_id</th>\n",
-                            "      <th>probe_shank</th>\n",
-                            "      <th>probe_electrode</th>\n",
-                            "      <th>name</th>\n",
-                            "      <th>original_reference_electrode</th>\n",
-                            "      <th>x</th>\n",
-                            "      <th>y</th>\n",
-                            "      <th>z</th>\n",
-                            "      <th>filtering</th>\n",
-                            "      <th>impedance</th>\n",
-                            "      <th>bad_channel</th>\n",
-                            "      <th>x_warped</th>\n",
-                            "      <th>y_warped</th>\n",
-                            "      <th>z_warped</th>\n",
-                            "      <th>contacts</th>\n",
-                            "      <th>region_name</th>\n",
-                            "      <th>subregion_name</th>\n",
-                            "      <th>subsubregion_name</th>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>nwb_file_name</th>\n",
-                            "      <th>electrode_group_name</th>\n",
-                            "      <th>electrode_id</th>\n",
-                            "      <th>lfp_merge_id</th>\n",
-                            "      <th>filter_name</th>\n",
-                            "      <th>filter_sampling_rate</th>\n",
-                            "      <th>target_interval_list_name</th>\n",
-                            "      <th>lfp_band_sampling_rate</th>\n",
-                            "      <th>lfp_electrode_group_name</th>\n",
-                            "      <th>reference_elect_id</th>\n",
-                            "      <th>region_id</th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th rowspan=\"4\" valign=\"top\">tonks20211103_.nwb</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">7</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">28</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">2f3c93d5-5d5d-2d47-75b3-c346dddbd312</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">Ripple 150-250 Hz</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">1000</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">test interval</th>\n",
-                            "      <th>100</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>28</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1000</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>28</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">8</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">32</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">2f3c93d5-5d5d-2d47-75b3-c346dddbd312</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">Ripple 150-250 Hz</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">1000</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">test interval</th>\n",
-                            "      <th>100</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1000</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
+                            "        /* Show the tooltip text when you mouse over the tooltip container */\n",
+                            "        .djtooltip:hover .djtooltiptext {\n",
+                            "            visibility: visible;\n",
+                            "        }\n",
+                            "    </style>\n",
+                            "    \n",
+                            "    <b></b>\n",
+                            "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
+                            "        <table border=\"1\" class=\"Relation\">\n",
+                            "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">mua_param_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">a name for this set of parameters</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">nwb_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">unit_filter_params_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">sorted_spikes_group_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">pos_merge_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">detection_interval</p>\n",
+                            "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">analysis_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">mua_times_object_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div> </th> </tr> </thead>\n",
+                            "            <tbody> <tr> <td>default</td>\n",
+                            "<td>mediumnwb20230802_.nwb</td>\n",
+                            "<td>default_exclusion</td>\n",
+                            "<td>test_group</td>\n",
+                            "<td>4eb59a18-045a-5768-d12e-b6473415ae1c</td>\n",
+                            "<td>pos 0 valid times</td>\n",
+                            "<td>mediumnwb20230802_235KSEV39O.nwb</td>\n",
+                            "<td>a93532eb-2947-4552-8877-19ea0d2dcc4f</td> </tr> </tbody>\n",
+                            "        </table>\n",
+                            "        \n",
+                            "        <p>Total: 1</p></div>\n",
+                            "        "
                         ],
                         "text/plain": [
-                            "                                                                                                                                                                                                                                             probe_id  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                 \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        probe_shank  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id               \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        probe_electrode  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                   \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                      0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                      0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                      0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                      0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        name  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19          28   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19          28   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19          32   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19          32   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         original_reference_electrode  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                                 \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                                   44   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                                   44   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                                   44   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                                   44   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                           x  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                           y  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                           z  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        filtering  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19             None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19             None   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19             None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19             None   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         impedance  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id              \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19               0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19               0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19               0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19               0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        bad_channel  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id               \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              False   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              False   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              False   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              False   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         x_warped  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         y_warped  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         z_warped  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        contacts  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id            \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        region_name  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id               \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                ca1   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                ca1   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                ca1   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                ca1   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        subregion_name  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                  \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  None   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  None   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        subsubregion_name  \n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                    \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                     None  \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                     None  \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                     None  \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                     None  "
+                            "*mua_param_nam *nwb_file_name *unit_filter_p *sorted_spikes *pos_merge_id  *detection_int analysis_file_ mua_times_obje\n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "default        mediumnwb20230 default_exclus test_group     4eb59a18-045a- pos 0 valid ti mediumnwb20230 a93532eb-2947-\n",
+                            " (Total: 1)"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "electrodes = (\n",
-                "    (sgc.Electrode() & {\"nwb_file_name\": nwb_file_name})\n",
-                "    * (\n",
-                "        lfp_analysis.LFPBandSelection.LFPBandElectrode()\n",
-                "        & {\n",
-                "            \"nwb_file_name\": nwb_file_name,\n",
-                "            \"filter_name\": filter_name,\n",
-                "            \"target_interval_list_name\": interval_list_name,\n",
-                "        }\n",
-                "    )\n",
-                "    * sgc.BrainRegion\n",
-                ").fetch(format=\"frame\")\n",
-                "electrodes"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "c400f47e-a21b-451a-8721-35191161dc6e",
-            "metadata": {},
-            "source": [
-                "For ripple detection, we want only tetrodes, and only the first good wire on each tetrode. We will assume that is the first wire on each tetrode. I will do this using pandas syntax but you could use datajoint to filter this table as well. Here is the filtered table.\n"
+                "MuaEventsV1()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "83b9c019-a171-4d77-bccc-7c9945af1692",
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th>probe_id</th>\n",
-                            "      <th>probe_shank</th>\n",
-                            "      <th>probe_electrode</th>\n",
-                            "      <th>name</th>\n",
-                            "      <th>original_reference_electrode</th>\n",
-                            "      <th>x</th>\n",
-                            "      <th>y</th>\n",
-                            "      <th>z</th>\n",
-                            "      <th>filtering</th>\n",
-                            "      <th>impedance</th>\n",
-                            "      <th>bad_channel</th>\n",
-                            "      <th>x_warped</th>\n",
-                            "      <th>y_warped</th>\n",
-                            "      <th>z_warped</th>\n",
-                            "      <th>contacts</th>\n",
-                            "      <th>region_name</th>\n",
-                            "      <th>subregion_name</th>\n",
-                            "      <th>subsubregion_name</th>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>nwb_file_name</th>\n",
-                            "      <th>electrode_group_name</th>\n",
-                            "      <th>electrode_id</th>\n",
-                            "      <th>lfp_merge_id</th>\n",
-                            "      <th>filter_name</th>\n",
-                            "      <th>filter_sampling_rate</th>\n",
-                            "      <th>target_interval_list_name</th>\n",
-                            "      <th>lfp_band_sampling_rate</th>\n",
-                            "      <th>lfp_electrode_group_name</th>\n",
-                            "      <th>reference_elect_id</th>\n",
-                            "      <th>region_id</th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th rowspan=\"4\" valign=\"top\">tonks20211103_.nwb</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">7</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">28</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">2f3c93d5-5d5d-2d47-75b3-c346dddbd312</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">Ripple 150-250 Hz</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">1000</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">test interval</th>\n",
-                            "      <th>100</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>28</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1000</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>28</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">8</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">32</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">2f3c93d5-5d5d-2d47-75b3-c346dddbd312</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">Ripple 150-250 Hz</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">1000</th>\n",
-                            "      <th rowspan=\"2\" valign=\"top\">test interval</th>\n",
-                            "      <th>100</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1000</th>\n",
-                            "      <th>CA1_test</th>\n",
-                            "      <th>-1</th>\n",
-                            "      <th>19</th>\n",
-                            "      <td>tetrode_12.5</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>0</td>\n",
-                            "      <td>32</td>\n",
-                            "      <td>44</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>False</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td></td>\n",
-                            "      <td>ca1</td>\n",
-                            "      <td>None</td>\n",
-                            "      <td>None</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
                         "text/plain": [
-                            "                                                                                                                                                                                                                                             probe_id  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                 \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         tetrode_12.5   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        probe_shank  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id               \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        probe_electrode  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                   \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                      0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                      0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                      0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                      0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        name  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19          28   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19          28   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19          32   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19          32   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         original_reference_electrode  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                                 \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                                   44   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                                   44   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                                   44   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                                   44   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                           x  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                           y  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                           z  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id        \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19         0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19         0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        filtering  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19             None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19             None   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19             None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19             None   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         impedance  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id              \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19               0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19               0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19               0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19               0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        bad_channel  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id               \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              False   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              False   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              False   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              False   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         x_warped  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         y_warped  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                         z_warped  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id             \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19              0.0   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19              0.0   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        contacts  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id            \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        region_name  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id               \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                ca1   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                ca1   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                ca1   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                ca1   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        subregion_name  \\\n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                  \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  None   \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                  None   \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                  None   \n",
-                            "\n",
-                            "                                                                                                                                                                                                                                        subsubregion_name  \n",
-                            "nwb_file_name      electrode_group_name electrode_id lfp_merge_id                         filter_name       filter_sampling_rate target_interval_list_name lfp_band_sampling_rate lfp_electrode_group_name reference_elect_id region_id                    \n",
-                            "tonks20211103_.nwb 7                    28           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                     None  \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                     None  \n",
-                            "                   8                    32           2f3c93d5-5d5d-2d47-75b3-c346dddbd312 Ripple 150-250 Hz 1000                 test interval             100                    CA1_test                 -1                 19                     None  \n",
-                            "                                                                                                                                                           1000                   CA1_test                 -1                 19                     None  "
+                            "UUID('4eb59a18-045a-5768-d12e-b6473415ae1c')"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "hpc_names = [\"ca1\", \"hippocampus\", \"CA1\", \"Hippocampus\"]\n",
-                "electrodes.loc[\n",
-                "    (electrodes.region_name.isin(hpc_names)) & (electrodes.probe_electrode == 0)\n",
-                "]"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "007840a2-8b8b-4d56-9bf6-be5160aa41e6",
-            "metadata": {},
-            "source": [
-                "We only want the electrode_id to put in the `electrode_list`:\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "id": "0eba0656-c4dd-42bd-b18f-23aac13eb70a",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "electrode_list = np.unique(\n",
-                "    (\n",
-                "        electrodes.loc[\n",
-                "            (electrodes.region_name.isin(hpc_names))\n",
-                "            & (electrodes.probe_electrode == 0)\n",
-                "        ]\n",
-                "        .reset_index()\n",
-                "        .electrode_id\n",
-                "    ).tolist()\n",
-                ")\n",
+                "from spyglass.position import PositionOutput\n",
                 "\n",
-                "electrode_list.sort()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "14133ef0-06d0-4e1e-827b-882227d8bfe9",
-            "metadata": {},
-            "source": [
-                "By default, `set_lfp_electrodes` will use all the available electrodes from `LFPBandV1`.\n",
+                "nwb_copy_file_name = \"mediumnwb20230802_.nwb\"\n",
                 "\n",
-                "We can insert into `RippleLFPSelection` and the `RippleLFPElectrode` part table,\n",
-                "passing the key for the entry from `LFPBandV1`, our `electrode_list`, and the\n",
-                "`group_name` into `set_lfp_electrodes`\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
-            "id": "345709c2-2892-407d-ab2d-d3fd36f67d69",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "group_name = \"CA1_test\"\n",
-                "\n",
-                "lfp_band_key = (\n",
-                "    lfp_analysis.LFPBandV1()\n",
-                "    & {\n",
-                "        \"filter_name\": filter_name,\n",
-                "        \"nwb_file_name\": nwb_file_name,\n",
-                "        \"lfp_band_sampling_rate\": 1000,\n",
-                "    }\n",
-                ").fetch1(\"KEY\")\n",
+                "trodes_s_key = {\n",
+                "    \"nwb_file_name\": nwb_copy_file_name,\n",
+                "    \"interval_list_name\": \"pos 0 valid times\",\n",
+                "    \"trodes_pos_params_name\": \"single_led_upsampled\",\n",
+                "}\n",
                 "\n",
-                "sgr.RippleLFPSelection.set_lfp_electrodes(\n",
-                "    lfp_band_key,\n",
-                "    electrode_list=electrode_list,\n",
-                "    group_name=group_name,\n",
-                ")"
+                "pos_merge_id = (PositionOutput.TrodesPosV1 & trodes_s_key).fetch1(\"merge_id\")\n",
+                "pos_merge_id"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
-            "id": "96eb2aae-e93a-4214-a5e2-8c729767634b",
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
                             "    <style type=\"text/css\">\n",
-                            "        .Table{\n",
+                            "        .Relation{\n",
                             "            border-collapse:collapse;\n",
                             "        }\n",
-                            "        .Table th{\n",
+                            "        .Relation th{\n",
                             "            background: #A0A0A0; color: #ffffff; padding:4px; border:#f0e0e0 1px solid;\n",
                             "            font-weight: normal; font-family: monospace; font-size: 100%;\n",
                             "        }\n",
-                            "        .Table td{\n",
+                            "        .Relation td{\n",
                             "            padding:4px; border:#f0e0e0 1px solid; font-size:100%;\n",
                             "        }\n",
-                            "        .Table tr:nth-child(odd){\n",
+                            "        .Relation tr:nth-child(odd){\n",
                             "            background: #ffffff;\n",
-                            "            color: #000000;\n",
                             "        }\n",
-                            "        .Table tr:nth-child(even){\n",
+                            "        .Relation tr:nth-child(even){\n",
                             "            background: #f3f1ff;\n",
-                            "            color: #000000;\n",
                             "        }\n",
                             "        /* Tooltip container */\n",
                             "        .djtooltip {\n",
                             "        }\n",
                             "        /* Tooltip text */\n",
                             "        .djtooltip .djtooltiptext {\n",
                             "            visibility: hidden;\n",
@@ -1016,260 +318,85 @@
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
                             "    <b></b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
-                            "        <table border=\"1\" class=\"Table\">\n",
+                            "        <table border=\"1\" class=\"Relation\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">lfp_merge_id</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">filter_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">descriptive name of this filter</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">filter_sampling_rate</p>\n",
-                            "                            <span class=\"djtooltiptext\">sampling rate for this filter</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">nwb_file_name</p>\n",
                             "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">target_interval_list_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">lfp_band_sampling_rate</p>\n",
-                            "                            <span class=\"djtooltiptext\">the sampling rate for this band</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">group_name</p>\n",
+                            "                            <p id=\"primary\">unit_filter_params_name</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">lfp_electrode_group_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">the name of this group of electrodes</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">electrode_group_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">electrode group name from NWBFile</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">electrode_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">the unique number for this electrode</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">reference_elect_id</p>\n",
-                            "                            <span class=\"djtooltiptext\">the reference electrode to use; -1 for no reference</span>\n",
+                            "                            <p id=\"primary\">sorted_spikes_group_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>0</td>\n",
-                            "<td>0</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>1</td>\n",
-                            "<td>4</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>11</td>\n",
-                            "<td>44</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>12</td>\n",
-                            "<td>49</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>13</td>\n",
-                            "<td>52</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>14</td>\n",
-                            "<td>56</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>16</td>\n",
-                            "<td>64</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>17</td>\n",
-                            "<td>68</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>18</td>\n",
-                            "<td>72</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>19</td>\n",
-                            "<td>76</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>2</td>\n",
-                            "<td>8</td>\n",
-                            "<td>-1</td></tr><tr><td>0087e094-8238-32b8-9e8d-ecb7d9352b3b</td>\n",
-                            "<td>Ripple 150-250 Hz</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>Winnie20220714_.nwb</td>\n",
-                            "<td>pos 9 valid times</td>\n",
-                            "<td>1000</td>\n",
-                            "<td>CA1</td>\n",
-                            "<td>tetrode_sample_Winnie</td>\n",
-                            "<td>20</td>\n",
-                            "<td>80</td>\n",
-                            "<td>-1</td> </tr> </tbody>\n",
+                            "            <tbody> <tr> <td>mediumnwb20230802_.nwb</td>\n",
+                            "<td>default_exclusion</td>\n",
+                            "<td>test_group</td> </tr> </tbody>\n",
                             "        </table>\n",
-                            "        <p>...</p>\n",
-                            "        <p>Total: 60265</p></div>\n",
+                            "        \n",
+                            "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*lfp_merge_id  *filter_name   *filter_sampli *nwb_file_name *target_interv *lfp_band_samp *group_name    *lfp_electrode *electrode_gro *electrode_id  *reference_ele\n",
-                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 0              0              -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 1              4              -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 11             44             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 12             49             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 13             52             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 14             56             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 16             64             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 17             68             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 18             72             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 19             76             -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 2              8              -1            \n",
-                            "0087e094-8238- Ripple 150-250 1000           Winnie20220714 pos 9 valid ti 1000           CA1            tetrode_sample 20             80             -1            \n",
-                            "   ...\n",
-                            " (Total: 60265)"
+                            "*nwb_file_name *unit_filter_p *sorted_spikes\n",
+                            "+------------+ +------------+ +------------+\n",
+                            "mediumnwb20230 default_exclus test_group    \n",
+                            " (Total: 1)"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sgr.RippleLFPSelection.RippleLFPElectrode()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "0b27717a-d4a4-4293-9ea9-cf759b09039e",
-            "metadata": {},
-            "source": [
-                "Here's the ripple selection key we'll use downstream\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 13,
-            "id": "a601b1ac-0d37-4215-b9c6-5797bf21a1a0",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "rip_sel_key = (sgrip.RippleLFPSelection & lfp_band_key).fetch1(\"KEY\")"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "0874596d-f9dd-433f-9548-bb1c03bf1df1",
-            "metadata": {},
-            "source": [
-                "## Setting Ripple Parameters\n"
+                "from spyglass.spikesorting.analysis.v1.group import (\n",
+                "    SortedSpikesGroup,\n",
+                ")\n",
+                "\n",
+                "sorted_spikes_group_key = {\n",
+                "    \"nwb_file_name\": nwb_copy_file_name,\n",
+                "    \"sorted_spikes_group_name\": \"test_group\",\n",
+                "    \"unit_filter_params_name\": \"default_exclusion\",\n",
+                "}\n",
+                "\n",
+                "SortedSpikesGroup & sorted_spikes_group_key"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "id": "3ac90755-f6b0-434c-ab57-6177e064a5f3",
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
                             "    <style type=\"text/css\">\n",
-                            "        .Table{\n",
+                            "        .Relation{\n",
                             "            border-collapse:collapse;\n",
                             "        }\n",
-                            "        .Table th{\n",
+                            "        .Relation th{\n",
                             "            background: #A0A0A0; color: #ffffff; padding:4px; border:#f0e0e0 1px solid;\n",
                             "            font-weight: normal; font-family: monospace; font-size: 100%;\n",
                             "        }\n",
-                            "        .Table td{\n",
+                            "        .Relation td{\n",
                             "            padding:4px; border:#f0e0e0 1px solid; font-size:100%;\n",
                             "        }\n",
-                            "        .Table tr:nth-child(odd){\n",
+                            "        .Relation tr:nth-child(odd){\n",
                             "            background: #ffffff;\n",
-                            "            color: #000000;\n",
                             "        }\n",
-                            "        .Table tr:nth-child(even){\n",
+                            "        .Relation tr:nth-child(even){\n",
                             "            background: #f3f1ff;\n",
-                            "            color: #000000;\n",
                             "        }\n",
                             "        /* Tooltip container */\n",
                             "        .djtooltip {\n",
                             "        }\n",
                             "        /* Tooltip text */\n",
                             "        .djtooltip .djtooltiptext {\n",
                             "            visibility: hidden;\n",
@@ -1296,136 +423,83 @@
                             "        .djtooltip:hover .djtooltiptext {\n",
                             "            visibility: visible;\n",
                             "        }\n",
                             "    </style>\n",
                             "    \n",
                             "    <b></b>\n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
-                            "        <table border=\"1\" class=\"Table\">\n",
+                            "        <table border=\"1\" class=\"Relation\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">ripple_param_name</p>\n",
+                            "                            <p id=\"primary\">mua_param_name</p>\n",
                             "                            <span class=\"djtooltiptext\">a name for this set of parameters</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">ripple_param_dict</p>\n",
-                            "                            <span class=\"djtooltiptext\">dictionary of parameters</span>\n",
+                            "                            <p id=\"primary\">nwb_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">unit_filter_params_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">sorted_spikes_group_name</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">pos_merge_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">detection_interval</p>\n",
+                            "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">analysis_file_name</p>\n",
+                            "                            <span class=\"djtooltiptext\">name of the file</span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">mua_times_object_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
                             "            <tbody> <tr> <td>default</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>default_ms</td>\n",
-                            "<td>=BLOB=</td></tr><tr><td>default_sharon</td>\n",
-                            "<td>=BLOB=</td> </tr> </tbody>\n",
+                            "<td>mediumnwb20230802_.nwb</td>\n",
+                            "<td>default_exclusion</td>\n",
+                            "<td>test_group</td>\n",
+                            "<td>4eb59a18-045a-5768-d12e-b6473415ae1c</td>\n",
+                            "<td>pos 0 valid times</td>\n",
+                            "<td>mediumnwb20230802_235KSEV39O.nwb</td>\n",
+                            "<td>a93532eb-2947-4552-8877-19ea0d2dcc4f</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
-                            "        <p>Total: 3</p></div>\n",
+                            "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*ripple_param_ ripple_par\n",
-                            "+------------+ +--------+\n",
-                            "default        =BLOB=    \n",
-                            "default_ms     =BLOB=    \n",
-                            "default_sharon =BLOB=    \n",
-                            " (Total: 3)"
-                        ]
-                    },
-                    "execution_count": 14,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "sgr.RippleParameters()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "80e88984-0581-4f3d-88cf-164c24885569",
-            "metadata": {},
-            "source": [
-                "Here are the default ripple parameters:\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 15,
-            "id": "837a1c8d-87b6-42d9-9cfa-787ef63f7284",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "{'ripple_param_name': 'default',\n",
-                            " 'ripple_param_dict': {'speed_name': 'head_speed',\n",
-                            "  'ripple_detection_algorithm': 'Kay_ripple_detector',\n",
-                            "  'ripple_detection_params': {'speed_threshold': 4.0,\n",
-                            "   'minimum_duration': 0.015,\n",
-                            "   'zscore_threshold': 2.0,\n",
-                            "   'smoothing_sigma': 0.004,\n",
-                            "   'close_ripple_threshold': 0.0}}}"
+                            "*mua_param_nam *nwb_file_name *unit_filter_p *sorted_spikes *pos_merge_id  *detection_int analysis_file_ mua_times_obje\n",
+                            "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
+                            "default        mediumnwb20230 default_exclus test_group     4eb59a18-045a- pos 0 valid ti mediumnwb20230 a93532eb-2947-\n",
+                            " (Total: 1)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "(sgrip.RippleParameters() & {\"ripple_param_name\": \"default\"}).fetch1()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "9774f9f7-6efa-4880-b19b-92ae10d92bb7",
-            "metadata": {},
-            "source": [
-                "- `filter_name`: which bandpass filter is used\n",
-                "- `speed_name`: the name of the speed parameters in `IntervalPositionInfo`\n",
-                "\n",
-                "For the `Kay_ripple_detector` (options are currently Kay and Karlsson, see `ripple_detection` package for specifics) the parameters are:\n",
-                "\n",
-                "- `speed_threshold` (cm/s): maximum speed the animal can move\n",
-                "- `minimum_duration` (s): minimum time above threshold\n",
-                "- `zscore_threshold` (std): minimum value to be considered a ripple, in standard\n",
-                "  deviations from mean\n",
-                "- `smoothing_sigma` (s): how much to smooth the signal in time\n",
-                "- `close_ripple_threshold` (s): exclude ripples closer than this amount\n"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "8adbbba5-78e2-41a0-9ba0-d06aa5cfd055",
-            "metadata": {},
-            "source": [
-                "## Check interval speed\n",
+                "mua_key = {\n",
+                "    \"mua_param_name\": \"default\",\n",
+                "    **sorted_spikes_group_key,\n",
+                "    \"pos_merge_id\": pos_merge_id,\n",
+                "    \"detection_interval\": \"pos 0 valid times\",\n",
+                "}\n",
                 "\n",
-                "The speed for this interval should exist under the default position parameter\n",
-                "set and for a given interval.\n"
+                "MuaEventsV1().populate(mua_key)\n",
+                "MuaEventsV1 & mua_key"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
-            "id": "cc3c95f0-3fd0-440c-93f9-338f01a1d893",
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.5.1 because version 1.6.0 is already loaded.\n",
-                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.4.0 because version 2.6.0-alpha is already loaded.\n",
-                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.2.0 because version 0.3.0 is already loaded.\n",
-                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
@@ -1438,622 +512,428 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>head_position_x</th>\n",
-                            "      <th>head_position_y</th>\n",
-                            "      <th>head_orientation</th>\n",
-                            "      <th>head_velocity_x</th>\n",
-                            "      <th>head_velocity_y</th>\n",
-                            "      <th>head_speed</th>\n",
+                            "      <th>start_time</th>\n",
+                            "      <th>end_time</th>\n",
+                            "      <th>duration</th>\n",
+                            "      <th>mean_zscore</th>\n",
+                            "      <th>median_zscore</th>\n",
+                            "      <th>max_zscore</th>\n",
+                            "      <th>min_zscore</th>\n",
+                            "      <th>speed_at_start</th>\n",
+                            "      <th>speed_at_end</th>\n",
+                            "      <th>max_speed</th>\n",
+                            "      <th>min_speed</th>\n",
+                            "      <th>median_speed</th>\n",
+                            "      <th>mean_speed</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>time</th>\n",
+                            "      <th>id</th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>1.635961e+09</th>\n",
-                            "      <td>98.670000</td>\n",
-                            "      <td>78.320000</td>\n",
-                            "      <td>1.878849</td>\n",
-                            "      <td>-0.212384</td>\n",
-                            "      <td>-1.050933e+00</td>\n",
-                            "      <td>1.072179</td>\n",
+                            "      <th>0</th>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>0.238</td>\n",
+                            "      <td>1.204139</td>\n",
+                            "      <td>1.220925</td>\n",
+                            "      <td>2.258331</td>\n",
+                            "      <td>0.028349</td>\n",
+                            "      <td>2.760825</td>\n",
+                            "      <td>1.517296</td>\n",
+                            "      <td>3.576624</td>\n",
+                            "      <td>1.427160</td>\n",
+                            "      <td>2.851154</td>\n",
+                            "      <td>2.616020</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1.635961e+09</th>\n",
-                            "      <td>98.615000</td>\n",
-                            "      <td>78.210000</td>\n",
-                            "      <td>1.899349</td>\n",
-                            "      <td>-0.143244</td>\n",
-                            "      <td>-1.136351e+00</td>\n",
-                            "      <td>1.145344</td>\n",
+                            "      <th>1</th>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>0.120</td>\n",
+                            "      <td>1.364368</td>\n",
+                            "      <td>1.349665</td>\n",
+                            "      <td>2.412096</td>\n",
+                            "      <td>0.015503</td>\n",
+                            "      <td>1.803533</td>\n",
+                            "      <td>0.497099</td>\n",
+                            "      <td>1.803533</td>\n",
+                            "      <td>0.464203</td>\n",
+                            "      <td>0.553494</td>\n",
+                            "      <td>0.722099</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1.635961e+09</th>\n",
-                            "      <td>98.633333</td>\n",
-                            "      <td>78.173333</td>\n",
-                            "      <td>1.919567</td>\n",
-                            "      <td>-0.031501</td>\n",
-                            "      <td>-1.123425e+00</td>\n",
-                            "      <td>1.123867</td>\n",
+                            "      <th>2</th>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>0.082</td>\n",
+                            "      <td>1.350428</td>\n",
+                            "      <td>1.490812</td>\n",
+                            "      <td>2.229001</td>\n",
+                            "      <td>0.016666</td>\n",
+                            "      <td>0.639882</td>\n",
+                            "      <td>0.830598</td>\n",
+                            "      <td>0.838116</td>\n",
+                            "      <td>0.639882</td>\n",
+                            "      <td>0.791716</td>\n",
+                            "      <td>0.772154</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1.635961e+09</th>\n",
-                            "      <td>98.596667</td>\n",
-                            "      <td>78.100000</td>\n",
-                            "      <td>1.932884</td>\n",
-                            "      <td>0.094982</td>\n",
-                            "      <td>-1.013202e+00</td>\n",
-                            "      <td>1.017644</td>\n",
+                            "      <th>3</th>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>0.074</td>\n",
+                            "      <td>1.609420</td>\n",
+                            "      <td>1.803123</td>\n",
+                            "      <td>2.578417</td>\n",
+                            "      <td>0.013637</td>\n",
+                            "      <td>2.690052</td>\n",
+                            "      <td>0.684351</td>\n",
+                            "      <td>2.690052</td>\n",
+                            "      <td>0.684351</td>\n",
+                            "      <td>1.327693</td>\n",
+                            "      <td>1.451886</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1.635961e+09</th>\n",
-                            "      <td>98.633333</td>\n",
-                            "      <td>78.100000</td>\n",
-                            "      <td>1.946067</td>\n",
-                            "      <td>0.194273</td>\n",
-                            "      <td>-8.272934e-01</td>\n",
-                            "      <td>0.849798</td>\n",
+                            "      <th>4</th>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>1.625936e+09</td>\n",
+                            "      <td>0.208</td>\n",
+                            "      <td>1.459232</td>\n",
+                            "      <td>1.441996</td>\n",
+                            "      <td>2.610289</td>\n",
+                            "      <td>0.040791</td>\n",
+                            "      <td>0.208621</td>\n",
+                            "      <td>1.136773</td>\n",
+                            "      <td>1.298535</td>\n",
+                            "      <td>0.162133</td>\n",
+                            "      <td>1.088990</td>\n",
+                            "      <td>0.935486</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1.635963e+09</th>\n",
-                            "      <td>96.323333</td>\n",
-                            "      <td>71.500000</td>\n",
-                            "      <td>-2.265535</td>\n",
-                            "      <td>-0.415082</td>\n",
-                            "      <td>-1.486577e-05</td>\n",
-                            "      <td>0.415082</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1.635963e+09</th>\n",
-                            "      <td>96.286667</td>\n",
-                            "      <td>71.500000</td>\n",
-                            "      <td>-2.158799</td>\n",
-                            "      <td>-0.413708</td>\n",
-                            "      <td>-3.243187e-06</td>\n",
-                            "      <td>0.413708</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1.635963e+09</th>\n",
-                            "      <td>96.250000</td>\n",
-                            "      <td>71.500000</td>\n",
-                            "      <td>-2.034444</td>\n",
-                            "      <td>-0.374655</td>\n",
-                            "      <td>-6.383825e-07</td>\n",
-                            "      <td>0.374655</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1.635963e+09</th>\n",
-                            "      <td>96.250000</td>\n",
-                            "      <td>71.500000</td>\n",
-                            "      <td>-2.034444</td>\n",
-                            "      <td>-0.307793</td>\n",
-                            "      <td>-1.133319e-07</td>\n",
-                            "      <td>0.307793</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1.635963e+09</th>\n",
-                            "      <td>96.250000</td>\n",
-                            "      <td>71.500000</td>\n",
-                            "      <td>-2.034444</td>\n",
-                            "      <td>-0.229237</td>\n",
-                            "      <td>-1.813955e-08</td>\n",
-                            "      <td>0.229237</td>\n",
+                            "      <th>160</th>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>0.212</td>\n",
+                            "      <td>3.099559</td>\n",
+                            "      <td>3.296528</td>\n",
+                            "      <td>5.312823</td>\n",
+                            "      <td>0.013042</td>\n",
+                            "      <td>1.183369</td>\n",
+                            "      <td>0.500407</td>\n",
+                            "      <td>1.183369</td>\n",
+                            "      <td>0.386452</td>\n",
+                            "      <td>0.827476</td>\n",
+                            "      <td>0.791367</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>161</th>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>0.406</td>\n",
+                            "      <td>2.234536</td>\n",
+                            "      <td>2.555549</td>\n",
+                            "      <td>4.133360</td>\n",
+                            "      <td>0.013230</td>\n",
+                            "      <td>0.483370</td>\n",
+                            "      <td>0.415434</td>\n",
+                            "      <td>0.967244</td>\n",
+                            "      <td>0.170981</td>\n",
+                            "      <td>0.615845</td>\n",
+                            "      <td>0.603776</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>162</th>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>0.106</td>\n",
+                            "      <td>1.272785</td>\n",
+                            "      <td>1.090846</td>\n",
+                            "      <td>2.567647</td>\n",
+                            "      <td>0.029594</td>\n",
+                            "      <td>1.173970</td>\n",
+                            "      <td>1.531232</td>\n",
+                            "      <td>1.586072</td>\n",
+                            "      <td>1.173970</td>\n",
+                            "      <td>1.533011</td>\n",
+                            "      <td>1.472277</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>163</th>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>0.130</td>\n",
+                            "      <td>2.206783</td>\n",
+                            "      <td>2.288842</td>\n",
+                            "      <td>3.916084</td>\n",
+                            "      <td>0.000061</td>\n",
+                            "      <td>1.843658</td>\n",
+                            "      <td>2.197606</td>\n",
+                            "      <td>2.263417</td>\n",
+                            "      <td>1.843658</td>\n",
+                            "      <td>2.212691</td>\n",
+                            "      <td>2.156476</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>164</th>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>1.625937e+09</td>\n",
+                            "      <td>0.088</td>\n",
+                            "      <td>1.682973</td>\n",
+                            "      <td>1.689252</td>\n",
+                            "      <td>3.048358</td>\n",
+                            "      <td>0.021588</td>\n",
+                            "      <td>1.288769</td>\n",
+                            "      <td>1.058330</td>\n",
+                            "      <td>1.334759</td>\n",
+                            "      <td>1.058330</td>\n",
+                            "      <td>1.296841</td>\n",
+                            "      <td>1.260912</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>48950 rows \u00d7 6 columns</p>\n",
+                            "<p>165 rows \u00d7 13 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "              head_position_x  head_position_y  head_orientation  \\\n",
-                            "time                                                               \n",
-                            "1.635961e+09        98.670000        78.320000          1.878849   \n",
-                            "1.635961e+09        98.615000        78.210000          1.899349   \n",
-                            "1.635961e+09        98.633333        78.173333          1.919567   \n",
-                            "1.635961e+09        98.596667        78.100000          1.932884   \n",
-                            "1.635961e+09        98.633333        78.100000          1.946067   \n",
-                            "...                       ...              ...               ...   \n",
-                            "1.635963e+09        96.323333        71.500000         -2.265535   \n",
-                            "1.635963e+09        96.286667        71.500000         -2.158799   \n",
-                            "1.635963e+09        96.250000        71.500000         -2.034444   \n",
-                            "1.635963e+09        96.250000        71.500000         -2.034444   \n",
-                            "1.635963e+09        96.250000        71.500000         -2.034444   \n",
-                            "\n",
-                            "              head_velocity_x  head_velocity_y  head_speed  \n",
-                            "time                                                        \n",
-                            "1.635961e+09        -0.212384    -1.050933e+00    1.072179  \n",
-                            "1.635961e+09        -0.143244    -1.136351e+00    1.145344  \n",
-                            "1.635961e+09        -0.031501    -1.123425e+00    1.123867  \n",
-                            "1.635961e+09         0.094982    -1.013202e+00    1.017644  \n",
-                            "1.635961e+09         0.194273    -8.272934e-01    0.849798  \n",
-                            "...                       ...              ...         ...  \n",
-                            "1.635963e+09        -0.415082    -1.486577e-05    0.415082  \n",
-                            "1.635963e+09        -0.413708    -3.243187e-06    0.413708  \n",
-                            "1.635963e+09        -0.374655    -6.383825e-07    0.374655  \n",
-                            "1.635963e+09        -0.307793    -1.133319e-07    0.307793  \n",
-                            "1.635963e+09        -0.229237    -1.813955e-08    0.229237  \n",
+                            "       start_time      end_time  duration  mean_zscore  median_zscore  \\\n",
+                            "id                                                                      \n",
+                            "0    1.625936e+09  1.625936e+09     0.238     1.204139       1.220925   \n",
+                            "1    1.625936e+09  1.625936e+09     0.120     1.364368       1.349665   \n",
+                            "2    1.625936e+09  1.625936e+09     0.082     1.350428       1.490812   \n",
+                            "3    1.625936e+09  1.625936e+09     0.074     1.609420       1.803123   \n",
+                            "4    1.625936e+09  1.625936e+09     0.208     1.459232       1.441996   \n",
+                            "..            ...           ...       ...          ...            ...   \n",
+                            "160  1.625937e+09  1.625937e+09     0.212     3.099559       3.296528   \n",
+                            "161  1.625937e+09  1.625937e+09     0.406     2.234536       2.555549   \n",
+                            "162  1.625937e+09  1.625937e+09     0.106     1.272785       1.090846   \n",
+                            "163  1.625937e+09  1.625937e+09     0.130     2.206783       2.288842   \n",
+                            "164  1.625937e+09  1.625937e+09     0.088     1.682973       1.689252   \n",
+                            "\n",
+                            "     max_zscore  min_zscore  speed_at_start  speed_at_end  max_speed  \\\n",
+                            "id                                                                     \n",
+                            "0      2.258331    0.028349        2.760825      1.517296   3.576624   \n",
+                            "1      2.412096    0.015503        1.803533      0.497099   1.803533   \n",
+                            "2      2.229001    0.016666        0.639882      0.830598   0.838116   \n",
+                            "3      2.578417    0.013637        2.690052      0.684351   2.690052   \n",
+                            "4      2.610289    0.040791        0.208621      1.136773   1.298535   \n",
+                            "..          ...         ...             ...           ...        ...   \n",
+                            "160    5.312823    0.013042        1.183369      0.500407   1.183369   \n",
+                            "161    4.133360    0.013230        0.483370      0.415434   0.967244   \n",
+                            "162    2.567647    0.029594        1.173970      1.531232   1.586072   \n",
+                            "163    3.916084    0.000061        1.843658      2.197606   2.263417   \n",
+                            "164    3.048358    0.021588        1.288769      1.058330   1.334759   \n",
+                            "\n",
+                            "     min_speed  median_speed  mean_speed  \n",
+                            "id                                        \n",
+                            "0     1.427160      2.851154    2.616020  \n",
+                            "1     0.464203      0.553494    0.722099  \n",
+                            "2     0.639882      0.791716    0.772154  \n",
+                            "3     0.684351      1.327693    1.451886  \n",
+                            "4     0.162133      1.088990    0.935486  \n",
+                            "..         ...           ...         ...  \n",
+                            "160   0.386452      0.827476    0.791367  \n",
+                            "161   0.170981      0.615845    0.603776  \n",
+                            "162   1.173970      1.533011    1.472277  \n",
+                            "163   1.843658      2.212691    2.156476  \n",
+                            "164   1.058330      1.296841    1.260912  \n",
                             "\n",
-                            "[48950 rows x 6 columns]"
+                            "[165 rows x 13 columns]"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "pos_key = sgp.PositionOutput.merge_get_part(\n",
-                "    {\n",
-                "        \"nwb_file_name\": nwb_file_name,\n",
-                "        \"position_info_param_name\": \"default\",\n",
-                "        \"interval_list_name\": \"pos 1 valid times\",\n",
-                "    }\n",
-                ").fetch1(\"KEY\")\n",
-                "(sgp.PositionOutput & pos_key).fetch1_dataframe()"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "1bc905e6-211a-4292-9f13-dfff906479a0",
-            "metadata": {},
-            "source": [
-                "We'll use the `head_speed` above as part of `RippleParameters`.\n"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "674d6896-8a93-4a51-ad45-f5a4218f007e",
-            "metadata": {},
-            "source": [
-                "## Run Ripple Detection\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "a5c3f1b4",
-            "metadata": {},
-            "source": [
-                "Now we can put everything together.\n"
+                "mua_times = (MuaEventsV1 & mua_key).fetch1_dataframe()\n",
+                "mua_times"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
-            "id": "8ddee771-470f-44e4-b0ac-1d2eef60f66d",
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[10:01:12][INFO] Spyglass: Computing ripple times for: {'lfp_merge_id': UUID('2f3c93d5-5d5d-2d47-75b3-c346dddbd312'), 'filter_name': 'Ripple 150-250 Hz', 'filter_sampling_rate': 1000, 'nwb_file_name': 'tonks20211103_.nwb', 'target_interval_list_name': 'test interval', 'lfp_band_sampling_rate': 1000, 'group_name': 'CA1_test', 'ripple_param_name': 'default', 'pos_merge_id': UUID('68959dc8-f8a3-c3c0-a534-096b3bc10f6c')}\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.5.1 because version 1.6.0 is already loaded.\n",
+                        "[14:44:19][WARNING] Spyglass: Upsampled position data, frame indices are invalid. Setting add_frame_ind=False\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.6.0 because version 1.5.1 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.6.0-alpha because version 2.5.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.3.0 because version 0.2.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.6.0 because version 1.5.1 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.6.0-alpha because version 2.5.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.3.0 because version 0.2.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.6.0 because version 1.5.1 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.6.0-alpha because version 2.5.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.3.0 because version 0.2.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.6.0 because version 1.5.1 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.6.0-alpha because version 2.5.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.3.0 because version 0.2.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.6.0 because version 1.5.1 is already loaded.\n",
                         "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.4.0 because version 2.6.0-alpha is already loaded.\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.6.0-alpha because version 2.5.0 is already loaded.\n",
                         "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.2.0 because version 0.3.0 is already loaded.\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.3.0 because version 0.2.0 is already loaded.\n",
                         "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/behavior.py:46: UserWarning: SpatialSeries 'series_0' has data shape (66792, 4) which is not compliant with NWB 2.5 and greater. The second dimension should have length <= 3 to represent at most x, y, z.\n",
-                        "  warnings.warn(\"SpatialSeries '%s' has data shape %s which is not compliant with NWB 2.5 and greater. \"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/behavior.py:46: UserWarning: SpatialSeries 'series_1' has data shape (48950, 4) which is not compliant with NWB 2.5 and greater. The second dimension should have length <= 3 to represent at most x, y, z.\n",
-                        "  warnings.warn(\"SpatialSeries '%s' has data shape %s which is not compliant with NWB 2.5 and greater. \"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/behavior.py:46: UserWarning: SpatialSeries 'series_2' has data shape (98507, 4) which is not compliant with NWB 2.5 and greater. The second dimension should have length <= 3 to represent at most x, y, z.\n",
-                        "  warnings.warn(\"SpatialSeries '%s' has data shape %s which is not compliant with NWB 2.5 and greater. \"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/behavior.py:46: UserWarning: SpatialSeries 'series_3' has data shape (44892, 4) which is not compliant with NWB 2.5 and greater. The second dimension should have length <= 3 to represent at most x, y, z.\n",
-                        "  warnings.warn(\"SpatialSeries '%s' has data shape %s which is not compliant with NWB 2.5 and greater. \"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/behavior.py:46: UserWarning: SpatialSeries 'series_4' has data shape (82313, 4) which is not compliant with NWB 2.5 and greater. The second dimension should have length <= 3 to represent at most x, y, z.\n",
-                        "  warnings.warn(\"SpatialSeries '%s' has data shape %s which is not compliant with NWB 2.5 and greater. \"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/behavior.py:46: UserWarning: SpatialSeries 'series_5' has data shape (81566, 4) which is not compliant with NWB 2.5 and greater. The second dimension should have length <= 3 to represent at most x, y, z.\n",
-                        "  warnings.warn(\"SpatialSeries '%s' has data shape %s which is not compliant with NWB 2.5 and greater. \"\n",
-                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/behavior.py:46: UserWarning: SpatialSeries 'series_6' has data shape (83811, 4) which is not compliant with NWB 2.5 and greater. The second dimension should have length <= 3 to represent at most x, y, z.\n",
-                        "  warnings.warn(\"SpatialSeries '%s' has data shape %s which is not compliant with NWB 2.5 and greater. \"\n",
-                        "[10:01:14][INFO] Spyglass: Writing new NWB file tonks20211103_41QOWS4VUO.nwb\n"
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.6.0 because version 1.5.1 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.6.0-alpha because version 2.5.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.3.0 because version 0.2.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-common' version 1.6.0 because version 1.5.1 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'core' version 2.6.0-alpha because version 2.5.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "/home/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/hdmf/spec/namespace.py:531: UserWarning: Ignoring cached namespace 'hdmf-experimental' version 0.3.0 because version 0.2.0 is already loaded.\n",
+                        "  warn(\"Ignoring cached namespace '%s' version %s because version %s is already loaded.\"\n",
+                        "[14:44:24][WARNING] Spyglass: Upsampled position data, frame indices are invalid. Setting add_frame_ind=False\n"
                     ]
+                },
+                {
+                    "data": {
+                        "image/png": "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snT33XcrKyvL6lCAfqEPI5XRf5HK6L9IZfRfpDL67+DHggsAAAAAAABAglD5BgAAAAAAACQIyTcAAAAAAAAgQUi+AQAAAAAAAAlC8g0AAAAAAABIEJJvQAqrqanRwoULNXLkSOXm5urkk0/W1q1bY6+3t7frlltu0bhx45STk6Njjz1Wa9eutTBiYL+ysjLZbLYu/26++WZJkmmaWrlypUpLS5WTk6M5c+Zo+/btFkcN7NdT/w2FQrrjjjt0wgknKC8vT6WlpbruuutUW1trddiApMN//h7ohhtukM1m08MPPzzwgQLd6E3//eqrr3TJJZfI4XCooKBAp59+uiorKy2MGviXw/Vh7t8GrwyrAwDQP06nU7Nnz9bcuXP1xhtvqKioSHv27NGwYcNi+yxZskSbNm3SM888o7KyMm3cuFE33XSTSktLdemll1oXPIa8Tz75RJFIJPb1F198oXnz5umKK66QJD344INas2aNnnzySU2dOlX33Xef5s2bpx07dqigoMCqsAFJPfdfr9erbdu26a677tJJJ50kp9OpxYsX65JLLtGnn35qYdTAfof7/I3asGGD/vrXv6q0tHSgQwQO6XD9d8+ePTrzzDP13e9+V/fcc48cDoe++uorZWdnWxUy0Mnh+jD3b4OXzTRN0+ogAPTdihUr9NFHH+mDDz445D7HH3+8rrrqKt11112xbaeccoouuugi/fSnPx2IMIFeWbx4sV577TXt2rVLklRaWqrFixfrjjvukCQFAgEVFxfrgQce0A033GBlqEAXB/Zfm83W5fVPPvlEX//611VRUaGjjjrKggiBQ+uu/9bU1GjmzJl66623dPHFF2vx4sVavHixtYEC3Ti4/1599dXKzMzU7373O6tDA3rl4D7M/dvgxbBTIEW98sorOvXUU3XFFVeoqKhIM2bM0BNPPNFpnzPPPFOvvPKKampqZJqmNm3apJ07d+r888+3KGqgq2AwqGeeeUb/83/+T9lsNu3bt0/19fU677zzYvtkZWXp7LPP1scff2xhpEBXB/ff7rhcLtlstk6VyUAy6K7/Goaha6+9VrfffruOO+44iyMEDu3g/msYhv785z9r6tSpOv/881VUVKSZM2dqw4YNVocKdKu7z2Du3wYvkm9Aitq7d6/Wrl2rKVOm6K233tKNN96oW2+9VU8//XRsn0ceeUTTp0/XuHHjZLfbdcEFF+jRRx/VmWeeaWHkQGcbNmxQW1ubFi1aJEmqr6+XJBUXF3far7i4OPYakCwO7r8H8/v9WrFihRYsWKDCwsKBDQ44jO767wMPPKCMjAzdeuut1gUG9MLB/bexsVHt7e36+c9/rgsuuEAbN27UZZddpvnz52vz5s3WBgt0o7vPYO7fBi/mfANSlGEYOvXUU7Vq1SpJ0owZM7R9+3atXbtW1113naT9H95/+ctf9Morr2jChAl6//33ddNNN2nMmDE699xzrQwfiPnP//xPXXjhhV3mFTq4isg0zUNWFgFWOVT/laRQKKSrr75ahmHo0UcftSA6oGcH99+tW7fqF7/4hbZt28bnLZLewf3XMAxJ0qWXXqolS5ZIkk4++WR9/PHHeuyxx3T22WdbFivQne6uIbh/G7xIvgEpasyYMZo+fXqnbccee6xefPFFSZLP59OPf/xjvfzyy7r44oslSSeeeKI+//xz/cd//Acf3kgKFRUVeuedd/TSSy/FtpWUlEjaXwE3ZsyY2PbGxsYu1XCAlbrrv1GhUEhXXnml9u3bp3fffZeqNySd7vrvBx98oMbGxk5zE0YiEd122216+OGHVV5ebkGkQFfd9d9Ro0YpIyOj2+vjDz/8cKBDBHrUXR/m/m1wY9gpkKJmz56tHTt2dNq2c+dOTZgwQdL+G79QKKS0tM6/5unp6bEng4DV1q9fr6KiotgFhiRNnDhRJSUlevvtt2PbgsGgNm/erFmzZlkRJtCt7vqv9K/E265du/TOO+9o5MiRFkUIHFp3/ffaa6/V3//+d33++eexf6Wlpbr99tv11ltvWRgt0Fl3/ddut+u0007r8foYSBbd9WHu3wY3Kt+AFLVkyRLNmjVLq1at0pVXXqktW7Zo3bp1WrdunSSpsLBQZ599tm6//Xbl5ORowoQJ2rx5s55++mmtWbPG4uiB/cND1q9fr+985zvKyPjXnyObzabFixdr1apVmjJliqZMmaJVq1YpNzdXCxYssDBi4F8O1X/D4bAuv/xybdu2Ta+99poikUhsrsIRI0bIbrdbFTIQc6j+O3LkyC7J4szMTJWUlOiYY44Z6DCBbh2q/0rS7bffrquuukpnnXWW5s6dqzfffFOvvvqq3nvvPWuCBbpxqD7M/dsgZwJIWa+++qp5/PHHm1lZWea0adPMdevWdXq9rq7OXLRokVlaWmpmZ2ebxxxzjPnQQw+ZhmFYFDHwL2+99ZYpydyxY0eX1wzDMO+++26zpKTEzMrKMs866yzzH//4hwVRAt07VP/dt2+fKanbf5s2bbImWOAgPX3+HmzChAnm//2//zfxQQG9dLj++5//+Z/m5MmTzezsbPOkk04yN2zYMMARAj3rqQ9z/zZ42UzTNC3K+wEAAAAAAACDGnO+AQAAAAAAAAlC8g0AAAAAAABIEJJvAAAAAAAAQIKQfAMAAAAAAAAShOQbAAAAAAAAkCAk3wAAAAAAAIAEIfkGAAAAAAAAJAjJNwAAAAAAgEFg3bp1mjNnjgoLC2Wz2dTW1tar42pqarRw4UKNHDlSubm5Ovnkk7V161ZJUigU0h133KETTjhBeXl5Ki0t1XXXXafa2tpObcyZM0c2m63Tv6uvvrrTPtu2bdO8efM0bNgwjRw5Uj/4wQ/U3t4ee72lpUUXXHCBSktLlZWVpfHjx+uWW26R2+2O7VNeXt7lPDabTW+++Wanc/3617/Wscceq5ycHB1zzDF6+umn+/Kt7FW8vUXyDQAAYBB77733+nTxHW/vvvuupk2bJsMwDrvva6+9phkzZvRqXwAAhqo5c+boySef7PY1r9erCy64QD/+8Y973Z7T6dTs2bOVmZmpN954Q19++aUeeughDRs2LNbmtm3bdNddd2nbtm166aWXtHPnTl1yySVd2vr+97+vurq62L/HH3889lptba3OPfdcTZ48WX/961/15ptvavv27Vq0aFFsn7S0NF166aV65ZVXtHPnTj355JN65513dOONN3Y51zvvvNPpXP/2b/8We23t2rW68847tXLlSm3fvl333HOPbr75Zr366qu9/r70Jt7espmmafb5KAAAACSdOXPm6OSTT9bDDz8c2xYMBtXa2qri4mLZbLYBj+nUU0/Vj370I1177bW92v9rX/uali5dqoULFyY4MgAAUtOcOXO0aNGiHpNA7733nubOnSun0xlLoh3KihUr9NFHH+mDDz7odQyffPKJvv71r6uiokJHHXVULK6Dr0MOtG7dOt11112qq6tTWtr+WrDPP/9cM2bM0K5duzR58uRuj3vkkUe0evVqVVVVSdpf+TZx4kR99tlnOvnkk7s9ZtasWZo9e7ZWr14d27Z48WJ9+umn+vDDD2Pb1q9frwcffFD79u1TWVmZbr31Vt10001HFG93qHwDAAAYxOx2u0pKSixJvH388cfatWuXrrjiil4fc/311+uXv/xlAqMCAAAHeuWVV3TqqafqiiuuUFFRkWbMmKEnnniix2NcLpdsNluXxN7vf/97jRo1Sscdd5yWLVsmj8cTey0QCMhut8cSWZKUk5MjSZ0SYgeqra3VSy+9pLPPPrvLa5dccomKioo0e/ZsvfDCC51eCwQCys7O7rQtJydHW7ZsUSgUkiQ98cQT+slPfqKf/exn+uqrr7Rq1Srdddddeuqpp/od76GQfAMAABgEFi1apM2bN+sXv/hFbO6T8vLyLsNOn3zySQ0bNkyvvfaajjnmGOXm5uryyy9XR0eHnnrqKZWVlWn48OH64Q9/qEgkEms/GAxq+fLlGjt2rPLy8jRz5ky99957Pcb03HPP6bzzzut08fu3v/1Nc+fOVUFBgQoLC3XKKafo008/jb1+ySWXaMuWLdq7d29cvz8AAKB7e/fu1dq1azVlyhS99dZbuvHGG3Xrrbceco40v9+vFStWaMGCBSosLIxtv+aaa/Tss8/qvffe01133aUXX3xR8+fPj73+b//2b6qvr9fq1asVDAbldDpjw2Pr6uo6nePb3/62cnNzNXbsWBUWFuo3v/lN7LX8/HytWbNGL7zwgl5//XWdc845uuqqq/TMM8/E9jn//PP1m9/8Rlu3bpVpmvr000/129/+VqFQSM3NzZKkn/70p3rooYc0f/58TZw4UfPnz9eSJUtiQ2X7Eu9hmQAAAEh5bW1t5hlnnGF+//vfN+vq6sy6ujozHA6bmzZtMiWZTqfTNE3TXL9+vZmZmWnOmzfP3LZtm7l582Zz5MiR5nnnnWdeeeWV5vbt281XX33VtNvt5nPPPRdrf8GCBeasWbPM999/39y9e7e5evVqMysry9y5c+chYzrppJPMn//85522HXfccebChQvNr776yty5c6f5/PPPm59//nmnfYqKiswnn3wyft8cAABS2M9+9jMzLy8v9i8tLc3MysrqtO3999/vdMzBf/97kpmZaZ5xxhmdtv3whz80Tz/99C77BoNB89JLLzVnzJhhulyuHtv99NNPTUnm1q1bY9t+//vfm8XFxWZ6erppt9vNZcuWmcXFxeYDDzzQ6di6ujrzq6++Mjds2GBOnz7d/F//63/1eK5bbrnFPOGEE2Jfe71e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",
+                        "text/plain": [
+                            "<Figure size 1500x400 with 2 Axes>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "key = {\n",
-                "    \"ripple_param_name\": \"default\",\n",
-                "    **rip_sel_key,\n",
-                "    \"pos_merge_id\": pos_key[\"merge_id\"],\n",
-                "}\n",
-                "sgrip.RippleTimesV1().populate(key)"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "id": "500d96cd-e558-4036-bc93-27704cb3f855",
-            "metadata": {},
-            "source": [
-                "And then `fetch1_dataframe` for ripple times\n"
+                "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
+                "\n",
+                "fig, axes = plt.subplots(2, 1, sharex=True, figsize=(15, 4))\n",
+                "speed = MuaEventsV1.get_speed(mua_key).to_numpy()\n",
+                "time = speed.index.to_numpy()\n",
+                "multiunit_firing_rate = MuaEventsV1.get_firing_rate(mua_key, time)\n",
+                "\n",
+                "time_slice = slice(\n",
+                "    np.searchsorted(time, mua_times.loc[10].start_time) - 1_000,\n",
+                "    np.searchsorted(time, mua_times.loc[10].start_time) + 5_000,\n",
+                ")\n",
+                "\n",
+                "axes[0].plot(\n",
+                "    time[time_slice],\n",
+                "    multiunit_firing_rate[time_slice],\n",
+                "    color=\"black\",\n",
+                ")\n",
+                "axes[0].set_ylabel(\"firing rate (Hz)\")\n",
+                "axes[0].set_title(\"multiunit\")\n",
+                "axes[1].fill_between(time[time_slice], speed[time_slice], color=\"lightgrey\")\n",
+                "axes[1].set_ylabel(\"speed (cm/s)\")\n",
+                "axes[1].set_xlabel(\"time (s)\")\n",
+                "\n",
+                "for id, mua_time in mua_times.loc[\n",
+                "    np.logical_and(\n",
+                "        mua_times[\"start_time\"] > time[time_slice].min(),\n",
+                "        mua_times[\"end_time\"] < time[time_slice].max(),\n",
+                "    )\n",
+                "].iterrows():\n",
+                "    axes[0].axvspan(\n",
+                "        mua_time[\"start_time\"], mua_time[\"end_time\"], color=\"red\", alpha=0.5\n",
+                "    )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
-            "id": "676b05bd-e8ec-41de-9df0-a823cd90aca3",
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[14:44:25][WARNING] Spyglass: Upsampled position data, frame indices are invalid. Setting add_frame_ind=False\n",
+                        "[14:44:29][WARNING] Spyglass: Upsampled position data, frame indices are invalid. Setting add_frame_ind=False\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "WARNING: TimeseriesGraph::_add_series y argument is not 1D array. Using squeeze.\n"
+                    ]
+                },
+                {
                     "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>start_time</th>\n",
-                            "      <th>end_time</th>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>id</th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>5</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>6</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>7</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>8</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>10</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>11</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>12</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>13</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>14</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>15</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>16</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>17</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>18</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>19</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>20</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>21</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>22</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>23</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>24</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>25</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>26</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>27</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>28</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>29</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>30</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>31</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>32</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>33</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>34</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>35</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>36</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>37</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>38</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>39</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>40</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>41</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>42</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>43</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>44</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>45</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>46</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>47</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>48</th>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "      <td>1.635961e+09</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
                         "text/plain": [
-                            "      start_time      end_time\n",
-                            "id                            \n",
-                            "0   1.635961e+09  1.635961e+09\n",
-                            "1   1.635961e+09  1.635961e+09\n",
-                            "2   1.635961e+09  1.635961e+09\n",
-                            "3   1.635961e+09  1.635961e+09\n",
-                            "4   1.635961e+09  1.635961e+09\n",
-                            "5   1.635961e+09  1.635961e+09\n",
-                            "6   1.635961e+09  1.635961e+09\n",
-                            "7   1.635961e+09  1.635961e+09\n",
-                            "8   1.635961e+09  1.635961e+09\n",
-                            "9   1.635961e+09  1.635961e+09\n",
-                            "10  1.635961e+09  1.635961e+09\n",
-                            "11  1.635961e+09  1.635961e+09\n",
-                            "12  1.635961e+09  1.635961e+09\n",
-                            "13  1.635961e+09  1.635961e+09\n",
-                            "14  1.635961e+09  1.635961e+09\n",
-                            "15  1.635961e+09  1.635961e+09\n",
-                            "16  1.635961e+09  1.635961e+09\n",
-                            "17  1.635961e+09  1.635961e+09\n",
-                            "18  1.635961e+09  1.635961e+09\n",
-                            "19  1.635961e+09  1.635961e+09\n",
-                            "20  1.635961e+09  1.635961e+09\n",
-                            "21  1.635961e+09  1.635961e+09\n",
-                            "22  1.635961e+09  1.635961e+09\n",
-                            "23  1.635961e+09  1.635961e+09\n",
-                            "24  1.635961e+09  1.635961e+09\n",
-                            "25  1.635961e+09  1.635961e+09\n",
-                            "26  1.635961e+09  1.635961e+09\n",
-                            "27  1.635961e+09  1.635961e+09\n",
-                            "28  1.635961e+09  1.635961e+09\n",
-                            "29  1.635961e+09  1.635961e+09\n",
-                            "30  1.635961e+09  1.635961e+09\n",
-                            "31  1.635961e+09  1.635961e+09\n",
-                            "32  1.635961e+09  1.635961e+09\n",
-                            "33  1.635961e+09  1.635961e+09\n",
-                            "34  1.635961e+09  1.635961e+09\n",
-                            "35  1.635961e+09  1.635961e+09\n",
-                            "36  1.635961e+09  1.635961e+09\n",
-                            "37  1.635961e+09  1.635961e+09\n",
-                            "38  1.635961e+09  1.635961e+09\n",
-                            "39  1.635961e+09  1.635961e+09\n",
-                            "40  1.635961e+09  1.635961e+09\n",
-                            "41  1.635961e+09  1.635961e+09\n",
-                            "42  1.635961e+09  1.635961e+09\n",
-                            "43  1.635961e+09  1.635961e+09\n",
-                            "44  1.635961e+09  1.635961e+09\n",
-                            "45  1.635961e+09  1.635961e+09\n",
-                            "46  1.635961e+09  1.635961e+09\n",
-                            "47  1.635961e+09  1.635961e+09\n",
-                            "48  1.635961e+09  1.635961e+09"
+                            "'https://figurl.org/f?v=gs://figurl/spikesortingview-10&d=sha1://08d7c35434e8469686fca8aff3ec9319bccb44f9&label=Multiunit%20Detection&zone=franklab.default'"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "ripple_times = (sgrip.RippleTimesV1() & key).fetch1_dataframe()\n",
-                "ripple_times"
+                "(MuaEventsV1 & mua_key).create_figurl(\n",
+                "    zscore_mua=True,\n",
+                ")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "bead0afa",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
-            "source": [
-                "## Up Next\n",
-                "\n",
-                "Next, we'll [extract mark indicator](./31_Extract_Mark_Indicators.ipynb).\n"
-            ]
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "spyglass",
             "language": "python",
             "name": "python3"
@@ -2064,20 +944,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
-        },
-        "widgets": {
-            "application/vnd.jupyter.widget-state+json": {
-                "state": {},
-                "version_major": 2,
-                "version_minor": 0
-            }
+            "version": "3.9.18"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `spyglass_neuro-0.5.1/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb` & `spyglass_neuro-0.5.2/notebooks/40_Extracting_Clusterless_Waveform_Features.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9809027515801082%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'text': {insert: [(0, '[2024-04-19 10:37:45,302][INFO]: "*

 * *            "Connecting sambray@lmf-db.cin.ucsf.edu:3306\\n'), (1, '[2024-04-19 "*

 * *            "10:37:45,330][INFO]: Connected sambray@lmf-db.cin.ucsf.edu:3306\\n'), (2, "*

 * *            "'/home/sambray/Documents/spyglass/src/spyglass/data_import/insert_sessions.py:58: "*

 * *            'UserWarning: Cannot insert data from mediumnwb20230802.nwb: mediumnwb20230802_.nwb is '*

 * *            "already in Nwbfile table.\\n')], delet […]*

```diff
@@ -53,17 +53,17 @@
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[2024-01-17 22:14:51,194][INFO]: Connecting root@localhost:3306\n",
-                        "[2024-01-17 22:14:51,274][INFO]: Connected root@localhost:3306\n",
-                        "/Users/edeno/Documents/GitHub/spyglass/src/spyglass/data_import/insert_sessions.py:58: UserWarning: Cannot insert data from mediumnwb20230802.nwb: mediumnwb20230802_.nwb is already in Nwbfile table.\n",
+                        "[2024-04-19 10:37:45,302][INFO]: Connecting sambray@lmf-db.cin.ucsf.edu:3306\n",
+                        "[2024-04-19 10:37:45,330][INFO]: Connected sambray@lmf-db.cin.ucsf.edu:3306\n",
+                        "/home/sambray/Documents/spyglass/src/spyglass/data_import/insert_sessions.py:58: UserWarning: Cannot insert data from mediumnwb20230802.nwb: mediumnwb20230802_.nwb is already in Nwbfile table.\n",
                         "  warnings.warn(\n"
                     ]
                 }
             ],
             "source": [
                 "from spyglass.utils.nwb_helper_fn import get_nwb_copy_filename\n",
                 "import spyglass.data_import as sgi\n",
@@ -107,38 +107,38 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:55][WARNING] Spyglass: Similar row(s) already inserted.\n"
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:53][WARNING] Spyglass: Similar row(s) already inserted.\n"
                     ]
                 }
             ],
             "source": [
                 "import spyglass.spikesorting.v1 as sgs\n",
                 "\n",
                 "sgs.SortGroup.set_group_by_shank(nwb_file_name=nwb_copy_file_name)\n",
@@ -174,38 +174,47 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][WARNING] Spyglass: Similar row(s) already inserted.\n"
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n",
+                        "[10:37:56][WARNING] Spyglass: Similar row(s) already inserted.\n"
                     ]
                 }
             ],
             "source": [
                 "recording_ids = (\n",
                 "    sgs.SpikeSortingRecordingSelection & {\"nwb_file_name\": nwb_copy_file_name}\n",
                 ").fetch(\"recording_id\")\n",
@@ -231,81 +240,169 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
+                    "data": {
+                        "text/plain": [
+                            "{'sorter': 'clusterless_thresholder',\n",
+                            " 'sorter_param_name': 'default_clusterless',\n",
+                            " 'sorter_params': {'detect_threshold': 100.0,\n",
+                            "  'method': 'locally_exclusive',\n",
+                            "  'peak_sign': 'neg',\n",
+                            "  'exclude_sweep_ms': 0.1,\n",
+                            "  'local_radius_um': 100,\n",
+                            "  'noise_levels': array([1.]),\n",
+                            "  'random_chunk_kwargs': {},\n",
+                            "  'outputs': 'sorting'}}"
+                        ]
+                    },
+                    "execution_count": 5,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "(sgs.SpikeSorterParameters() & {\"sorter\": \"clusterless_thresholder\"}).fetch1()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 23,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n"
+                    ]
+                },
+                {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n",
-                        "[22:14:56][INFO] Spyglass: Similar row(s) already inserted.\n"
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:38][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n",
+                        "[12:03:39][INFO] Spyglass: Similar row(s) already inserted.\n"
                     ]
                 }
             ],
             "source": [
                 "group_keys = []\n",
                 "for recording_id in recording_ids:\n",
                 "    key = {\n",
                 "        \"recording_id\": recording_id,\n",
                 "        \"sorter\": \"clusterless_thresholder\",\n",
                 "        \"sorter_param_name\": \"default_clusterless\",\n",
                 "        \"nwb_file_name\": nwb_copy_file_name,\n",
                 "        \"interval_list_name\": str(\n",
                 "            (\n",
-                "                sgs.ArtifactDetectionSelection & {\"recording_id\": recording_id}\n",
+                "                sgs.ArtifactDetectionSelection\n",
+                "                & {\"recording_id\": recording_id, \"artifact_param_name\": \"none\"}\n",
                 "            ).fetch1(\"artifact_id\")\n",
                 "        ),\n",
                 "    }\n",
                 "    group_keys.append(key)\n",
                 "    sgs.SpikeSortingSelection.insert_selection(key)\n",
-                "\n",
-                "sgs.SpikeSorting.populate(group_keys)"
+                "sort_keys = (sgs.SpikeSortingSelection & group_keys).fetch(\"KEY\")\n",
+                "sgs.SpikeSorting.populate(sort_keys)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For clusterless decoding we do not need any manual curation, but for the sake of the pipeline, we need to store the output of the thresholding in the `CurationV1` table and insert this into the `SpikeSortingOutput` table.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 31,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "b9e53383606f4cbebdb5f8ccf1b56878",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "detect peaks using locally_exclusive:   0%|          | 0/1476 [00:00<?, ?it/s]"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
+                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
+                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
+                        "[12:10:21][INFO] Spyglass: Writing new NWB file mediumnwb20230802_UB40ETS0L4.nwb\n",
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/hdmf/build/objectmapper.py:668: MissingRequiredBuildWarning: NWBFile 'root' is missing required value for attribute 'source_script_file_name'.\n",
+                        "  warnings.warn(msg, MissingRequiredBuildWarning)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "sgs.SpikeSorting().populate(\n",
+                "    sgs.SpikeSortingSelection\n",
+                "    & {\n",
+                "        \"nwb_file_name\": nwb_copy_file_name,\n",
+                "        \"sorter\": \"clusterless_thresholder\",\n",
+                "        \"sorter_param_name\": \"default_clusterless\",\n",
+                "    }\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 34,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from spyglass.spikesorting.spikesorting_merge import SpikeSortingOutput\n",
                 "\n",
                 "sorting_ids = (\n",
-                "    sgs.SpikeSortingSelection & {\"nwb_file_name\": nwb_copy_file_name}\n",
+                "    sgs.SpikeSortingSelection\n",
+                "    & {\n",
+                "        \"nwb_file_name\": nwb_copy_file_name,\n",
+                "        \"sorter\": \"clusterless_thresholder\",\n",
+                "        \"sorter_param_name\": \"default_clusterless\",\n",
+                "    }\n",
                 ").fetch(\"sorting_id\")\n",
                 "\n",
                 "for sorting_id in sorting_ids:\n",
                 "    try:\n",
                 "        sgs.CurationV1.insert_curation(sorting_id=sorting_id)\n",
                 "    except KeyError as e:\n",
                 "        pass\n",
@@ -366,18 +463,28 @@
                 "\n",
                 "_Note_: Members of the Frank Lab can use \"ampl_10_jobs_v2\" instead of \"amplitude\"\n",
                 "for significant speed improvements.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/sambray/mambaforge-pypy3/envs/spyglass/lib/python3.9/site-packages/non_local_detector/likelihoods/clusterless_kde.py:4: TqdmExperimentalWarning: Using `tqdm.autonotebook.tqdm` in notebook mode. Use `tqdm.tqdm` instead to force console mode (e.g. in jupyter console)\n",
+                        "  from tqdm.autonotebook import tqdm\n",
+                        "[2024-04-19 12:40:14,102][INFO]: Connecting sambray@lmf-db.cin.ucsf.edu:3306\n",
+                        "[2024-04-19 12:40:14,138][INFO]: Connected sambray@lmf-db.cin.ucsf.edu:3306\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
                             "    <style type=\"text/css\">\n",
                             "        .Table{\n",
                             "            border-collapse:collapse;\n",
@@ -450,15 +557,15 @@
                             "*features_para params    \n",
                             "+------------+ +--------+\n",
                             "amplitude      =BLOB=    \n",
                             "amplitude, spi =BLOB=    \n",
                             " (Total: 2)"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from spyglass.decoding.v1.waveform_features import WaveformFeaturesParams\n",
                 "\n",
@@ -495,15 +602,15 @@
             "metadata": {},
             "source": [
                 "Now that we've inserted the waveform features parameters, we need to define which parameters to use for each SortGroup. This is done by the `UnitWaveformFeaturesSelection` table. We need to link the primary key `merge_id` from the `SpikeSortingOutput` table to a features parameter set.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -563,131 +670,110 @@
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">spikesorting_merge_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">features_param_name</p>\n",
                             "                            <span class=\"djtooltiptext\">a name for this set of parameters</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>0751a1e1-a406-7f87-ae6f-ce4ffc60621c</td>\n",
-                            "<td>amplitude</td></tr><tr><td>485a4ddf-332d-35b5-3ad4-0561736c1844</td>\n",
-                            "<td>amplitude</td></tr><tr><td>4a712103-c223-864f-82e0-6c23de79cc14</td>\n",
-                            "<td>amplitude</td></tr><tr><td>4a72c253-b3ca-8c13-e615-736a7ebff35c</td>\n",
-                            "<td>amplitude</td></tr><tr><td>5c53bd33-d57c-fbba-e0fb-55e0bcb85d03</td>\n",
-                            "<td>amplitude</td></tr><tr><td>614d796c-0b95-6364-aaa0-b6cb1e7bbb83</td>\n",
-                            "<td>amplitude</td></tr><tr><td>6acb99b8-6a0c-eb83-1141-5f603c5895e0</td>\n",
-                            "<td>amplitude</td></tr><tr><td>6d039a63-17ad-0b78-4b1e-f02d5f3dbbc5</td>\n",
-                            "<td>amplitude</td></tr><tr><td>74e10781-1228-4075-0870-af224024ffdc</td>\n",
-                            "<td>amplitude</td></tr><tr><td>7e3fa66e-727e-1541-819a-b01309bb30ae</td>\n",
-                            "<td>amplitude</td></tr><tr><td>86897349-ff68-ac72-02eb-739dd88936e6</td>\n",
-                            "<td>amplitude</td></tr><tr><td>8bbddc0f-d6ae-6260-9400-f884a6e25ae8</td>\n",
+                            "            <tbody> <tr> <td>003bf29a-fa09-05be-5cac-b7ea70a48c0c</td>\n",
+                            "<td>amplitude</td></tr><tr><td>004faf9a-72cb-4416-ae13-3f85d538604f</td>\n",
+                            "<td>amplitude</td></tr><tr><td>0061a9df-3954-99d4-d738-fd13ab7119fe</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00775472-67a6-5836-b68a-d15186ae3b3c</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00a1861f-bbf0-5e78-3dc6-36551b2657b0</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00a9f0d0-b682-2b12-6a2b-08e4129291ce</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00bd2bbf-ccdb-7be3-f1a0-5e337d87a5a4</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00bdda4f-7059-6c72-c571-a80ad323fda2</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00db0baa-4ec0-3d20-897a-ea4a067ebbba</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00e5a16b-c4f2-e8dc-3083-17f542dadc36</td>\n",
+                            "<td>amplitude</td></tr><tr><td>00f25c1b-d5a3-6ca6-c501-ef0e544f6284</td>\n",
+                            "<td>amplitude</td></tr><tr><td>012fdb25-bd7e-aedd-c41b-bb7e177ceeb8</td>\n",
                             "<td>amplitude</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        <p>...</p>\n",
-                            "        <p>Total: 23</p></div>\n",
+                            "        <p>Total: 3504</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "*spikesorting_ *features_para\n",
                             "+------------+ +------------+\n",
-                            "0751a1e1-a406- amplitude     \n",
-                            "485a4ddf-332d- amplitude     \n",
-                            "4a712103-c223- amplitude     \n",
-                            "4a72c253-b3ca- amplitude     \n",
-                            "5c53bd33-d57c- amplitude     \n",
-                            "614d796c-0b95- amplitude     \n",
-                            "6acb99b8-6a0c- amplitude     \n",
-                            "6d039a63-17ad- amplitude     \n",
-                            "74e10781-1228- amplitude     \n",
-                            "7e3fa66e-727e- amplitude     \n",
-                            "86897349-ff68- amplitude     \n",
-                            "8bbddc0f-d6ae- amplitude     \n",
+                            "003bf29a-fa09- amplitude     \n",
+                            "004faf9a-72cb- amplitude     \n",
+                            "0061a9df-3954- amplitude     \n",
+                            "00775472-67a6- amplitude     \n",
+                            "00a1861f-bbf0- amplitude     \n",
+                            "00a9f0d0-b682- amplitude     \n",
+                            "00bd2bbf-ccdb- amplitude     \n",
+                            "00bdda4f-7059- amplitude     \n",
+                            "00db0baa-4ec0- amplitude     \n",
+                            "00e5a16b-c4f2- amplitude     \n",
+                            "00f25c1b-d5a3- amplitude     \n",
+                            "012fdb25-bd7e- amplitude     \n",
                             "   ...\n",
-                            " (Total: 23)"
+                            " (Total: 3504)"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from spyglass.decoding.v1.waveform_features import UnitWaveformFeaturesSelection\n",
                 "\n",
                 "UnitWaveformFeaturesSelection()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First we find the units we need:\n"
+                "First we find the units we need.  We can use the method `SpikeSortingOutput.get_restricted_merge_ids()` to perform the needed joins to find them:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 6,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "array([UUID('485a4ddf-332d-35b5-3ad4-0561736c1844'),\n",
-                            "       UUID('6acb99b8-6a0c-eb83-1141-5f603c5895e0'),\n",
-                            "       UUID('f7237e18-4e73-4aee-805b-90735e9147de'),\n",
-                            "       UUID('7e3fa66e-727e-1541-819a-b01309bb30ae'),\n",
-                            "       UUID('6d039a63-17ad-0b78-4b1e-f02d5f3dbbc5'),\n",
-                            "       UUID('e0e9133a-7a4e-1321-a43a-e8afcb2f25da'),\n",
-                            "       UUID('9959b614-2318-f597-6651-a3a82124d28a'),\n",
-                            "       UUID('c0eb6455-fc41-c200-b62e-e3ca81b9a3f7'),\n",
-                            "       UUID('912e250e-56d8-ee33-4525-c844d810971b'),\n",
-                            "       UUID('d7d2c97a-0e6e-d1b8-735c-d55dc66a30e1'),\n",
-                            "       UUID('abb92dce-4410-8f17-a501-a4104bda0dcf'),\n",
-                            "       UUID('74e10781-1228-4075-0870-af224024ffdc'),\n",
-                            "       UUID('8bbddc0f-d6ae-6260-9400-f884a6e25ae8'),\n",
-                            "       UUID('614d796c-0b95-6364-aaa0-b6cb1e7bbb83'),\n",
-                            "       UUID('b332482b-e430-169d-8ac0-0a73ce968ed7'),\n",
-                            "       UUID('86897349-ff68-ac72-02eb-739dd88936e6'),\n",
-                            "       UUID('4a712103-c223-864f-82e0-6c23de79cc14'),\n",
-                            "       UUID('cf858380-e8a3-49de-c2a9-1a277e307a68'),\n",
-                            "       UUID('cc4ee561-f974-f8e5-0ea4-83185263ac67'),\n",
-                            "       UUID('4a72c253-b3ca-8c13-e615-736a7ebff35c'),\n",
-                            "       UUID('b92a94d8-ee1e-2097-a81f-5c1e1556ed24'),\n",
-                            "       UUID('5c53bd33-d57c-fbba-e0fb-55e0bcb85d03'),\n",
-                            "       UUID('0751a1e1-a406-7f87-ae6f-ce4ffc60621c')], dtype=object)"
-                        ]
-                    },
-                    "execution_count": 9,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "from spyglass.spikesorting.spikesorting_merge import SpikeSortingOutput\n",
-                "\n",
-                "merge_ids = (\n",
-                "    (SpikeSortingOutput.CurationV1 * sgs.SpikeSortingSelection)\n",
-                "    & {\n",
+                "nwb_copy_file_name = \"mediumnwb20230802_.nwb\"\n",
+                "from spyglass.spikesorting.spikesorting_merge import SpikeSortingOutput"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "key = {\n",
+                "    \"nwb_file_name\": nwb_copy_file_name,\n",
+                "    \"sorter\": \"clusterless_thresholder\",\n",
+                "    \"sorter_param_name\": \"default_clusterless\",\n",
+                "}\n",
+                "merge_ids = SpikeSortingOutput().get_restricted_merge_ids(\n",
+                "    {\n",
                 "        \"nwb_file_name\": nwb_copy_file_name,\n",
                 "        \"sorter\": \"clusterless_thresholder\",\n",
                 "        \"sorter_param_name\": \"default_clusterless\",\n",
-                "    }\n",
-                ").fetch(\"merge_id\")\n",
-                "merge_ids"
+                "    },\n",
+                "    sources=[\"v1\"],\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Then we link them with the features parameters:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -747,52 +833,52 @@
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">spikesorting_merge_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">features_param_name</p>\n",
                             "                            <span class=\"djtooltiptext\">a name for this set of parameters</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>0751a1e1-a406-7f87-ae6f-ce4ffc60621c</td>\n",
-                            "<td>amplitude</td></tr><tr><td>485a4ddf-332d-35b5-3ad4-0561736c1844</td>\n",
-                            "<td>amplitude</td></tr><tr><td>4a712103-c223-864f-82e0-6c23de79cc14</td>\n",
-                            "<td>amplitude</td></tr><tr><td>4a72c253-b3ca-8c13-e615-736a7ebff35c</td>\n",
-                            "<td>amplitude</td></tr><tr><td>5c53bd33-d57c-fbba-e0fb-55e0bcb85d03</td>\n",
-                            "<td>amplitude</td></tr><tr><td>614d796c-0b95-6364-aaa0-b6cb1e7bbb83</td>\n",
-                            "<td>amplitude</td></tr><tr><td>6acb99b8-6a0c-eb83-1141-5f603c5895e0</td>\n",
-                            "<td>amplitude</td></tr><tr><td>6d039a63-17ad-0b78-4b1e-f02d5f3dbbc5</td>\n",
-                            "<td>amplitude</td></tr><tr><td>74e10781-1228-4075-0870-af224024ffdc</td>\n",
-                            "<td>amplitude</td></tr><tr><td>7e3fa66e-727e-1541-819a-b01309bb30ae</td>\n",
-                            "<td>amplitude</td></tr><tr><td>86897349-ff68-ac72-02eb-739dd88936e6</td>\n",
-                            "<td>amplitude</td></tr><tr><td>8bbddc0f-d6ae-6260-9400-f884a6e25ae8</td>\n",
+                            "            <tbody> <tr> <td>0233e49a-b849-7eab-7434-9c298eea87b8</td>\n",
+                            "<td>amplitude</td></tr><tr><td>07239cea-7578-5409-692c-18c9d26b4d36</td>\n",
+                            "<td>amplitude</td></tr><tr><td>08be9775-370d-6492-0b4e-a5db4ce7a128</td>\n",
+                            "<td>amplitude</td></tr><tr><td>11819f33-11d5-f0f8-2590-ce3d60b76f3a</td>\n",
+                            "<td>amplitude</td></tr><tr><td>1c2ea289-2e7f-dcda-0464-ce97d3d6a392</td>\n",
+                            "<td>amplitude</td></tr><tr><td>20f24092-d191-0c58-55c8-d43d453f9fd4</td>\n",
+                            "<td>amplitude</td></tr><tr><td>2598b48e-49a0-3389-dd15-0230e8d326e4</td>\n",
+                            "<td>amplitude</td></tr><tr><td>483055a5-9775-27b7-856e-01543bd920aa</td>\n",
+                            "<td>amplitude</td></tr><tr><td>50ae3f7e-65a8-5fc2-5304-ab534b90fa46</td>\n",
+                            "<td>amplitude</td></tr><tr><td>50b29d01-2d74-e37e-2842-ad56d833c5f9</td>\n",
+                            "<td>amplitude</td></tr><tr><td>5e756e76-68be-21b7-7764-cb78d9aa4ef8</td>\n",
+                            "<td>amplitude</td></tr><tr><td>67f156e1-5da7-9c89-03b1-cc2dba88dacd</td>\n",
                             "<td>amplitude</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        <p>...</p>\n",
-                            "        <p>Total: 23</p></div>\n",
+                            "        <p>Total: 26</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "*spikesorting_ *features_para\n",
                             "+------------+ +------------+\n",
-                            "0751a1e1-a406- amplitude     \n",
-                            "485a4ddf-332d- amplitude     \n",
-                            "4a712103-c223- amplitude     \n",
-                            "4a72c253-b3ca- amplitude     \n",
-                            "5c53bd33-d57c- amplitude     \n",
-                            "614d796c-0b95- amplitude     \n",
-                            "6acb99b8-6a0c- amplitude     \n",
-                            "6d039a63-17ad- amplitude     \n",
-                            "74e10781-1228- amplitude     \n",
-                            "7e3fa66e-727e- amplitude     \n",
-                            "86897349-ff68- amplitude     \n",
-                            "8bbddc0f-d6ae- amplitude     \n",
+                            "0233e49a-b849- amplitude     \n",
+                            "07239cea-7578- amplitude     \n",
+                            "08be9775-370d- amplitude     \n",
+                            "11819f33-11d5- amplitude     \n",
+                            "1c2ea289-2e7f- amplitude     \n",
+                            "20f24092-d191- amplitude     \n",
+                            "2598b48e-49a0- amplitude     \n",
+                            "483055a5-9775- amplitude     \n",
+                            "50ae3f7e-65a8- amplitude     \n",
+                            "50b29d01-2d74- amplitude     \n",
+                            "5e756e76-68be- amplitude     \n",
+                            "67f156e1-5da7- amplitude     \n",
                             "   ...\n",
-                            " (Total: 23)"
+                            " (Total: 26)"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "selection_keys = [\n",
                 "    {\n",
@@ -811,668 +897,17 @@
             "metadata": {},
             "source": [
                 "Finally, we extract the waveform features, by populating the `UnitWaveformFeatures` table:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 13,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "c4f79735339147cf93143b0d329f7b0c",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:15:08,494][WARNING]: Skipped checksum for file with hash: 6629fd95-636a-4ad4-c9af-cee507de2130, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_AMBBKQ9RIY.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:15:08][INFO] Spyglass: Writing new NWB file mediumnwb20230802_NQEPSMKPK0.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "71ac6cac75cd4ddcb21e16dc9432b655",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:15:19,450][WARNING]: Skipped checksum for file with hash: 6d04cbdb-e1e4-f44f-7274-0e1ab0356d75, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_W1MLF0Q86S.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:15:19][INFO] Spyglass: Writing new NWB file mediumnwb20230802_F02UG5Z5FR.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "a90dc146fa6548a8a2b2af7495d4be29",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:15:30,787][WARNING]: Skipped checksum for file with hash: 8993754e-7dbe-94a1-403d-8c55aa9c6c42, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_JN4A4GSLZB.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:15:31][INFO] Spyglass: Writing new NWB file mediumnwb20230802_OTV91MLKDT.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "3d8380674f7246c3ac47438cb638ec48",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:15:41,633][WARNING]: Skipped checksum for file with hash: 9e24661c-b021-6ad4-f224-89e331334f18, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_T2DBO3EMZ8.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:15:41][INFO] Spyglass: Writing new NWB file mediumnwb20230802_TSPNTCGNN1.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "a5bd42b4afcd445894660a3601248554",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:15:52,561][WARNING]: Skipped checksum for file with hash: f64f34ee-e72d-e566-a048-65f2ea31708a, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_USMRXAAV8I.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:15:52][INFO] Spyglass: Writing new NWB file mediumnwb20230802_QSK70WFDJH.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "ecfd8f43660a41278fbc6826f4517fc7",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:16:03,559][WARNING]: Skipped checksum for file with hash: 6d13e338-41bd-b011-beb5-4de53d9d467b, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_JA2OA12RPN.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:16:03][INFO] Spyglass: Writing new NWB file mediumnwb20230802_DO45HKXYTB.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "ccb7eec245734ddaab37d65a48db80b2",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:16:14,288][WARNING]: Skipped checksum for file with hash: d740eb7d-ce29-e140-06a2-c56655e0842a, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_L92EE1VRPB.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:16:14][INFO] Spyglass: Writing new NWB file mediumnwb20230802_KFIYRJ4HFO.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "8f4db4312708442d9d9baee7361e2d18",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:16:24,130][WARNING]: Skipped checksum for file with hash: 1f386cd3-89da-0233-03ff-76ba94e91a3a, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_TX2ZX3DAP4.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:16:24][INFO] Spyglass: Writing new NWB file mediumnwb20230802_0YIM5K3H47.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "52f1bb4db348413390887bab91a4eb05",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:16:35,048][WARNING]: Skipped checksum for file with hash: fa76d419-77a4-697a-325d-5c2ddbe517f9, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_0R6AWXMC6G.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:16:35][INFO] Spyglass: Writing new NWB file mediumnwb20230802_CTLEGE2TWZ.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "49b70c6fdc0c4d82b707b0f64c746992",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:16:46,009][WARNING]: Skipped checksum for file with hash: ce4cb0c3-3dd0-70fd-8ea0-98a8b84592d9, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_7UIA2ILMG6.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:16:46][INFO] Spyglass: Writing new NWB file mediumnwb20230802_7EN0N1U4U1.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "83e34dff95084145a5d1a2eceb29f091",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:16:56,814][WARNING]: Skipped checksum for file with hash: e43f95ff-9779-b980-00a3-99e104864462, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_AKOI7OTASI.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:16:57][INFO] Spyglass: Writing new NWB file mediumnwb20230802_DHKWBWWAMC.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "497faa2d251246abb45174b1aac4f327",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:17:05,013][WARNING]: Skipped checksum for file with hash: ff81d274-17f7-702d-a2b4-92ac43c29316, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_Y2YF504C5D.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:17:05][INFO] Spyglass: Writing new NWB file mediumnwb20230802_PEN0D79Q0B.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "f8c583bb202347f0bb8678c3c249cb4b",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:17:15,903][WARNING]: Skipped checksum for file with hash: e282a8e5-844b-20f6-345c-cded12e761a9, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_DUNM1TZUGR.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:17:16][INFO] Spyglass: Writing new NWB file mediumnwb20230802_WP7SIXDJ2A.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "fd115ce374c043feac8f7e3ec4cb887c",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:17:26,609][WARNING]: Skipped checksum for file with hash: 7d05460d-7366-27c9-2ba7-de2ad5d402f2, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_4JXWFJ3JRI.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:17:26][INFO] Spyglass: Writing new NWB file mediumnwb20230802_B82OS6W1QA.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "d48a5f3da4394f2dbdb4c7281caba2ed",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:17:37,652][WARNING]: Skipped checksum for file with hash: c202eb9e-ca43-0a72-4086-57a5bb6eb937, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_5TY04H3B5T.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:17:37][INFO] Spyglass: Writing new NWB file mediumnwb20230802_XO17FQLN6T.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "872ea3e1911745ce9ee2626bda69d164",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:17:47,269][WARNING]: Skipped checksum for file with hash: 4357905c-c6b9-3990-4d62-740a54cfc667, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_X84BYVM2B0.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:17:47][INFO] Spyglass: Writing new NWB file mediumnwb20230802_OCFI0GFLZ9.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "3bb4a5c8097d451896b9552caf862676",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:17:58,240][WARNING]: Skipped checksum for file with hash: 4c1103ac-eaca-b282-e5ff-aa2194e65a43, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_2R6VQ8EDL4.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:17:58][INFO] Spyglass: Writing new NWB file mediumnwb20230802_60M9VSZX0W.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "a30f15ba40cf4c9cb0050f0e1ddb1396",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:18:09,119][WARNING]: Skipped checksum for file with hash: 023c874f-8114-3ef6-7fcf-813844787d5f, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_L7HDY9IDHO.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:18:09][INFO] Spyglass: Writing new NWB file mediumnwb20230802_Z5HJ68LHYW.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "b0109646253a42c19df9dafc465548a6",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:18:20,605][WARNING]: Skipped checksum for file with hash: fde8b240-6adc-86f0-6391-f3f6fad72ee9, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_HWU3E4EKP4.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:18:20][INFO] Spyglass: Writing new NWB file mediumnwb20230802_U5U5JVGY4F.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "cf5715c3dee74d71ac325fc77c0eec93",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:18:31,780][WARNING]: Skipped checksum for file with hash: c592e63b-4db1-40be-632e-0180e6fa02d7, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_SGAU9PX7US.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:18:32][INFO] Spyglass: Writing new NWB file mediumnwb20230802_0D5Z0NSIP8.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "e0ea746638354277bd96180aac672309",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:18:42,644][WARNING]: Skipped checksum for file with hash: 148d9058-e6dc-e959-4c4d-75db9aa0b6e4, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_EF6N6XI3AH.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:18:42][INFO] Spyglass: Writing new NWB file mediumnwb20230802_EYV2NARUKU.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "a0f6340431f84fe98d2bcfdbedbde443",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:18:54,570][WARNING]: Skipped checksum for file with hash: b4b6404f-aaf8-c4cc-9abe-ceea56e103f3, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_O7ZZ0F1XN7.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:18:54][INFO] Spyglass: Writing new NWB file mediumnwb20230802_T4XBCIW44T.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/spikeinterface/core/waveform_extractor.py:275: UserWarning: Sorting object is not dumpable, which might result in downstream errors for parallel processing. To make the sorting dumpable, use the `sorting.save()` function.\n",
-                        "  warn(\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "d95a33c36dcb4b52923648866fef862d",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "extract waveforms memmap:   0%|          | 0/2 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-17 22:19:05,568][WARNING]: Skipped checksum for file with hash: 26f7bdc7-da8d-6ad5-3f4a-554ceb48755e, and path: /Users/edeno/Documents/GitHub/spyglass/DATA/analysis/mediumnwb20230802/mediumnwb20230802_0TKF5589B7.nwb\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/ecephys.py:90: UserWarning: ElectricalSeries 'e-series': The second dimension of data does not match the length of electrodes. Your data may be transposed.\n",
-                        "  warnings.warn(\"%s '%s': The second dimension of data does not match the length of electrodes. \"\n",
-                        "/Users/edeno/miniconda3/envs/spyglass/lib/python3.9/site-packages/pynwb/base.py:193: UserWarning: TimeSeries 'analog': Length of data does not match length of timestamps. Your data may be transposed. Time should be on the 0th dimension\n",
-                        "  warn(\"%s '%s': Length of data does not match length of timestamps. Your data may be transposed. \"\n",
-                        "[22:19:05][INFO] Spyglass: Writing new NWB file mediumnwb20230802_UD55CR8LZK.nwb\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "from spyglass.decoding.v1.waveform_features import UnitWaveformFeatures\n",
                 "\n",
                 "UnitWaveformFeatures.populate(selection_keys)"
             ]
         },
         {
@@ -1780,13 +1215,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.18"
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `spyglass_neuro-0.5.1/notebooks/41_Decoding_Clusterless.ipynb` & `spyglass_neuro-0.5.2/notebooks/41_Decoding_Clusterless.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966560845321387%*

 * *Differences: {"'cells'": "{2: {'execution_count': 27, 'outputs': {0: {'data': {'text/html': {insert: [(61, "*

 * *            '\'                        </div></th><th><div class="djtooltip">\\n\'), (62, '*

 * *            '\'                            <p id="primary">sorting_id</p>\\n\'), (63, '*

 * *            '\'                            <span class="djtooltiptext"></span>\\n\'), (64, '*

 * *            '\'                        </div></th><th><div class="djtooltip">\\n\'), (65, '*

 * *            '\'                            <p id="n […]*

```diff
@@ -48,27 +48,18 @@
                 "dj.config.load(\n",
                 "    Path(\"../dj_local_conf.json\").absolute()\n",
                 ")  # load config for database connection info"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 27,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-01-29 10:24:06,266][INFO]: Connecting root@localhost:3306\n",
-                        "[2024-01-29 10:24:06,337][INFO]: Connected root@localhost:3306\n",
-                        "[10:24:07][WARNING] Spyglass: Please update position_tools to >= 0.1.0\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
                             "    <style type=\"text/css\">\n",
                             "        .Table{\n",
                             "            border-collapse:collapse;\n",
@@ -119,192 +110,198 @@
                             "        }\n",
                             "    </style>\n",
                             "    \n",
                             "    \n",
                             "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
                             "        <table border=\"1\" class=\"Table\">\n",
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sorting_id</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">merge_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">features_param_name</p>\n",
                             "                            <span class=\"djtooltiptext\">a name for this set of parameters</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"primary\">sorting_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
+                            "                            <p id=\"nonprimary\">curation_id</p>\n",
+                            "                            <span class=\"djtooltiptext\"></span>\n",
+                            "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"nonprimary\">recording_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"nonprimary\">sorter</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"nonprimary\">sorter_param_name</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"nonprimary\">nwb_file_name</p>\n",
                             "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"nonprimary\">interval_list_name</p>\n",
                             "                            <span class=\"djtooltiptext\">descriptive name of this interval list</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"nonprimary\">curation_id</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>08a302b6-5505-40fa-b4d5-62162f8eef58</td>\n",
-                            "<td>485a4ddf-332d-35b5-3ad4-0561736c1844</td>\n",
+                            "            <tbody> <tr> <td>0233e49a-b849-7eab-7434-9c298eea87b8</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>449b64e3-db0b-437e-a1b9-0d29928aa2dd</td>\n",
+                            "<td>85cb4efd-5dd9-4637-8c47-50927da56ecb</td>\n",
+                            "<td>0</td>\n",
+                            "<td>d6ec337b-f131-47fa-8d04-f152459539ab</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>45f6b9a1-eef3-46eb-866d-d0999afebda6</td>\n",
-                            "<td>0</td></tr><tr><td>0ca508ee-af4c-4a89-8181-d48bd209bfd4</td>\n",
-                            "<td>6acb99b8-6a0c-eb83-1141-5f603c5895e0</td>\n",
+                            "<td>d4d3d806-13dc-42b9-a149-267fa170aa8f</td></tr><tr><td>07239cea-7578-5409-692c-18c9d26b4d36</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>328da21c-1d9c-41e2-9800-76b3484b707b</td>\n",
+                            "<td>17abb5a3-cc9a-4a7f-8fbf-ae3bcffad239</td>\n",
+                            "<td>0</td>\n",
+                            "<td>9b34c86e-f2d0-4c6c-a7b8-302ef30b0fff</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>686d9951-1c0f-4d5e-9f5c-09e6fd8bdd4c</td>\n",
-                            "<td>0</td></tr><tr><td>209dc048-6fae-4315-b293-c06fff29f947</td>\n",
-                            "<td>f7237e18-4e73-4aee-805b-90735e9147de</td>\n",
+                            "<td>24608f0d-ffca-4f56-8dd3-a274b7248b63</td></tr><tr><td>08be9775-370d-6492-0b4e-a5db4ce7a128</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>aff78f2f-2ba0-412a-95cc-447c3a2f4683</td>\n",
+                            "<td>2056130f-b8c9-46d1-9c27-4287d237f63f</td>\n",
+                            "<td>0</td>\n",
+                            "<td>e9ea1b3c-6e7b-4960-a593-0dd6d5ab0990</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>719e8a86-fcf1-4ffc-8c1f-ea912f67ad5d</td>\n",
-                            "<td>0</td></tr><tr><td>21a9a593-f6f3-4b82-99d7-8fc46556eff3</td>\n",
-                            "<td>7e3fa66e-727e-1541-819a-b01309bb30ae</td>\n",
+                            "<td>c96e245d-efef-4ab6-b549-683270857dbb</td></tr><tr><td>11819f33-11d5-f0f8-2590-ce3d60b76f3a</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>2402805a-04f9-4a88-9ccf-071376c8de19</td>\n",
+                            "<td>71add870-7efe-4e64-b5fc-079c7b6d4a8a</td>\n",
+                            "<td>0</td>\n",
+                            "<td>8f4b5933-7f9d-4ca1-a262-9a7978630101</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>d581b117-160e-4311-b096-7781a4de4394</td>\n",
-                            "<td>0</td></tr><tr><td>406a20e3-5a9f-4fec-b046-a6561f72461e</td>\n",
-                            "<td>6d039a63-17ad-0b78-4b1e-f02d5f3dbbc5</td>\n",
+                            "<td>9d5a025a-2b46-47b3-94f4-70d58db68e60</td></tr><tr><td>1c2ea289-2e7f-dcda-0464-ce97d3d6a392</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>f1427e00-2974-4301-b2ac-b4dc29277c51</td>\n",
+                            "<td>46b8a445-1513-44ce-8a14-d1c9dec80d74</td>\n",
+                            "<td>0</td>\n",
+                            "<td>0d247564-2302-4ace-9157-c3891eceaf2c</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>0e848c38-9105-4ea4-b6ba-dbdd5b46a088</td>\n",
-                            "<td>0</td></tr><tr><td>4131c51b-c56d-41fa-b046-46635fc17fd9</td>\n",
-                            "<td>e0e9133a-7a4e-1321-a43a-e8afcb2f25da</td>\n",
+                            "<td>56cbb21e-8fe8-4f4a-b2b0-537ad6039543</td></tr><tr><td>20f24092-d191-0c58-55c8-d43d453f9fd4</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>9e332d82-1daf-4e92-bb50-12e4f9430875</td>\n",
+                            "<td>aec60cb7-017c-42ed-91be-0fb2a5f75948</td>\n",
+                            "<td>0</td>\n",
+                            "<td>747f4eea-6df3-422b-941e-b5aaad7ec607</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>9ed11db5-c42e-491a-8caf-7d9a37a65f13</td>\n",
-                            "<td>0</td></tr><tr><td>4c5a629a-71d9-481d-ab11-a4cb0fc16087</td>\n",
-                            "<td>9959b614-2318-f597-6651-a3a82124d28a</td>\n",
+                            "<td>65009b63-5830-45b5-9954-cd5341aa8cef</td></tr><tr><td>2598b48e-49a0-3389-dd15-0230e8d326e4</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>3a2c3eed-413a-452a-83c8-0e4648141bde</td>\n",
+                            "<td>e26863d0-7a77-455c-b687-0af1bd626486</td>\n",
+                            "<td>0</td>\n",
+                            "<td>34ea9dd3-b728-4bd3-872c-7a4e37fb2ac9</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>2b9fbf14-74a0-4294-a805-26702340aac9</td>\n",
-                            "<td>0</td></tr><tr><td>4d629c07-1931-4e1f-a3a8-cbf1b72161e3</td>\n",
-                            "<td>c0eb6455-fc41-c200-b62e-e3ca81b9a3f7</td>\n",
+                            "<td>e4daaf56-e40d-41d3-8523-097237d98bbd</td></tr><tr><td>483055a5-9775-27b7-856e-01543bd920aa</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>f07bc0b0-de6b-4424-8ef9-766213aaca26</td>\n",
+                            "<td>9af6681f-2e37-496e-823e-7acbdd436a27</td>\n",
+                            "<td>0</td>\n",
+                            "<td>73c9e01c-b37c-41a2-8571-0df13c32bf76</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>5c68f0f0-f577-4905-8a09-e4d171d0a22d</td>\n",
-                            "<td>0</td></tr><tr><td>554a9a3c-0461-48be-8435-123eed59c228</td>\n",
-                            "<td>912e250e-56d8-ee33-4525-c844d810971b</td>\n",
+                            "<td>3da02b84-1a7f-4f2a-81bf-2e92c4d88e96</td></tr><tr><td>50ae3f7e-65a8-5fc2-5304-ab534b90fa46</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>7f128981-6868-4976-ba20-248655dcac21</td>\n",
+                            "<td>2483d0c7-4cfe-4d6f-8dd6-2e13a8289d94</td>\n",
+                            "<td>0</td>\n",
+                            "<td>03cc7709-66e7-47ac-a3bd-63add028d9f8</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>f4b9301f-bc91-455b-9474-c801093f3856</td>\n",
-                            "<td>0</td></tr><tr><td>7bb007f2-26d3-463f-b7dc-7bd4d271725e</td>\n",
-                            "<td>d7d2c97a-0e6e-d1b8-735c-d55dc66a30e1</td>\n",
+                            "<td>8cfc1ccb-8de3-4eee-9e18-f8b8f5c45821</td></tr><tr><td>50b29d01-2d74-e37e-2842-ad56d833c5f9</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>a9b7cec0-1256-49cf-abf0-8c45fd155379</td>\n",
+                            "<td>1dcecaac-8e0d-4d18-8296-cdb50eef9506</td>\n",
+                            "<td>0</td>\n",
+                            "<td>d8a8c564-13c7-4fab-9a33-1eac416869da</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>74270cba-36ee-4afb-ab50-2a6cc948e68c</td>\n",
-                            "<td>0</td></tr><tr><td>80e1f37f-48a7-4087-bd37-7a37b6a2c160</td>\n",
-                            "<td>abb92dce-4410-8f17-a501-a4104bda0dcf</td>\n",
+                            "<td>96678676-89dd-42e4-89f6-ce56c618ce83</td></tr><tr><td>5e756e76-68be-21b7-7764-cb78d9aa4ef8</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>3c40ebdc-0b61-4105-9971-e1348bd49bc7</td>\n",
+                            "<td>552176ab-d870-41c4-8621-07e71f6e9a19</td>\n",
+                            "<td>0</td>\n",
+                            "<td>fa4faf43-e747-43ca-b8a5-53a02d7938ec</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>0f91197e-bebb-4dc6-ad41-5bf89c3eed28</td>\n",
-                            "<td>0</td></tr><tr><td>8848c4a8-a2f2-4f3d-82cd-51b13b8bae3c</td>\n",
-                            "<td>74e10781-1228-4075-0870-af224024ffdc</td>\n",
+                            "<td>07036486-e9f5-4dba-8662-7fb5ff2a6711</td></tr><tr><td>67f156e1-5da7-9c89-03b1-cc2dba88dacd</td>\n",
                             "<td>amplitude</td>\n",
-                            "<td>257c077b-8f3b-4abb-a631-6b8084d6a1ea</td>\n",
+                            "<td>8f45b210-c8f9-4a27-96c2-9b85f16b3451</td>\n",
+                            "<td>0</td>\n",
+                            "<td>30895f0f-1eec-481d-b763-edae7667ef00</td>\n",
                             "<td>clusterless_thresholder</td>\n",
                             "<td>default_clusterless</td>\n",
                             "<td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>e289e03d-32ad-461a-a1cc-c88537343149</td>\n",
-                            "<td>0</td> </tr> </tbody>\n",
+                            "<td>22fb2b64-fc3c-44af-a8c1-dacc9010beab</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        <p>...</p>\n",
-                            "        <p>Total: 23</p></div>\n",
+                            "        <p>Total: 26</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "*sorting_id    *merge_id      *features_para recording_id   sorter         sorter_param_n nwb_file_name  interval_list_ curation_id   \n",
+                            "*merge_id      *features_para *sorting_id    curation_id    recording_id   sorter         sorter_param_n nwb_file_name  interval_list_\n",
                             "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
-                            "08a302b6-5505- 485a4ddf-332d- amplitude      449b64e3-db0b- clusterless_th default_cluste mediumnwb20230 45f6b9a1-eef3- 0             \n",
-                            "0ca508ee-af4c- 6acb99b8-6a0c- amplitude      328da21c-1d9c- clusterless_th default_cluste mediumnwb20230 686d9951-1c0f- 0             \n",
-                            "209dc048-6fae- f7237e18-4e73- amplitude      aff78f2f-2ba0- clusterless_th default_cluste mediumnwb20230 719e8a86-fcf1- 0             \n",
-                            "21a9a593-f6f3- 7e3fa66e-727e- amplitude      2402805a-04f9- clusterless_th default_cluste mediumnwb20230 d581b117-160e- 0             \n",
-                            "406a20e3-5a9f- 6d039a63-17ad- amplitude      f1427e00-2974- clusterless_th default_cluste mediumnwb20230 0e848c38-9105- 0             \n",
-                            "4131c51b-c56d- e0e9133a-7a4e- amplitude      9e332d82-1daf- clusterless_th default_cluste mediumnwb20230 9ed11db5-c42e- 0             \n",
-                            "4c5a629a-71d9- 9959b614-2318- amplitude      3a2c3eed-413a- clusterless_th default_cluste mediumnwb20230 2b9fbf14-74a0- 0             \n",
-                            "4d629c07-1931- c0eb6455-fc41- amplitude      f07bc0b0-de6b- clusterless_th default_cluste mediumnwb20230 5c68f0f0-f577- 0             \n",
-                            "554a9a3c-0461- 912e250e-56d8- amplitude      7f128981-6868- clusterless_th default_cluste mediumnwb20230 f4b9301f-bc91- 0             \n",
-                            "7bb007f2-26d3- d7d2c97a-0e6e- amplitude      a9b7cec0-1256- clusterless_th default_cluste mediumnwb20230 74270cba-36ee- 0             \n",
-                            "80e1f37f-48a7- abb92dce-4410- amplitude      3c40ebdc-0b61- clusterless_th default_cluste mediumnwb20230 0f91197e-bebb- 0             \n",
-                            "8848c4a8-a2f2- 74e10781-1228- amplitude      257c077b-8f3b- clusterless_th default_cluste mediumnwb20230 e289e03d-32ad- 0             \n",
+                            "0233e49a-b849- amplitude      85cb4efd-5dd9- 0              d6ec337b-f131- clusterless_th default_cluste mediumnwb20230 d4d3d806-13dc-\n",
+                            "07239cea-7578- amplitude      17abb5a3-cc9a- 0              9b34c86e-f2d0- clusterless_th default_cluste mediumnwb20230 24608f0d-ffca-\n",
+                            "08be9775-370d- amplitude      2056130f-b8c9- 0              e9ea1b3c-6e7b- clusterless_th default_cluste mediumnwb20230 c96e245d-efef-\n",
+                            "11819f33-11d5- amplitude      71add870-7efe- 0              8f4b5933-7f9d- clusterless_th default_cluste mediumnwb20230 9d5a025a-2b46-\n",
+                            "1c2ea289-2e7f- amplitude      46b8a445-1513- 0              0d247564-2302- clusterless_th default_cluste mediumnwb20230 56cbb21e-8fe8-\n",
+                            "20f24092-d191- amplitude      aec60cb7-017c- 0              747f4eea-6df3- clusterless_th default_cluste mediumnwb20230 65009b63-5830-\n",
+                            "2598b48e-49a0- amplitude      e26863d0-7a77- 0              34ea9dd3-b728- clusterless_th default_cluste mediumnwb20230 e4daaf56-e40d-\n",
+                            "483055a5-9775- amplitude      9af6681f-2e37- 0              73c9e01c-b37c- clusterless_th default_cluste mediumnwb20230 3da02b84-1a7f-\n",
+                            "50ae3f7e-65a8- amplitude      2483d0c7-4cfe- 0              03cc7709-66e7- clusterless_th default_cluste mediumnwb20230 8cfc1ccb-8de3-\n",
+                            "50b29d01-2d74- amplitude      1dcecaac-8e0d- 0              d8a8c564-13c7- clusterless_th default_cluste mediumnwb20230 96678676-89dd-\n",
+                            "5e756e76-68be- amplitude      552176ab-d870- 0              fa4faf43-e747- clusterless_th default_cluste mediumnwb20230 07036486-e9f5-\n",
+                            "67f156e1-5da7- amplitude      8f45b210-c8f9- 0              30895f0f-1eec- clusterless_th default_cluste mediumnwb20230 22fb2b64-fc3c-\n",
                             "   ...\n",
-                            " (Total: 23)"
+                            " (Total: 26)"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from spyglass.spikesorting.spikesorting_merge import SpikeSortingOutput\n",
                 "import spyglass.spikesorting.v1 as sgs\n",
-                "from spyglass.decoding.v1.waveform_features import UnitWaveformFeaturesSelection\n",
+                "from spyglass.decoding.v1.waveform_features import (\n",
+                "    UnitWaveformFeaturesSelection,\n",
+                "    UnitWaveformFeatures,\n",
+                ")\n",
                 "\n",
                 "\n",
                 "nwb_copy_file_name = \"mediumnwb20230802_.nwb\"\n",
                 "\n",
                 "sorter_keys = {\n",
                 "    \"nwb_file_name\": nwb_copy_file_name,\n",
                 "    \"sorter\": \"clusterless_thresholder\",\n",
                 "    \"sorter_param_name\": \"default_clusterless\",\n",
                 "}\n",
                 "\n",
                 "feature_key = {\"features_param_name\": \"amplitude\"}\n",
                 "\n",
-                "(sgs.SpikeSortingSelection & sorter_keys) * SpikeSortingOutput.CurationV1 * (\n",
+                "(\n",
                 "    UnitWaveformFeaturesSelection.proj(merge_id=\"spikesorting_merge_id\")\n",
-                "    & feature_key\n",
+                "    * SpikeSortingOutput.CurationV1\n",
+                "    * sgs.SpikeSortingSelection\n",
+                ") & SpikeSortingOutput().get_restricted_merge_ids(\n",
+                "    sorter_keys, sources=[\"v1\"], as_dict=True\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -364,72 +361,72 @@
                             "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">spikesorting_merge_id</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">features_param_name</p>\n",
                             "                            <span class=\"djtooltiptext\">a name for this set of parameters</span>\n",
                             "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>0751a1e1-a406-7f87-ae6f-ce4ffc60621c</td>\n",
-                            "<td>amplitude</td></tr><tr><td>485a4ddf-332d-35b5-3ad4-0561736c1844</td>\n",
-                            "<td>amplitude</td></tr><tr><td>4a712103-c223-864f-82e0-6c23de79cc14</td>\n",
-                            "<td>amplitude</td></tr><tr><td>4a72c253-b3ca-8c13-e615-736a7ebff35c</td>\n",
-                            "<td>amplitude</td></tr><tr><td>5c53bd33-d57c-fbba-e0fb-55e0bcb85d03</td>\n",
-                            "<td>amplitude</td></tr><tr><td>614d796c-0b95-6364-aaa0-b6cb1e7bbb83</td>\n",
-                            "<td>amplitude</td></tr><tr><td>6acb99b8-6a0c-eb83-1141-5f603c5895e0</td>\n",
-                            "<td>amplitude</td></tr><tr><td>6d039a63-17ad-0b78-4b1e-f02d5f3dbbc5</td>\n",
-                            "<td>amplitude</td></tr><tr><td>74e10781-1228-4075-0870-af224024ffdc</td>\n",
-                            "<td>amplitude</td></tr><tr><td>7e3fa66e-727e-1541-819a-b01309bb30ae</td>\n",
-                            "<td>amplitude</td></tr><tr><td>86897349-ff68-ac72-02eb-739dd88936e6</td>\n",
-                            "<td>amplitude</td></tr><tr><td>8bbddc0f-d6ae-6260-9400-f884a6e25ae8</td>\n",
+                            "            <tbody> <tr> <td>0233e49a-b849-7eab-7434-9c298eea87b8</td>\n",
+                            "<td>amplitude</td></tr><tr><td>07239cea-7578-5409-692c-18c9d26b4d36</td>\n",
+                            "<td>amplitude</td></tr><tr><td>08be9775-370d-6492-0b4e-a5db4ce7a128</td>\n",
+                            "<td>amplitude</td></tr><tr><td>11819f33-11d5-f0f8-2590-ce3d60b76f3a</td>\n",
+                            "<td>amplitude</td></tr><tr><td>1c2ea289-2e7f-dcda-0464-ce97d3d6a392</td>\n",
+                            "<td>amplitude</td></tr><tr><td>20f24092-d191-0c58-55c8-d43d453f9fd4</td>\n",
+                            "<td>amplitude</td></tr><tr><td>2598b48e-49a0-3389-dd15-0230e8d326e4</td>\n",
+                            "<td>amplitude</td></tr><tr><td>483055a5-9775-27b7-856e-01543bd920aa</td>\n",
+                            "<td>amplitude</td></tr><tr><td>50ae3f7e-65a8-5fc2-5304-ab534b90fa46</td>\n",
+                            "<td>amplitude</td></tr><tr><td>50b29d01-2d74-e37e-2842-ad56d833c5f9</td>\n",
+                            "<td>amplitude</td></tr><tr><td>5e756e76-68be-21b7-7764-cb78d9aa4ef8</td>\n",
+                            "<td>amplitude</td></tr><tr><td>67f156e1-5da7-9c89-03b1-cc2dba88dacd</td>\n",
                             "<td>amplitude</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        <p>...</p>\n",
-                            "        <p>Total: 23</p></div>\n",
+                            "        <p>Total: 26</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "*spikesorting_ *features_para\n",
                             "+------------+ +------------+\n",
-                            "0751a1e1-a406- amplitude     \n",
-                            "485a4ddf-332d- amplitude     \n",
-                            "4a712103-c223- amplitude     \n",
-                            "4a72c253-b3ca- amplitude     \n",
-                            "5c53bd33-d57c- amplitude     \n",
-                            "614d796c-0b95- amplitude     \n",
-                            "6acb99b8-6a0c- amplitude     \n",
-                            "6d039a63-17ad- amplitude     \n",
-                            "74e10781-1228- amplitude     \n",
-                            "7e3fa66e-727e- amplitude     \n",
-                            "86897349-ff68- amplitude     \n",
-                            "8bbddc0f-d6ae- amplitude     \n",
+                            "0233e49a-b849- amplitude     \n",
+                            "07239cea-7578- amplitude     \n",
+                            "08be9775-370d- amplitude     \n",
+                            "11819f33-11d5- amplitude     \n",
+                            "1c2ea289-2e7f- amplitude     \n",
+                            "20f24092-d191- amplitude     \n",
+                            "2598b48e-49a0- amplitude     \n",
+                            "483055a5-9775- amplitude     \n",
+                            "50ae3f7e-65a8- amplitude     \n",
+                            "50b29d01-2d74- amplitude     \n",
+                            "5e756e76-68be- amplitude     \n",
+                            "67f156e1-5da7- amplitude     \n",
                             "   ...\n",
-                            " (Total: 23)"
+                            " (Total: 26)"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from spyglass.decoding.v1.waveform_features import UnitWaveformFeaturesSelection\n",
                 "\n",
-                "spikesorting_merge_id = (\n",
-                "    (sgs.SpikeSortingSelection & sorter_keys)\n",
-                "    * SpikeSortingOutput.CurationV1\n",
-                "    * (\n",
-                "        UnitWaveformFeaturesSelection.proj(merge_id=\"spikesorting_merge_id\")\n",
-                "        & feature_key\n",
-                "    )\n",
-                ").fetch(\"merge_id\")\n",
+                "# find the merge ids that correspond to the sorter key restrictions\n",
+                "merge_ids = SpikeSortingOutput().get_restricted_merge_ids(\n",
+                "    sorter_keys, sources=[\"v1\"], as_dict=True\n",
+                ")\n",
                 "\n",
-                "waveform_selection_keys = [\n",
-                "    {\"spikesorting_merge_id\": merge_id, \"features_param_name\": \"amplitude\"}\n",
-                "    for merge_id in spikesorting_merge_id\n",
-                "]\n",
+                "# find the previously populated waveform selection keys that correspond to these sorts\n",
+                "waveform_selection_keys = (\n",
+                "    UnitWaveformFeaturesSelection().proj(merge_id=\"spikesorting_merge_id\")\n",
+                "    & merge_ids\n",
+                "    & feature_key\n",
+                ").fetch(as_dict=True)\n",
+                "for key in waveform_selection_keys:\n",
+                "    key[\"spikesorting_merge_id\"] = key.pop(\"merge_id\")\n",
                 "\n",
                 "UnitWaveformFeaturesSelection & waveform_selection_keys"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -2955,13 +2952,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.18"
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `spyglass_neuro-0.5.1/notebooks/42_Decoding_SortedSpikes.ipynb` & `spyglass_neuro-0.5.2/notebooks/42_Decoding_SortedSpikes.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9905303204702569%*

 * *Differences: {"'cells'": "{1: {'execution_count': 6}, 2: {'source': {insert: [(3, 'sources (e.g. multiple "*

 * *            'tetrode groups or intervals) into a single entry. Here we will group together the '*

 * *            "spiking of multiple tetrode groups to use for decoding.\\n')], delete: [3]}}, 3: "*

 * *            "{'execution_count': 7, 'outputs': {1: {'data': {'text/html': {insert: [(70, "*

 * *            "'<td>=BLOB=</td>\\n'), (71, '<td>=BLOB=</td></tr><tr><td>MS2220180629</td>\\n'), (76, "*

 * *            "'        <p>Total:  […]*

```diff
@@ -17,15 +17,15 @@
                 "\n",
                 "This time, instead of extracting waveform features, we can proceed directly from the SpikeSortingOutput table to specify which units we want to decode. The rest of the decoding process is the same as before.\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "import datajoint as dj\n",
                 "\n",
                 "dj.config.load(\n",
@@ -36,35 +36,26 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## SortedSpikesGroup\n",
                 "\n",
                 "`SortedSpikesGroup` is a child table of `SpikeSortingOutput` in the spikesorting pipeline. It allows us to group the spikesorting results from multiple \n",
-                "sources (e.g. multiple terode groups or intervals) into a single entry. Here we will group together the spiking of multiple tetrode groups to use for decoding.\n",
+                "sources (e.g. multiple tetrode groups or intervals) into a single entry. Here we will group together the spiking of multiple tetrode groups to use for decoding.\n",
                 "\n",
                 "\n",
                 "This table allows us filter units by their annotation labels from curation (e.g only include units labeled \"good\", exclude units labeled \"noise\") by defining parameters from `UnitSelectionParams`. When accessing data through `SortedSpikesGroup` the table will include only units with at least one label in `include_labels` and no labels in `exclude_labels`. We can look at those here:\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "[2024-02-02 12:06:04,725][INFO]: Connecting sambray@lmf-db.cin.ucsf.edu:3306\n",
-                        "[2024-02-02 12:06:04,762][INFO]: Connected sambray@lmf-db.cin.ucsf.edu:3306\n",
-                        "[12:06:05][WARNING] Spyglass: Please update position_tools to >= 0.1.0\n"
-                    ]
-                },
-                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "{'unit_filter_params_name': 'default_exclusion', 'include_labels': [], 'exclude_labels': ['noise', 'mua']}\n"
                     ]
                 },
                 {
@@ -137,30 +128,33 @@
                             "                        </div> </th> </tr> </thead>\n",
                             "            <tbody> <tr> <td>all_units</td>\n",
                             "<td>=BLOB=</td>\n",
                             "<td>=BLOB=</td></tr><tr><td>default_exclusion</td>\n",
                             "<td>=BLOB=</td>\n",
                             "<td>=BLOB=</td></tr><tr><td>exclude_noise</td>\n",
                             "<td>=BLOB=</td>\n",
+                            "<td>=BLOB=</td></tr><tr><td>MS2220180629</td>\n",
+                            "<td>=BLOB=</td>\n",
                             "<td>=BLOB=</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
-                            "        <p>Total: 3</p></div>\n",
+                            "        <p>Total: 4</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "*unit_filter_p include_la exclude_la\n",
                             "+------------+ +--------+ +--------+\n",
                             "all_units      =BLOB=     =BLOB=    \n",
                             "default_exclus =BLOB=     =BLOB=    \n",
                             "exclude_noise  =BLOB=     =BLOB=    \n",
-                            " (Total: 3)"
+                            "MS2220180629   =BLOB=     =BLOB=    \n",
+                            " (Total: 4)"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from spyglass.spikesorting.analysis.v1.group import UnitSelectionParams\n",
                 "\n",
@@ -183,15 +177,15 @@
             "metadata": {},
             "source": [
                 "Now we can make our sorted spikes group with this unit selection parameter"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -305,15 +299,15 @@
                             "+------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+ +------------+\n",
                             "642242ff-5f0e- 75286bf3-f876- 01c5b8e9-933d- mountainsort4  franklab_tetro mediumnwb20230 0a6611b3-c593- 1             \n",
                             "a4b5a94d-ba41- 143dff79-3779- a8a1d29d-ffdf- mountainsort4  franklab_tetro mediumnwb20230 3d782852-a56b- 1             \n",
                             "874775be-df0f- a900c1c8-909d- 747f4eea-6df3- mountainsort4  franklab_tetro mediumnwb20230 9cf9e3cd-7115- 1             \n",
                             " (Total: 3)"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from spyglass.spikesorting.spikesorting_merge import SpikeSortingOutput\n",
                 "import spyglass.spikesorting.v1 as sgs\n",
@@ -322,119 +316,29 @@
                 "\n",
                 "sorter_keys = {\n",
                 "    \"nwb_file_name\": nwb_copy_file_name,\n",
                 "    \"sorter\": \"mountainsort4\",\n",
                 "    \"curation_id\": 1,\n",
                 "}\n",
                 "# check the set of sorting we'll use\n",
-                "(sgs.SpikeSortingSelection & sorter_keys) * SpikeSortingOutput.CurationV1"
+                "(\n",
+                "    sgs.SpikeSortingSelection & sorter_keys\n",
+                ") * SpikeSortingOutput.CurationV1 & sorter_keys"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 6,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "\n",
-                            "    \n",
-                            "    <style type=\"text/css\">\n",
-                            "        .Table{\n",
-                            "            border-collapse:collapse;\n",
-                            "        }\n",
-                            "        .Table th{\n",
-                            "            background: #A0A0A0; color: #ffffff; padding:4px; border:#f0e0e0 1px solid;\n",
-                            "            font-weight: normal; font-family: monospace; font-size: 100%;\n",
-                            "        }\n",
-                            "        .Table td{\n",
-                            "            padding:4px; border:#f0e0e0 1px solid; font-size:100%;\n",
-                            "        }\n",
-                            "        .Table tr:nth-child(odd){\n",
-                            "            background: #ffffff;\n",
-                            "            color: #000000;\n",
-                            "        }\n",
-                            "        .Table tr:nth-child(even){\n",
-                            "            background: #f3f1ff;\n",
-                            "            color: #000000;\n",
-                            "        }\n",
-                            "        /* Tooltip container */\n",
-                            "        .djtooltip {\n",
-                            "        }\n",
-                            "        /* Tooltip text */\n",
-                            "        .djtooltip .djtooltiptext {\n",
-                            "            visibility: hidden;\n",
-                            "            width: 120px;\n",
-                            "            background-color: black;\n",
-                            "            color: #fff;\n",
-                            "            text-align: center;\n",
-                            "            padding: 5px 0;\n",
-                            "            border-radius: 6px;\n",
-                            "            /* Position the tooltip text - see examples below! */\n",
-                            "            position: absolute;\n",
-                            "            z-index: 1;\n",
-                            "        }\n",
-                            "        #primary {\n",
-                            "            font-weight: bold;\n",
-                            "            color: black;\n",
-                            "        }\n",
-                            "        #nonprimary {\n",
-                            "            font-weight: normal;\n",
-                            "            color: white;\n",
-                            "        }\n",
-                            "\n",
-                            "        /* Show the tooltip text when you mouse over the tooltip container */\n",
-                            "        .djtooltip:hover .djtooltiptext {\n",
-                            "            visibility: visible;\n",
-                            "        }\n",
-                            "    </style>\n",
-                            "    \n",
-                            "    <b></b>\n",
-                            "        <div style=\"max-height:1000px;max-width:1500px;overflow:auto;\">\n",
-                            "        <table border=\"1\" class=\"Table\">\n",
-                            "            <thead> <tr style=\"text-align: right;\"> <th> <div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">nwb_file_name</p>\n",
-                            "                            <span class=\"djtooltiptext\">name of the NWB file</span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">unit_filter_params_name</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div></th><th><div class=\"djtooltip\">\n",
-                            "                            <p id=\"primary\">sorted_spikes_group_name</p>\n",
-                            "                            <span class=\"djtooltiptext\"></span>\n",
-                            "                        </div> </th> </tr> </thead>\n",
-                            "            <tbody> <tr> <td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>all_units</td>\n",
-                            "<td>test_group</td> </tr> </tbody>\n",
-                            "        </table>\n",
-                            "        \n",
-                            "        <p>Total: 1</p></div>\n",
-                            "        "
-                        ],
-                        "text/plain": [
-                            "*nwb_file_name *unit_filter_p *sorted_spikes\n",
-                            "+------------+ +------------+ +------------+\n",
-                            "mediumnwb20230 all_units      test_group    \n",
-                            " (Total: 1)"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
             "source": [
-                "from spyglass.decoding.v1.sorted_spikes import SortedSpikesGroup\n",
-                "\n",
-                "SortedSpikesGroup()"
+                "Finding the merge id's corresponding to an interpretable restriction such as `merge_id` or `interval_list` can require several join steps with upstream tables.  To simplify this process we can use the included helper function `SpikeSortingOutput().get_restricted_merge_ids()` to perform the necessary joins and return the matching merge id's"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "    \n",
@@ -498,41 +402,38 @@
                             "                            <p id=\"primary\">unit_filter_params_name</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div></th><th><div class=\"djtooltip\">\n",
                             "                            <p id=\"primary\">sorted_spikes_group_name</p>\n",
                             "                            <span class=\"djtooltiptext\"></span>\n",
                             "                        </div> </th> </tr> </thead>\n",
                             "            <tbody> <tr> <td>mediumnwb20230802_.nwb</td>\n",
-                            "<td>all_units</td>\n",
-                            "<td>test_group</td></tr><tr><td>mediumnwb20230802_.nwb</td>\n",
                             "<td>default_exclusion</td>\n",
                             "<td>test_group</td> </tr> </tbody>\n",
                             "        </table>\n",
                             "        \n",
-                            "        <p>Total: 2</p></div>\n",
+                            "        <p>Total: 1</p></div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "*nwb_file_name *unit_filter_p *sorted_spikes\n",
                             "+------------+ +------------+ +------------+\n",
-                            "mediumnwb20230 all_units      test_group    \n",
                             "mediumnwb20230 default_exclus test_group    \n",
-                            " (Total: 2)"
+                            " (Total: 1)"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# get the merge_ids for the selected sorting\n",
-                "spikesorting_merge_ids = (\n",
-                "    (sgs.SpikeSortingSelection & sorter_keys) * SpikeSortingOutput.CurationV1\n",
-                ").fetch(\"merge_id\")\n",
+                "spikesorting_merge_ids = SpikeSortingOutput().get_restricted_merge_ids(\n",
+                "    sorter_keys, restrict_by_artifact=False\n",
+                ")\n",
                 "\n",
                 "# create a new sorted spikes group\n",
                 "unit_filter_params_name = \"default_exclusion\"\n",
                 "SortedSpikesGroup().create_group(\n",
                 "    group_name=\"test_group\",\n",
                 "    nwb_file_name=nwb_copy_file_name,\n",
                 "    keys=[\n",
@@ -1532,13 +1433,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.18"
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `spyglass_neuro-0.5.1/notebooks/README.md` & `spyglass_neuro-0.5.2/notebooks/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,22 +51,22 @@
 This series of notebooks covers the process of decoding the position of the
 animal from spiking data. It relies on the position data from the Position
 pipeline and the output of spike sorting from the Spike Sorting pipeline.
 Decoding can be from sorted or from unsorted data using spike waveform features
 (so-called clusterless decoding).
 
 The first notebook
-([Extracting Clusterless Waveform Features](./41_Extracting_Clusterless_Waveform_Features.ipynb))
+([Extracting Clusterless Waveform Features](./40_Extracting_Clusterless_Waveform_Features.ipynb))
 in this series shows how to retrieve the spike waveform features used for
 clusterless decoding.
 
-The second notebook ([Clusterless Decoding](./42_Decoding_Clusterless.ipynb))
+The second notebook ([Clusterless Decoding](./41_Decoding_Clusterless.ipynb))
 shows a detailed example of how to decode the position of the animal from the
 spike waveform features. The third notebook
-([Decoding](./43_Decoding_SortedSpikes.ipynb)) shows how to decode the position
+([Decoding](./42_Decoding_SortedSpikes.ipynb)) shows how to decode the position
 of the animal from the sorted spikes.
 
 ## Developer note
 
 The `py_scripts` directory contains the same notebook data in `.py` form to
 facilitate GitHub PR reviews. To update them, run the following from the root
 Spyglass directory
@@ -75,7 +75,15 @@
 pip install jupytext
 jupytext --to py notebooks/*ipynb
 mv notebooks/*py notebooks/py_scripts
 black .
 ```
 
 Unfortunately, jupytext-generated py script are not black-compliant by default.
+
+You can ensure black compliance with the `pre-commit` hook by running
+
+```bash
+pip install pre-commit
+```
+
+This will run black whenever you commit changes to the repository.
```

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/00_Setup.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/00_Setup.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/01_Insert_Data.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/01_Insert_Data.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/02_Data_Sync.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/02_Data_Sync.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/03_Merge_Tables.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/03_Merge_Tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ---
 # jupyter:
 #   jupytext:
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.16.0
+#       jupytext_version: 1.15.2
 #   kernelspec:
 #     display_name: spy
 #     language: python
 #     name: python3
 # ---
 
 # # Merge Tables
@@ -133,25 +133,25 @@
 
 LFPOutput.merge_view()
 
 # UUIDs help retain unique entries across all part tables. We can fetch NWB file
 # by referencing this or other features.
 #
 
-uuid_key = LFPOutput.fetch(limit=1, as_dict=True)[-1]
+uuid_key = (LFPOutput & nwb_file_dict).fetch(limit=1, as_dict=True)[-1]
 restrict = LFPOutput & uuid_key
 restrict
 
-result1 = restrict.fetch_nwb()
+result1 = restrict.fetch_nwb(restrict.fetch1("KEY"))
 result1
 
 nwb_key = LFPOutput.merge_restrict(nwb_file_dict).fetch(as_dict=True)[0]
 nwb_key
 
-result2 = (LFPOutput & nwb_key).fetch_nwb()
+result2 = LFPOutput().fetch_nwb(nwb_key)
 result2 == result1
 
 # ## Selecting data
 #
 
 # There are also functions for retrieving part/parent table(s) and fetching data.
 #
```

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/04_PopulateConfigFile.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/04_PopulateConfigFile.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/20_Position_Trodes.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/20_Position_Trodes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/21_DLC.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/21_DLC.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/22_DLC_Loop.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/22_DLC_Loop.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/24_Linearization.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/24_Linearization.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/30_LFP.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/30_LFP.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/31_Theta.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/31_Theta.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/41_Extracting_Clusterless_Waveform_Features.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/42_Decoding_Clusterless.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/42_Decoding_Clusterless.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/43_Decoding_SortedSpikes.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/43_Decoding_SortedSpikes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/notebooks/py_scripts/51_MUA_Detection.py` & `spyglass_neuro-0.5.2/notebooks/py_scripts/51_MUA_Detection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/settings.py` & `spyglass_neuro-0.5.2/src/spyglass/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,25 +56,27 @@
         self._debug_mode = kwargs.get("debug_mode", False)
         self._test_mode = kwargs.get("test_mode", False)
         self._dlc_base = None
         self.load_failed = False
 
         self.relative_dirs = {
             # {PREFIX}_{KEY}_DIR, default dir relative to base_dir
+            # NOTE: Adding new dir requires edit to HHMI hub
             "spyglass": {
                 "raw": "raw",
                 "analysis": "analysis",
                 "recording": "recording",
                 "sorting": "spikesorting",
                 "waveforms": "waveforms",
                 "temp": "tmp",
                 "video": "video",
+                "export": "export",
             },
             "kachery": {
-                "cloud": "kachery_storage",
+                "cloud": ".kachery-cloud",
                 "storage": "kachery_storage",
                 "temp": "tmp",
             },
             "dlc": {
                 "project": "projects",
                 "video": "video",
                 "output": "output",
@@ -177,18 +179,21 @@
 
                 env_loc = (  # Ignore env vars if base was passed to func
                     os.environ.get(dir_env_fmt)
                     if not self.supplied_base_dir
                     else None
                 )
 
+                source_config = (
+                    dj_dlc
+                    if prefix == "dlc"
+                    else dj_kachery if prefix == "kachery" else dj_spyglass
+                )
                 dir_location = (
-                    dj_spyglass.get(dir)
-                    or dj_kachery.get(dir)
-                    or dj_dlc.get(dir)
+                    source_config.get(dir)
                     or env_loc
                     or str(Path(this_base) / dir_str)
                 ).replace('"', "")
 
                 config_dirs.update({dir_env_fmt: str(dir_location)})
 
         kachery_zone_dict = {
@@ -452,14 +457,15 @@
                     "raw": self.raw_dir,
                     "analysis": self.analysis_dir,
                     "recording": self.recording_dir,
                     "sorting": self.sorting_dir,
                     "waveforms": self.waveforms_dir,
                     "temp": self.temp_dir,
                     "video": self.video_dir,
+                    "export": self.export_dir,
                 },
                 "kachery_dirs": {
                     "cloud": self.config.get(
                         self.dir_to_var("cloud", "kachery")
                     ),
                     "storage": self.config.get(
                         self.dir_to_var("storage", "kachery")
@@ -510,14 +516,18 @@
         return self.config.get(self.dir_to_var("temp"))
 
     @property
     def video_dir(self) -> str:
         return self.config.get(self.dir_to_var("video"))
 
     @property
+    def export_dir(self) -> str:
+        return self.config.get(self.dir_to_var("export"))
+
+    @property
     def debug_mode(self) -> bool:
         """Returns True if debug_mode is set.
 
         Supports skipping inserts for Dockerized development.
         """
         return self._debug_mode
 
@@ -553,26 +563,28 @@
     raw_dir = None
     recording_dir = None
     temp_dir = None
     analysis_dir = None
     sorting_dir = None
     waveforms_dir = None
     video_dir = None
+    export_dir = None
     dlc_project_dir = None
     dlc_video_dir = None
     dlc_output_dir = None
 else:
     config = sg_config.config
     base_dir = sg_config.base_dir
     raw_dir = sg_config.raw_dir
     recording_dir = sg_config.recording_dir
     temp_dir = sg_config.temp_dir
     analysis_dir = sg_config.analysis_dir
     sorting_dir = sg_config.sorting_dir
     waveforms_dir = sg_config.waveforms_dir
     video_dir = sg_config.video_dir
+    export_dir = sg_config.export_dir
     debug_mode = sg_config.debug_mode
     test_mode = sg_config.test_mode
     prepopulate = config.get("prepopulate", False)
     dlc_project_dir = sg_config.dlc_project_dir
     dlc_video_dir = sg_config.dlc_video_dir
     dlc_output_dir = sg_config.dlc_output_dir
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/cli/cli.py` & `spyglass_neuro-0.5.2/src/spyglass/cli/cli.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/__init__.py` & `spyglass_neuro-0.5.2/src/spyglass/common/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,17 +38,15 @@
     interval_list_intersect,
     interval_list_union,
     intervals_by_length,
 )
 from spyglass.common.common_lab import Institution, Lab, LabMember, LabTeam
 from spyglass.common.common_nwbfile import (
     AnalysisNwbfile,
-    AnalysisNwbfileKachery,
     Nwbfile,
-    NwbfileKachery,
 )
 from spyglass.common.common_position import (
     IntervalLinearizationSelection,
     IntervalLinearizedPosition,
     IntervalPositionInfo,
     IntervalPositionInfoSelection,
     LinearizationParameters,
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_behav.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_behav.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_device.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_device.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_dio.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_dio.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_ephys.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_ephys.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,14 +407,15 @@
     lfp_object_id: varchar(40)  # the NWB object ID for loading this object from the file
     lfp_sampling_rate: float    # the sampling rate, in HZ
     """
 
     def make(self, key):
         # get the NWB object with the data; FIX: change to fetch with
         # additional infrastructure
+        lfp_file_name = AnalysisNwbfile().create(key["nwb_file_name"])  # logged
 
         rawdata = Raw().nwb_object(key)
         sampling_rate, interval_list_name = (Raw() & key).fetch1(
             "sampling_rate", "interval_list_name"
         )
         sampling_rate = int(np.round(sampling_rate))
 
@@ -461,16 +462,14 @@
             )
             return None
         # get the list of selected LFP Channels from LFPElectrode
         electrode_keys = (LFPSelection.LFPElectrode & key).fetch("KEY")
         electrode_id_list = list(k["electrode_id"] for k in electrode_keys)
         electrode_id_list.sort()
 
-        lfp_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
-
         lfp_file_abspath = AnalysisNwbfile().get_abs_path(lfp_file_name)
         (
             lfp_object_id,
             timestamp_interval,
         ) = FirFilterParameters().filter_data_nwb(
             lfp_file_abspath,
             rawdata,
@@ -498,14 +497,15 @@
                 "nwb_file_name": key["nwb_file_name"],
                 "interval_list_name": key["interval_list_name"],
                 "valid_times": lfp_valid_times,
                 "pipeline": "lfp_v0",
             },
             replace=True,
         )
+        AnalysisNwbfile().log(key, table=self.full_table_name)
         self.insert1(key)
 
     def nwb_object(self, key):
         # return the NWB object in the raw NWB file
         lfp_file_name = (
             LFP() & {"nwb_file_name": key["nwb_file_name"]}
         ).fetch1("analysis_file_name")
@@ -662,14 +662,18 @@
     ---
     -> AnalysisNwbfile
     -> IntervalList
     filtered_data_object_id: varchar(40)  # the NWB object ID for loading this object from the file
     """
 
     def make(self, key):
+        # create the analysis nwb file to store the results.
+        lfp_band_file_name = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
         # get the NWB object with the lfp data; FIX: change to fetch with additional infrastructure
         lfp_object = (
             LFP() & {"nwb_file_name": key["nwb_file_name"]}
         ).fetch_nwb()[0]["lfp"]
 
         # get the electrodes to be filtered and their references
         lfp_band_elect_id, lfp_band_ref_id = (
@@ -770,16 +774,14 @@
         filter_coeff = filter[0]["filter_coeff"]
         if len(filter_coeff) == 0:
             logger.info(
                 f"Error in LFPBand: no filter found with data sampling rate of {lfp_band_sampling_rate}"
             )
             return None
 
-        # create the analysis nwb file to store the results.
-        lfp_band_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
         lfp_band_file_abspath = AnalysisNwbfile().get_abs_path(
             lfp_band_file_name
         )
         # filter the data and write to an the nwb file
         filtered_data, new_timestamps = FirFilterParameters().filter_data(
             timestamps,
             lfp_data,
@@ -849,14 +851,15 @@
             # check that the valid times are the same
             assert np.isclose(
                 tmp_valid_times[0], lfp_band_valid_times
             ).all(), (
                 "previously saved lfp band times do not match current times"
             )
 
+        AnalysisNwbfile().log(lfp_band_file_name, table=self.full_table_name)
         self.insert1(key)
 
     def fetch1_dataframe(self, *attrs, **kwargs):
         filtered_nwb = self.fetch_nwb()[0]
         return pd.DataFrame(
             filtered_nwb["filtered_data"].data,
             index=pd.Index(
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_filter.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_filter.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_interval.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 ax.plot(interval, [interval_y, interval_y])
                 ax.scatter(
                     interval, [interval_y, interval_y], alpha=0.8, zorder=2
                 )
                 ax.text(
                     interval[0] + np.diff(interval)[0] / 2,
                     interval_y,
-                    epoch.strip(" valid times"),
+                    epoch.replace(" valid times", ""),
                     ha="center",
                     va="bottom",
                 )
 
         ax.set_ylim((-0.25, 2.25))
         ax.set_yticks(np.arange(3))
         ax.set_yticklabels(["pos valid times", "raw data valid times", "epoch"])
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_lab.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_lab.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             skip_duplicates=True,
         )
 
     def _load_admin(cls):
         """Load admin list."""
         cls._admin = list(
             (cls.LabMemberInfo & {"admin": True}).fetch("datajoint_user_name")
-        )
+        ) + ["root"]
 
     @property
     def admin(cls) -> list:
         """Return the list of admin users.
 
         Note: This is cached. If adding a new admin, run _load_admin
         """
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_nwbfile.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_nwbfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import os
 import random
 import stat
 import string
 from pathlib import Path
+from time import time
 
 import datajoint as dj
+import h5py
 import numpy as np
 import pandas as pd
 import pynwb
 import spikeinterface as si
 from hdmf.common import DynamicTable
 
+from spyglass import __version__ as sg_version
 from spyglass.settings import analysis_dir, raw_dir
 from spyglass.utils import SpyglassMixin, logger
 from spyglass.utils.dj_helper_fn import get_child_tables
 from spyglass.utils.nwb_helper_fn import get_electrode_indices, get_nwb_file
 
 schema = dj.schema("common_nwbfile")
 
@@ -147,28 +150,30 @@
 
 # TODO: add_to_kachery will not work because we can't update the entry after it's been used in another table.
 # We therefore need another way to keep track of the
 @schema
 class AnalysisNwbfile(SpyglassMixin, dj.Manual):
     definition = """
     # Table for holding the NWB files that contain results of analysis, such as spike sorting.
-    analysis_file_name: varchar(64)               # name of the file
+    analysis_file_name: varchar(64)                # name of the file
     ---
     -> Nwbfile                                     # name of the parent NWB file. Used for naming and metadata copy
     analysis_file_abs_path: filepath@analysis      # the full path to the file
     analysis_file_description = "": varchar(2000)  # an optional description of this analysis
     analysis_parameters = NULL: blob               # additional relevant parameters. Currently used only for analyses
                                                    # that span multiple NWB files
     INDEX (analysis_file_abs_path)
     """
-    # NOTE the INDEX above is implicit from filepath@... above but needs to be explicit
-    # so that alter() can work
+    # NOTE the INDEX above is implicit from filepath@...
+    # above but needs to be explicit so that alter() can work
 
     # See #630, #664. Excessive key length.
 
+    _creation_times = {}
+
     def create(self, nwb_file_name):
         """Open the NWB file, create a copy, write the copy to disk and return the name of the new file.
 
         Note that this does NOT add the file to the schema; that needs to be done after data are written to it.
 
         Parameters
         ----------
@@ -176,46 +181,65 @@
             The name of an NWB file to be copied.
 
         Returns
         -------
         analysis_file_name : str
             The name of the new NWB file.
         """
+        # To allow some times to occur before create
+        creation_time = self._creation_times.pop("pre_create_time", time())
+
         nwb_file_abspath = Nwbfile.get_abs_path(nwb_file_name)
+        alter_source_script = False
         with pynwb.NWBHDF5IO(
             path=nwb_file_abspath, mode="r", load_namespaces=True
         ) as io:
             nwbf = io.read()
             # pop off the unnecessary elements to save space
             nwb_fields = nwbf.fields
             for field in nwb_fields:
                 if field not in NWB_KEEP_FIELDS:
                     nwb_object = getattr(nwbf, field)
                     if isinstance(nwb_object, pynwb.core.LabelledDict):
                         for module in list(nwb_object.keys()):
                             nwb_object.pop(module)
+            # add the version of spyglass that created this file
+            if nwbf.source_script is None:
+                nwbf.source_script = f"spyglass={sg_version}"
+            else:
+                alter_source_script = True
 
             analysis_file_name = self.__get_new_file_name(nwb_file_name)
             # write the new file
             logger.info(f"Writing new NWB file {analysis_file_name}")
             analysis_file_abs_path = AnalysisNwbfile.get_abs_path(
                 analysis_file_name
             )
             # export the new NWB file
             with pynwb.NWBHDF5IO(
                 path=analysis_file_abs_path, mode="w", manager=io.manager
             ) as export_io:
                 export_io.export(io, nwbf)
+        if alter_source_script:
+            self._alter_spyglass_version(analysis_file_abs_path)
 
         # change the permissions to only allow owner to write
         permissions = stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IROTH
         os.chmod(analysis_file_abs_path, permissions)
 
+        self._creation_times[analysis_file_name] = creation_time
+
         return analysis_file_name
 
+    @staticmethod
+    def _alter_spyglass_version(nwb_file_path):
+        """Change the source script to the current version of spyglass"""
+        with h5py.File(nwb_file_path, "a") as f:
+            f["/general/source_script"][()] = f"spyglass={sg_version}"
+
     @classmethod
     def __get_new_file_name(cls, nwb_file_name):
         # each file ends with a random string of 10 digits, so we generate that
         # string and redo if by some miracle it's already there
         file_in_table = True
         while file_in_table:
             analysis_file_name = (
@@ -280,39 +304,52 @@
         Parameters
         ----------
         nwb_file_name : str
             The name of the parent NWB file.
         analysis_file_name : str
             The name of the analysis NWB file that was created.
         """
-        key = dict()
-        key["nwb_file_name"] = nwb_file_name
-        key["analysis_file_name"] = analysis_file_name
-        key["analysis_file_description"] = ""
-        key["analysis_file_abs_path"] = AnalysisNwbfile.get_abs_path(
-            analysis_file_name
-        )
+        key = {
+            "nwb_file_name": nwb_file_name,
+            "analysis_file_name": analysis_file_name,
+            "analysis_file_description": "",
+            "analysis_file_abs_path": AnalysisNwbfile.get_abs_path(
+                analysis_file_name
+            ),
+        }
         self.insert1(key)
 
-    @staticmethod
-    def get_abs_path(analysis_nwb_file_name):
+    @classmethod
+    def get_abs_path(cls, analysis_nwb_file_name):
         """Return the absolute path for a stored analysis NWB file given just the file name.
 
         The spyglass config from settings.py must be set.
 
         Parameters
         ----------
         analysis_nwb_file_name : str
             The name of the NWB file that has been inserted into the AnalysisNwbfile() schema
 
         Returns
         -------
         analysis_nwb_file_abspath : str
             The absolute path for the given file name.
         """
+        # If an entry exists in the database get the stored datajoint filepath
+        file_key = {"analysis_file_name": analysis_nwb_file_name}
+        if cls & file_key:
+            try:
+                # runs if file exists locally
+                return (cls & file_key).fetch1("analysis_file_abs_path")
+            except FileNotFoundError as e:
+                # file exists in database but not locally
+                # parse the intended path from the error message
+                return str(e).split(": ")[1].replace("'", "")
+
+        # File not in database, define what it should be
         # see if the file exists and is stored in the base analysis dir
         test_path = f"{analysis_dir}/{analysis_nwb_file_name}"
 
         if os.path.exists(test_path):
             return test_path
         else:
             # use the new path
@@ -322,16 +359,16 @@
             if not analysis_file_base_path.exists():
                 os.mkdir(str(analysis_file_base_path))
             return str(analysis_file_base_path / analysis_nwb_file_name)
 
     def add_nwb_object(
         self, analysis_file_name, nwb_object, table_name="pandas_table"
     ):
-        # TODO: change to add_object with checks for object type and a name parameter, which should be specified if
-        # it is not an NWB container
+        # TODO: change to add_object with checks for object type and a name
+        # parameter, which should be specified if it is not an NWB container
         """Add an NWB object to the analysis file in the scratch area and returns the NWB object ID
 
         Parameters
         ----------
         analysis_file_name : str
             The name of the analysis NWB file.
         nwb_object : pynwb.core.NWBDataInterface
@@ -423,15 +460,18 @@
                 if metrics is not None:
                     for metric in metrics:
                         if metrics[metric]:
                             unit_ids = np.array(list(metrics[metric].keys()))
                             metric_values = np.array(
                                 list(metrics[metric].values())
                             )
-                            # sort by unit_ids and apply that sorting to values to ensure that things go in the right order
+
+                            # sort by unit_ids and apply that sorting to values
+                            # to ensure that things go in the right order
+
                             metric_values = metric_values[np.argsort(unit_ids)]
                             logger.info(
                                 f"Adding metric {metric} : {metric_values}"
                             )
                             nwbf.add_unit_column(
                                 name=metric,
                                 description=f"{metric} metric",
@@ -635,46 +675,94 @@
         child_tables = get_child_tables(AnalysisNwbfile)
         (AnalysisNwbfile - child_tables).delete_quick()
 
         # a separate external files clean up required - this is to be done
         # during times when no other transactions are in progress.
         AnalysisNwbfile.cleanup(True)
 
-        # also check to see whether there are directories in the spikesorting folder with this
+    def log(self, analysis_file_name, table=None):
+        """Passthrough to the AnalysisNwbfileLog table. Avoid new imports."""
+        if isinstance(analysis_file_name, dict):
+            analysis_file_name = analysis_file_name["analysis_file_name"]
+        time_delta = time() - self._creation_times[analysis_file_name]
+        file_size = Path(self.get_abs_path(analysis_file_name)).stat().st_size
+
+        AnalysisNwbfileLog().log(
+            analysis_file_name=analysis_file_name,
+            time_delta=time_delta,
+            file_size=file_size,
+            table=table,
+        )
+
+    def increment_access(self, keys, table=None):
+        """Passthrough to the AnalysisNwbfileLog table. Avoid new imports."""
+        if not isinstance(keys, list):
+            key = [keys]
+
+        for key in keys:
+            AnalysisNwbfileLog().increment_access(key, table=table)
 
 
 @schema
-class NwbfileKachery(SpyglassMixin, dj.Computed):
+class AnalysisNwbfileLog(dj.Manual):
     definition = """
-    -> Nwbfile
+    id: int auto_increment
     ---
-    nwb_file_uri: varchar(200)  # the uri the NWB file for kachery
+    -> AnalysisNwbfile
+    dj_user                       : varchar(64) # user who created the file
+    timestamp = CURRENT_TIMESTAMP : timestamp   # when the file was created
+    table = null                  : varchar(64) # creating table
+    time_delta = null             : float       # how long it took to create
+    file_size = null              : float       # size of the file in bytes
+    accessed = 0                  : int         # n times accessed
+    unique index (analysis_file_name)
     """
 
-    def make(self, key):
-        import kachery_client as kc
+    def log(
+        self,
+        analysis_file_name=None,
+        time_delta=None,
+        file_size=None,
+        table=None,
+    ):
+        """Log the creation of an analysis NWB file.
 
-        logger.info(f'Linking {key["nwb_file_name"]} and storing in kachery...')
-        key["nwb_file_uri"] = kc.link_file(
-            Nwbfile().get_abs_path(key["nwb_file_name"])
+        Parameters
+        ----------
+        analysis_file_name : str
+            The name of the analysis NWB file.
+        """
+        self.insert1(
+            {
+                "dj_user": dj.config["database.user"],
+                "analysis_file_name": analysis_file_name,
+                "time_delta": time_delta,
+                "file_size": file_size,
+                "table": table,
+            }
         )
-        self.insert1(key)
 
+    def increment_access(self, key, table=None):
+        """Increment the accessed field for the given analysis file name.
 
-@schema
-class AnalysisNwbfileKachery(SpyglassMixin, dj.Computed):
-    definition = """
-    -> AnalysisNwbfile
-    ---
-    analysis_file_uri: varchar(200)  # the uri of the file
-    """
+        Parameters
+        ----------
+        key : Union[str, dict]
+            The name of the analysis NWB file, or a key to the table.
+        table : str, optional
+            The table that created the file.
+        """
+        if isinstance(key, str):
+            key = {"analysis_file_name": key}
 
-    def make(self, key):
-        import kachery_client as kc
+        if not (query := self & key):
+            self.log(**key, table=table)
+        entries = query.fetch(as_dict=True)
 
-        logger.info(
-            f'Linking {key["analysis_file_name"]} and storing in kachery...'
-        )
-        key["analysis_file_uri"] = kc.link_file(
-            AnalysisNwbfile().get_abs_path(key["analysis_file_name"])
-        )
-        self.insert1(key)
+        inserts = []
+        for entry in entries:
+            entry["accessed"] += 1
+            if table and not entry.get("table"):
+                entry["table"] = table
+            inserts.append(entry)
+
+        self.insert(inserts, replace=True)
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_position.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,17 @@
     head_orientation_object_id : varchar(40)
     head_velocity_object_id : varchar(40)
     """
 
     def make(self, key):
         logger.info(f"Computing position for: {key}")
 
-        analysis_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
+        analysis_file_name = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
 
         raw_position = RawPosition.PosObject & key
         spatial_series = raw_position.fetch_nwb()[0]["raw_position"]
         spatial_df = raw_position.fetch1_dataframe()
 
         position_info_parameters = (PositionInfoParameters() & key).fetch1()
 
@@ -114,14 +116,16 @@
                     analysis_fname=analysis_file_name,
                 ),
             )
         )
 
         AnalysisNwbfile().add(key["nwb_file_name"], analysis_file_name)
 
+        AnalysisNwbfile().log(key, table=self.full_table_name)
+
         self.insert1(key)
 
     @staticmethod
     def generate_pos_components(
         spatial_series,
         position_info,
         analysis_fname,
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_region.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_region.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_ripple.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_ripple.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_sensors.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_sensors.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_session.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_session.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_subject.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_subject.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/common_task.py` & `spyglass_neuro-0.5.2/src/spyglass/common/common_task.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/populate_all_common.py` & `spyglass_neuro-0.5.2/src/spyglass/common/populate_all_common.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/signal_processing.py` & `spyglass_neuro-0.5.2/src/spyglass/common/signal_processing.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/common/prepopulate/prepopulate.py` & `spyglass_neuro-0.5.2/src/spyglass/common/prepopulate/prepopulate.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/data_import/insert_sessions.py` & `spyglass_neuro-0.5.2/src/spyglass/data_import/insert_sessions.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/__init__.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/decoding_merge.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/decoding_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v0/clusterless.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/clusterless.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,18 @@
     -> UnitMarkParameters
     ---
     -> AnalysisNwbfile
     marks_object_id: varchar(40) # the NWB object that stores the marks
     """
 
     def make(self, key):
+        # create a new AnalysisNwbfile and a timeseries for the marks and save
+        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
         # get the list of mark parameters
         mark_param = (MarkParameters & key).fetch1()
 
         # check that the mark type is supported
         if not MarkParameters().supported_mark_type(mark_param["mark_type"]):
             Warning(
                 f'Mark type {mark_param["mark_type"]} not supported; skipping'
@@ -203,29 +207,26 @@
             timestamps = timestamps[sorted_timestamp_ind]
 
         if "threshold" in mark_param["mark_param_dict"]:
             timestamps, marks = UnitMarks._threshold(
                 timestamps, marks, mark_param["mark_param_dict"]
             )
 
-        # create a new AnalysisNwbfile and a timeseries for the marks and save
-        key["analysis_file_name"] = AnalysisNwbfile().create(
-            key["nwb_file_name"]
-        )
         nwb_object = pynwb.TimeSeries(
             name="marks",
             data=marks,
             unit="uV",
             timestamps=timestamps,
             description="spike features for clusterless decoding",
         )
         key["marks_object_id"] = AnalysisNwbfile().add_nwb_object(
             key["analysis_file_name"], nwb_object
         )
         AnalysisNwbfile().add(key["nwb_file_name"], key["analysis_file_name"])
+        AnalysisNwbfile().log(key, table=self.full_table_name)
         self.insert1(key)
 
     def fetch1_dataframe(self) -> pd.DataFrame:
         """Convenience function for returning the marks in a readable format"""
         return self.fetch_dataframe()[0]
 
     def fetch_dataframe(self) -> list[pd.DataFrame]:
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v0/core.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/core.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v0/dj_decoder_conversion.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/dj_decoder_conversion.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v0/sorted_spikes.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/sorted_spikes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v0/visualization.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v0/visualization_1D_view.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_1D_view.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v0/visualization_2D_view.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v0/visualization_2D_view.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v1/clusterless.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/clusterless.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             results["discrete_transition_coefficients"] = (
                 classifier.discrete_transition_coefficients_
             )
 
         # Insert results
         # in future use https://github.com/rly/ndx-xarray and analysis nwb file?
 
-        nwb_file_name = key["nwb_file_name"].strip("_.nwb")
+        nwb_file_name = key["nwb_file_name"].replace("_.nwb", "")
 
         # Generate a unique path for the results file
         path_exists = True
         while path_exists:
             results_path = (
                 Path(config["SPYGLASS_ANALYSIS_DIR"])
                 / nwb_file_name
@@ -462,15 +462,15 @@
 
     def get_ahead_behind_distance(self):
         # TODO: allow specification of specific time interval
         # TODO: allow specification of track graph
         # TODO: Handle decode intervals, store in table
 
         classifier = self.fetch_model()
-        results = self.fetch_results()
+        results = self.fetch_results().squeeze()
         posterior = results.acausal_posterior.unstack("state_bins").sum("state")
 
         if getattr(classifier.environments[0], "track_graph") is not None:
             linear_position_info = self.fetch_linear_position_info(
                 self.fetch1("KEY")
             )
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v1/core.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/core.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v1/dj_decoder_conversion.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/dj_decoder_conversion.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v1/sorted_spikes.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/sorted_spikes.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             results["discrete_transition_coefficients"] = (
                 classifier.discrete_transition_coefficients_
             )
 
         # Insert results
         # in future use https://github.com/rly/ndx-xarray and analysis nwb file?
 
-        nwb_file_name = key["nwb_file_name"].strip("_.nwb")
+        nwb_file_name = key["nwb_file_name"].replace("_.nwb", "")
 
         # Generate a unique path for the results file
         path_exists = True
         while path_exists:
             results_path = (
                 Path(config["SPYGLASS_ANALYSIS_DIR"])
                 / nwb_file_name
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/decoding/v1/waveform_features.py` & `spyglass_neuro-0.5.2/src/spyglass/decoding/v1/waveform_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from itertools import chain
+from time import time
 
 import datajoint as dj
 import numpy as np
 import pandas as pd
 import pynwb
 import spikeinterface as si
 
@@ -98,14 +99,15 @@
     -> UnitWaveformFeaturesSelection
     ---
     -> AnalysisNwbfile
     object_id: varchar(40) # the NWB object that stores the waveforms
     """
 
     def make(self, key):
+        AnalysisNwbfile()._creation_times["pre_create_time"] = time()
         # get the list of feature parameters
         params = (WaveformFeaturesParams & key).fetch1("params")
 
         # check that the feature type is supported
         if not WaveformFeaturesParams.check_supported_waveform_features(
             params["waveform_features_params"]
         ):
@@ -160,14 +162,16 @@
             waveform_features,
         )
 
         AnalysisNwbfile().add(
             nwb_file_name,
             key["analysis_file_name"],
         )
+        AnalysisNwbfile().log(key, table=self.full_table_name)
+
         self.insert1(key)
 
     @staticmethod
     def _fetch_waveform(
         merge_key: dict, waveform_extraction_params: dict
     ) -> si.WaveformExtractor:
         # get the recording from the parent table
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/lfp_electrode.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_electrode.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/lfp_imported.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_imported.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/lfp_merge.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/lfp_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/analysis/v1/lfp_band.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/analysis/v1/lfp_band.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,18 @@
     ---
     -> AnalysisNwbfile               # the name of the nwb file with the lfp data
     -> IntervalList                  # the final interval list of valid times for the data
     lfp_band_object_id: varchar(40)  # the NWB object ID for loading this object from the file
     """
 
     def make(self, key):
+        # create the analysis nwb file to store the results.
+        lfp_band_file_name = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
         # get the NWB object with the lfp data; FIX: change to fetch with additional infrastructure
         lfp_key = {"merge_id": key["lfp_merge_id"]}
         lfp_object = (LFPOutput & lfp_key).fetch_nwb()[0]["lfp"]
 
         # get the electrodes to be filtered and their references
         lfp_band_elect_id, lfp_band_ref_id = (
             LFPBandSelection().LFPBandElectrode() & key
@@ -272,16 +276,14 @@
         if len(filter_coeff) == 0:
             logger.error(
                 "LFPBand: no filter found with data "
                 + f"sampling rate of {lfp_band_sampling_rate}"
             )
             return None
 
-        # create the analysis nwb file to store the results.
-        lfp_band_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
         lfp_band_file_abspath = AnalysisNwbfile().get_abs_path(
             lfp_band_file_name
         )
         # filter the data and write to an the nwb file
         filtered_data, new_timestamps = FirFilterParameters().filter_data(
             timestamps,
             lfp_data,
@@ -358,14 +360,15 @@
             # check that the valid times are the same
             assert np.isclose(
                 tmp_valid_times[0], lfp_band_valid_times
             ).all(), (
                 "previously saved lfp band times do not match current times"
             )
 
+        AnalysisNwbfile().log(key, table=self.full_table_name)
         self.insert1(key)
 
     def fetch1_dataframe(self, *attrs, **kwargs):
         """Fetches the filtered data as a dataframe"""
         filtered_nwb = self.fetch_nwb()[0]
         return pd.DataFrame(
             filtered_nwb["lfp_band"].data,
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     -> AnalysisNwbfile          # the name of the nwb file with the lfp data
     -> IntervalList             # the final interval list of valid times for the data
     lfp_object_id: varchar(40)  # the NWB object ID for loading this object from the file
     lfp_sampling_rate: float    # the sampling rate, in HZ
     """
 
     def make(self, key):
+        lfp_file_name = AnalysisNwbfile().create(key["nwb_file_name"])  # logged
         # get the NWB object with the data
         nwbf_key = {"nwb_file_name": key["nwb_file_name"]}
         rawdata = (Raw & nwbf_key).fetch_nwb()[0]["raw"]
 
         # CBroz: assumes Raw sampling rate matches FirFilterParameters set?
         #        if we just pull rate from Raw, why include in Param table?
         sampling_rate, raw_interval_list_name = (Raw & nwbf_key).fetch1(
@@ -123,16 +124,14 @@
             return None  # See #849
 
         # get the list of selected LFP Channels from LFPElectrode
         electrode_keys = (LFPElectrodeGroup.LFPElectrode & key).fetch("KEY")
         electrode_id_list = list(k["electrode_id"] for k in electrode_keys)
         electrode_id_list.sort()
 
-        lfp_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
-
         lfp_file_abspath = AnalysisNwbfile().get_abs_path(lfp_file_name)
         (
             lfp_object_id,
             timestamp_interval,
         ) = FirFilterParameters().filter_data_nwb(
             lfp_file_abspath,
             rawdata,
@@ -189,14 +188,15 @@
 
         # finally, we insert this into the LFP output table.
         from spyglass.lfp.lfp_merge import LFPOutput
 
         orig_key["analysis_file_name"] = lfp_file_name
         orig_key["lfp_object_id"] = lfp_object_id
         LFPOutput.insert1(orig_key)
+        AnalysisNwbfile().log(key, table=self.full_table_name)
 
     def fetch1_dataframe(self, *attrs, **kwargs):
         nwb_lfp = self.fetch_nwb()[0]
         return pd.DataFrame(
             nwb_lfp["lfp"].data,
             index=pd.Index(nwb_lfp["lfp"].timestamps, name="time"),
         )
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp_artifact.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_MAD_detection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py` & `spyglass_neuro-0.5.2/src/spyglass/lfp/v1/lfp_artifact_difference_detection.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/linearization/merge.py` & `spyglass_neuro-0.5.2/src/spyglass/linearization/merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/linearization/v0/main.py` & `spyglass_neuro-0.5.2/src/spyglass/linearization/v0/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     -> AnalysisNwbfile
     linearized_position_object_id : varchar(40)
     """
 
     def make(self, key):
         logger.info(f"Computing linear position for: {key}")
 
-        key["analysis_file_name"] = AnalysisNwbfile().create(
+        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
             key["nwb_file_name"]
         )
 
         position_nwb = (
             IntervalPositionInfo
             & {
                 "nwb_file_name": key["nwb_file_name"],
@@ -180,9 +180,11 @@
         nwb_analysis_file.add(
             nwb_file_name=key["nwb_file_name"],
             analysis_file_name=key["analysis_file_name"],
         )
 
         self.insert1(key)
 
+        AnalysisNwbfile().log(key, table=self.full_table_name)
+
     def fetch1_dataframe(self):
         return self.fetch_nwb()[0]["linearized_position"].set_index("time")
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/linearization/v1/main.py` & `spyglass_neuro-0.5.2/src/spyglass/linearization/v1/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def make(self, key):
         orig_key = copy.deepcopy(key)
         logger.info(f"Computing linear position for: {key}")
 
         position_nwb = PositionOutput().fetch_nwb(
             {"merge_id": key["pos_merge_id"]}
         )[0]
-        key["analysis_file_name"] = AnalysisNwbfile().create(
+        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
             position_nwb["nwb_file_name"]
         )
         position = np.asarray(
             position_nwb["position"].get_spatial_series().data
         )
         time = np.asarray(
             position_nwb["position"].get_spatial_series().timestamps
@@ -177,9 +177,11 @@
 
         part_name = to_camel_case(self.table_name.split("__")[-1])
 
         LinearizedPositionOutput._merge_insert(
             [orig_key], part_name=part_name, skip_duplicates=True
         )
 
+        AnalysisNwbfile().log(key, table=self.full_table_name)
+
     def fetch1_dataframe(self):
         return self.fetch_nwb()[0]["linearized_position"].set_index("time")
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/lock/file_lock.py` & `spyglass_neuro-0.5.2/src/spyglass/lock/file_lock.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/mua/v1/mua.py` & `spyglass_neuro-0.5.2/src/spyglass/mua/v1/mua.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/position_merge.py` & `spyglass_neuro-0.5.2/src/spyglass/position/position_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/__init__.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/dlc_decorators.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_decorators.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/dlc_reader.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_reader.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/dlc_utils.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/dlc_utils.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_centroid.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_centroid.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,18 @@
         idx = pd.IndexSlice
         output_dir = infer_output_dir(key=key, makedir=False)
         with OutputLogger(
             name=f"{key['nwb_file_name']}_{key['epoch']}_{key['dlc_model_name']}_log",
             path=f"{output_dir.as_posix()}/log.log",
             print_console=False,
         ) as logger:
+            # Add to Analysis NWB file
+            analysis_file_name = AnalysisNwbfile().create(  # logged
+                key["nwb_file_name"]
+            )
             logger.logger.info("-----------------------")
             logger.logger.info("Centroid Calculation")
 
             # Get labels to smooth from Parameters table
             cohort_entries = DLCSmoothInterpCohort.BodyPart & key
             params = (DLCCentroidParams() & key).fetch1("params")
             centroid_method = params.pop("centroid_method")
@@ -294,16 +298,14 @@
                 timestamps=final_df.index.to_numpy(),
                 data=pos_df[
                     pos_df.columns.levels[0][0]
                 ].video_frame_ind.to_numpy(),
                 description="video_frame_ind",
                 comments="no comments",
             )
-            # Add to Analysis NWB file
-            analysis_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
             nwb_analysis_file = AnalysisNwbfile()
             key.update(
                 {
                     "analysis_file_name": analysis_file_name,
                     "dlc_position_object_id": nwb_analysis_file.add_nwb_object(
                         analysis_file_name, position
                     ),
@@ -315,14 +317,15 @@
 
             nwb_analysis_file.add(
                 nwb_file_name=key["nwb_file_name"],
                 analysis_file_name=key["analysis_file_name"],
             )
             self.insert1(key)
             logger.logger.info("inserted entry into DLCCentroid")
+            AnalysisNwbfile().log(key, table=self.full_table_name)
 
     def fetch1_dataframe(self):
         nwb_data = self.fetch_nwb()[0]
         index = pd.Index(
             np.asarray(
                 nwb_data["dlc_position"].get_spatial_series().timestamps
             ),
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_cohort.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_cohort.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_model.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_model.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_orient.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_orient.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,17 @@
     ---
     -> AnalysisNwbfile
     dlc_orientation_object_id : varchar(80)
     """
 
     def make(self, key):
         # Get labels to smooth from Parameters table
+        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
         cohort_entries = DLCSmoothInterpCohort.BodyPart & key
         pos_df = pd.concat(
             {
                 bodypart: (
                     DLCSmoothInterpCohort.BodyPart
                     & {**key, **{"bodypart": bodypart}}
                 ).fetch1_dataframe()
@@ -126,17 +129,14 @@
                 truncate=8,
             )
             # convert back to between -pi and pi
             orientation = np.angle(np.exp(1j * orientation))
         final_df = pd.DataFrame(
             orientation, columns=["orientation"], index=pos_df.index
         )
-        key["analysis_file_name"] = AnalysisNwbfile().create(
-            key["nwb_file_name"]
-        )
         spatial_series = (RawPosition() & key).fetch_nwb()[0]["raw_position"]
         orientation = pynwb.behavior.CompassDirection()
         orientation.create_spatial_series(
             name="orientation",
             timestamps=final_df.index.to_numpy(),
             conversion=1.0,
             data=final_df["orientation"].to_numpy(),
@@ -151,14 +151,15 @@
 
         nwb_analysis_file.add(
             nwb_file_name=key["nwb_file_name"],
             analysis_file_name=key["analysis_file_name"],
         )
 
         self.insert1(key)
+        AnalysisNwbfile().log(key, table=self.full_table_name)
 
     def fetch1_dataframe(self):
         nwb_data = self.fetch_nwb()[0]
         index = pd.Index(
             np.asarray(
                 nwb_data["dlc_orientation"].get_spatial_series().timestamps
             ),
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_pose_estimation.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_pose_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,18 @@
     ):
         """
         Insert PoseEstimationTask in inferred output dir.
         From Datajoint Elements
 
         Parameters
         ----------
-        key: DataJoint key specifying a pairing of VideoRecording and Model.
-        task_mode (bool): Default 'trigger' computation.
-        Or 'load' existing results.
+        key: dict
+            DataJoint key specifying a pairing of VideoRecording and Model.
+        task_mode: bool, optional
+            Default 'trigger' computation. Or 'load' existing results.
         params (dict): Optional. Parameters passed to DLC's analyze_videos:
             videotype, gputouse, save_as_csv, batchsize, cropping,
             TFGPUinference, dynamic, robust_nframes, allow_growth, use_shelve
         """
         from .dlc_utils import check_videofile, get_video_path
 
         video_path, video_filename, _, _ = get_video_path(key)
@@ -271,23 +272,23 @@
                             c: dlc_result.df.get(body_part).get(c).values
                             for c in dlc_result.df.get(body_part).columns
                         }
                     )
             idx = pd.IndexSlice
             for body_part, part_df in body_parts_df.items():
                 logger.logger.info("converting to cm")
+                key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+                    key["nwb_file_name"]
+                )
                 part_df = convert_to_cm(part_df, meters_per_pixel)
                 logger.logger.info("adding timestamps to DataFrame")
                 part_df = add_timestamps(
                     part_df, pos_time=pos_time, video_time=video_time
                 )
                 key["bodypart"] = body_part
-                key["analysis_file_name"] = AnalysisNwbfile().create(
-                    key["nwb_file_name"]
-                )
                 position = pynwb.behavior.Position()
                 likelihood = pynwb.behavior.BehavioralTimeSeries()
                 position.create_spatial_series(
                     name="position",
                     timestamps=part_df.time.to_numpy(),
                     conversion=METERS_PER_CM,
                     data=part_df.loc[:, idx[("x", "y")]].to_numpy(),
@@ -325,14 +326,15 @@
                     )
                 )
                 nwb_analysis_file.add(
                     nwb_file_name=key["nwb_file_name"],
                     analysis_file_name=key["analysis_file_name"],
                 )
                 self.BodyPart.insert1(key)
+                AnalysisNwbfile().log(key, table=self.full_table_name)
 
     def fetch_dataframe(self, *attrs, **kwargs):
         entries = (self.BodyPart & self).fetch("KEY")
         nwb_data_dict = {
             entry["bodypart"]: (self.BodyPart() & entry).fetch_nwb()[0]
             for entry in entries
         }
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_position.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,17 @@
 
         output_dir = infer_output_dir(key=key, makedir=False)
         with OutputLogger(
             name=f"{key['nwb_file_name']}_{key['epoch']}_{key['dlc_model_name']}_log",
             path=f"{output_dir.as_posix()}/log.log",
             print_console=False,
         ) as logger:
+            key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+                key["nwb_file_name"]
+            )
             logger.logger.info("-----------------------")
             idx = pd.IndexSlice
             # Get labels to smooth from Parameters table
             params = (DLCSmoothInterpParams() & key).fetch1("params")
             # Get DLC output dataframe
             logger.logger.info("fetching Pose Estimation Dataframe")
             dlc_df = (DLCPoseEstimation.BodyPart() & key).fetch1_dataframe()
@@ -220,17 +223,14 @@
             final_df = smooth_df.drop(["likelihood"], axis=1)
             final_df = final_df.rename_axis("time").reset_index()
             position_nwb_data = (
                 (DLCPoseEstimation.BodyPart() & key)
                 .fetch_nwb()[0]["dlc_pose_estimation_position"]
                 .get_spatial_series()
             )
-            key["analysis_file_name"] = AnalysisNwbfile().create(
-                key["nwb_file_name"]
-            )
             # Add dataframe to AnalysisNwbfile
             nwb_analysis_file = AnalysisNwbfile()
             position = pynwb.behavior.Position()
             video_frame_ind = pynwb.behavior.BehavioralTimeSeries()
             logger.logger.info("Creating NWB objects")
             position.create_spatial_series(
                 name="position",
@@ -263,14 +263,15 @@
             )
             nwb_analysis_file.add(
                 nwb_file_name=key["nwb_file_name"],
                 analysis_file_name=key["analysis_file_name"],
             )
             self.insert1(key)
             logger.logger.info("inserted entry into DLCSmoothInterp")
+            AnalysisNwbfile().log(key, table=self.full_table_name)
 
     def fetch1_dataframe(self):
         nwb_data = self.fetch_nwb()[0]
         index = pd.Index(
             np.asarray(
                 nwb_data["dlc_smooth_interp_position"]
                 .get_spatial_series()
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_project.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_project.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_selection.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,18 @@
     orientation_object_id   : varchar(80)
     velocity_object_id      : varchar(80)
     pose_eval_result        : longblob
     """
 
     def make(self, key):
         orig_key = copy.deepcopy(key)
+        # Add to Analysis NWB file
+        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
         key["pose_eval_result"] = self.evaluate_pose_estimation(key)
 
         pos_nwb = (DLCCentroid & key).fetch_nwb()[0]
         ori_nwb = (DLCOrientation & key).fetch_nwb()[0]
 
         pos_obj = pos_nwb["dlc_position"].spatial_series["position"]
         vel_obj = pos_nwb["dlc_velocity"].time_series["velocity"]
@@ -106,18 +110,14 @@
             unit=vid_frame_obj.unit,
             timestamps=np.asarray(vid_frame_obj.timestamps),
             data=np.asarray(vid_frame_obj.data),
             description=vid_frame_obj.description,
             comments=vid_frame_obj.comments,
         )
 
-        # Add to Analysis NWB file
-        key["analysis_file_name"] = AnalysisNwbfile().create(
-            key["nwb_file_name"]
-        )
         nwb_analysis_file = AnalysisNwbfile()
         key["orientation_object_id"] = nwb_analysis_file.add_nwb_object(
             key["analysis_file_name"], orientation
         )
         key["position_object_id"] = nwb_analysis_file.add_nwb_object(
             key["analysis_file_name"], position
         )
@@ -134,14 +134,15 @@
         from ..position_merge import PositionOutput
 
         part_name = to_camel_case(self.table_name.split("__")[-1])
         # TODO: The next line belongs in a merge table function
         PositionOutput._merge_insert(
             [orig_key], part_name=part_name, skip_duplicates=True
         )
+        AnalysisNwbfile().log(key, table=self.full_table_name)
 
     def fetch1_dataframe(self):
         nwb_data = self.fetch_nwb()[0]
         index = pd.Index(
             np.asarray(nwb_data["position"].get_spatial_series().timestamps),
             name="time",
         )
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_dlc_training.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_dlc_training.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/position/v1/position_trodes_position.py` & `spyglass_neuro-0.5.2/src/spyglass/position/v1/position_trodes_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,17 @@
     velocity_object_id : varchar(80)
     """
 
     def make(self, key):
         logger.info(f"Computing position for: {key}")
         orig_key = copy.deepcopy(key)
 
-        analysis_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
+        analysis_file_name = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
 
         raw_position = RawPosition.PosObject & key
         spatial_series = raw_position.fetch_nwb()[0]["raw_position"]
         spatial_df = raw_position.fetch1_dataframe()
 
         position_info_parameters = (TrodesPosParams() & key).fetch1("params")
         position_info = self.calculate_position_info(
@@ -197,14 +199,15 @@
 
         part_name = to_camel_case(self.table_name.split("__")[-1])
 
         # TODO: The next line belongs in a merge table function
         PositionOutput._merge_insert(
             [orig_key], part_name=part_name, skip_duplicates=True
         )
+        AnalysisNwbfile().log(key, table=self.full_table_name)
 
     @staticmethod
     def generate_pos_components(*args, **kwargs):
         return IntervalPositionInfo().generate_pos_components(*args, **kwargs)
 
     @staticmethod
     def calculate_position_info(*args, **kwargs):
@@ -284,16 +287,21 @@
         )[0].as_posix()
         nwb_base_filename = key["nwb_file_name"].replace(".nwb", "")
         current_dir = Path(os.getcwd())
         output_video_filename = (
             f"{current_dir.as_posix()}/{nwb_base_filename}_"
             f"{epoch:02d}_{key['trodes_pos_params_name']}.mp4"
         )
+        red_cols = (
+            ["xloc", "yloc"]
+            if "xloc" in raw_position_df.columns
+            else ["xloc1", "yloc1"]
+        )
         centroids = {
-            "red": np.asarray(raw_position_df[["xloc", "yloc"]]),
+            "red": np.asarray(raw_position_df[red_cols]),
             "green": np.asarray(raw_position_df[["xloc2", "yloc2"]]),
         }
         position_mean = np.asarray(
             position_info_df[["position_x", "position_y"]]
         )
         orientation_mean = np.asarray(position_info_df[["orientation"]])
         position_time = np.asarray(position_info_df.index)
@@ -326,22 +334,24 @@
         -------
         converted_data : ndarray, shape (n_time, 2)
         """
         return data / cm_to_pixels
 
     @staticmethod
     def fill_nan(variable, video_time, variable_time):
+        # TODO: Reduce duplication across dlc_utils and common_position
         video_ind = np.digitize(variable_time, video_time[1:])
 
         n_video_time = len(video_time)
         try:
             n_variable_dims = variable.shape[1]
             filled_variable = np.full((n_video_time, n_variable_dims), np.nan)
         except IndexError:
             filled_variable = np.full((n_video_time,), np.nan)
+
         filled_variable[video_ind] = variable
 
         return filled_variable
 
     def make_video(
         self,
         video_filename,
@@ -446,8 +456,11 @@
                 frame = cv2.cvtColor(frame, cv2.COLOR_RGB2BGR)
                 out.write(frame)
             else:
                 break
 
         video.release()
         out.release()
-        cv2.destroyAllWindows()
+        try:
+            cv2.destroyAllWindows()
+        except cv2.error:  # if cv is already closed or does not have func
+            pass
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/ripple/v1/ripple.py` & `spyglass_neuro-0.5.2/src/spyglass/ripple/v1/ripple.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,14 +140,32 @@
                 close_ripple_threshold=0.0,  # sec
             ),
         }
         self.insert1(
             {"ripple_param_name": "default", "ripple_param_dict": default_dict},
             skip_duplicates=True,
         )
+        default_dict_trodes = {
+            "speed_name": "speed",
+            "ripple_detection_algorithm": "Kay_ripple_detector",
+            "ripple_detection_params": dict(
+                speed_threshold=4.0,  # cm/s
+                minimum_duration=0.015,  # sec
+                zscore_threshold=2.0,  # std
+                smoothing_sigma=0.004,  # sec
+                close_ripple_threshold=0.0,  # sec
+            ),
+        }
+        self.insert1(
+            {
+                "ripple_param_name": "default_trodes",
+                "ripple_param_dict": default_dict_trodes,
+            },
+            skip_duplicates=True,
+        )
 
 
 @schema
 class RippleTimesV1(SpyglassMixin, dj.Computed):
     definition = """
     -> RippleLFPSelection
     -> RippleParameters
@@ -369,15 +387,14 @@
         consensus_color="black",
         speed_color="black",
         view_height=800,
         use_ripple_filtered_lfps=False,
         lfp_offset=1,
         lfp_channel_ind=None,
     ):
-
         ripple_times = self.fetch1_dataframe()
 
         def _add_ripple_times(
             view,
             ripple_times=ripple_times,
             ripple_times_color=ripple_times_color,
         ):
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/sharing/sharing_kachery.py` & `spyglass_neuro-0.5.2/src/spyglass/sharing/sharing_kachery.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/imported.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/imported.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/analysis/v1/group.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/analysis/v1/group.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/__init__.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/curation_figurl.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/curation_figurl.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/merged_sorting_extractor.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/merged_sorting_extractor.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/sortingview.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/sortingview_helper_fn.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/sortingview_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_artifact.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_artifact.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_curation.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_curation.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,38 @@
 import warnings
 from pathlib import Path
 from typing import List
 
 import datajoint as dj
 import numpy as np
 import spikeinterface as si
+from packaging import version
+
+if version.parse(si.__version__) < version.parse("0.99.1"):
+    raise ImportError(
+        "SpikeInterface version must updated. "
+        + "Please run `pip install spikeinterface==0.99.1` to update."
+    )
 import spikeinterface.preprocessing as sip
 import spikeinterface.qualitymetrics as sq
 
+from spyglass.common import BrainRegion, Electrode
 from spyglass.common.common_interval import IntervalList
 from spyglass.common.common_nwbfile import AnalysisNwbfile
 from spyglass.settings import waveforms_dir
 from spyglass.spikesorting.v0.merged_sorting_extractor import (
     MergedSortingExtractor,
 )
 from spyglass.spikesorting.v0.spikesorting_recording import (
     SortInterval,
     SpikeSortingRecording,
 )
 from spyglass.utils import SpyglassMixin, logger
 
+from .spikesorting_recording import SortGroup
 from .spikesorting_sorting import SpikeSorting
 
 schema = dj.schema("spikesorting_curation")
 
 valid_labels = ["reject", "noise", "artifact", "mua", "accept"]
 
 
@@ -215,14 +224,15 @@
 
         Returns
         -------
         analysis_file_name : str
         units_object_id : str
 
         """
+        analysis_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
 
         sort_interval_valid_times = (
             IntervalList & {"interval_list_name": sort_interval_list_name}
         ).fetch1("valid_times")
 
         units = dict()
         units_valid_times = dict()
@@ -235,15 +245,14 @@
             spike_times_in_samples = sorting.get_unit_spike_train(
                 unit_id=unit_id
             )
             units[unit_id] = timestamps[spike_times_in_samples]
             units_valid_times[unit_id] = sort_interval_valid_times
             units_sort_interval[unit_id] = [sort_interval]
 
-        analysis_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
         object_ids = AnalysisNwbfile().add_units(
             analysis_file_name,
             units,
             units_valid_times,
             units_sort_interval,
             metrics=metrics,
             labels=labels,
@@ -313,14 +322,17 @@
     ---
     waveform_extractor_path: varchar(400)
     -> AnalysisNwbfile
     waveforms_object_id: varchar(40)   # Object ID for the waveforms in NWB file
     """
 
     def make(self, key):
+        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
         recording = Curation.get_recording(key)
         if recording.get_num_segments() > 1:
             recording = si.concatenate_recordings([recording])
 
         sorting = Curation.get_curated_sorting(key)
 
         logger.info("Extracting waveforms...")
@@ -338,23 +350,21 @@
         waveforms = si.extract_waveforms(
             recording=recording,
             sorting=sorting,
             folder=key["waveform_extractor_path"],
             **waveform_params,
         )
 
-        key["analysis_file_name"] = AnalysisNwbfile().create(
-            key["nwb_file_name"]
-        )
         object_id = AnalysisNwbfile().add_units_waveforms(
             key["analysis_file_name"], waveform_extractor=waveforms
         )
         key["waveforms_object_id"] = object_id
         AnalysisNwbfile().add(key["nwb_file_name"], key["analysis_file_name"])
 
+        AnalysisNwbfile().log(key, table=self.full_table_name)
         self.insert1(key)
 
     def load_waveforms(self, key: dict):
         """Returns a spikeinterface waveform extractor specified by key
 
         Parameters
         ----------
@@ -499,14 +509,17 @@
     ---
     quality_metrics_path: varchar(500)
     -> AnalysisNwbfile
     object_id: varchar(40) # Object ID for the metrics in NWB file
     """
 
     def make(self, key):
+        key["analysis_file_name"] = AnalysisNwbfile().create(  # logged
+            key["nwb_file_name"]
+        )
         waveform_extractor = Waveforms().load_waveforms(key)
         qm = {}
         params = (MetricParameters & key).fetch1("metric_params")
         for metric_name, metric_params in params.items():
             metric = self._compute_metric(
                 waveform_extractor, metric_name, **metric_params
             )
@@ -515,21 +528,19 @@
         key["quality_metrics_path"] = str(
             Path(waveforms_dir) / Path(qm_name + ".json")
         )
         # save metrics dict as json
         logger.info(f"Computed all metrics: {qm}")
         self._dump_to_json(qm, key["quality_metrics_path"])
 
-        key["analysis_file_name"] = AnalysisNwbfile().create(
-            key["nwb_file_name"]
-        )
         key["object_id"] = AnalysisNwbfile().add_units_metrics(
             key["analysis_file_name"], metrics=qm
         )
         AnalysisNwbfile().add(key["nwb_file_name"], key["analysis_file_name"])
+        AnalysisNwbfile().log(key, table=self.full_table_name)
 
         self.insert1(key)
 
     def _get_quality_metrics_name(self, key):
         wf_name = Waveforms()._get_waveform_extractor_name(key)
         qm_name = wf_name + "_qm"
         return qm_name
@@ -613,32 +624,30 @@
 
 def _get_peak_offset(
     waveform_extractor: si.WaveformExtractor, peak_sign: str, **metric_params
 ):
     """Computes the shift of the waveform peak from center of window."""
     if "peak_sign" in metric_params:
         del metric_params["peak_sign"]
-    peak_offset_inds = (
-        si.postprocessing.get_template_extremum_channel_peak_shift(
-            waveform_extractor=waveform_extractor,
-            peak_sign=peak_sign,
-            **metric_params,
-        )
+    peak_offset_inds = si.core.get_template_extremum_channel_peak_shift(
+        waveform_extractor=waveform_extractor,
+        peak_sign=peak_sign,
+        **metric_params,
     )
     peak_offset = {key: int(abs(val)) for key, val in peak_offset_inds.items()}
     return peak_offset
 
 
 def _get_peak_channel(
     waveform_extractor: si.WaveformExtractor, peak_sign: str, **metric_params
 ):
     """Computes the electrode_id of the channel with the extremum peak for each unit."""
     if "peak_sign" in metric_params:
         del metric_params["peak_sign"]
-    peak_channel_dict = si.postprocessing.get_template_extremum_channel(
+    peak_channel_dict = si.core.get_template_extremum_channel(
         waveform_extractor=waveform_extractor,
         peak_sign=peak_sign,
         **metric_params,
     )
     peak_channel = {key: int(val) for key, val in peak_channel_dict.items()}
     return peak_channel
 
@@ -917,25 +926,29 @@
         snr=0: float            # SNR for each unit
         firing_rate=-1: float   # firing rate
         num_spikes=-1: int   # total number of spikes
         peak_channel=null: int # channel of maximum amplitude for each unit
         """
 
     def make(self, key):
+        AnalysisNwbfile()._creation_times["pre_create_time"] = time.time()
         unit_labels_to_remove = ["reject"]
         # check that the Curation has metrics
         metrics = (Curation & key).fetch1("quality_metrics")
         if metrics == {}:
-            Warning(
-                f"Metrics for Curation {key} should normally be calculated before insertion here"
+            logger.warning(
+                f"Metrics for Curation {key} should normally be calculated "
+                + "before insertion here"
             )
 
         sorting = Curation.get_curated_sorting(key)
         unit_ids = sorting.get_unit_ids()
-        # Get the labels for the units, add only those units that do not have 'reject' or 'noise' labels
+
+        # Get the labels for the units, add only those units that do not have
+        # 'reject' or 'noise' labels
         unit_labels = (Curation & key).fetch1("curation_labels")
         accepted_units = []
         for unit_id in unit_ids:
             if unit_id in unit_labels:
                 if (
                     len(set(unit_labels_to_remove) & set(unit_labels[unit_id]))
                     == 0
@@ -983,14 +996,16 @@
             timestamps,
             sort_interval_list_name,
             sort_interval,
             metrics=final_metrics,
             unit_ids=accepted_units,
             labels=labels,
         )
+
+        AnalysisNwbfile().log(key, table=self.full_table_name)
         self.insert1(key)
 
         # now add the units
         # Remove the non primary key entries.
         del key["units_object_id"]
         del key["analysis_file_name"]
 
@@ -1025,14 +1040,45 @@
     @classmethod
     def get_sorting(cls, key):
         """Returns the sorting related to this curation. Useful for operations downstream of merge table"""
         # expand the key
         sorting_key = (cls & key).fetch1("KEY")
         return Curation.get_curated_sorting(sorting_key)
 
+    @classmethod
+    def get_sort_group_info(cls, key):
+        """Returns the sort group information for the curation
+        (e.g. brain region, electrode placement, etc.)
+
+        Parameters
+        ----------
+        key : dict
+            restriction on CuratedSpikeSorting table
+
+        Returns
+        -------
+        sort_group_info : Table
+            Table with information about the sort groups
+        """
+        electrode_restrict_list = []
+        for entry in cls & key:
+            # Just take one electrode entry per sort group
+            electrode_restrict_list.extend(
+                ((SortGroup.SortGroupElectrode() & entry) * Electrode).fetch(
+                    limit=1
+                )
+            )
+        # Run joins with the tables with info and return
+        sort_group_info = (
+            (Electrode & electrode_restrict_list)
+            * (cls & key)
+            * SortGroup.SortGroupElectrode()
+        ) * BrainRegion()
+        return sort_group_info
+
 
 @schema
 class UnitInclusionParameters(SpyglassMixin, dj.Manual):
     definition = """
     unit_inclusion_param_name: varchar(80) # the name of the list of thresholds for unit inclusion
     ---
     inclusion_param_dict: blob # the dictionary of inclusion / exclusion parameters
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_populator.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_populator.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_recording.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_recording.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/spikesorting_sorting.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/spikesorting_sorting.py`

 * *Files 5% similar despite different names*

```diff
@@ -200,14 +200,18 @@
         sorter_params["tempdir"] = sorter_temp_dir.name
 
         if sorter == "clusterless_thresholder":
             # need to remove tempdir and whiten from sorter_params
             sorter_params.pop("tempdir", None)
             sorter_params.pop("whiten", None)
             sorter_params.pop("outputs", None)
+            if "local_radius_um" in sorter_params:
+                sorter_params["radius_um"] = sorter_params.pop(
+                    "local_radius_um"
+                )  # correct existing parameter sets for spikeinterface>=0.99.1
 
             # Detect peaks for clusterless decoding
             detected_spikes = detect_peaks(recording, **sorter_params)
             sorting = si.NumpySorting.from_times_labels(
                 times_list=detected_spikes["sample_index"],
                 labels_list=np.zeros(len(detected_spikes), dtype=np.int),
                 sampling_frequency=recording.get_sampling_frequency(),
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingRecordingView.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/SpikeSortingView.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v0/figurl_views/prepare_spikesortingview_data.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/__init__.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/artifact.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/artifact.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/curation.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/curation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+from time import time
 from typing import Dict, List, Union
 
 import datajoint as dj
 import numpy as np
 import pynwb
 import spikeinterface as si
 import spikeinterface.curation as sc
 import spikeinterface.extractors as se
 
+from spyglass.common import BrainRegion, Electrode
 from spyglass.common.common_ephys import Raw
 from spyglass.common.common_nwbfile import AnalysisNwbfile
-from spyglass.spikesorting.v1.recording import SpikeSortingRecording
+from spyglass.spikesorting.v1.recording import (
+    SortGroup,
+    SpikeSortingRecording,
+    SpikeSortingRecordingSelection,
+)
 from spyglass.spikesorting.v1.sorting import SpikeSorting, SpikeSortingSelection
 from spyglass.utils.dj_mixin import SpyglassMixin
 
 schema = dj.schema("spikesorting_v1_curation")
 
 valid_labels = ["reject", "noise", "artifact", "mua", "accept"]
 
@@ -70,14 +76,16 @@
             [[11,12],[46,48],[51,54],[50,53]]
         }
 
         Returns
         -------
         curation_key : dict
         """
+        AnalysisNwbfile()._creation_times["pre_create_time"] = time()
+
         sort_query = cls & {"sorting_id": sorting_id}
         parent_curation_id = max(parent_curation_id, -1)
         if parent_curation_id == -1:
             parent_curation_id = -1
             # check to see if this sorting with a parent of -1
             # has already been inserted and if so, warn the user
             query = sort_query & {"parent_curation_id": -1}
@@ -116,14 +124,15 @@
             "merges_applied": apply_merge,
             "description": description,
         }
         cls.insert1(
             key,
             skip_duplicates=True,
         )
+        AnalysisNwbfile().log(analysis_file_name, table=cls.full_table_name)
 
         return key
 
     @classmethod
     def insert_metric_curation(cls, key: Dict, apply_merge=False):
         """Insert a row into CurationV1.
 
@@ -256,14 +265,50 @@
             units_to_merge = _merge_dict_to_list(merge_groups)
             return sc.MergeUnitsSorting(
                 parent_sorting=si_sorting, units_to_merge=units_to_merge
             )
         else:
             return si_sorting
 
+    @classmethod
+    def get_sort_group_info(cls, key: dict) -> dj.Table:
+        """Returns the sort group information for the curation
+        (e.g. brain region, electrode placement, etc.)
+
+        Parameters
+        ----------
+        key : dict
+            restriction on CuratedSpikeSorting table
+
+        Returns
+        -------
+        sort_group_info : Table
+            Table with information about the sort groups
+        """
+        table = (
+            (cls & key) * SpikeSortingSelection()
+        ) * SpikeSortingRecordingSelection().proj(
+            "recording_id", "sort_group_id"
+        )
+        electrode_restrict_list = []
+        for entry in table:
+            # pull just one electrode from each sort group for info
+            electrode_restrict_list.extend(
+                ((SortGroup.SortGroupElectrode() & entry) * Electrode).fetch(
+                    limit=1
+                )
+            )
+
+        sort_group_info = (
+            (Electrode & electrode_restrict_list)
+            * table
+            * SortGroup.SortGroupElectrode()
+        ) * BrainRegion()
+        return (cls & key).proj() * sort_group_info
+
 
 def _write_sorting_to_nwb_with_curation(
     sorting_id: str,
     labels: Union[None, Dict[str, List[str]]] = None,
     merge_groups: Union[None, List[List[str]]] = None,
     metrics: Union[None, Dict[str, Dict[str, float]]] = None,
     apply_merge: bool = False,
@@ -292,14 +337,15 @@
         object_id of the units table in the analysis NWB file
     """
     # FETCH:
     # - primary key for the associated sorting and recording
     nwb_file_name = (SpikeSortingSelection & {"sorting_id": sorting_id}).fetch1(
         "nwb_file_name"
     )
+    analysis_nwb_file = AnalysisNwbfile().create(nwb_file_name)
 
     # get sorting
     sorting_analysis_file_abs_path = AnalysisNwbfile.get_abs_path(
         (SpikeSorting & {"sorting_id": sorting_id}).fetch1("analysis_file_name")
     )
     with pynwb.NWBHDF5IO(
         sorting_analysis_file_abs_path, "r", load_namespaces=True
@@ -320,15 +366,14 @@
             for merge_unit_id in merge_group:
                 units_dict.pop(merge_unit_id, None)
         merge_groups = None
 
     unit_ids = list(units_dict.keys())
 
     # create new analysis nwb file
-    analysis_nwb_file = AnalysisNwbfile().create(nwb_file_name)
     analysis_nwb_file_abs_path = AnalysisNwbfile.get_abs_path(analysis_nwb_file)
     with pynwb.NWBHDF5IO(
         path=analysis_nwb_file_abs_path,
         mode="a",
         load_namespaces=True,
     ) as io:
         nwbf = io.read()
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/figurl_curation.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/figurl_curation.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,42 +114,37 @@
     -> FigURLCurationSelection
     ---
     url: varchar(1000)
     """
 
     def make(self, key: dict):
         # FETCH
-        sorting_analysis_file_name = (
-            FigURLCurationSelection * CurationV1 & key
-        ).fetch1("analysis_file_name")
-        object_id = (FigURLCurationSelection * CurationV1 & key).fetch1(
-            "object_id"
+        query = (
+            FigURLCurationSelection * CurationV1 * SpikeSortingSelection & key
         )
-        recording_label = (SpikeSortingSelection & key).fetch1("recording_id")
-        metrics_figurl = (FigURLCurationSelection & key).fetch1(
-            "metrics_figurl"
+        (
+            sorting_fname,
+            object_id,
+            recording_label,
+            metrics_figurl,
+        ) = query.fetch1(
+            "analysis_file_name", "object_id", "recording_id", "metrics_figurl"
         )
 
         # DO
-        sorting_analysis_file_abs_path = AnalysisNwbfile.get_abs_path(
-            sorting_analysis_file_name
-        )
-        recording = CurationV1.get_recording(
-            (FigURLCurationSelection & key).fetch1()
-        )
-        sorting = CurationV1.get_sorting(
-            (FigURLCurationSelection & key).fetch1()
-        )
-        sorting_label = (FigURLCurationSelection & key).fetch1("sorting_id")
-        curation_uri = (FigURLCurationSelection & key).fetch1("curation_uri")
+        sel_query = FigURLCurationSelection & key
+        sel_key = sel_query.fetch1()
+        sorting_fpath = AnalysisNwbfile.get_abs_path(sorting_fname)
+        recording = CurationV1.get_recording(sel_key)
+        sorting = CurationV1.get_sorting(sel_key)
+        sorting_label = sel_query.fetch1("sorting_id")
+        curation_uri = sel_query.fetch1("curation_uri")
 
         metric_dict = {}
-        with pynwb.NWBHDF5IO(
-            sorting_analysis_file_abs_path, "r", load_namespaces=True
-        ) as io:
+        with pynwb.NWBHDF5IO(sorting_fpath, "r", load_namespaces=True) as io:
             nwbf = io.read()
             nwb_sorting = nwbf.objects[object_id].to_dataframe()
             unit_ids = nwb_sorting.index
             for metric in metrics_figurl:
                 metric_dict[metric] = dict(zip(unit_ids, nwb_sorting[metric]))
 
         unit_metrics = _reformat_metrics(metric_dict)
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/metric_curation.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import uuid
+from time import time
 from typing import Any, Dict, List, Union
 
 import datajoint as dj
 import numpy as np
 import pynwb
 import spikeinterface as si
 import spikeinterface.preprocessing as sp
@@ -199,14 +200,15 @@
     -> MetricCurationSelection
     ---
     -> AnalysisNwbfile
     object_id: varchar(40) # Object ID for the metrics in NWB file
     """
 
     def make(self, key):
+        AnalysisNwbfile()._creation_times["pre_create_time"] = time()
         # FETCH
         nwb_file_name = (
             SpikeSortingSelection * MetricCurationSelection & key
         ).fetch1("nwb_file_name")
 
         waveform_params = (
             WaveformParameters * MetricCurationSelection & key
@@ -270,14 +272,15 @@
         )
 
         # INSERT
         AnalysisNwbfile().add(
             nwb_file_name,
             key["analysis_file_name"],
         )
+        AnalysisNwbfile().log(key, table=self.full_table_name)
         self.insert1(key)
 
     @classmethod
     def get_waveforms(cls):
         return NotImplementedError
 
     @classmethod
@@ -519,20 +522,20 @@
     Returns
     -------
     analysis_nwb_file : str
         name of analysis NWB file containing the sorting and curation information
     object_id : str
         object_id of the units table in the analysis NWB file
     """
-
-    unit_ids = [int(i) for i in waveforms.sorting.get_unit_ids()]
-
     # create new analysis nwb file
     analysis_nwb_file = AnalysisNwbfile().create(nwb_file_name)
     analysis_nwb_file_abs_path = AnalysisNwbfile.get_abs_path(analysis_nwb_file)
+
+    unit_ids = [int(i) for i in waveforms.sorting.get_unit_ids()]
+
     with pynwb.NWBHDF5IO(
         path=analysis_nwb_file_abs_path,
         mode="a",
         load_namespaces=True,
     ) as io:
         nwbf = io.read()
         # Write waveforms to the nwb file
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/metric_utils.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/metric_utils.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/recording.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+from time import time
 from typing import Iterable, List, Optional, Tuple, Union
 
 import datajoint as dj
 import numpy as np
 import probeinterface as pi
 import pynwb
 import spikeinterface as si
@@ -246,14 +247,15 @@
     -> SpikeSortingRecordingSelection
     ---
     -> AnalysisNwbfile
     object_id: varchar(40) # Object ID for the processed recording in NWB file
     """
 
     def make(self, key):
+        AnalysisNwbfile()._creation_times["pre_create_time"] = time()
         # DO:
         # - get valid times for sort interval
         # - proprocess recording
         # - write recording to NWB file
         sort_interval_valid_times = self._get_sort_interval_valid_times(key)
         recording, timestamps = self._get_preprocessed_recording(key)
         recording_nwb_file_name, recording_object_id = _write_recording_to_nwb(
@@ -278,14 +280,17 @@
                 "pipeline": "spikesorting_recording_v1",
             }
         )
         AnalysisNwbfile().add(
             (SpikeSortingRecordingSelection & key).fetch1("nwb_file_name"),
             key["analysis_file_name"],
         )
+        AnalysisNwbfile().log(
+            recording_nwb_file_name, table=self.full_table_name
+        )
         self.insert1(key)
 
     @classmethod
     def get_recording(cls, key: dict) -> si.BaseRecording:
         """Get recording related to this curation as spikeinterface BaseRecording
 
         Parameters
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/sorting.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/sorting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import tempfile
 import time
 import uuid
 from typing import Iterable
 
 import datajoint as dj
 import numpy as np
@@ -18,15 +19,14 @@
 from spyglass.settings import temp_dir
 from spyglass.spikesorting.v1.recording import (  # noqa: F401
     SpikeSortingRecording,
     SpikeSortingRecordingSelection,
     _consolidate_intervals,
 )
 from spyglass.utils import SpyglassMixin, logger
-import os
 
 schema = dj.schema("spikesorting_v1_sorting")
 
 
 @schema
 class SpikeSorterParameters(SpyglassMixin, dj.Lookup):
     definition = """
@@ -148,14 +148,15 @@
         """Runs spike sorting on the data and parameters specified by the
         SpikeSortingSelection table and inserts a new entry to SpikeSorting table.
         """
         # FETCH:
         # - information about the recording
         # - artifact free intervals
         # - spike sorter and sorter params
+        AnalysisNwbfile()._creation_times["pre_create_time"] = time.time()
 
         recording_key = (
             SpikeSortingRecording * SpikeSortingSelection & key
         ).fetch1()
         artifact_removed_intervals = (
             IntervalList
             & {
@@ -228,14 +229,18 @@
             )
 
         if sorter == "clusterless_thresholder":
             # need to remove tempdir and whiten from sorter_params
             sorter_params.pop("tempdir", None)
             sorter_params.pop("whiten", None)
             sorter_params.pop("outputs", None)
+            if "local_radius_um" in sorter_params:
+                sorter_params["radius_um"] = sorter_params.pop(
+                    "local_radius_um"
+                )  # correct existing parameter sets for spikeinterface>=0.99.1
 
             # Detect peaks for clusterless decoding
             detected_spikes = detect_peaks(recording, **sorter_params)
             sorting = si.NumpySorting.from_times_labels(
                 times_list=detected_spikes["sample_index"],
                 labels_list=np.zeros(len(detected_spikes), dtype=np.int),
                 sampling_frequency=recording.get_sampling_frequency(),
@@ -291,14 +296,15 @@
         # INSERT
         # - new entry to AnalysisNwbfile
         # - new entry to SpikeSorting
         AnalysisNwbfile().add(
             (SpikeSortingSelection & key).fetch1("nwb_file_name"),
             key["analysis_file_name"],
         )
+        AnalysisNwbfile().log(key, table=self.full_table_name)
         self.insert1(key, skip_duplicates=True)
 
     @classmethod
     def get_sorting(cls, key: dict) -> si.BaseSorting:
         """Get sorting in the analysis NWB file as spikeinterface BaseSorting
 
         Parameters
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/spikesorting/v1/utils.py` & `spyglass_neuro-0.5.2/src/spyglass/spikesorting/v1/utils.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/utils/database_settings.py` & `spyglass_neuro-0.5.2/src/spyglass/utils/database_settings.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/utils/dj_chains.py` & `spyglass_neuro-0.5.2/src/spyglass/utils/dj_chains.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,20 +119,21 @@
         Child or destination of chain.
     _connection : datajoint.Connection, optional
         Connection to database used to create FreeTable objects. Defaults to
         parent.connection.
     _link_symbol : str
         Symbol used to represent the link between parent and child. Hardcoded
         to " -> ".
-    _has_link : bool
+    has_link : bool
         Cached attribute to store whether parent is linked to child. False if
         child is not in parent.descendants or nx.NetworkXNoPath is raised by
         nx.shortest_path.
-    _has_directed_link : bool
-        True if directed graph is used to find path. False if undirected graph.
+    link_type : str
+        'directed' or 'undirected' based on whether path is found with directed
+        or undirected graph. None if no path is found.
     graph : nx.DiGraph
         Directed graph of parent's dependencies from datajoint.connection.
     names : List[str]
         List of full table names in chain.
     objects : List[dj.FreeTable]
         List of FreeTable objects for each table in chain.
     attr_maps : List[dict]
@@ -171,62 +172,68 @@
             and MERGE_PK in child.heading.names
         ):
             raise TypeError("Child is a merge table. Use TableChains instead.")
 
         self._link_symbol = " -> "
         self.parent = parent
         self.child = child
-        self._has_link = True
-        self._has_directed_link = None
+        self.link_type = None
+        self._searched = False
 
         if child.full_table_name not in self.graph.nodes:
             logger.warning(
                 "Can't find item in graph. Try importing: "
                 + f"{child.full_table_name}"
             )
+            self._searched = True
 
     def __str__(self):
         """Return string representation of chain: parent -> child."""
-        if not self._has_link:
+        if not self.has_link:
             return "No link"
         return (
             to_camel_case(self.parent.table_name)
             + self._link_symbol
             + to_camel_case(self.child.table_name)
         )
 
     def __repr__(self):
         """Return full representation of chain: parent -> {links} -> child."""
-        return (
-            "Chain: "
-            + self._link_symbol.join([t.table_name for t in self.objects])
-            if self.names
-            else "No link"
+        if not self.has_link:
+            return "No link"
+        return "Chain: " + self._link_symbol.join(
+            [t.table_name for t in self.objects]
         )
 
     def __len__(self):
         """Return number of tables in chain."""
+        if not self.has_link:
+            return 0
         return len(self.names)
 
     def __getitem__(self, index: Union[int, str]) -> dj.FreeTable:
         """Return FreeTable object at index."""
+        if not self.has_link:
+            return None
         if isinstance(index, str):
             for i, name in enumerate(self.names):
                 if index in name:
                     return self.objects[i]
         return self.objects[index]
 
     @property
     def has_link(self) -> bool:
         """Return True if parent is linked to child.
 
-        Cached as hidden attribute _has_link to set False if nx.NetworkXNoPath
-        is raised by nx.shortest_path.
+        If not searched, search for path. If searched and no link is found,
+        return False. If searched and link is found, return True.
         """
-        return self._has_link
+        if not self._searched:
+            _ = self.path
+        return self.link_type is not None
 
     def pk_link(self, src, trg, data) -> float:
         """Return 1 if data["primary"] else float("inf").
 
         Currently unused. Preserved for future debugging. shortest_path accepts
         an option weight callable parameter.
         nx.shortest_path(G, source, target,weight=pk_link)
@@ -238,15 +245,15 @@
 
         Parameters
         ----------
         directed : bool, optional
             If True, use directed graph. If False, use undirected graph.
             Defaults to True. Undirected permits paths to traverse from merge
             part-parent -> merge part -> merge table. Undirected excludes
-            PERIPHERAL_TABLES likne interval_list, nwbfile, etc.
+            PERIPHERAL_TABLES like interval_list, nwbfile, etc.
 
         Returns
         -------
         OrderedDict
             Dictionary of full table names in chain. Keys are full table names.
             Values are free_table (dj.FreeTable representation) and attr_map
             (dict of new_name: old_name). Attribute maps on the table upstream
@@ -261,89 +268,91 @@
         if not directed:
             self.graph = self.graph.to_undirected()
             self.graph.remove_nodes_from(PERIPHERAL_TABLES)
         try:
             path = nx.shortest_path(self.graph, source, target)
         except nx.NetworkXNoPath:
             return None
+        except nx.NodeNotFound:
+            self._searched = True
+            return None
 
         ret = OrderedDict()
         prev_table = None
         for i, table in enumerate(path):
             if table.isnumeric():  # get proj() attribute map for alias node
                 if not prev_table:
                     raise ValueError("Alias node found without prev table.")
-                attr_map = self.graph[table][prev_table]["attr_map"]
+                try:
+                    attr_map = self.graph[table][prev_table]["attr_map"]
+                except KeyError:  # Why is this only DLCCentroid??
+                    attr_map = self.graph[prev_table][table]["attr_map"]
                 ret[prev_table]["attr_map"] = attr_map
             else:
                 free_table = dj.FreeTable(self._connection, table)
                 ret[table] = {"free_table": free_table, "attr_map": {}}
                 prev_table = table
         return ret
 
     @cached_property
     def path(self) -> OrderedDict:
         """Return list of full table names in chain."""
-        if not self._has_link:
+        if self._searched and not self.has_link:
             return None
 
         link = None
         if link := self.find_path(directed=True):
-            self._has_directed_link = True
+            self.link_type = "directed"
         elif link := self.find_path(directed=False):
-            self._has_directed_link = False
+            self.link_type = "undirected"
+        self._searched = True
 
-        if link:
-            return link
-
-        self._has_link = False
-        return None
+        return link
 
     @cached_property
     def names(self) -> List[str]:
         """Return list of full table names in chain."""
-        if self._has_link:
-            return list(self.path.keys())
-        return None
+        if not self.has_link:
+            return None
+        return list(self.path.keys())
 
     @cached_property
     def objects(self) -> List[dj.FreeTable]:
         """Return list of FreeTable objects for each table in chain.
 
         Unused. Preserved for future debugging.
         """
-        if self._has_link:
-            return [v["free_table"] for v in self.path.values()]
-        return None
+        if not self.has_link:
+            return None
+        return [v["free_table"] for v in self.path.values()]
 
     @cached_property
     def attr_maps(self) -> List[dict]:
         """Return list of attribute maps for each table in chain.
 
         Unused. Preserved for future debugging.
         """
-        #
-        if self._has_link:
-            return [v["attr_map"] for v in self.path.values()]
-        return None
+        if not self.has_link:
+            return None
+        return [v["attr_map"] for v in self.path.values()]
 
     def join(
         self, restriction: str = None, reverse_order: bool = False
     ) -> dj.expression.QueryExpression:
         """Return join of tables in chain with restriction applied to parent.
 
         Parameters
         ----------
         restriction : str, optional
             Restriction to apply to first table in the order.
             Defaults to self.parent.restriction.
         reverse_order : bool, optional
             If True, join tables in reverse order. Defaults to False.
         """
-        if not self._has_link:
+        if not self.has_link:
             return None
 
         restriction = restriction or self.parent.restriction or True
         path = (
             OrderedDict(reversed(self.path.items()))
             if reverse_order
             else self.path
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/utils/dj_helper_fn.py` & `spyglass_neuro-0.5.2/src/spyglass/utils/dj_helper_fn.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 
 import inspect
 import os
 from typing import Type
 
 import datajoint as dj
 import numpy as np
+from datajoint.user_tables import UserTable
 
+from spyglass.utils.dj_chains import PERIPHERAL_TABLES
 from spyglass.utils.logging import logger
 from spyglass.utils.nwb_helper_fn import get_nwb_file
 
 
+def unique_dicts(list_of_dict):
+    """Remove duplicate dictionaries from a list."""
+    return [dict(t) for t in {tuple(d.items()) for d in list_of_dict}]
+
+
 def deprecated_factory(classes: list, old_module: str = "") -> list:
     """Creates a list of classes and logs a warning when instantiated
 
     Parameters
     ---------
     classes : list
         list of tuples containing old_class, new_class
@@ -101,14 +108,82 @@
     replace_ind = np.where(
         np.isin(original_table[key_column], new_val_array[:, 0])
     )
     original_table[replace_column][replace_ind] = new_val_array[:, 1]
     return original_table
 
 
+def get_fetching_table_from_stack(stack):
+    """Get all classes from a stack of tables."""
+    classes = set()
+    for frame_info in stack:
+        locals_dict = frame_info.frame.f_locals
+        for obj in locals_dict.values():
+            if not isinstance(obj, UserTable):
+                continue  # skip non-tables
+            if (name := obj.full_table_name) in PERIPHERAL_TABLES:
+                continue  # skip common_nwbfile tables
+            classes.add(name)
+    if len(classes) > 1:
+        logger.warn(
+            f"Multiple classes found in stack: {classes}. "
+            "Please submit a bug report with the snippet used."
+        )
+        classes = None  # predict only one but not sure, so return None
+    return next(iter(classes)) if classes else None
+
+
+def get_nwb_table(query_expression, tbl, attr_name, *attrs, **kwargs):
+    """Get the NWB file name and path from the given DataJoint query.
+
+    Parameters
+    ----------
+    query_expression : query
+        A DataJoint query expression (e.g., join, restrict) or a table to call fetch on.
+    tbl : table
+        DataJoint table to fetch from.
+    attr_name : str
+        Attribute name to fetch from the table.
+    *attrs : list
+        Attributes from normal DataJoint fetch call.
+    **kwargs : dict
+        Keyword arguments from normal DataJoint fetch call.
+
+    Returns
+    -------
+    nwb_files : list
+        List of NWB file names.
+    file_path_fn : function
+        Function to get the absolute path to the NWB file.
+    """
+    from spyglass.common.common_nwbfile import AnalysisNwbfile, Nwbfile
+
+    kwargs["as_dict"] = True  # force return as dictionary
+    attrs = attrs or query_expression.heading.names  # if none, all
+
+    which = "analysis" if "analysis" in attr_name else "nwb"
+    tbl_map = {  # map to file_name_str and file_path_fn
+        "analysis": ["analysis_file_name", AnalysisNwbfile.get_abs_path],
+        "nwb": ["nwb_file_name", Nwbfile.get_abs_path],
+    }
+    file_name_str, file_path_fn = tbl_map[which]
+
+    # TODO: check that the query_expression restricts tbl - CBroz
+    nwb_files = (
+        query_expression * tbl.proj(nwb2load_filepath=attr_name)
+    ).fetch(file_name_str)
+
+    if which == "analysis":  # log access of analysis files to log table
+        AnalysisNwbfile().increment_access(
+            nwb_files, table=get_fetching_table_from_stack(inspect.stack())
+        )
+
+    return nwb_files, file_path_fn
+
+
 def fetch_nwb(query_expression, nwb_master, *attrs, **kwargs):
     """Get an NWB object from the given DataJoint query.
 
     Parameters
     ----------
     query_expression : query
         A DataJoint query expression (e.g., join, restrict) or a table to call fetch on.
@@ -124,40 +199,28 @@
 
     Returns
     -------
     nwb_objects : list
         List of dicts containing fetch results and NWB objects.
     """
     kwargs["as_dict"] = True  # force return as dictionary
+
     tbl, attr_name = nwb_master
 
     if not attrs:
         attrs = query_expression.heading.names
 
-    # get the list of analysis or nwb files
-    file_name_str = (
-        "analysis_file_name" if "analysis" in nwb_master[1] else "nwb_file_name"
-    )
-    # TODO: avoid this import?
-    from ..common.common_nwbfile import AnalysisNwbfile, Nwbfile
-
-    file_path_fn = (
-        AnalysisNwbfile.get_abs_path
-        if "analysis" in nwb_master[1]
-        else Nwbfile.get_abs_path
+    nwb_files, file_path_fn = get_nwb_table(
+        query_expression, tbl, attr_name, *attrs, **kwargs
     )
 
-    # TODO: check that the query_expression restricts tbl - CBroz
-    nwb_files = (
-        query_expression * tbl.proj(nwb2load_filepath=attr_name)
-    ).fetch(file_name_str)
     for file_name in nwb_files:
         file_path = file_path_fn(file_name)
-        if not os.path.exists(file_path):
-            # retrieve the file from kachery. This also opens the file and stores the file object
+        if not os.path.exists(file_path):  # retrieve the file from kachery.
+            # This also opens the file and stores the file object
             get_nwb_file(file_path)
 
     rec_dicts = (
         query_expression * tbl.proj(nwb2load_filepath=attr_name)
     ).fetch(*attrs, "nwb2load_filepath", **kwargs)
 
     if not rec_dicts or not np.any(
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/utils/dj_merge_tables.py` & `spyglass_neuro-0.5.2/src/spyglass/utils/dj_merge_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,38 @@
 from IPython.core.display import HTML
 
 from spyglass.utils.logging import logger
 
 RESERVED_PRIMARY_KEY = "merge_id"
 RESERVED_SECONDARY_KEY = "source"
 RESERVED_SK_LENGTH = 32
+MERGE_DEFINITION = (
+    f"\n    {RESERVED_PRIMARY_KEY}: uuid\n    ---\n"
+    + f"    {RESERVED_SECONDARY_KEY}: varchar({RESERVED_SK_LENGTH})\n    "
+)
+
+
+def is_merge_table(table):
+    """Return True if table definition matches the default Merge table.
+
+    Regex removes comments and blank lines before comparison.
+    """
+    if not isinstance(table, dj.Table):
+        return False
+    if isinstance(table, dj.FreeTable):
+        fields, pk = table.heading.names, table.primary_key
+        return fields == [
+            RESERVED_PRIMARY_KEY,
+            RESERVED_SECONDARY_KEY,
+        ] and pk == [RESERVED_PRIMARY_KEY]
+    return MERGE_DEFINITION == re.sub(
+        r"\n\s*\n",
+        "\n",
+        re.sub(r"#.*\n", "\n", getattr(table, "definition", "")),
+    )
 
 
 class Merge(dj.Manual):
     """Adds funcs to support standard Merge table operations.
 
     Many methods have the @classmethod decorator to permit MergeTable.method()
     symtax. This makes access to instance attributes (e.g., (MergeTable &
@@ -30,29 +54,24 @@
     view rather than the master table itself.
     """
 
     def __init__(self):
         super().__init__()
         self._reserved_pk = RESERVED_PRIMARY_KEY
         self._reserved_sk = RESERVED_SECONDARY_KEY
-        merge_def = (
-            f"\n    {self._reserved_pk}: uuid\n    ---\n"
-            + f"    {self._reserved_sk}: varchar({RESERVED_SK_LENGTH})\n    "
-        )
         if not self.is_declared:
-            # remove comments after # from each line of definition
-            if self._remove_comments(self.definition) != merge_def:
+            if not is_merge_table(self):  # Check definition
                 logger.warn(
-                    "Merge table with non-default definition\n\t"
-                    + f"Expected: {merge_def.strip()}\n\t"
+                    "Merge table with non-default definition\n"
+                    + f"Expected: {MERGE_DEFINITION.strip()}\n"
                     + f"Actual  : {self.definition.strip()}"
                 )
             for part in self.parts(as_objects=True):
                 if part.primary_key != self.primary_key:
-                    logger.warn(
+                    logger.warn(  # PK is only 'merge_id' in parts, no others
                         f"Unexpected primary key in {part.table_name}"
                         + f"\n\tExpected: {self.primary_key}"
                         + f"\n\tActual  : {part.primary_key}"
                     )
         self._source_class_dict = {}
 
     def _remove_comments(self, definition):
@@ -328,14 +347,17 @@
                     keys = (part_parent & row).fetch("KEY")  # get pk
                     if len(keys) > 1:
                         raise ValueError(
                             "Ambiguous entry. Data has mult rows in "
                             + f"{part_name}:\n\tData:{row}\n\t{keys}"
                         )
                     key = keys[0]
+                    if part & key:
+                        print(f"Key already in part {part_name}: {key}")
+                        continue
                     master_sk = {cls()._reserved_sk: part_name}
                     uuid = dj.hash.key_hash(key | master_sk)
                     master_pk = {cls()._reserved_pk: uuid}
 
                     master_entries.append({**master_pk, **master_sk})
                     parts_entries[part].append({**master_pk, **key})
 
@@ -773,28 +795,34 @@
             keys = parent_class.key_source
         parent_class.populate(keys)
         successes = (parent_class & keys).fetch("KEY", as_dict=True)
         self.insert(successes)
 
     def delete(self, force_permission=False, *args, **kwargs):
         """Alias for cautious_delete, overwrites datajoint.table.Table.delete"""
-        for part in self.merge_get_part(
-            restriction=self.restriction,
-            multi_source=True,
-            return_empties=False,
+        if not (
+            parts := self.merge_get_part(
+                restriction=self.restriction,
+                multi_source=True,
+                return_empties=False,
+            )
         ):
+            return
+
+        for part in parts:
             part.delete(force_permission=force_permission, *args, **kwargs)
 
-    def super_delete(self, *args, **kwargs):
+    def super_delete(self, warn=True, *args, **kwargs):
         """Alias for datajoint.table.Table.delete.
 
-        Added to support MRO of SpyglassMixin"""
-        logger.warning("!! Using super_delete. Bypassing cautious_delete !!")
-
-        self._log_use(start=time(), super_delete=True)
+        Added to support MRO of SpyglassMixin
+        """
+        if warn:
+            logger.warning("!! Bypassing cautious_delete !!")
+            self._log_use(start=time(), super_delete=True)
         super().delete(*args, **kwargs)
 
 
 _Merge = Merge
 
 # Underscore as class name avoids errors when this included in a Diagram
 # Aliased because underscore otherwise excludes from API docs.
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/utils/dj_mixin.py` & `spyglass_neuro-0.5.2/src/spyglass/utils/dj_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,40 @@
+from atexit import register as exit_register
+from atexit import unregister as exit_unregister
 from collections import OrderedDict
 from functools import cached_property
+from inspect import stack as inspect_stack
+from os import environ
 from time import time
 from typing import Dict, List, Union
 
 import datajoint as dj
+from datajoint.condition import make_condition
 from datajoint.errors import DataJointError
 from datajoint.expression import QueryExpression
 from datajoint.logging import logger as dj_logger
 from datajoint.table import Table
 from datajoint.utils import get_master, user_choice
+from networkx import NetworkXError
 from pymysql.err import DataError
 
 from spyglass.utils.database_settings import SHARED_MODULES
 from spyglass.utils.dj_chains import TableChain, TableChains
-from spyglass.utils.dj_helper_fn import fetch_nwb
+from spyglass.utils.dj_helper_fn import fetch_nwb, get_nwb_table
 from spyglass.utils.dj_merge_tables import RESERVED_PRIMARY_KEY as MERGE_PK
+from spyglass.utils.dj_merge_tables import Merge, is_merge_table
 from spyglass.utils.logging import logger
 
+try:
+    import pynapple  # noqa F401
+except ImportError:
+    pynapple = None
+
+EXPORT_ENV_VAR = "SPYGLASS_EXPORT_ID"
+
 
 class SpyglassMixin:
     """Mixin for Spyglass DataJoint tables.
 
     Provides methods for fetching NWBFile objects and checking user permission
     prior to deleting. As a mixin class, all Spyglass tables can inherit custom
     methods from a central location.
@@ -58,28 +72,30 @@
     _member_pk = None  # LabMember primary key. Mixin ambivalent table structure
 
     def __init__(self, *args, **kwargs):
         """Initialize SpyglassMixin.
 
         Checks that schema prefix is in SHARED_MODULES.
         """
-        if (
-            self.database  # Connected to a database
-            and not self.is_declared  # New table
-            and self.database.split("_")[0]  # Prefix
-            not in [
-                *SHARED_MODULES,  # Shared modules
-                dj.config["database.user"],  # User schema
-                "temp",
-                "test",
-            ]
-        ):
+        if self.is_declared:
+            return
+        if self.database and self.database.split("_")[0] not in [
+            *SHARED_MODULES,
+            dj.config["database.user"],
+            "temp",
+            "test",
+        ]:
             logger.error(
                 f"Schema prefix not in SHARED_MODULES: {self.database}"
             )
+        if is_merge_table(self) and not isinstance(self, Merge):
+            raise TypeError(
+                "Table definition matches Merge but does not inherit class: "
+                + self.full_table_name
+            )
 
     # ------------------------------- fetch_nwb -------------------------------
 
     @cached_property
     def _nwb_table_tuple(self) -> tuple:
         """NWBFile table class.
 
@@ -115,43 +131,117 @@
     def fetch_nwb(self, *attrs, **kwargs):
         """Fetch NWBFile object from relevant table.
 
         Implementing class must have a foreign key reference to Nwbfile or
         AnalysisNwbfile (i.e., "-> (Analysis)Nwbfile" in definition)
         or a _nwb_table attribute. If both are present, the attribute takes
         precedence.
+
+        Additional logic support Export table logging.
         """
+        table, tbl_attr = self._nwb_table_tuple
+
+        if self.export_id and "analysis" in tbl_attr:
+            tbl_pk = "analysis_file_name"
+            fnames = (self * table).fetch(tbl_pk)
+            logger.debug(
+                f"Export {self.export_id}: fetch_nwb {self.table_name}, {fnames}"
+            )
+            self._export_table.File.insert(
+                [
+                    {"export_id": self.export_id, tbl_pk: fname}
+                    for fname in fnames
+                ],
+                skip_duplicates=True,
+            )
+            self._export_table.Table.insert1(
+                dict(
+                    export_id=self.export_id,
+                    table_name=self.full_table_name,
+                    restriction=make_condition(self, self.restriction, set()),
+                ),
+                skip_duplicates=True,
+            )
+
         return fetch_nwb(self, self._nwb_table_tuple, *attrs, **kwargs)
 
+    def fetch_pynapple(self, *attrs, **kwargs):
+        """Get a pynapple object from the given DataJoint query.
+
+        Parameters
+        ----------
+        *attrs : list
+            Attributes from normal DataJoint fetch call.
+        **kwargs : dict
+            Keyword arguments from normal DataJoint fetch call.
+
+        Returns
+        -------
+        pynapple_objects : list of pynapple objects
+            List of dicts containing pynapple objects.
+
+        Raises
+        ------
+        ImportError
+            If pynapple is not installed.
+
+        """
+        if pynapple is None:
+            raise ImportError("Pynapple is not installed.")
+
+        nwb_files, file_path_fn = get_nwb_table(
+            self,
+            self._nwb_table_tuple[0],
+            self._nwb_table_tuple[1],
+            *attrs,
+            **kwargs,
+        )
+
+        return [
+            pynapple.load_file(file_path_fn(file_name))
+            for file_name in nwb_files
+        ]
+
     # ------------------------ delete_downstream_merge ------------------------
 
     @cached_property
     def _merge_tables(self) -> Dict[str, dj.FreeTable]:
         """Dict of merge tables downstream of self: {full_table_name: FreeTable}.
 
         Cache of items in parents of self.descendants(as_objects=True). Both
         descendant and parent must have the reserved primary key 'merge_id'.
         """
         self.connection.dependencies.load()
         merge_tables = {}
+        visited = set()
 
         def search_descendants(parent):
+            # TODO: Add check that parents are in the graph. If not, raise error
+            #       asking user to import the table.
+            # TODO: Make a `is_merge_table` helper, and check for false
+            #       positives in the mixin init.
             for desc in parent.descendants(as_objects=True):
                 if (
                     MERGE_PK not in desc.heading.names
                     or not (master_name := get_master(desc.full_table_name))
                     or master_name in merge_tables
                 ):
                     continue
-                master = dj.FreeTable(self.connection, master_name)
-                if MERGE_PK in master.heading.names:
-                    merge_tables[master_name] = master
-                    search_descendants(master)
+                master_ft = dj.FreeTable(self.connection, master_name)
+                if is_merge_table(master_ft):
+                    merge_tables[master_name] = master_ft
+                if master_name not in visited:
+                    visited.add(master_name)
+                    search_descendants(master_ft)
 
-        _ = search_descendants(self)
+        try:
+            _ = search_descendants(self)
+        except NetworkXError as e:
+            table_name = "".join(e.args[0].split("`")[1:4])
+            raise ValueError(f"Please import {table_name} and try again.")
 
         logger.info(
             f"Building merge cache for {self.table_name}.\n\t"
             + f"Found {len(merge_tables)} downstream merge tables"
         )
 
         return merge_tables
@@ -185,14 +275,15 @@
         )
 
     def _get_chain(self, substring) -> TableChains:
         """Return chain from self to merge table with substring in name."""
         for name, chain in self._merge_chains.items():
             if substring.lower() in name:
                 return chain
+        raise ValueError(f"No chain found with '{substring}' in name.")
 
     def _commit_merge_deletes(
         self, merge_join_dict: Dict[str, List[QueryExpression]], **kwargs
     ) -> None:
         """Commit merge deletes.
 
         Parameters
@@ -309,22 +400,27 @@
             Join of table link with Session table.
 
         Returns
         -------
         str
             Summary of experimenters for session(s).
         """
+
         Session = self._delete_deps[-1]
         SesExp = Session.Experimenter
-        empty_pk = {self._member_pk: "NULL"}
 
+        # Not called in delete permission check, only bare _get_exp_summary
+        if self._member_pk in self.heading.names:
+            return self * SesExp
+
+        empty_pk = {self._member_pk: "NULL"}
         format = dj.U(self._session_pk, self._member_pk)
-        sess_link = self._session_connection.join(
-            self.restriction, reverse_order=True
-        )
+
+        restr = self.restriction or True
+        sess_link = self._session_connection.join(restr, reverse_order=True)
 
         exp_missing = format & (sess_link - SesExp).proj(**empty_pk)
         exp_present = format & (sess_link * SesExp - exp_missing).proj()
 
         return exp_missing + exp_present
 
     @cached_property
@@ -358,26 +454,28 @@
         """
         LabMember, LabTeam, Session = self._delete_deps
 
         dj_user = dj.config["database.user"]
         if dj_user in LabMember().admin:  # bypass permission check for admin
             return
 
-        if not self._session_connection:
+        if (
+            not self._session_connection  # Table has no session
+            or self._member_pk in self.heading.names  # Table has experimenter
+        ):
             logger.warn(  # Permit delete if no session connection
                 "Could not find lab team associated with "
                 + f"{self.__class__.__name__}."
                 + "\nBe careful not to delete others' data."
             )
             return
 
         sess_summary = self._get_exp_summary()
         experimenters = sess_summary.fetch(self._member_pk)
         if None in experimenters:
-            # TODO: Check if allow delete of remainder?
             raise PermissionError(
                 "Please ensure all Sessions have an experimenter in "
                 + f"SessionExperimenter:\n{sess_summary}"
             )
 
         user_name = LabMember().get_djuser_name(dj_user)
         for experimenter in set(experimenters):
@@ -399,15 +497,15 @@
     @cached_property
     def _usage_table(self):
         """Temporary inclusion for usage tracking."""
         from spyglass.common.common_usage import CautiousDelete
 
         return CautiousDelete()
 
-    def _log_use(self, start, merge_deletes=None, super_delete=False):
+    def _log_delete(self, start, merge_deletes=None, super_delete=False):
         """Log use of cautious_delete."""
         if isinstance(merge_deletes, QueryExpression):
             merge_deletes = merge_deletes.fetch(as_dict=True)
         safe_insert = dict(
             duration=time() - start,
             dj_user=dj.config["database.user"],
             origin=self.full_table_name,
@@ -469,27 +567,173 @@
                 not self._test_mode
                 or not safemode
                 or user_choice("Commit deletes?", default="no") == "yes"
             ):
                 self._commit_merge_deletes(merge_deletes, **kwargs)
             else:
                 logger.info("Delete aborted.")
-                self._log_use(start)
+                self._log_delete(start)
                 return
 
         super().delete(*args, **kwargs)  # Additional confirm here
 
-        self._log_use(start=start, merge_deletes=merge_deletes)
+        self._log_delete(start=start, merge_deletes=merge_deletes)
 
     def cdel(self, force_permission=False, *args, **kwargs):
         """Alias for cautious_delete."""
         self.cautious_delete(force_permission=force_permission, *args, **kwargs)
 
     def delete(self, force_permission=False, *args, **kwargs):
         """Alias for cautious_delete, overwrites datajoint.table.Table.delete"""
         self.cautious_delete(force_permission=force_permission, *args, **kwargs)
 
-    def super_delete(self, *args, **kwargs):
+    def super_delete(self, warn=True, *args, **kwargs):
         """Alias for datajoint.table.Table.delete."""
-        logger.warning("!! Using super_delete. Bypassing cautious_delete !!")
-        self._log_use(start=time(), super_delete=True)
+        if warn:
+            logger.warning("!! Bypassing cautious_delete !!")
+            self._log_delete(start=time(), super_delete=True)
         super().delete(*args, **kwargs)
+
+    # ------------------------------- Export Log -------------------------------
+
+    @cached_property
+    def _spyglass_version(self):
+        """Get Spyglass version from dj.config."""
+        from spyglass import __version__ as sg_version
+
+        return ".".join(sg_version.split(".")[:3])  # Major.Minor.Patch
+
+    @cached_property
+    def _export_table(self):
+        """Lazy load export selection table."""
+        from spyglass.common.common_usage import ExportSelection
+
+        return ExportSelection()
+
+    @property
+    def export_id(self):
+        """ID of export in progress.
+
+        NOTE: User of an env variable to store export_id may not be thread safe.
+        Exports must be run in sequence, not parallel.
+        """
+
+        return int(environ.get(EXPORT_ENV_VAR, 0))
+
+    @export_id.setter
+    def export_id(self, value):
+        """Set ID of export using `table.export_id = X` notation."""
+        if self.export_id != 0 and self.export_id != value:
+            raise RuntimeError("Export already in progress.")
+        environ[EXPORT_ENV_VAR] = str(value)
+        exit_register(self._export_id_cleanup)  # End export on exit
+
+    @export_id.deleter
+    def export_id(self):
+        """Delete ID of export using `del table.export_id` notation."""
+        self._export_id_cleanup()
+
+    def _export_id_cleanup(self):
+        """Cleanup export ID."""
+        if environ.get(EXPORT_ENV_VAR):
+            del environ[EXPORT_ENV_VAR]
+        exit_unregister(self._export_id_cleanup)  # Remove exit hook
+
+    def _start_export(self, paper_id, analysis_id):
+        """Start export process."""
+        if self.export_id:
+            logger.info(f"Export {self.export_id} in progress. Starting new.")
+            self._stop_export(warn=False)
+
+        self.export_id = self._export_table.insert1_return_pk(
+            dict(
+                paper_id=paper_id,
+                analysis_id=analysis_id,
+                spyglass_version=self._spyglass_version,
+            )
+        )
+
+    def _stop_export(self, warn=True):
+        """End export process."""
+        if not self.export_id and warn:
+            logger.warning("Export not in progress.")
+        del self.export_id
+
+    def _log_fetch(self, *args, **kwargs):
+        """Log fetch for export."""
+        if not self.export_id or self.database == "common_usage":
+            return
+
+        banned = [
+            "head",  # Prevents on Table().head() call
+            "tail",  # Prevents on Table().tail() call
+            "preview",  # Prevents on Table() call
+            "_repr_html_",  # Prevents on Table() call in notebook
+            "cautious_delete",  # Prevents add on permission check during delete
+            "get_abs_path",  # Assumes that fetch_nwb will catch file/table
+        ]
+        called = [i.function for i in inspect_stack()]
+        if set(banned) & set(called):  # if called by any in banned, return
+            return
+
+        logger.debug(f"Export {self.export_id}: fetch()   {self.table_name}")
+
+        restr = self.restriction or True
+        limit = kwargs.get("limit")
+        offset = kwargs.get("offset")
+        if limit or offset:  # Use result as restr if limit/offset
+            restr = self.restrict(restr).fetch(
+                log_fetch=False, as_dict=True, limit=limit, offset=offset
+            )
+
+        restr_str = make_condition(self, restr, set())
+
+        if isinstance(restr_str, str) and len(restr_str) > 2048:
+            raise RuntimeError(
+                "Export cannot handle restrictions > 2048.\n\t"
+                + "If required, please open an issue on GitHub.\n\t"
+                + f"Restriction: {restr_str}"
+            )
+        self._export_table.Table.insert1(
+            dict(
+                export_id=self.export_id,
+                table_name=self.full_table_name,
+                restriction=restr_str,
+            ),
+            skip_duplicates=True,
+        )
+
+    def fetch(self, *args, log_fetch=True, **kwargs):
+        """Log fetch for export."""
+        ret = super().fetch(*args, **kwargs)
+        if log_fetch:
+            self._log_fetch(*args, **kwargs)
+        return ret
+
+    def fetch1(self, *args, log_fetch=True, **kwargs):
+        """Log fetch1 for export."""
+        ret = super().fetch1(*args, **kwargs)
+        if log_fetch:
+            self._log_fetch(*args, **kwargs)
+        return ret
+
+    # ------------------------- Other helper methods -------------------------
+
+    def _auto_increment(self, key, pk, *args, **kwargs):
+        """Auto-increment primary key."""
+        if not key.get(pk):
+            key[pk] = (dj.U().aggr(self, n=f"max({pk})").fetch1("n") or 0) + 1
+        return key
+
+    def file_like(self, name=None, **kwargs):
+        """Convenience method for wildcard search on file name fields."""
+        if not name:
+            return self & True
+        attr = None
+        for field in self.heading.names:
+            if "file" in field:
+                attr = field
+                break
+        if not attr:
+            logger.error(f"No file-like field found in {self.full_table_name}")
+            return
+        return self & f"{attr} LIKE '%{name}%'"
```

### Comparing `spyglass_neuro-0.5.1/src/spyglass/utils/logging.py` & `spyglass_neuro-0.5.2/src/spyglass/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/src/spyglass/utils/nwb_helper_fn.py` & `spyglass_neuro-0.5.2/src/spyglass/utils/nwb_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/README.md` & `spyglass_neuro-0.5.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/conftest.py` & `spyglass_neuro-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/container.py` & `spyglass_neuro-0.5.2/tests/container.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/conftest.py` & `spyglass_neuro-0.5.2/tests/common/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_behav.py` & `spyglass_neuro-0.5.2/tests/common/test_behav.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_device.py` & `spyglass_neuro-0.5.2/tests/common/test_device.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_dio.py` & `spyglass_neuro-0.5.2/tests/common/test_dio.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_ephys.py` & `spyglass_neuro-0.5.2/tests/common/test_ephys.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_filter.py` & `spyglass_neuro-0.5.2/tests/common/test_filter.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_insert.py` & `spyglass_neuro-0.5.2/tests/common/test_insert.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_interval.py` & `spyglass_neuro-0.5.2/tests/common/test_interval.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_interval_helpers.py` & `spyglass_neuro-0.5.2/tests/common/test_interval_helpers.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_lab.py` & `spyglass_neuro-0.5.2/tests/common/test_lab.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_nwbfile.py` & `spyglass_neuro-0.5.2/tests/common/test_nwbfile.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_position.py` & `spyglass_neuro-0.5.2/tests/common/test_position.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_region.py` & `spyglass_neuro-0.5.2/tests/common/test_region.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_sensors.py` & `spyglass_neuro-0.5.2/tests/common/test_sensors.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/common/test_session.py` & `spyglass_neuro-0.5.2/tests/common/test_session.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/data_import/test_insert_sessions.py` & `spyglass_neuro-0.5.2/tests/data_import/test_insert_sessions.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/lfp/conftest.py` & `spyglass_neuro-0.5.2/tests/lfp/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/lfp/test_lfp.py` & `spyglass_neuro-0.5.2/tests/lfp/test_lfp.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/linearization/conftest.py` & `spyglass_neuro-0.5.2/tests/linearization/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/position/test_trodes.py` & `spyglass_neuro-0.5.2/tests/position/test_trodes.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/utils/conftest.py` & `spyglass_neuro-0.5.2/tests/utils/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     if teardown:
         schema_test.drop(force=True)
 
 
 @pytest.fixture(scope="module")
 def chains(Nwbfile):
     """Return example TableChains object from Nwbfile."""
+    from spyglass.lfp.lfp_merge import LFPOutput  # noqa: F401
+    from spyglass.linearization.merge import (
+        LinearizedPositionOutput,
+    )  # noqa: F401
+    from spyglass.position.position_merge import PositionOutput  # noqa: F401
+
     yield Nwbfile._get_chain("linear")
 
 
 @pytest.fixture(scope="module")
 def chain(chains):
     """Return example TableChain object from chains."""
     yield chains[0]
```

### Comparing `spyglass_neuro-0.5.1/tests/utils/test_chains.py` & `spyglass_neuro-0.5.2/tests/utils/test_chains.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+from datajoint.utils import to_camel_case
 
 
 @pytest.fixture(scope="session")
 def TableChain():
     from spyglass.utils.dj_chains import TableChain
 
     return TableChain
@@ -27,24 +28,21 @@
     with pytest.raises(TypeError):
         TableChain(Nwbfile, pos_merge_tables[0])
 
 
 def test_chain_str(chain):
     """Test that the str of a TableChain object is as expected."""
     chain = chain
-    str_got = str(chain)
-    str_exp = (
-        chain.parent.table_name + chain._link_symbol + chain.child.table_name
-    )
-    assert str_got == str_exp, "Unexpected str of TableChain object."
+    parent = to_camel_case(chain.parent.table_name)
+    child = to_camel_case(chain.child.table_name)
 
+    str_got = str(chain)
+    str_exp = parent + chain._link_symbol + child
 
-def test_chain_str_no_link(no_link_chain):
-    """Test that the str of a TableChain object with no link is as expected."""
-    assert str(no_link_chain) == "No link", "Unexpected str of no link chain."
+    assert str_got == str_exp, "Unexpected str of TableChain object."
 
 
 def test_chain_repr(chain):
     """Test that the repr of a TableChain object is as expected."""
     repr_got = repr(chain)
     repr_ext = "Chain: " + chain._link_symbol.join(
         [t.table_name for t in chain.objects]
@@ -62,7 +60,12 @@
     by_int = chain[0]
     by_str = chain[chain.names[0]]
     assert by_int == by_str, "Getitem by int and str not equal."
 
 
 def test_nolink_join(no_link_chain):
     assert no_link_chain.join() is None, "Unexpected join of no link chain."
+
+
+def test_chain_str_no_link(no_link_chain):
+    """Test that the str of a TableChain object with no link is as expected."""
+    assert str(no_link_chain) == "No link", "Unexpected str of no link chain."
```

### Comparing `spyglass_neuro-0.5.1/tests/utils/test_db_settings.py` & `spyglass_neuro-0.5.2/tests/utils/test_db_settings.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/utils/test_merge.py` & `spyglass_neuro-0.5.2/tests/utils/test_merge.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/utils/test_mixin.py` & `spyglass_neuro-0.5.2/tests/utils/test_mixin.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/tests/utils/test_nwb_helper_fn.py` & `spyglass_neuro-0.5.2/tests/utils/test_nwb_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/.gitignore` & `spyglass_neuro-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/LICENSE` & `spyglass_neuro-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/README.md` & `spyglass_neuro-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,12 +79,12 @@
 ## License/Copyright
 
 License and Copyright notice can be found at
 [https://lorenfranklab.github.io/spyglass/latest/LICENSE/](https://lorenfranklab.github.io/spyglass/latest/LICENSE/)
 
 ## Citation
 
-> Lee, K.H.\*, Denovellis, E.L.\*, Ly, R., Magland, J., Soules, J., Comrie, A.E., Gramling, D.P., Guidera, J.A., Nevers, R., Adenekan, P., Brozdowski, C., Bray, S., Monroe, E., Bak, J.H., Coulter, M.E., Sun, X., Tritt, A., Rübel, O., Nguyen, T., Yatsenko, D., Chu, J., Kemere, C., Garcia, S., Buccino, A., Frank, L.M., 2024. Spyglass: a data analysis framework for reproducible and shareable neuroscience research. bioRxiv. [10.1101/2024.01.25.577295](https://doi.org/10.1101/2024.01.25.577295 ).
+> Lee, K.H.\*, Denovellis, E.L.\*, Ly, R., Magland, J., Soules, J., Comrie, A.E., Gramling, D.P., Guidera, J.A., Nevers, R., Adenekan, P., Brozdowski, C., Bray, S., Monroe, E., Bak, J.H., Coulter, M.E., Sun, X., Broyles, E., Shin, D., Chiang, S., Holobetz, C., Tritt, A., Rübel, O., Nguyen, T., Yatsenko, D., Chu, J., Kemere, C., Garcia, S., Buccino, A., Frank, L.M., 2024. Spyglass: a data analysis framework for reproducible and shareable neuroscience research. bioRxiv. [10.1101/2024.01.25.577295](https://doi.org/10.1101/2024.01.25.577295).
 
 *\* Equal contribution*
 
 See paper related code [here](https://github.com/LorenFrankLab/spyglass-paper).
```

### Comparing `spyglass_neuro-0.5.1/pyproject.toml` & `spyglass_neuro-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spyglass_neuro-0.5.1/PKG-INFO` & `spyglass_neuro-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: spyglass-neuro
-Version: 0.5.1
+Version: 0.5.2
 Summary: Neuroscience data analysis framework for reproducible research
 Project-URL: Homepage, https://github.com/LorenFrankLab/spyglass
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/spyglass/issues
 Author-email: Loren Frank <loren.frank@ucsf.edu>, Kyu Hyun Lee <kyuhyun.lee@ucsf.edu>, Eric Denovellis <eric.denovellis@ucsf.edu>, Ryan Ly <rly@lbl.gov>, Daniel Gramling <daniel.gramling@ucsf.edu>, Chris Brozdowski <chris.broz@ucsf.edu>
 License: Copyright (c) 2020-present Loren Frank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -159,12 +159,12 @@
 ## License/Copyright
 
 License and Copyright notice can be found at
 [https://lorenfranklab.github.io/spyglass/latest/LICENSE/](https://lorenfranklab.github.io/spyglass/latest/LICENSE/)
 
 ## Citation
 
-> Lee, K.H.\*, Denovellis, E.L.\*, Ly, R., Magland, J., Soules, J., Comrie, A.E., Gramling, D.P., Guidera, J.A., Nevers, R., Adenekan, P., Brozdowski, C., Bray, S., Monroe, E., Bak, J.H., Coulter, M.E., Sun, X., Tritt, A., Rübel, O., Nguyen, T., Yatsenko, D., Chu, J., Kemere, C., Garcia, S., Buccino, A., Frank, L.M., 2024. Spyglass: a data analysis framework for reproducible and shareable neuroscience research. bioRxiv. [10.1101/2024.01.25.577295](https://doi.org/10.1101/2024.01.25.577295 ).
+> Lee, K.H.\*, Denovellis, E.L.\*, Ly, R., Magland, J., Soules, J., Comrie, A.E., Gramling, D.P., Guidera, J.A., Nevers, R., Adenekan, P., Brozdowski, C., Bray, S., Monroe, E., Bak, J.H., Coulter, M.E., Sun, X., Broyles, E., Shin, D., Chiang, S., Holobetz, C., Tritt, A., Rübel, O., Nguyen, T., Yatsenko, D., Chu, J., Kemere, C., Garcia, S., Buccino, A., Frank, L.M., 2024. Spyglass: a data analysis framework for reproducible and shareable neuroscience research. bioRxiv. [10.1101/2024.01.25.577295](https://doi.org/10.1101/2024.01.25.577295).
 
 *\* Equal contribution*
 
 See paper related code [here](https://github.com/LorenFrankLab/spyglass-paper).
```

