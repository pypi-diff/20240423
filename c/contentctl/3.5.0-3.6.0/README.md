# Comparing `tmp/contentctl-3.5.0.tar.gz` & `tmp/contentctl-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentctl-3.5.0.tar", max compression
+gzip compressed data, was "contentctl-3.6.0.tar", max compression
```

## Comparing `contentctl-3.5.0.tar` & `contentctl-3.6.0.tar`

### file list

```diff
@@ -1,175 +1,175 @@
--rw-r--r--   0        0        0    11344 2024-04-12 17:31:40.635777 contentctl-3.5.0/LICENSE.md
--rw-r--r--   0        0        0    17550 2024-04-12 17:31:40.635777 contentctl-3.5.0/README.md
--rw-r--r--   0        0        0       22 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/__init__.py
--rw-r--r--   0        0        0     1418 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/acs_deploy.py
--rw-r--r--   0        0        0     2999 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/apav_deploy.py
--rw-r--r--   0        0        0     6965 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/api_deploy.py
--rw-r--r--   0        0        0      704 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/convert.py
--rw-r--r--   0        0        0     5580 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/DataManipulation.py
--rw-r--r--   0        0        0     7257 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/DetectionTestingManager.py
--rw-r--r--   0        0        0    11155 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/GitService.py
--rw-r--r--   0        0        0     2259 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
--rw-r--r--   0        0        0    53389 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
--rw-r--r--   0        0        0     5327 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
--rw-r--r--   0        0        0      370 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
--rw-r--r--   0        0        0     3244 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/progress_bar.py
--rw-r--r--   0        0        0     7015 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingView.py
--rw-r--r--   0        0        0     2050 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
--rw-r--r--   0        0        0     1386 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
--rw-r--r--   0        0        0     4706 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
--rw-r--r--   0        0        0      857 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/doc_gen.py
--rw-r--r--   0        0        0     5273 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/generate.py
--rw-r--r--   0        0        0     3102 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/initialize.py
--rw-r--r--   0        0        0     9333 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/initialize_old.py
--rw-r--r--   0        0        0      992 2024-04-12 17:31:40.635777 contentctl-3.5.0/contentctl/actions/new_content.py
--rw-r--r--   0        0        0    10193 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/release_notes.py
--rw-r--r--   0        0        0     1102 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/reporting.py
--rw-r--r--   0        0        0     3863 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/test.py
--rw-r--r--   0        0        0     2595 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/actions/validate.py
--rw-r--r--   0        0        0    31622 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/contentctl.py
--rw-r--r--   0        0        0     4392 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/enrichments/attack_enrichment.py
--rw-r--r--   0        0        0     3242 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/enrichments/cve_enrichment.py
--rw-r--r--   0        0        0     3418 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/enrichments/splunk_app_enrichment.py
--rw-r--r--   0        0        0     3032 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/config_handler.py
--rw-r--r--   0        0        0     7238 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/link_validator.py
--rw-r--r--   0        0        0        0 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/logger.py
--rw-r--r--   0        0        0    15577 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/helper/utils.py
--rw-r--r--   0        0        0     5861 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/backend_splunk_ba.py
--rw-r--r--   0        0        0     2472 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/baseline_builder.py
--rw-r--r--   0        0        0     2270 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/basic_builder.py
--rw-r--r--   0        0        0    18813 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/detection_builder.py
--rw-r--r--   0        0        0    13161 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/director.py
--rw-r--r--   0        0        0     1244 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/investigation_builder.py
--rw-r--r--   0        0        0     4979 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/new_content_generator.py
--rw-r--r--   0        0        0     5610 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/new_content_questions.py
--rw-r--r--   0        0        0     2100 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/playbook_builder.py
--rw-r--r--   0        0        0    19512 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/sigma_converter.py
--rw-r--r--   0        0        0     7584 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/ssa_detection_builder.py
--rw-r--r--   0        0        0     4755 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/story_builder.py
--rw-r--r--   0        0        0     1385 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/input/yml_reader.py
--rw-r--r--   0        0        0    15069 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/detection_abstract.py
--rw-r--r--   0        0        0     3015 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
--rw-r--r--   0        0        0     7519 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/app.py
--rw-r--r--   0        0        0     1028 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/base_test.py
--rw-r--r--   0        0        0     4752 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/base_test_result.py
--rw-r--r--   0        0        0     1931 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/baseline.py
--rw-r--r--   0        0        0      711 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/baseline_tags.py
--rw-r--r--   0        0        0     6069 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/config.py
--rw-r--r--   0        0        0     3518 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/constants.py
--rw-r--r--   0        0        0    36903 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/correlation_search.py
--rw-r--r--   0        0        0      434 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/data_source.py
--rw-r--r--   0        0        0     1137 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment.py
--rw-r--r--   0        0        0      141 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_email.py
--rw-r--r--   0        0        0      164 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_notable.py
--rw-r--r--   0        0        0      201 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_phantom.py
--rw-r--r--   0        0        0      111 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_rba.py
--rw-r--r--   0        0        0      193 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_scheduling.py
--rw-r--r--   0        0        0      129 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/deployment_slack.py
--rw-r--r--   0        0        0      644 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/detection.py
--rw-r--r--   0        0        0     6338 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/detection_tags.py
--rw-r--r--   0        0        0     2963 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/enums.py
--rw-r--r--   0        0        0     1285 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/integration_test.py
--rw-r--r--   0        0        0      429 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/integration_test_result.py
--rw-r--r--   0        0        0     2151 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/investigation.py
--rw-r--r--   0        0        0      191 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/investigation_tags.py
--rw-r--r--   0        0        0     2397 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/lookup.py
--rw-r--r--   0        0        0     3255 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/macro.py
--rw-r--r--   0        0        0      219 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/mitre_attack_enrichment.py
--rw-r--r--   0        0        0     1605 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/notable_action.py
--rw-r--r--   0        0        0     1288 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/observable.py
--rw-r--r--   0        0        0     1081 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/playbook.py
--rw-r--r--   0        0        0      315 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/playbook_tags.py
--rw-r--r--   0        0        0     6353 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/repo_config.py
--rw-r--r--   0        0        0     4288 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/risk_analysis_action.py
--rw-r--r--   0        0        0      904 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/risk_object.py
--rw-r--r--   0        0        0      325 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/security_content_object.py
--rw-r--r--   0        0        0     5806 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/ssa_detection.py
--rw-r--r--   0        0        0     5668 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/ssa_detection_tags.py
--rw-r--r--   0        0        0     1532 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/story.py
--rw-r--r--   0        0        0     1213 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/story_tags.py
--rw-r--r--   0        0        0    25020 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/test_config.py
--rw-r--r--   0        0        0     2600 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/test_group.py
--rw-r--r--   0        0        0      711 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/threat_object.py
--rw-r--r--   0        0        0     1412 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test.py
--rw-r--r--   0        0        0      606 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_attack_data.py
--rw-r--r--   0        0        0      255 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_baseline.py
--rw-r--r--   0        0        0      182 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_old.py
--rw-r--r--   0        0        0     2874 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/objects/unit_test_result.py
--rw-r--r--   0        0        0     6174 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/api_json_output.py
--rw-r--r--   0        0        0     1701 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/attack_nav_output.py
--rw-r--r--   0        0        0     2130 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/attack_nav_writer.py
--rw-r--r--   0        0        0     5938 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/ba_yml_output.py
--rw-r--r--   0        0        0    24175 2024-04-12 17:31:40.639777 contentctl-3.5.0/contentctl/output/conf_output.py
--rw-r--r--   0        0        0     2960 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/conf_writer.py
--rw-r--r--   0        0        0      960 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/detection_writer.py
--rw-r--r--   0        0        0     3238 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/doc_md_output.py
--rw-r--r--   0        0        0     3935 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/finding_report_writer.py
--rw-r--r--   0        0        0     1089 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/jinja_writer.py
--rw-r--r--   0        0        0      209 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/json_writer.py
--rw-r--r--   0        0        0     2254 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/new_content_yml_output.py
--rw-r--r--   0        0        0     3084 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/svg_output.py
--rw-r--r--   0        0        0      745 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/analyticstories_detections.j2
--rw-r--r--   0        0        0      496 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/analyticstories_investigations.j2
--rw-r--r--   0        0        0      592 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/analyticstories_stories.j2
--rw-r--r--   0        0        0      717 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/app.conf.j2
--rw-r--r--   0        0        0     1047 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/app.manifest.j2
--rw-r--r--   0        0        0      181 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/collections.j2
--rw-r--r--   0        0        0       54 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/content-version.j2
--rw-r--r--   0        0        0      670 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/detection_count.j2
--rw-r--r--   0        0        0      671 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/detection_coverage.j2
--rw-r--r--   0        0        0     1002 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_detection_page.j2
--rw-r--r--   0        0        0     6586 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_detections.j2
--rw-r--r--   0        0        0     1471 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_navigation.j2
--rw-r--r--   0        0        0      203 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_navigation_pages.j2
--rw-r--r--   0        0        0     1681 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_playbooks.j2
--rw-r--r--   0        0        0      679 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_playbooks_page.j2
--rw-r--r--   0        0        0     1822 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_stories.j2
--rw-r--r--   0        0        0      874 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/doc_story_page.j2
--rw-r--r--   0        0        0      994 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/es_investigations_investigations.j2
--rw-r--r--   0        0        0      369 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/es_investigations_stories.j2
--rw-r--r--   0        0        0     1753 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/finding_report.j2
--rw-r--r--   0        0        0      177 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/header.j2
--rw-r--r--   0        0        0      424 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/macros.j2
--rw-r--r--   0        0        0      282 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/macros_detections.j2
--rw-r--r--   0        0        0      221 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/panel.j2
--rw-r--r--   0        0        0     1645 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/savedsearches_baselines.j2
--rw-r--r--   0        0        0     6213 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/savedsearches_detections.j2
--rw-r--r--   0        0        0     1180 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/savedsearches_investigations.j2
--rw-r--r--   0        0        0      897 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt
--rw-r--r--   0        0        0     2538 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt
--rw-r--r--   0        0        0     2432 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt
--rw-r--r--   0        0        0      467 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/README.md
--rw-r--r--   0        0        0      168 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/analytic_stories.conf
--rw-r--r--   0        0        0      685 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/app.conf
--rw-r--r--   0        0        0      319 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/commands.conf
--rw-r--r--   0        0        0       34 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/content-version.conf
--rw-r--r--   0        0        0      208 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/nav/default.xml
--rw-r--r--   0        0        0     8635 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml
--rw-r--r--   0        0        0      696 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml
--rw-r--r--   0        0        0      156 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/distsearch.conf
--rw-r--r--   0        0        0     4257 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/usage_searches.conf
--rw-r--r--   0        0        0      168 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/default/use_case_library.conf
--rw-r--r--   0        0        0      423 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/metadata/default.meta
--rw-r--r--   0        0        0     3658 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon.png
--rw-r--r--   0        0        0     2656 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt.png
--rw-r--r--   0        0        0     7442 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png
--rw-r--r--   0        0        0     3657 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png
--rw-r--r--   0        0        0     1416 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/transforms.j2
--rw-r--r--   0        0        0      925 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/templates/workflow_actions.j2
--rw-r--r--   0        0        0     2682 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/yml_output.py
--rw-r--r--   0        0        0      240 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/output/yml_writer.py
--rw-r--r--   0        0        0      133 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/README
--rw-r--r--   0        0        0     6390 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/app_default.yml
--rw-r--r--   0        0        0     9381 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/datamodels_cim.conf
--rw-r--r--   0        0        0      480 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/datamodels_custom.conf
--rw-r--r--   0        0        0      426 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_anomaly.yml
--rw-r--r--   0        0        0      342 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_baseline.yml
--rw-r--r--   0        0        0      528 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_correlation.yml
--rw-r--r--   0        0        0      336 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_hunting.yml
--rw-r--r--   0        0        0      556 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/deployments/00_default_ttp.yml
--rw-r--r--   0        0        0     3342 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml
--rw-r--r--   0        0        0      159 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/macros/security_content_ctime.yml
--rw-r--r--   0        0        0      162 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/macros/security_content_summariesonly.yml
--rw-r--r--   0        0        0     3095 2024-04-12 17:31:40.643777 contentctl-3.5.0/contentctl/templates/stories/cobalt_strike.yml
--rw-r--r--   0        0        0      815 2024-04-12 17:31:40.643777 contentctl-3.5.0/pyproject.toml
--rw-r--r--   0        0        0    18805 1970-01-01 00:00:00.000000 contentctl-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-23 21:34:59.965770 contentctl-3.6.0/LICENSE.md
+-rw-r--r--   0        0        0    17550 2024-04-23 21:34:59.969770 contentctl-3.6.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/__init__.py
+-rw-r--r--   0        0        0     1418 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/acs_deploy.py
+-rw-r--r--   0        0        0     2999 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/apav_deploy.py
+-rw-r--r--   0        0        0     6965 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/api_deploy.py
+-rw-r--r--   0        0        0      704 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/convert.py
+-rw-r--r--   0        0        0     5580 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/DataManipulation.py
+-rw-r--r--   0        0        0     7257 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/DetectionTestingManager.py
+-rw-r--r--   0        0        0    11155 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/GitService.py
+-rw-r--r--   0        0        0     2259 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
+-rw-r--r--   0        0        0    53389 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
+-rw-r--r--   0        0        0     5327 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
+-rw-r--r--   0        0        0      370 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
+-rw-r--r--   0        0        0     3244 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/progress_bar.py
+-rw-r--r--   0        0        0     7015 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingView.py
+-rw-r--r--   0        0        0     2050 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
+-rw-r--r--   0        0        0     1386 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
+-rw-r--r--   0        0        0     4706 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
+-rw-r--r--   0        0        0      857 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/doc_gen.py
+-rw-r--r--   0        0        0     5273 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/generate.py
+-rw-r--r--   0        0        0     3102 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/initialize.py
+-rw-r--r--   0        0        0     9333 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/initialize_old.py
+-rw-r--r--   0        0        0      992 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/new_content.py
+-rw-r--r--   0        0        0    10193 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/release_notes.py
+-rw-r--r--   0        0        0     1102 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/reporting.py
+-rw-r--r--   0        0        0     3863 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/test.py
+-rw-r--r--   0        0        0     2595 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/validate.py
+-rw-r--r--   0        0        0    31622 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/contentctl.py
+-rw-r--r--   0        0        0     4392 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/enrichments/attack_enrichment.py
+-rw-r--r--   0        0        0     3242 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/enrichments/cve_enrichment.py
+-rw-r--r--   0        0        0     3418 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/enrichments/splunk_app_enrichment.py
+-rw-r--r--   0        0        0     3032 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/config_handler.py
+-rw-r--r--   0        0        0     7238 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/link_validator.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/logger.py
+-rw-r--r--   0        0        0    15577 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/utils.py
+-rw-r--r--   0        0        0     5861 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/backend_splunk_ba.py
+-rw-r--r--   0        0        0     2472 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/baseline_builder.py
+-rw-r--r--   0        0        0     2270 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/basic_builder.py
+-rw-r--r--   0        0        0    18813 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/detection_builder.py
+-rw-r--r--   0        0        0    13161 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/director.py
+-rw-r--r--   0        0        0     1244 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/investigation_builder.py
+-rw-r--r--   0        0        0     4979 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/new_content_generator.py
+-rw-r--r--   0        0        0     5610 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/new_content_questions.py
+-rw-r--r--   0        0        0     2100 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/playbook_builder.py
+-rw-r--r--   0        0        0    19512 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/sigma_converter.py
+-rw-r--r--   0        0        0     7584 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/ssa_detection_builder.py
+-rw-r--r--   0        0        0     4755 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/story_builder.py
+-rw-r--r--   0        0        0     1385 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/yml_reader.py
+-rw-r--r--   0        0        0    15307 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/abstract_security_content_objects/detection_abstract.py
+-rw-r--r--   0        0        0     3015 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
+-rw-r--r--   0        0        0     7519 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/app.py
+-rw-r--r--   0        0        0     1028 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/base_test.py
+-rw-r--r--   0        0        0     4752 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/base_test_result.py
+-rw-r--r--   0        0        0     1931 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/baseline.py
+-rw-r--r--   0        0        0      711 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/baseline_tags.py
+-rw-r--r--   0        0        0     6069 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/config.py
+-rw-r--r--   0        0        0     3518 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/constants.py
+-rw-r--r--   0        0        0    36903 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/correlation_search.py
+-rw-r--r--   0        0        0      434 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/data_source.py
+-rw-r--r--   0        0        0     1137 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment.py
+-rw-r--r--   0        0        0      141 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_email.py
+-rw-r--r--   0        0        0      164 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_notable.py
+-rw-r--r--   0        0        0      201 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_phantom.py
+-rw-r--r--   0        0        0      111 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_rba.py
+-rw-r--r--   0        0        0      193 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_scheduling.py
+-rw-r--r--   0        0        0      129 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_slack.py
+-rw-r--r--   0        0        0      644 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/detection.py
+-rw-r--r--   0        0        0     6338 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/detection_tags.py
+-rw-r--r--   0        0        0     2963 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/enums.py
+-rw-r--r--   0        0        0     1285 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/integration_test.py
+-rw-r--r--   0        0        0      429 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/integration_test_result.py
+-rw-r--r--   0        0        0     2151 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/investigation.py
+-rw-r--r--   0        0        0      191 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/investigation_tags.py
+-rw-r--r--   0        0        0     2397 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/lookup.py
+-rw-r--r--   0        0        0     3255 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/macro.py
+-rw-r--r--   0        0        0      219 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/mitre_attack_enrichment.py
+-rw-r--r--   0        0        0     1605 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/notable_action.py
+-rw-r--r--   0        0        0     1288 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/observable.py
+-rw-r--r--   0        0        0     1081 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/playbook.py
+-rw-r--r--   0        0        0      315 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/playbook_tags.py
+-rw-r--r--   0        0        0     6353 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/repo_config.py
+-rw-r--r--   0        0        0     4288 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/risk_analysis_action.py
+-rw-r--r--   0        0        0      904 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/risk_object.py
+-rw-r--r--   0        0        0      325 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/security_content_object.py
+-rw-r--r--   0        0        0     5806 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/ssa_detection.py
+-rw-r--r--   0        0        0     5668 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/ssa_detection_tags.py
+-rw-r--r--   0        0        0     1532 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/story.py
+-rw-r--r--   0        0        0     1213 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/story_tags.py
+-rw-r--r--   0        0        0    25020 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/test_config.py
+-rw-r--r--   0        0        0     2600 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/test_group.py
+-rw-r--r--   0        0        0      711 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/threat_object.py
+-rw-r--r--   0        0        0     1412 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test.py
+-rw-r--r--   0        0        0      606 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_attack_data.py
+-rw-r--r--   0        0        0      255 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_baseline.py
+-rw-r--r--   0        0        0      182 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_old.py
+-rw-r--r--   0        0        0     2874 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_result.py
+-rw-r--r--   0        0        0     6174 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/api_json_output.py
+-rw-r--r--   0        0        0     1701 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/attack_nav_output.py
+-rw-r--r--   0        0        0     2130 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/attack_nav_writer.py
+-rw-r--r--   0        0        0     5938 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/ba_yml_output.py
+-rw-r--r--   0        0        0    24175 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/conf_output.py
+-rw-r--r--   0        0        0     2960 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/conf_writer.py
+-rw-r--r--   0        0        0      960 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/detection_writer.py
+-rw-r--r--   0        0        0     3238 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/doc_md_output.py
+-rw-r--r--   0        0        0     3935 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/finding_report_writer.py
+-rw-r--r--   0        0        0     1089 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/jinja_writer.py
+-rw-r--r--   0        0        0      209 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/json_writer.py
+-rw-r--r--   0        0        0     2254 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/new_content_yml_output.py
+-rw-r--r--   0        0        0     3084 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/svg_output.py
+-rw-r--r--   0        0        0      745 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/analyticstories_detections.j2
+-rw-r--r--   0        0        0      496 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/analyticstories_investigations.j2
+-rw-r--r--   0        0        0      592 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/analyticstories_stories.j2
+-rw-r--r--   0        0        0      717 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/app.conf.j2
+-rw-r--r--   0        0        0     1047 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/app.manifest.j2
+-rw-r--r--   0        0        0      181 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/collections.j2
+-rw-r--r--   0        0        0       54 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/content-version.j2
+-rw-r--r--   0        0        0      670 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/detection_count.j2
+-rw-r--r--   0        0        0      671 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/detection_coverage.j2
+-rw-r--r--   0        0        0     1002 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_detection_page.j2
+-rw-r--r--   0        0        0     6586 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_detections.j2
+-rw-r--r--   0        0        0     1471 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_navigation.j2
+-rw-r--r--   0        0        0      203 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_navigation_pages.j2
+-rw-r--r--   0        0        0     1681 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_playbooks.j2
+-rw-r--r--   0        0        0      679 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_playbooks_page.j2
+-rw-r--r--   0        0        0     1822 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_stories.j2
+-rw-r--r--   0        0        0      874 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_story_page.j2
+-rw-r--r--   0        0        0      994 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/es_investigations_investigations.j2
+-rw-r--r--   0        0        0      369 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/es_investigations_stories.j2
+-rw-r--r--   0        0        0     1753 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/finding_report.j2
+-rw-r--r--   0        0        0      177 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/header.j2
+-rw-r--r--   0        0        0      424 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/macros.j2
+-rw-r--r--   0        0        0      282 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/macros_detections.j2
+-rw-r--r--   0        0        0      221 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/panel.j2
+-rw-r--r--   0        0        0     1645 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/savedsearches_baselines.j2
+-rw-r--r--   0        0        0     6288 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/savedsearches_detections.j2
+-rw-r--r--   0        0        0     1180 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/savedsearches_investigations.j2
+-rw-r--r--   0        0        0      897 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt
+-rw-r--r--   0        0        0     2538 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt
+-rw-r--r--   0        0        0     2432 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt
+-rw-r--r--   0        0        0      467 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README.md
+-rw-r--r--   0        0        0      168 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/analytic_stories.conf
+-rw-r--r--   0        0        0      685 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/app.conf
+-rw-r--r--   0        0        0      319 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/commands.conf
+-rw-r--r--   0        0        0       34 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/content-version.conf
+-rw-r--r--   0        0        0      208 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/nav/default.xml
+-rw-r--r--   0        0        0     8635 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml
+-rw-r--r--   0        0        0      696 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml
+-rw-r--r--   0        0        0      156 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/distsearch.conf
+-rw-r--r--   0        0        0     4257 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/usage_searches.conf
+-rw-r--r--   0        0        0      168 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/use_case_library.conf
+-rw-r--r--   0        0        0      423 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/metadata/default.meta
+-rw-r--r--   0        0        0     3658 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon.png
+-rw-r--r--   0        0        0     2656 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt.png
+-rw-r--r--   0        0        0     7442 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png
+-rw-r--r--   0        0        0     3657 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png
+-rw-r--r--   0        0        0     1416 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/transforms.j2
+-rw-r--r--   0        0        0      925 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/workflow_actions.j2
+-rw-r--r--   0        0        0     2682 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/output/yml_output.py
+-rw-r--r--   0        0        0      240 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/output/yml_writer.py
+-rw-r--r--   0        0        0      133 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/README
+-rw-r--r--   0        0        0     6390 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/app_default.yml
+-rw-r--r--   0        0        0     9381 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/datamodels_cim.conf
+-rw-r--r--   0        0        0      480 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/datamodels_custom.conf
+-rw-r--r--   0        0        0      426 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_anomaly.yml
+-rw-r--r--   0        0        0      342 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_baseline.yml
+-rw-r--r--   0        0        0      528 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_correlation.yml
+-rw-r--r--   0        0        0      336 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_hunting.yml
+-rw-r--r--   0        0        0      556 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_ttp.yml
+-rw-r--r--   0        0        0     3342 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml
+-rw-r--r--   0        0        0      159 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/macros/security_content_ctime.yml
+-rw-r--r--   0        0        0      162 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/macros/security_content_summariesonly.yml
+-rw-r--r--   0        0        0     3095 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/stories/cobalt_strike.yml
+-rw-r--r--   0        0        0      815 2024-04-23 21:34:59.977770 contentctl-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0    18805 1970-01-01 00:00:00.000000 contentctl-3.6.0/PKG-INFO
```

### Comparing `contentctl-3.5.0/LICENSE.md` & `contentctl-3.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/README.md` & `contentctl-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/acs_deploy.py` & `contentctl-3.6.0/contentctl/actions/acs_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/apav_deploy.py` & `contentctl-3.6.0/contentctl/actions/apav_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/api_deploy.py` & `contentctl-3.6.0/contentctl/actions/api_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/convert.py` & `contentctl-3.6.0/contentctl/actions/convert.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/DataManipulation.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/DataManipulation.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/DetectionTestingManager.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/DetectionTestingManager.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/GitService.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/GitService.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/progress_bar.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/progress_bar.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingView.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingView.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py` & `contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/doc_gen.py` & `contentctl-3.6.0/contentctl/actions/doc_gen.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/generate.py` & `contentctl-3.6.0/contentctl/actions/generate.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/initialize.py` & `contentctl-3.6.0/contentctl/actions/initialize.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/initialize_old.py` & `contentctl-3.6.0/contentctl/actions/initialize_old.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/new_content.py` & `contentctl-3.6.0/contentctl/actions/new_content.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/release_notes.py` & `contentctl-3.6.0/contentctl/actions/release_notes.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/reporting.py` & `contentctl-3.6.0/contentctl/actions/reporting.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/test.py` & `contentctl-3.6.0/contentctl/actions/test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/actions/validate.py` & `contentctl-3.6.0/contentctl/actions/validate.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/contentctl.py` & `contentctl-3.6.0/contentctl/contentctl.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/enrichments/attack_enrichment.py` & `contentctl-3.6.0/contentctl/enrichments/attack_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/enrichments/cve_enrichment.py` & `contentctl-3.6.0/contentctl/enrichments/cve_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/enrichments/splunk_app_enrichment.py` & `contentctl-3.6.0/contentctl/enrichments/splunk_app_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/helper/config_handler.py` & `contentctl-3.6.0/contentctl/helper/config_handler.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/helper/link_validator.py` & `contentctl-3.6.0/contentctl/helper/link_validator.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/helper/utils.py` & `contentctl-3.6.0/contentctl/helper/utils.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/backend_splunk_ba.py` & `contentctl-3.6.0/contentctl/input/backend_splunk_ba.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/baseline_builder.py` & `contentctl-3.6.0/contentctl/input/baseline_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/basic_builder.py` & `contentctl-3.6.0/contentctl/input/basic_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/detection_builder.py` & `contentctl-3.6.0/contentctl/input/detection_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/director.py` & `contentctl-3.6.0/contentctl/input/director.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/investigation_builder.py` & `contentctl-3.6.0/contentctl/input/investigation_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/new_content_generator.py` & `contentctl-3.6.0/contentctl/input/new_content_generator.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/new_content_questions.py` & `contentctl-3.6.0/contentctl/input/new_content_questions.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/playbook_builder.py` & `contentctl-3.6.0/contentctl/input/playbook_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/sigma_converter.py` & `contentctl-3.6.0/contentctl/input/sigma_converter.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/ssa_detection_builder.py` & `contentctl-3.6.0/contentctl/input/ssa_detection_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/story_builder.py` & `contentctl-3.6.0/contentctl/input/story_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/input/yml_reader.py` & `contentctl-3.6.0/contentctl/input/yml_reader.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/detection_abstract.py` & `contentctl-3.6.0/contentctl/objects/abstract_security_content_objects/detection_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     source: str = None
     nes_fields: str = None
     providing_technologies: list = None
     runtime: str = None
     enabled_by_default: bool = False
 
+
     class Config:
         use_enum_values = True
 
 
     # A list of groups of tests, relying on the same data
     test_groups: Union[list[TestGroup], None] = None
 
@@ -342,7 +343,14 @@
                 result["message"] = "NO RESULT - Test not run"
 
             # Add the result to our list
             summary_dict["tests"].append(result)
 
         # Return the summary
         return summary_dict
+
+
+    def getMetadata(self)->dict[str,str]:
+        return {'detection_id':str(self.id),
+                'deprecated':'1' if self.status==DetectionStatus.deprecated.value else '0',
+                'detection_version':str(self.version)}
+
```

### Comparing `contentctl-3.5.0/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py` & `contentctl-3.6.0/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/app.py` & `contentctl-3.6.0/contentctl/objects/app.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/base_test.py` & `contentctl-3.6.0/contentctl/objects/base_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/base_test_result.py` & `contentctl-3.6.0/contentctl/objects/base_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/baseline.py` & `contentctl-3.6.0/contentctl/objects/baseline.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/baseline_tags.py` & `contentctl-3.6.0/contentctl/objects/baseline_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/config.py` & `contentctl-3.6.0/contentctl/objects/config.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/constants.py` & `contentctl-3.6.0/contentctl/objects/constants.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/correlation_search.py` & `contentctl-3.6.0/contentctl/objects/correlation_search.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/deployment.py` & `contentctl-3.6.0/contentctl/objects/deployment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/detection.py` & `contentctl-3.6.0/contentctl/objects/detection.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/detection_tags.py` & `contentctl-3.6.0/contentctl/objects/detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/enums.py` & `contentctl-3.6.0/contentctl/objects/enums.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/integration_test.py` & `contentctl-3.6.0/contentctl/objects/integration_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/investigation.py` & `contentctl-3.6.0/contentctl/objects/investigation.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/lookup.py` & `contentctl-3.6.0/contentctl/objects/lookup.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/macro.py` & `contentctl-3.6.0/contentctl/objects/macro.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/notable_action.py` & `contentctl-3.6.0/contentctl/objects/notable_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/observable.py` & `contentctl-3.6.0/contentctl/objects/observable.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/playbook.py` & `contentctl-3.6.0/contentctl/objects/playbook.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/repo_config.py` & `contentctl-3.6.0/contentctl/objects/repo_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/risk_analysis_action.py` & `contentctl-3.6.0/contentctl/objects/risk_analysis_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/risk_object.py` & `contentctl-3.6.0/contentctl/objects/risk_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/ssa_detection.py` & `contentctl-3.6.0/contentctl/objects/ssa_detection.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/ssa_detection_tags.py` & `contentctl-3.6.0/contentctl/objects/ssa_detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/story.py` & `contentctl-3.6.0/contentctl/objects/story.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/story_tags.py` & `contentctl-3.6.0/contentctl/objects/story_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/test_config.py` & `contentctl-3.6.0/contentctl/objects/test_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/test_group.py` & `contentctl-3.6.0/contentctl/objects/test_group.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/threat_object.py` & `contentctl-3.6.0/contentctl/objects/threat_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/unit_test.py` & `contentctl-3.6.0/contentctl/objects/unit_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/unit_test_attack_data.py` & `contentctl-3.6.0/contentctl/objects/unit_test_attack_data.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/objects/unit_test_result.py` & `contentctl-3.6.0/contentctl/objects/unit_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/api_json_output.py` & `contentctl-3.6.0/contentctl/output/api_json_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/attack_nav_output.py` & `contentctl-3.6.0/contentctl/output/attack_nav_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/attack_nav_writer.py` & `contentctl-3.6.0/contentctl/output/attack_nav_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/ba_yml_output.py` & `contentctl-3.6.0/contentctl/output/ba_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/conf_output.py` & `contentctl-3.6.0/contentctl/output/conf_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/conf_writer.py` & `contentctl-3.6.0/contentctl/output/conf_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/detection_writer.py` & `contentctl-3.6.0/contentctl/output/detection_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/doc_md_output.py` & `contentctl-3.6.0/contentctl/output/doc_md_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/finding_report_writer.py` & `contentctl-3.6.0/contentctl/output/finding_report_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/jinja_writer.py` & `contentctl-3.6.0/contentctl/output/jinja_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/new_content_yml_output.py` & `contentctl-3.6.0/contentctl/output/new_content_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/svg_output.py` & `contentctl-3.6.0/contentctl/output/svg_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/analyticstories_detections.j2` & `contentctl-3.6.0/contentctl/output/templates/analyticstories_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/analyticstories_stories.j2` & `contentctl-3.6.0/contentctl/output/templates/analyticstories_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/app.conf.j2` & `contentctl-3.6.0/contentctl/output/templates/app.conf.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/app.manifest.j2` & `contentctl-3.6.0/contentctl/output/templates/app.manifest.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/detection_count.j2` & `contentctl-3.6.0/contentctl/output/templates/detection_count.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/detection_coverage.j2` & `contentctl-3.6.0/contentctl/output/templates/detection_coverage.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/doc_detection_page.j2` & `contentctl-3.6.0/contentctl/output/templates/doc_detection_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/doc_detections.j2` & `contentctl-3.6.0/contentctl/output/templates/doc_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/doc_navigation.j2` & `contentctl-3.6.0/contentctl/output/templates/doc_navigation.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/doc_playbooks.j2` & `contentctl-3.6.0/contentctl/output/templates/doc_playbooks.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/doc_playbooks_page.j2` & `contentctl-3.6.0/contentctl/output/templates/doc_playbooks_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/doc_stories.j2` & `contentctl-3.6.0/contentctl/output/templates/doc_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/doc_story_page.j2` & `contentctl-3.6.0/contentctl/output/templates/doc_story_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/es_investigations_investigations.j2` & `contentctl-3.6.0/contentctl/output/templates/es_investigations_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/finding_report.j2` & `contentctl-3.6.0/contentctl/output/templates/finding_report.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/savedsearches_baselines.j2` & `contentctl-3.6.0/contentctl/output/templates/savedsearches_baselines.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/savedsearches_detections.j2` & `contentctl-3.6.0/contentctl/output/templates/savedsearches_detections.j2`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 action.correlationsearch.label = {{APP_NAME}} - Experimental - {{ detection.name }} - Rule
 {% elif detection.type | lower == "correlation" %}
 action.correlationsearch.label = {{APP_NAME}} - RIR - {{ detection.name }} - Rule
 {% else %}
 action.correlationsearch.label = {{APP_NAME}} - {{ detection.name }} - Rule
 {% endif %}
 action.correlationsearch.annotations = {{ detection.annotations | tojson }}
+action.correlationsearch.metadata = {{ detection.getMetadata() | tojson }}
 {% if detection.deployment.scheduling.schedule_window is defined %}
 schedule_window = {{ detection.deployment.scheduling.schedule_window }}
 {% endif %}
 {% if detection.deployment is defined %}
 {% if detection.deployment.notable.rule_title is defined %}
 action.notable = 1
 {% if detection.nes_fields is defined %}
```

### Comparing `contentctl-3.5.0/contentctl/output/templates/savedsearches_investigations.j2` & `contentctl-3.6.0/contentctl/output/templates/savedsearches_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/app.conf` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/app.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/default/usage_searches.conf` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/usage_searches.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon.png` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt.png` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png` & `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/transforms.j2` & `contentctl-3.6.0/contentctl/output/templates/transforms.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/templates/workflow_actions.j2` & `contentctl-3.6.0/contentctl/output/templates/workflow_actions.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/output/yml_output.py` & `contentctl-3.6.0/contentctl/output/yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/templates/app_default.yml` & `contentctl-3.6.0/contentctl/templates/app_default.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/templates/datamodels_cim.conf` & `contentctl-3.6.0/contentctl/templates/datamodels_cim.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/templates/deployments/00_default_correlation.yml` & `contentctl-3.6.0/contentctl/templates/deployments/00_default_correlation.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/templates/deployments/00_default_ttp.yml` & `contentctl-3.6.0/contentctl/templates/deployments/00_default_ttp.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml` & `contentctl-3.6.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/contentctl/templates/stories/cobalt_strike.yml` & `contentctl-3.6.0/contentctl/templates/stories/cobalt_strike.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.5.0/pyproject.toml` & `contentctl-3.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contentctl"
-version = "3.5.0"
+version = "3.6.0"
 description = "Splunk Content Control Tool"
 authors = ["STRT <research@splunk.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 contentctl = 'contentctl.contentctl:main'
```

### Comparing `contentctl-3.5.0/PKG-INFO` & `contentctl-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentctl
-Version: 3.5.0
+Version: 3.6.0
 Summary: Splunk Content Control Tool
 License: Apache 2.0
 Author: STRT
 Author-email: research@splunk.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

