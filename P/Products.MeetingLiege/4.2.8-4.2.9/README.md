# Comparing `tmp/Products.MeetingLiege-4.2.8.tar.gz` & `tmp/Products.MeetingLiege-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.MeetingLiege-4.2.8.tar", last modified: Mon Mar 20 08:36:21 2023, max compression
+gzip compressed data, was "dist/Products.MeetingLiege-4.2.9.tar", last modified: Thu Oct  5 08:56:11 2023, max compression
```

## Comparing `Products.MeetingLiege-4.2.8.tar` & `Products.MeetingLiege-4.2.9.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20776 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14590 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      119 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      422 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/indexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2066 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/events.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15159 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      631 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accept_and_return.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      585 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-council_from_meeting-config-college.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      626 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToInternalReviewer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/askAdvicesByInternalReviewer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      374 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_meeting-config-college_from_meeting-config-council.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToGeneralManager.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToAdministrativeReviewer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      664 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToItemCreated.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      882 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/header-bg.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      595 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetReviewer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      740 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_negative_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/askAdvicesByDirector.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/adopts_next_council_agenda.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetReviewer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      619 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetManager.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      374 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_meeting-config-council_from_meeting-config-college.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      631 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accepted_and_returned.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      672 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/logo.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/sendToCouncilEmergency.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      585 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-college_from_meeting-config-council.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/return.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToGeneralManager.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      662 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToInternalReviewer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetManager.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3397 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/wf_down_finances.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accepted_but_modified.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      702 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToFinance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/marked_not_applicable.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    48075 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/spinner.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToValidatedFromSentToCouncilEmergency.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/mark_not_applicable.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/askAdvicesByItemCreator.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      697 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_with_remarks_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accept_but_modify.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3270 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/show_council_data.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/pre_accept.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/pre_accepted.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      646 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToDirector.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      465 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_not_required_finance.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToAdministrativeReviewer.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/returned.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToDirector.png
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_styles/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4322 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3970 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege_restrictedpowerobservers.css.dtml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1560 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_styles/imioapps_properties.props
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8241 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_edit.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42491 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_view.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7611 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/overrides.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7809 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   123744 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1942 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/imio.history.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13206 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/PloneMeeting.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      405 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/eea.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      820 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/collective.eeafaceted.z3ctable.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8239 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16181 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1034 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      684 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      928 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      539 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2472 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7039 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/plone.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      690 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/imio.actionspanel.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      743 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/datagridfield.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9365 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23981 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1173 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      942 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/eea.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3168 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.history.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      347 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/sync_pos.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      153 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/portal_languages.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/MeetingLiege_bourgmestre_marker.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      600 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    12632 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/import_data.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/MeetingLiege_testing_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      730 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/secretary_remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      581 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/decision.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11274 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/SignatureCadranel.jpg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3555 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/logo.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      973 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/courrierCollege.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1032 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/cahier.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/legalAnalysis.png
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      880 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/toolset.xml
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    10107 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/import_data.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      106 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      301 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/propertiestool.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcollegeliege_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   103764 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcollegeliege_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingcouncilliege_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10946 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingcouncilliege_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcouncilliege_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    54862 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcouncilliege_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitembourgmestre_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    83167 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitembourgmestre_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingbourgmestre_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5389 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingbourgmestre_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingcollegeliege_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10946 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingcollegeliege_workflow/definition.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingadviceliege_workflow/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12571 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingadviceliege_workflow/definition.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      890 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/skins.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/types/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3237 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/types/meetingadvicefinances.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1336 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      226 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/types.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/MeetingLiege_marker.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      383 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/actions.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1114 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/toolset.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1059 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/positive.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/attach.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      790 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/medical.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      730 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/secretary_remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/budget.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      642 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/securite.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      510 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/formulaire.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      445 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/courrier.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/remarks.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/legalAdvice.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/negative.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      507 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/rapport.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/deliberation.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/deliberation_to_sign.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/nil.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      834 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/courrierCollege.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1032 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/cahier.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      857 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/juridique.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/MeetingLiege_liege_marker.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    29421 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/synthese_avis_df.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25771 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/college-oj.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19327 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/projet-deliberation.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24283 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/deliberation.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26494 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/college-pv.odt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9874 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/stats_DF_advice.ods
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      880 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/__init__.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/toolset.xml
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    41969 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/import_data.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       23 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1085 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        6 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/version.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5924 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1434 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      235 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/generate.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    54242 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/MeetingLiege.zargo
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2962 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/generate.conf
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       23 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6770 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/pm_updates.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4491 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14980 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/events.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/refresh.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      597 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/Extensions/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16044 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/Extensions/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/Extensions/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      846 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/README.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1248 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testFaceted.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      956 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testAdvices.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1300 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeetingCategory.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1342 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testContacts.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14411 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomAdvices.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4053 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomContacts.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1323 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testChangeItemOrderView.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1204 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testUtils.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1183 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomMeeting.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3165 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/MeetingLiegeTestCase.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1214 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testColumns.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1251 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testSetup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1620 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testToolPloneMeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    74754 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomMeetingItem.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1548 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testWorkflows.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11316 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/helpers.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1395 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeetingItem.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2477 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testWFAdaptations.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1249 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testValidators.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1260 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testPortlets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1075 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testAnnexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   146895 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomWorkflows.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1514 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testSearches.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1204 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testViews.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1313 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeetingConfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3245 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomViews.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3536 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/overrides.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2409 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      504 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19471 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/overrides.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/templates/item_main_infos.pt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/overrides/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/overrides/images/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      196 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/overrides/images/details.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3270 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/overrides/images/more_infos.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       22 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1740 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/migrations/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13355 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/migrations/migrate_to_4200.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11451 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/migrations/migrate_to_4_1.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/migrations/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/src/Products/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      726 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/docs/LICENSE.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1371 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20776 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1199 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16937 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      108 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2023-03-20 08:36:21.000000 Products.MeetingLiege-4.2.8/setup.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21249 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14590 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      119 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      422 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/indexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2066 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/events.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15159 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      631 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accept_and_return.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      585 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-council_from_meeting-config-college.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      626 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToInternalReviewer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/askAdvicesByInternalReviewer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      374 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_meeting-config-college_from_meeting-config-council.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      651 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToGeneralManager.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      638 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToAdministrativeReviewer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      664 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToItemCreated.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      882 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/header-bg.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      595 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetReviewer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      740 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_negative_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/askAdvicesByDirector.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      103 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/adopts_next_council_agenda.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetReviewer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      619 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetManager.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      542 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      374 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_meeting-config-council_from_meeting-config-college.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      631 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accepted_and_returned.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      672 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/logo.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/sendToCouncilEmergency.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      585 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-college_from_meeting-config-council.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/return.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToGeneralManager.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      662 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToInternalReviewer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetManager.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3397 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/wf_down_finances.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accepted_but_modified.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      702 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToFinance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/marked_not_applicable.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    48075 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/spinner.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToValidatedFromSentToCouncilEmergency.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/mark_not_applicable.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      329 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/askAdvicesByItemCreator.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      697 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_with_remarks_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accept_but_modify.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3270 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/show_council_data.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/pre_accept.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      596 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/pre_accepted.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      646 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToDirector.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      465 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_not_required_finance.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToAdministrativeReviewer.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      394 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/returned.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      613 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToDirector.png
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_styles/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4322 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3970 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege_restrictedpowerobservers.css.dtml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1560 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_styles/imioapps_properties.props
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8241 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_edit.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42665 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_view.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7611 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/overrides.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7809 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   123836 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1942 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/imio.history.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13206 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/PloneMeeting.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      405 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/eea.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      820 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/collective.eeafaceted.z3ctable.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8239 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16181 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1034 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      684 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      928 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      539 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2472 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7039 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/plone.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      690 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/imio.actionspanel.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      743 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/datagridfield.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9365 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23981 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1173 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      731 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      942 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      555 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/eea.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3168 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.history.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      347 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/sync_pos.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      153 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/portal_languages.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/MeetingLiege_bourgmestre_marker.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      600 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/__init__.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    12608 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/import_data.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/MeetingLiege_testing_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      880 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      730 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/secretary_remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      742 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      581 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/decision.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11274 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/SignatureCadranel.jpg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3555 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/logo.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      492 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      216 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      973 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/courrierCollege.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1032 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/cahier.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      332 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/legalAnalysis.png
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      880 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/__init__.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/toolset.xml
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    10049 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/import_data.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      106 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      301 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/propertiestool.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcollegeliege_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   103764 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcollegeliege_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingcouncilliege_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10946 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingcouncilliege_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcouncilliege_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    54862 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcouncilliege_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitembourgmestre_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    83167 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitembourgmestre_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingbourgmestre_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5389 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingbourgmestre_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingcollegeliege_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10946 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingcollegeliege_workflow/definition.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingadviceliege_workflow/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    12571 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingadviceliege_workflow/definition.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      890 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/skins.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/types/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3237 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/types/meetingadvicefinances.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1336 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      226 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/types.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/MeetingLiege_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      383 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/actions.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      423 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1114 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/toolset.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1059 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      583 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/positive.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3352 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/attach.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      790 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/medical.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      730 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/secretary_remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      630 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/budget.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      642 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/securite.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      510 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/formulaire.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      445 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/courrier.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      705 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/remarks.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      761 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/legalAdvice.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      885 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/negative.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      507 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/rapport.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      636 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/deliberation.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      328 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/deliberation_to_sign.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      305 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/nil.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      834 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/courrierCollege.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1032 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/cahier.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      857 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/juridique.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      177 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/MeetingLiege_liege_marker.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    29421 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/synthese_avis_df.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25771 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/college-oj.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19327 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/projet-deliberation.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24283 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/deliberation.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    26494 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/college-pv.odt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9874 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/stats_DF_advice.ods
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      880 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/__init__.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      167 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/toolset.xml
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)    42005 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/import_data.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       23 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1085 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        6 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/version.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5924 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1434 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      235 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/generate.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    54242 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/MeetingLiege.zargo
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2962 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/generate.conf
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       23 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6770 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/pm_updates.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4491 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14980 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/refresh.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      597 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/Extensions/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    16044 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/Extensions/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/Extensions/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      846 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/README.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1248 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testFaceted.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      956 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testAdvices.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1300 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeetingCategory.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1342 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testContacts.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    14411 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomAdvices.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4053 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomContacts.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1323 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1204 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testUtils.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1183 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomMeeting.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3165 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/MeetingLiegeTestCase.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1214 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testColumns.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1251 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testSetup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1620 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    74888 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomMeetingItem.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1548 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testWorkflows.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11316 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/helpers.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1395 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeetingItem.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2592 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testWFAdaptations.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1249 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testValidators.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1260 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testPortlets.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1075 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testAnnexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   147053 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomWorkflows.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      951 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1514 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testSearches.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1204 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testViews.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1313 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeetingConfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3245 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomViews.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3536 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2409 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      504 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    19475 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/overrides.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      683 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/templates/item_main_infos.pt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/overrides/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/overrides/images/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      196 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/overrides/images/details.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3270 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/overrides/images/more_infos.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       22 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1740 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/migrations/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13355 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/migrations/migrate_to_4200.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11451 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/migrations/migrate_to_4_1.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/migrations/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/src/Products/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      726 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/docs/LICENSE.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1371 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    21249 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1199 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17322 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      108 2023-10-05 08:56:10.000000 Products.MeetingLiege-4.2.9/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2023-10-05 08:56:11.000000 Products.MeetingLiege-4.2.9/setup.cfg
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/PKG-INFO` & `Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: Products.MeetingLiege
-Version: 4.2.8
+Version: 4.2.9
 Summary: PloneMeeting profile for city of Liege
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: Profile for Products.PloneMeeting for Ville de Liège
         ====================================================
         
         
         Products.MeetingLiege Changelog
         ===============================
         
+        4.2.9 (2023-10-05)
+        ------------------
+        
+        - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+          [gbastien]
+        - Fixed `MLAdviceActionsPanelView` that inherits from `AdviceActionsPanelView` and
+          not `BaseActionsPanelView` so we get the `renderOwnDeleteWithComments`.
+          [gbastien]
+        - Adapted code as `MeetingConfig.useCopies` field was removed.
+          [gbastien]
+        
         4.2.8 (2023-03-20)
         ------------------
         
         - Fixed cachekey for `CustomMeetingItem._roles_in_context`.
           [gbastien]
         - Fixed `meetingitem_view.pt` to use `structure` to display groups in charge.
           [gbastien]
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products.MeetingLiege.egg-info/SOURCES.txt` & `Products.MeetingLiege-4.2.9/src/Products.MeetingLiege.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/events.zcml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/events.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/setuphandlers.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accept_and_return.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accept_and_return.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-council_from_meeting-config-college.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-council_from_meeting-config-college.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToInternalReviewer.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToInternalReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToGeneralManager.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToGeneralManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToAdministrativeReviewer.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToAdministrativeReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToItemCreated.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToItemCreated.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/header-bg.gif` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/header-bg.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetReviewer.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_finance.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_negative_finance.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_negative_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetReviewer.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetManager.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToCabinetManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/will_be_clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accepted_and_returned.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accepted_and_returned.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/logo.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/logo.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/sendToCouncilEmergency.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/sendToCouncilEmergency.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-college_from_meeting-config-council.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_meeting-config-college_from_meeting-config-council.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToGeneralManager.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToGeneralManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToInternalReviewer.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToInternalReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetManager.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToCabinetManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/wf_down_finances.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/wf_down_finances.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accepted_but_modified.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accepted_but_modified.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToFinance.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToFinance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/spinner.gif` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/spinner.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToValidatedFromSentToCouncilEmergency.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToValidatedFromSentToCouncilEmergency.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_with_remarks_finance.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/advice_standard_positive_with_remarks_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/accept_but_modify.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/accept_but_modify.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-council_from_meeting-config-college.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/show_council_data.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/show_council_data.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/clone_to_other_mc_emergency_meeting-config-college_from_meeting-config-council.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToDirector.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToAdministrativeReviewer.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/backToProposedToAdministrativeReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_images/proposeToDirector.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_images/proposeToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege.css.dtml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege.css.dtml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege_restrictedpowerobservers.css.dtml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_styles/meetingliege_restrictedpowerobservers.css.dtml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_styles/imioapps_properties.props` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_styles/imioapps_properties.props`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_edit.pt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_view.pt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/skins/meetingliege_templates/meetingitem_view.pt`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 <span tal:condition="not: advisers">-</span>
                 — <a class="discreet"
                      tal:attributes="href string:${context_url}#advices"
                      i18n:translate="legend_details" i18n:domain="plone">Details</a>
             </div>
 
             <tal:comment replace="nothing">Copy groups for this item</tal:comment>
-            <tal:copyGroups condition="python: context.isCopiesEnabled()">
+            <tal:copyGroups condition="python: context.attribute_is_used('copyGroups')">
                 <div class="discreet" tal:define="copyGroups python: context.getAllCopyGroups();
                                                   copy_groups_have_access python: context.check_copy_groups_have_access();">
                     <span class="item_attribute_label"
                           i18n:translate="PloneMeeting_label_copyGroups"></span>
                     <span tal:define="css_class string:fa fa-question-circle help-doc pmHelp"
                           i18n:attributes="title"
                           tal:attributes="title python: context.getCopyGroupsHelpMsg(cfg);
@@ -551,15 +551,18 @@
       <div id="clonable_to_other_mcs_content">
         <tal:displayOtherMeetingConfigsClonableTo tal:condition="otherMCs">
             <span tal:replace="structure python: context.displayOtherMeetingConfigsClonableTo()">Other mc clonable to (Emergency, privacy)</span>
         </tal:displayOtherMeetingConfigsClonableTo>
         <span tal:condition="not: otherMCs">-</span>
         <div tal:condition="otherMCs">
           <fieldset>
-            <legend i18n:translate="">Data that will be used on new item</legend>
+            <legend i18n:translate="">
+              Data that will be used on new item to
+              <span i18n:name="cfg_titles" tal:content="python: context.displayOtherMeetingConfigsClonableToPossibleValues()" />
+            </legend>
             <tal:otherMeetingConfigsClonableToFieldTitle condition="python: 'otherMeetingConfigsClonableToFieldTitle' in usedAttrs">
               <span class="item_attribute_label"
                     i18n:translate="PloneMeeting_label_itemTitle"></span>:&nbsp;&nbsp;
               <span metal:use-macro="python: here.widget('otherMeetingConfigsClonableToFieldTitle', mode='view')" />
             </tal:otherMeetingConfigsClonableToFieldTitle>
             <tal:loop tal:repeat="other_mc_field_name python: context.get_enable_clone_to_other_mc_fields(cfg, ignored_field_names=['otherMeetingConfigsClonableToFieldTitle'])">
                 <tal:field define="fieldName python: other_mc_field_name; ajaxEdit python:True">
```

#### html2text {}

```diff
@@ -46,15 +46,15 @@
 Description Detailed description Budgetary informations, manage fields
 budgetRelated and budgetInfos
 Budget
 XXX added by MeetingLiege Label for Council Motivation
 Decision DecisionSuite DecisionEnd
 Other meetingConfigs clonable to
 Other mc clonable to (Emergency, privacy) -
-Data that will be used on new item :  
+Data that will be used on new item to :  
 Annexes and advices
   Advices XXX added by MeetingLiege, item with finance advice Finance advice
   text XXX added by MeetingLiege, link to College item if accessible _A_c_c_e_s_s_ _t_h_e
   _C_o_l_l_e_g_e_ _i_t_e_m_ _c_o_n_t_a_i_n_i_n_g_ _g_i_v_e_n_ _f_i_n_a_n_c_e_ _a_d_v_i_c_e_.
 Text check list
 Text check list Nothing to display.
 In and out moves Notes Committee observations Committee transcript Votes
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/overrides.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/overrides.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/configure.zcml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/adapters.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from Products.MeetingLiege.utils import gm_group_uid
 from Products.MeetingLiege.utils import not_copy_group_uids
 from Products.MeetingLiege.utils import treasury_group_cec_uid
 from Products.PloneMeeting.adapters import CompoundCriterionBaseAdapter
 from Products.PloneMeeting.adapters import ItemPrettyLinkAdapter
 from Products.PloneMeeting.adapters import MeetingPrettyLinkAdapter
 from Products.PloneMeeting.adapters import query_user_groups_cachekey
+from Products.PloneMeeting.config import MEETING_REMOVE_MOG_WFA
 from Products.PloneMeeting.config import NOT_GIVEN_ADVICE_VALUE
 from Products.PloneMeeting.config import PMMessageFactory as _
 from Products.PloneMeeting.config import READER_USECASES
 from Products.PloneMeeting.content.advice import MeetingAdvice
 from Products.PloneMeeting.content.meeting import Meeting
 from Products.PloneMeeting.interfaces import IMeetingConfigCustom
 from Products.PloneMeeting.interfaces import IMeetingCustom
@@ -97,15 +98,16 @@
     'mark_not_applicable',
     'refused',
     'delayed',
     'pre_accepted',
     'return_to_proposing_group',
     'waiting_advices',
     'waiting_advices_proposing_group_send_back',
-    'waiting_advices_adviser_send_back')
+    'waiting_advices_adviser_send_back',
+    MEETING_REMOVE_MOG_WFA)
 # add our own wfAdaptations
 ownWfAdaptations = ('returned', 'accepted_and_returned', 'sent_to_council_emergency')
 customWfAdaptations = keptWfAdaptations + ownWfAdaptations
 MeetingConfig.wfAdaptations = customWfAdaptations
 
 LIEGE_WAITING_ADVICES_FROM_STATES = {
     'meeting-config-college':
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/imio.history.pot` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/PloneMeeting.pot` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/collective.eeafaceted.z3ctable.pot` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/collective.eeafaceted.z3ctable.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/datagridfield.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/datagridfield.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/eea.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/eea.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.history.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/plone.pot` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/imio.actionspanel.pot` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/datagridfield.pot` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/datagridfield.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/datagridfield.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/datagridfield.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/eea.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/eea.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/images/attach.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/import_steps.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/zbourgmestre/import_data.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/zbourgmestre/import_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     'reader_copy_groups',
     'reader_groupsincharge',
     'suffix_proposing_group_internalreviewers',
     'suffix_proposing_group_observers',
     'suffix_proposing_group_reviewers',
     'suffix_proposing_group_creators',
     'suffix_proposing_group_administrativereviewers')
-bourgmestreMeeting.usedItemAttributes = ['observations', ]
+bourgmestreMeeting.usedItemAttributes = ['observations', 'copyGroups']
 bourgmestreMeeting.usedMeetingAttributes = ['signatures', 'assembly', 'observations', ]
 bourgmestreMeeting.recordMeetingHistoryStates = []
 bourgmestreMeeting.xhtmlTransformFields = ()
 bourgmestreMeeting.xhtmlTransformTypes = ()
 bourgmestreMeeting.hideCssClassesTo = ('powerobservers', 'restrictedpowerobservers')
 bourgmestreMeeting.itemConditionsInterface = \
     'Products.MeetingLiege.interfaces.IMeetingItemBourgmestreWorkflowConditions'
@@ -270,15 +270,14 @@
     {'meeting_transition': 'close',
      'item_action': 'accept',
      'tal_expression': ''}, )
 bourgmestreMeeting.meetingPowerObserversStates = ('closed', 'created', )
 bourgmestreMeeting.powerAdvisersGroups = ()
 bourgmestreMeeting.itemBudgetInfosStates = ()
 bourgmestreMeeting.enableLabels = True
-bourgmestreMeeting.useCopies = True
 bourgmestreMeeting.hideItemHistoryCommentsToUsersOutsideProposingGroup = True
 bourgmestreMeeting.selectableCopyGroups = []
 bourgmestreMeeting.podTemplates = bourgmestreTemplates
 bourgmestreMeeting.meetingConfigsToCloneTo = []
 bourgmestreMeeting.recurringItems = []
 bourgmestreMeeting.itemTemplates = []
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/positive.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/attach.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/secretary_remarks.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/budget.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/financialAnalysis.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/decision.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/decision.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/remarks.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/SignatureCadranel.jpg` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/SignatureCadranel.jpg`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/negative.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/logo.gif` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/logo.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/courrierCollege.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/courrierCollege.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/images/cahier.gif` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/import_steps.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/testing/import_data.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/testing/import_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 collegeMeeting.isDefault = True
 collegeMeeting.shortName = 'College'
 collegeMeeting.usedItemAttributes = ['budgetInfos',
                                      'detailedDescription',
                                      'observations',
                                      'toDiscuss',
                                      'completeness',
-                                     'otherMeetingConfigsClonableToFieldLabelForCouncil',
                                      'otherMeetingConfigsClonableToPrivacy',
                                      'archivingRef',
                                      'motivation',
                                      'textCheckList',
                                      'itemIsSigned']
 collegeMeeting.itemConditionsInterface = ml_import_data.collegeMeeting.itemConditionsInterface
 collegeMeeting.itemActionsInterface = ml_import_data.collegeMeeting.itemActionsInterface
@@ -77,16 +76,16 @@
 councilMeeting.shortName = 'Council'
 councilMeeting.usedItemAttributes = ['budgetInfos',
                                      'category',
                                      'labelForCouncil',
                                      'observations',
                                      'privacy',
                                      'motivation',
-                                     'itemIsSigned']
-
+                                     'itemIsSigned',
+                                     'copyGroups']
 councilMeeting.itemConditionsInterface = ml_import_data.councilMeeting.itemConditionsInterface
 councilMeeting.itemActionsInterface = ml_import_data.councilMeeting.itemActionsInterface
 councilMeeting.meetingConditionsInterface = ml_import_data.councilMeeting.meetingConditionsInterface
 councilMeeting.meetingActionsInterface = ml_import_data.councilMeeting.meetingActionsInterface
 councilMeeting.transitionsForPresentingAnItem = ml_import_data.councilMeeting.transitionsForPresentingAnItem
 councilMeeting.itemWFValidationLevels = ml_import_data.councilMeeting.itemWFValidationLevels
 councilMeeting.workflowAdaptations = ml_import_data.councilMeeting.workflowAdaptations
@@ -154,26 +153,26 @@
 bourgmestreMeeting.maxDaysDecisions = 60
 bourgmestreMeeting.usedItemAttributes = [
     'category',
     'budgetInfos',
     'observations',
     'privacy',
     'motivation',
-    'itemIsSigned']
+    'itemIsSigned',
+    'copyGroups']
 bourgmestreMeeting.insertingMethodsOnAddItem = (
     {'insertingMethod': 'at_the_end',
      'reverse': '0'}, )
 bourgmestreMeeting.useAdvices = True
 bourgmestreMeeting.selectableAdvisers = []
 bourgmestreMeeting.itemAdviceStates = []
 bourgmestreMeeting.itemAdviceEditStates = []
 bourgmestreMeeting.itemAdviceViewStates = []
 bourgmestreMeeting.itemDecidedStates = [
     'accepted', 'refused', 'delayed', 'marked_not_applicable']
-bourgmestreMeeting.useCopies = True
 bourgmestreMeeting.useVotes = False
 bourgmestreMeeting.recurringItems = []
 bourgmestreMeeting.itemTemplates = []
 
 data = deepcopy(pm_import_data.data)
 data.meetingConfigs = (collegeMeeting, councilMeeting, bourgmestreMeeting)
 # necessary for testSetup.test_pm_ToolAttributesAreOnlySetOnFirstImportData
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcollegeliege_workflow/definition.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcollegeliege_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingcouncilliege_workflow/definition.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingcouncilliege_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcouncilliege_workflow/definition.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitemcouncilliege_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingitembourgmestre_workflow/definition.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingitembourgmestre_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingbourgmestre_workflow/definition.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingbourgmestre_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingcollegeliege_workflow/definition.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingcollegeliege_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows/meetingadviceliege_workflow/definition.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows/meetingadviceliege_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/skins.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/types/meetingadvicefinances.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/types/meetingadvicefinances.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/cssregistry.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/import_steps.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/default/workflows.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/positive.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/attach.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/medical.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/medical.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/secretary_remarks.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/budget.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/securite.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/securite.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/remarks.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/legalAdvice.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/negative.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/deliberation.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/deliberation.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/courrierCollege.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/courrierCollege.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/cahier.gif` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/images/juridique.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/images/juridique.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/synthese_avis_df.odt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/synthese_avis_df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/college-oj.odt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/college-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/projet-deliberation.odt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/projet-deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/deliberation.odt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/college-pv.odt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/college-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/templates/stats_DF_advice.ods` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/templates/stats_DF_advice.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/import_steps.xml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles/liege/import_data.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles/liege/import_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,16 @@
                                      'otherMeetingConfigsClonableToEmergency',
                                      'otherMeetingConfigsClonableToPrivacy',
                                      'archivingRef',
                                      'takenOverBy',
                                      'motivation',
                                      'decisionSuite',
                                      'decisionEnd',
-                                     'textCheckList', ]
+                                     'textCheckList',
+                                     'copyGroups']
 collegeMeeting.usedMeetingAttributes = ['signatures',
                                         'assembly',
                                         'assembly_excused',
                                         'observations', ]
 collegeMeeting.xhtmlTransformFields = ('MeetingItem.description', 'MeetingItem.detailedDescription',
                                        'MeetingItem.decision', 'MeetingItem.observations', )
 collegeMeeting.xhtmlTransformTypes = ('removeBlanks',)
@@ -514,15 +515,14 @@
                                        'pre_accepted', 'accepted', 'accepted_but_modified', )
 collegeMeeting.keepAccessToItemWhenAdvice = 'is_given'
 collegeMeeting.hideItemHistoryCommentsToUsersOutsideProposingGroup = True
 collegeMeeting.transitionReinitializingDelays = 'backToProposedToDirector'
 collegeMeeting.defaultAdviceHiddenDuringRedaction = ['meetingadvice', 'meetingadvicefinances']
 collegeMeeting.enforceAdviceMandatoriness = False
 collegeMeeting.enableAdviceInvalidation = False
-collegeMeeting.useCopies = True
 collegeMeeting.selectableCopyGroups = [orgs[0].getIdSuffixed('reviewers'),
                                        orgs[1].getIdSuffixed('reviewers'),
                                        orgs[2].getIdSuffixed('reviewers'),
                                        orgs[3].getIdSuffixed('reviewers'),
                                        orgs[4].getIdSuffixed('reviewers'),
                                        orgs[5].getIdSuffixed('reviewers'),
                                        orgs[6].getIdSuffixed('reviewers'), ]
@@ -671,15 +671,16 @@
                                      'category',
                                      'description',
                                      'detailedDescription',
                                      'observations',
                                      'privacy',
                                      'motivation',
                                      'decisionSuite',
-                                     'decisionEnd']
+                                     'decisionEnd',
+                                     'copyGroups']
 councilMeeting.usedMeetingAttributes = ['signatures',
                                         'assembly',
                                         'assembly_excused',
                                         'observations', ]
 councilMeeting.xhtmlTransformFields = ('MeetingItem.description', 'MeetingItem.detailedDescription',
                                        'MeetingItem.decision', 'MeetingItem.observations', )
 councilMeeting.xhtmlTransformTypes = ('removeBlanks',)
@@ -728,15 +729,14 @@
 councilMeeting.meetingTopicStates = ('created', 'frozen')
 councilMeeting.decisionTopicStates = ('decided', 'closed')
 councilMeeting.meetingAppDefaultView = 'searchmyitems'
 councilMeeting.useAdvices = False
 councilMeeting.enforceAdviceMandatoriness = False
 councilMeeting.enableAdviceInvalidation = False
 councilMeeting.hideItemHistoryCommentsToUsersOutsideProposingGroup = True
-councilMeeting.useCopies = True
 councilMeeting.selectableCopyGroups = [orgs[0].getIdSuffixed('reviewers'),
                                        orgs[1].getIdSuffixed('reviewers'),
                                        orgs[2].getIdSuffixed('reviewers'),
                                        orgs[3].getIdSuffixed('reviewers'),
                                        orgs[4].getIdSuffixed('reviewers'),
                                        orgs[5].getIdSuffixed('reviewers'),
                                        orgs[6].getIdSuffixed('reviewers'), ]
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/testing.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/interfaces.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/utils.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/utils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/MeetingLiege.zargo` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/MeetingLiege.zargo`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/generate.conf` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/generate.conf`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/model/pm_updates.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/model/pm_updates.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/config.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/config.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/events.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/testing.zcml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/Extensions/utils.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/Extensions/utils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/README.txt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testFaceted.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testAdvices.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeetingCategory.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testContacts.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomAdvices.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomContacts.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testChangeItemOrderView.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testUtils.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomMeeting.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/MeetingLiegeTestCase.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/MeetingLiegeTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testColumns.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testSetup.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testToolPloneMeeting.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomMeetingItem.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomMeetingItem.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     """
         Tests the MeetingItem adapted methods
     """
 
     def test_InitFieldsWhenItemSentToCouncil(self):
         '''When an item is sent from College to Council, fields 'title' and 'privacy'
            are initialized from what is defined on the College item.'''
+        self._enableField('otherMeetingConfigsClonableToFieldLabelForCouncil')
         # create a college item
         self.changeUser('pmManager')
         item = self.create('MeetingItem')
         item.setOtherMeetingConfigsClonableToFieldLabelForCouncil('<p>My label for council</p>')
         # before we used field 'privacyForCouncil' to init privacy on Council item
         # now use the field MeetingItem.otherMeetingConfigsClonableToPrivacy
         item.setOtherMeetingConfigsClonableToPrivacy((self.meetingConfig2.getId(), ))
@@ -49,14 +50,15 @@
         '''When an item is sent from College to Council, following fields are kept :
            - labelForCouncil;
            - financeAdvice;
            - decisionSuite;
            - decisionEnd;
            - toDiscuss.
         '''
+        self._enableField('otherMeetingConfigsClonableToFieldLabelForCouncil')
         # create a college item
         self.changeUser('pmManager')
         item = self.create('MeetingItem')
 
         # make item sendable to Council when 'itemcreated'
         cfg = self.meetingConfig
         usedItemAttrs = cfg.getUsedItemAttributes()
@@ -1316,16 +1318,15 @@
         self.assertEqual(item.listArchivingRefs().keys(), ['1'])
         item.setArchivingRef('2')
         self.assertEqual(item.listArchivingRefs().keys(), ['2'])
 
     def test_TreasuryCopyGroup(self):
         """TREASURY_GROUP_ID 'incopy' suffix is set in copy of items
            having finances advice when at least validated."""
-        cfg = self.meetingConfig
-        cfg.setUseCopies(True)
+        self._enableField('copyGroups')
         self.changeUser('admin')
         self._createFinanceGroups()
         self._createRHGroups()
         _configureCollegeCustomAdvisers(self.portal)
         self.changeUser('pmManager')
         item = self.create('MeetingItem')
         # bypass finances advice
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testWorkflows.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/helpers.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeetingItem.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testWFAdaptations.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testWFAdaptations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 #
 # File: testWFAdaptations.py
 #
 # GNU General Public License (GPL)
 #
 
 from Products.MeetingLiege.tests.MeetingLiegeTestCase import MeetingLiegeTestCase
+from Products.PloneMeeting.config import MEETING_REMOVE_MOG_WFA
 from Products.PloneMeeting.tests.testWFAdaptations import testWFAdaptations as pmtwfa
 
 
 class testWFAdaptations(MeetingLiegeTestCase, pmtwfa):
 
     def test_pm_WFA_availableWFAdaptations(self):
         '''Most of wfAdaptations make no sense, we just use 'return_to_proposing_group'.'''
         self.assertEquals(sorted(self.meetingConfig.listWorkflowAdaptations()),
                           ['accepted_and_returned',
                            'accepted_but_modified',
                            'delayed',
                            'item_validation_no_validate_shortcuts',
                            'item_validation_shortcuts',
                            'mark_not_applicable',
+                           MEETING_REMOVE_MOG_WFA,
                            'no_decide',
                            'no_freeze',
                            'no_publication',
                            'only_creator_may_delete',
                            'pre_accepted',
                            'refused',
                            'return_to_proposing_group',
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testValidators.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testPortlets.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testAnnexes.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomWorkflows.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomWorkflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1794,14 +1794,15 @@
         _check_access_council_item(councilItem)
         return collegeItem, councilItem, collegeMeeting, councilMeeting
 
     def test_CouncilItemSentToCollegeWhenDelayed(self):
         """While an item in the council is set to 'delayed', it is sent
            in 'itemcreated' state back to the College and ready to process
            back to the council."""
+        self._enableField('otherMeetingConfigsClonableToFieldLabelForCouncil')
         cfg = self.meetingConfig
         cfgId = cfg.getId()
         cfg2 = self.meetingConfig2
         cfg2Id = cfg2.getId()
         collegeItem, councilItem, collegeMeeting, councilMeeting = self._setupCollegeItemSentToCouncil()
         self.do(councilItem, 'delay')
 
@@ -1823,14 +1824,15 @@
         self.assertEqual(backCollegeItem.query_state(), 'itemcreated')
         self.assertEqual(backCollegeItem.adapted().getItemWithFinanceAdvice(), backCollegeItem)
 
     def test_CouncilItemSentToCollegeWhenReturned(self):
         """While an item in the council is set to 'delayed', it is sent
            in 'validated' state back to the College and ready to process
            back to the council."""
+        self._enableField('otherMeetingConfigsClonableToFieldLabelForCouncil')
         cfg = self.meetingConfig
         cfgId = cfg.getId()
         cfg2 = self.meetingConfig2
         cfg2Id = cfg2.getId()
         collegeItem, councilItem, collegeMeeting, councilMeeting = self._setupCollegeItemSentToCouncil()
         # change proposingGroup to 'vendors' so we test that item is correctly validated
         # even if it is not accessible during the process when in it 'itemcreated'
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/__init__.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeeting.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testSearches.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testViews.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testMeetingConfig.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/tests/testCustomViews.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/tests/testCustomViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/overrides.zcml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/__init__.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/overrides.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/overrides.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from imio.helpers.cache import get_plone_groups_for_user
 from imio.history.interfaces import IImioHistory
 from imio.history.utils import getLastWFAction
 from plone import api
 from plone.memoize.view import memoize_contextless
 from Products.MeetingLiege import logger
 from Products.PloneMeeting.browser.advicechangedelay import AdviceDelaysView
-from Products.PloneMeeting.browser.overrides import BaseActionsPanelView
+from Products.PloneMeeting.browser.overrides import AdviceActionsPanelView
 from Products.PloneMeeting.browser.overrides import PMContentHistoryView
 from Products.PloneMeeting.browser.views import FolderDocumentGenerationHelperView
 from Products.PloneMeeting.browser.views import ItemDocumentGenerationHelperView
 from Products.PloneMeeting.utils import get_event_field_data
 from zope.component import getAdapter
 
 import time
 
 
-class MLAdviceActionsPanelView(BaseActionsPanelView):
+class MLAdviceActionsPanelView(AdviceActionsPanelView):
     """
       Specific actions displayed on a meetingadvice.
     """
     def __init__(self, context, request):
         super(MLAdviceActionsPanelView, self).__init__(context, request)
 
     @memoize_contextless
```

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/configure.zcml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/templates/item_main_infos.pt` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/templates/item_main_infos.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/browser/overrides/images/more_infos.png` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/browser/overrides/images/more_infos.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/profiles.zcml` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/migrations/migrate_to_4200.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/src/Products/MeetingLiege/migrations/migrate_to_4_1.py` & `Products.MeetingLiege-4.2.9/src/Products/MeetingLiege/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/docs/LICENSE.txt` & `Products.MeetingLiege-4.2.9/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/docs/LICENSE.GPL` & `Products.MeetingLiege-4.2.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/setup.py` & `Products.MeetingLiege-4.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-version = '4.2.8'
+version = '4.2.9'
 
 setup(
     name='Products.MeetingLiege',
     version=version,
     description="PloneMeeting profile for city of Liege",
     long_description=open("README.rst").read() + "\n" +
     open("CHANGES.rst").read(),
```

### Comparing `Products.MeetingLiege-4.2.8/PKG-INFO` & `Products.MeetingLiege-4.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: Products.MeetingLiege
-Version: 4.2.8
+Version: 4.2.9
 Summary: PloneMeeting profile for city of Liege
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL
 Description: Profile for Products.PloneMeeting for Ville de Liège
         ====================================================
         
         
         Products.MeetingLiege Changelog
         ===============================
         
+        4.2.9 (2023-10-05)
+        ------------------
+        
+        - Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+          [gbastien]
+        - Fixed `MLAdviceActionsPanelView` that inherits from `AdviceActionsPanelView` and
+          not `BaseActionsPanelView` so we get the `renderOwnDeleteWithComments`.
+          [gbastien]
+        - Adapted code as `MeetingConfig.useCopies` field was removed.
+          [gbastien]
+        
         4.2.8 (2023-03-20)
         ------------------
         
         - Fixed cachekey for `CustomMeetingItem._roles_in_context`.
           [gbastien]
         - Fixed `meetingitem_view.pt` to use `structure` to display groups in charge.
           [gbastien]
```

### Comparing `Products.MeetingLiege-4.2.8/MANIFEST.in` & `Products.MeetingLiege-4.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.MeetingLiege-4.2.8/CHANGES.rst` & `Products.MeetingLiege-4.2.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Products.MeetingLiege Changelog
 ===============================
 
+4.2.9 (2023-10-05)
+------------------
+
+- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
+  [gbastien]
+- Fixed `MLAdviceActionsPanelView` that inherits from `AdviceActionsPanelView` and
+  not `BaseActionsPanelView` so we get the `renderOwnDeleteWithComments`.
+  [gbastien]
+- Adapted code as `MeetingConfig.useCopies` field was removed.
+  [gbastien]
+
 4.2.8 (2023-03-20)
 ------------------
 
 - Fixed cachekey for `CustomMeetingItem._roles_in_context`.
   [gbastien]
 - Fixed `meetingitem_view.pt` to use `structure` to display groups in charge.
   [gbastien]
```

