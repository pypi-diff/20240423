# Comparing `tmp/aleksis_core-4.0.0.dev6.tar.gz` & `tmp/aleksis_core-4.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_core-4.0.0.dev6.tar", max compression
+gzip compressed data, was "aleksis_core-4.0.0.dev7.tar", max compression
```

## Comparing `aleksis_core-4.0.0.dev6.tar` & `aleksis_core-4.0.0.dev7.tar`

### file list

```diff
@@ -1,577 +1,579 @@
--rw-r--r--   0        0        0    42442 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/CHANGELOG.rst
--rw-r--r--   0        0        0    14353 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/LICENCE.rst
--rw-r--r--   0        0        0     3786 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/README.rst
--rw-r--r--   0        0        0      194 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/__init__.py
--rw-r--r--   0        0        0      464 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/__main__.py
--rw-r--r--   0        0        0      510 2024-04-04 06:54:53.759696 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2024-04-04 06:54:54.547687 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     2168 2024-04-04 06:54:56.667662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0    11656 2024-04-04 06:54:55.499676 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2533 2024-04-04 06:54:53.791696 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0        0        0     3716 2024-04-04 06:54:56.743662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/checks.cpython-311.pyc
--rw-r--r--   0        0        0    23254 2024-04-04 06:54:56.411666 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2024-04-04 06:54:56.747662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/health_checks.cpython-311.pyc
--rw-r--r--   0        0        0    10749 2024-04-04 06:54:56.447665 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0    40416 2024-04-04 06:54:56.431665 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0   103971 2024-04-04 06:54:56.071669 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    25279 2024-04-04 06:54:56.919660 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1144 2024-04-04 06:54:55.515676 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/registries.cpython-311.pyc
--rw-r--r--   0        0        0    18563 2024-04-04 06:54:56.687662 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0    44148 2024-04-04 06:54:54.563687 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     3825 2024-04-04 06:54:56.455665 aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0     1002 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/admin.py
--rw-r--r--   0        0        0     8751 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/apps.py
--rw-r--r--   0        0        0     1338 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/celery.py
--rw-r--r--   0        0        0     2759 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/checks.py
--rw-r--r--   0        0        0    14836 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/data_checks.py
--rw-r--r--   0        0        0      741 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/decorators.py
--rw-r--r--   0        0        0     5506 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/filters.py
--rw-r--r--   0        0        0    30667 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/forms.py
--rw-r--r--   0        0        0     3178 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/apollo.js
--rw-r--r--   0        0        0     1757 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/dateTimeFormats.js
--rw-r--r--   0        0        0      197 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/i18n.js
--rw-r--r--   0        0        0      157 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/router.js
--rw-r--r--   0        0        0      133 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/sentry.js
--rw-r--r--   0        0        0     1091 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/vuetify.js
--rw-r--r--   0        0        0     4682 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/LegacyBaseTemplate.vue
--rw-r--r--   0        0        0      158 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/Parent.vue
--rw-r--r--   0        0        0      335 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/About.vue
--rw-r--r--   0        0        0     1971 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/AboutAleksis.vue
--rw-r--r--   0        0        0     3831 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppCard.vue
--rw-r--r--   0        0        0     1003 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppsList.vue
--rw-r--r--   0        0        0      351 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/installedApps.graphql
--rw-r--r--   0        0        0     2412 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/AccountMenu.vue
--rw-r--r--   0        0        0    10484 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/App.vue
--rw-r--r--   0        0        0      314 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/BrandLogo.vue
--rw-r--r--   0        0        0     1064 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/ErrorPage.vue
--rw-r--r--   0        0        0     1471 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/LanguageForm.vue
--rw-r--r--   0        0        0     4635 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SideNav.vue
--rw-r--r--   0        0        0     1454 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SidenavSearch.vue
--rw-r--r--   0        0        0      748 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SnackbarItem.vue
--rw-r--r--   0        0        0     1932 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/Splash.vue
--rw-r--r--   0        0        0      124 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/customMenu.graphql
--rw-r--r--   0        0        0      205 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/dynamicRoutes.graphql
--rw-r--r--   0        0        0       42 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/messages.graphql
--rw-r--r--   0        0        0       59 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/ping.graphql
--rw-r--r--   0        0        0      139 2024-04-04 06:54:07.908226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/searchSnippets.graphql
--rw-r--r--   0        0        0      412 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/systemProperties.graphql
--rw-r--r--   0        0        0      329 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/whoAmI.graphql
--rw-r--r--   0        0        0     2568 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
--rw-r--r--   0        0        0     1894 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
--rw-r--r--   0        0        0      220 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
--rw-r--r--   0        0        0       84 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
--rw-r--r--   0        0        0     3564 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue
--rw-r--r--   0        0        0     1190 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue
--rw-r--r--   0        0        0    13721 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/Calendar.vue
--rw-r--r--   0        0        0      624 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarControlBar.vue
--rw-r--r--   0        0        0      309 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarDownloadAllButton.vue
--rw-r--r--   0        0        0     5903 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarOverview.vue
--rw-r--r--   0        0        0     2072 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarSelect.vue
--rw-r--r--   0        0        0      364 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarStatusChip.vue
--rw-r--r--   0        0        0     1521 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue
--rw-r--r--   0        0        0     1560 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarWithControls.vue
--rw-r--r--   0        0        0      318 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CancelledCalendarStatusChip.vue
--rw-r--r--   0        0        0      405 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/GenericCalendarFeedDetails.vue
--rw-r--r--   0        0        0      386 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/GenericCalendarFeedEventBar.vue
--rw-r--r--   0        0        0      426 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendar.graphql
--rw-r--r--   0        0        0      154 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarFeeds.graphql
--rw-r--r--   0        0        0      561 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarMixin.js
--rw-r--r--   0        0        0     1096 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js
--rw-r--r--   0        0        0     9850 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue
--rw-r--r--   0        0        0     1021 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql
--rw-r--r--   0        0        0       93 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/setCalendarStatus.graphql
--rw-r--r--   0        0        0      715 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue
--rw-r--r--   0        0        0     5242 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue
--rw-r--r--   0        0        0      434 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/event_bar/BirthdaysEventBar.vue
--rw-r--r--   0        0        0     3611 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
--rw-r--r--   0        0        0     2806 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
--rw-r--r--   0        0        0      925 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
--rw-r--r--   0        0        0      432 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
--rw-r--r--   0        0        0      191 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
--rw-r--r--   0        0        0      118 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
--rw-r--r--   0        0        0     3009 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ActionSelect.vue
--rw-r--r--   0        0        0      655 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/AvatarClickbox.vue
--rw-r--r--   0        0        0      212 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/BackButton.vue
--rw-r--r--   0        0        0      823 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ButtonMenu.vue
--rw-r--r--   0        0        0    13494 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDBar.vue
--rw-r--r--   0        0        0     3819 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDIterator.vue
--rw-r--r--   0        0        0     6938 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDList.vue
--rw-r--r--   0        0        0     1559 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue
--rw-r--r--   0        0        0      981 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/DetailView.vue
--rw-r--r--   0        0        0     1483 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/FilterBar.vue
--rw-r--r--   0        0        0     5173 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/InlineCRUDList.vue
--rw-r--r--   0        0        0      435 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ListView.vue
--rw-r--r--   0        0        0      268 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/MessageBox.vue
--rw-r--r--   0        0        0     1914 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ObjectOverview.vue
--rw-r--r--   0        0        0      269 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/SmallContainer.vue
--rw-r--r--   0        0        0      292 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/TableLink.vue
--rw-r--r--   0        0        0     2017 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/UpdateIndicator.vue
--rw-r--r--   0        0        0      716 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/BaseButton.vue
--rw-r--r--   0        0        0      456 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/CancelButton.vue
--rw-r--r--   0        0        0     1229 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue
--rw-r--r--   0        0        0      361 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/CreateButton.vue
--rw-r--r--   0        0        0      370 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/DeleteButton.vue
--rw-r--r--   0        0        0      357 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/EditButton.vue
--rw-r--r--   0        0        0     1139 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/FilterButton.vue
--rw-r--r--   0        0        0      335 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/PrimaryActionButton.vue
--rw-r--r--   0        0        0      357 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/SaveButton.vue
--rw-r--r--   0        0        0      427 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/SecondaryActionButton.vue
--rw-r--r--   0        0        0      440 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/ClosableSnackbar.vue
--rw-r--r--   0        0        0     1273 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue
--rw-r--r--   0        0        0     3269 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
--rw-r--r--   0        0        0     5971 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue
--rw-r--r--   0        0        0     2244 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue
--rw-r--r--   0        0        0     1038 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue
--rw-r--r--   0        0        0     1360 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ColorField.vue
--rw-r--r--   0        0        0     2622 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateField.vue
--rw-r--r--   0        0        0     2401 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateTimeField.vue
--rw-r--r--   0        0        0     3229 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue
--rw-r--r--   0        0        0     1006 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue
--rw-r--r--   0        0        0     4834 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue
--rw-r--r--   0        0        0      695 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/SexSelect.vue
--rw-r--r--   0        0        0     2390 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/TimeField.vue
--rw-r--r--   0        0        0     1267 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/WeekDayField.vue
--rw-r--r--   0        0        0      355 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group/GroupChip.vue
--rw-r--r--   0        0        0      706 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group/GroupCollection.vue
--rw-r--r--   0        0        0     2125 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group_type/GroupType.vue
--rw-r--r--   0        0        0      696 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group_type/groupType.graphql
--rw-r--r--   0        0        0     2697 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/HolidayInlineList.vue
--rw-r--r--   0        0        0      742 2024-04-04 06:54:07.912226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/holiday.graphql
--rw-r--r--   0        0        0     2966 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationItem.vue
--rw-r--r--   0        0        0     2616 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationList.vue
--rw-r--r--   0        0        0      107 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
--rw-r--r--   0        0        0      207 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/myNotifications.graphql
--rw-r--r--   0        0        0     1017 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/pdf/DownloadPDF.vue
--rw-r--r--   0        0        0       78 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/pdf/pdf.graphql
--rw-r--r--   0        0        0     1410 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AdditionalImage.vue
--rw-r--r--   0        0        0     1252 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AvatarContent.vue
--rw-r--r--   0        0        0     3389 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonActions.vue
--rw-r--r--   0        0        0      527 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
--rw-r--r--   0        0        0      862 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonChip.vue
--rw-r--r--   0        0        0      759 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonCollection.vue
--rw-r--r--   0        0        0     2482 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonList.vue
--rw-r--r--   0        0        0     8273 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonOverview.vue
--rw-r--r--   0        0        0      108 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/avatarContent.graphql
--rw-r--r--   0        0        0      301 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personActions.graphql
--rw-r--r--   0        0        0      345 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personList.graphql
--rw-r--r--   0        0        0      589 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personOverview.graphql
--rw-r--r--   0        0        0     1488 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/RoomInlineList.vue
--rw-r--r--   0        0        0      630 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/room.graphql
--rw-r--r--   0        0        0     2516 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermField.vue
--rw-r--r--   0        0        0     2952 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue
--rw-r--r--   0        0        0      742 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/schoolTerm.graphql
--rw-r--r--   0        0        0     3859 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactor.vue
--rw-r--r--   0        0        0     1490 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
--rw-r--r--   0        0        0      589 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
--rw-r--r--   0        0        0      385 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/twoFactor.graphql
--rw-r--r--   0        0        0      422 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/css/global.scss
--rw-r--r--   0        0        0     2841 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/index.js
--rw-r--r--   0        0        0    15106 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/de.json
--rw-r--r--   0        0        0    13925 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/en.json
--rw-r--r--   0        0        0    18225 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/ru.json
--rw-r--r--   0        0        0    17582 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/uk.json
--rw-r--r--   0        0        0     3052 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/aleksis.js
--rw-r--r--   0        0        0     1060 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/calendarFeedDetails.js
--rw-r--r--   0        0        0      386 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/calendarFeedEventBar.js
--rw-r--r--   0        0        0     2695 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/createOrPatchMixin.js
--rw-r--r--   0        0        0     1540 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/deleteMixin.js
--rw-r--r--   0        0        0      538 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/error404.js
--rw-r--r--   0        0        0     2419 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/formRulesMixin.js
--rw-r--r--   0        0        0      490 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/loadingMixin.js
--rw-r--r--   0        0        0     3450 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/menus.js
--rw-r--r--   0        0        0     3296 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/mutateMixin.js
--rw-r--r--   0        0        0     2256 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/offline.js
--rw-r--r--   0        0        0      762 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/permissions.js
--rw-r--r--   0        0        0     3060 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/queryMixin.js
--rw-r--r--   0        0        0     2154 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/routes.js
--rw-r--r--   0        0        0      524 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/sexChoiceMixin.js
--rw-r--r--   0        0        0      766 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/syncSortMixin.js
--rw-r--r--   0        0        0     1684 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/useRegisterSW.js
--rw-r--r--   0        0        0     7148 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/plugins/aleksis.js
--rw-r--r--   0        0        0      450 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/routeValidators.js
--rw-r--r--   0        0        0    34409 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/frontend/routes.js
--rw-r--r--   0        0        0     2642 2024-04-04 06:54:07.916226 aleksis_core-4.0.0.dev6/aleksis/core/health_checks.py
--rw-r--r--   0        0        0      487 2024-04-04 06:54:57.175657 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74550 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      894 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    64425 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   127576 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2024-04-04 06:54:57.167657 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1118 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      942 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    78337 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2024-04-04 06:54:57.171657 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      810 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2510 2024-04-04 06:54:57.187656 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    84014 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 06:54:57.191656 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2024-04-04 06:54:57.099658 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74480 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 06:54:57.103658 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    79209 2024-04-04 06:54:57.191656 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   137668 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2024-04-04 06:54:57.179657 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1321 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2024-04-04 06:54:57.099658 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74420 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 06:54:57.095658 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    78198 2024-04-04 06:54:57.175657 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   135337 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2024-04-04 06:54:57.167657 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2024-04-04 06:54:07.920226 aleksis_core-4.0.0.dev6/aleksis/core/management/__init__.py
--rw-r--r--   0        0        0     3957 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/management/commands/convert_urls_to_routes.py
--rw-r--r--   0        0        0     1082 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/management/commands/vite.py
--rw-r--r--   0        0        0      439 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/management/commands/webpack_bundle.py
--rw-r--r--   0        0        0     5688 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/managers.py
--rw-r--r--   0        0        0    49187 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0001_initial.py
--rw-r--r--   0        0        0     2198 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0002_school_term.py
--rw-r--r--   0        0        0      531 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0003_drop_image_cropping.py
--rw-r--r--   0        0        0      796 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
--rw-r--r--   0        0        0     1252 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0005_timestamped_activity_notification.py
--rw-r--r--   0        0        0     1567 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0006_dashboard_widget_size.py
--rw-r--r--   0        0        0     1207 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0007_dashboard_widget_order.py
--rw-r--r--   0        0        0     1936 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0008_data_check_result.py
--rw-r--r--   0        0        0     1052 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0009_default_dashboard.py
--rw-r--r--   0        0        0      952 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0010_external_link_widget.py
--rw-r--r--   0        0        0      829 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0011_globalpermissions_options.py
--rw-r--r--   0        0        0      501 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0012_valid_from_announcement.py
--rw-r--r--   0        0        0     2073 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0013_pdf_file.py
--rw-r--r--   0        0        0      533 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0014_alter_pdffile_file.py
--rw-r--r--   0        0        0     1174 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0015_oauth_permissions.py
--rw-r--r--   0        0        0     1341 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0016_taskuserassignment.py
--rw-r--r--   0        0        0      426 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0017_dashboardwidget_broken.py
--rw-r--r--   0        0        0      897 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0018_pdffile_html_file.py
--rw-r--r--   0        0        0     2116 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      542 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0020_pdf_file_person_optional.py
--rw-r--r--   0        0        0     1084 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
--rw-r--r--   0        0        0      923 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0022_public_favicon.py
--rw-r--r--   0        0        0     6340 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0023_oauth_application_model.py
--rw-r--r--   0        0        0      714 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0024_oauth_grant_types_optional.py
--rw-r--r--   0        0        0     1717 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0025_oauth_align_user_fk.py
--rw-r--r--   0        0        0      582 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
--rw-r--r--   0        0        0      457 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0027_person_place_of_birth.py
--rw-r--r--   0        0        0      947 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0028_char_field_not_null.py
--rw-r--r--   0        0        0     1465 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0029_invitations.py
--rw-r--r--   0        0        0     1776 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0030_user_attributes.py
--rw-r--r--   0        0        0      526 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0031_oauthapplication_icon.py
--rw-r--r--   0        0        0      340 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0032_remove_person_is_active.py
--rw-r--r--   0        0        0     2416 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0033_update_photo_avatar.py
--rw-r--r--   0        0        0      816 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0034_invite_permission.py
--rw-r--r--   0        0        0     1805 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0035_preference_model_unique.py
--rw-r--r--   0        0        0      626 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0036_additionalfields_helptext_required.py
--rw-r--r--   0        0        0      917 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0037_add_static_content_widget.py
--rw-r--r--   0        0        0      522 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0038_notification_send_at.py
--rw-r--r--   0        0        0     1029 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0039_personal_ical_url.py
--rw-r--r--   0        0        0      613 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
--rw-r--r--   0        0        0      516 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0041_update_gender_choices.py
--rw-r--r--   0        0        0      547 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0042_pdffile_empty.py
--rw-r--r--   0        0        0     2261 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0043_task_assignment_meta.py
--rw-r--r--   0        0        0      532 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0044_task_assignment_result_fetched.py
--rw-r--r--   0        0        0      486 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
--rw-r--r--   0        0        0   290966 2024-04-04 06:54:07.924226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0046_notification_create_field_icon.py
--rw-r--r--   0        0        0     2510 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0047_add_room_model.py
--rw-r--r--   0        0        0   893996 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0048_delete_personalicalurl.py
--rw-r--r--   0        0        0      533 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
--rw-r--r--   0        0        0     6221 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0050_managed_by_app_label.py
--rw-r--r--   0        0        0     5606 2024-04-04 06:54:07.928226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0051_calendarevent_and_holiday.py
--rw-r--r--   0        0        0   909270 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0052_site_related_name.py
--rw-r--r--   0        0        0      914 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0053_freebusy.py
--rw-r--r--   0        0        0     1994 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0054_create_organisation_model.py
--rw-r--r--   0        0        0     1738 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0055_customevent.py
--rw-r--r--   0        0        0      332 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0056_rename_customevent_personalevent.py
--rw-r--r--   0        0        0      505 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0057_drop_otp_yubikey.py
--rw-r--r--   0        0        0      720 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0058_migrate_preferences_to_global.py
--rw-r--r--   0        0        0     5514 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0059_drop_site.py
--rw-r--r--   0        0        0     1165 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0060_person_unique_short_name_email.py
--rw-r--r--   0        0        0      500 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/0061_remove_group_additional_fields.py
--rw-r--r--   0        0        0        0 2024-04-04 06:54:07.932226 aleksis_core-4.0.0.dev6/aleksis/core/migrations/__init__.py
--rw-r--r--   0        0        0    25176 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/mixins.py
--rw-r--r--   0        0        0    64469 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/models.py
--rw-r--r--   0        0        0    15497 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/preferences.py
--rw-r--r--   0        0        0      611 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/registries.py
--rw-r--r--   0        0        0    17713 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/rules.py
--rw-r--r--   0        0        0    11074 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/__init__.py
--rw-r--r--   0        0        0     7649 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/base.py
--rw-r--r--   0        0        0     4023 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/calendar.py
--rw-r--r--   0        0        0     3049 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/celery_progress.py
--rw-r--r--   0        0        0      585 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/custom_menu.py
--rw-r--r--   0        0        0      459 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/dynamic_routes.py
--rw-r--r--   0        0        0     2005 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/group.py
--rw-r--r--   0        0        0     1309 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/group_type.py
--rw-r--r--   0        0        0     1430 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/holiday.py
--rw-r--r--   0        0        0     1743 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/installed_apps.py
--rw-r--r--   0        0        0      265 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/message.py
--rw-r--r--   0        0        0     1296 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/notification.py
--rw-r--r--   0        0        0     1145 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/oauth.py
--rw-r--r--   0        0        0      554 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/pdf.py
--rw-r--r--   0        0        0      124 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/permissions.py
--rw-r--r--   0        0        0    10060 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/person.py
--rw-r--r--   0        0        0     3382 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/personal_event.py
--rw-r--r--   0        0        0     1270 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/room.py
--rw-r--r--   0        0        0     2147 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/school_term.py
--rw-r--r--   0        0        0      868 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/search.py
--rw-r--r--   0        0        0     1343 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/site_preferences.py
--rw-r--r--   0        0        0     1697 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/system_properties.py
--rw-r--r--   0        0        0     3297 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/two_factor.py
--rw-r--r--   0        0        0      829 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/schema/user.py
--rw-r--r--   0        0        0      418 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/search_indexes.py
--rw-r--r--   0        0        0    39858 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/settings.py
--rw-r--r--   0        0        0    49621 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-banner.svg
--rw-r--r--   0        0        0     1862 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-favicon.png
--rw-r--r--   0        0        0    17172 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.png
--rw-r--r--   0        0        0     7843 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.svg
--rw-r--r--   0        0        0    31902 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.png
--rw-r--r--   0        0        0     7346 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.svg
--rw-r--r--   0        0        0    19126 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/fallback.png
--rw-r--r--   0        0        0     2237 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/img/hero.svg
--rw-r--r--   0        0        0      490 2024-04-04 06:54:07.936226 aleksis_core-4.0.0.dev6/aleksis/core/static/js/copy_button.js
--rw-r--r--   0        0        0      521 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/edit_dashboard.js
--rw-r--r--   0        0        0      618 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/helper.js
--rw-r--r--   0        0        0      984 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/include_ajax_live.js
--rw-r--r--   0        0        0     4351 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/main.js
--rw-r--r--   0        0        0     1654 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/multi_select.js
--rw-r--r--   0        0        0     3495 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/search.js
--rw-r--r--   0        0        0     2581 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/js/serviceworker.js
--rw-r--r--   0        0        0      271 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/print-simple.css
--rw-r--r--   0        0        0     1627 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/print.css
--rw-r--r--   0        0        0      187 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/print_landscape.css
--rw-r--r--   0        0        0     1064 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/public/materialize-custom.scss
--rw-r--r--   0        0        0    15749 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/public/style.scss
--rw-r--r--   0        0        0    11345 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/static/public/theme.scss
--rw-r--r--   0        0        0     5408 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/tables.py
--rw-r--r--   0        0        0     2330 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/tasks.py
--rw-r--r--   0        0        0      838 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/403.html
--rw-r--r--   0        0        0      789 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/404.html
--rw-r--r--   0        0        0      918 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/500.html
--rw-r--r--   0        0        0       76 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/503.html
--rw-r--r--   0        0        0      851 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/account_inactive.html
--rw-r--r--   0        0        0      169 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email/base_message.txt
--rw-r--r--   0        0        0      525 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0        0        0     1255 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email_confirm.html
--rw-r--r--   0        0        0     1182 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_change.html
--rw-r--r--   0        0        0     1377 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset.html
--rw-r--r--   0        0        0      825 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     2305 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      649 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      500 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_set.html
--rw-r--r--   0        0        0      888 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup.html
--rw-r--r--   0        0        0      838 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup_closed.html
--rw-r--r--   0        0        0      820 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_email_required.html
--rw-r--r--   0        0        0     1160 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_sent.html
--rw-r--r--   0        0        0      979 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/chips.html
--rw-r--r--   0        0        0      350 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/materialize-chips.html
--rw-r--r--   0        0        0      225 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/msgbox.html
--rw-r--r--   0        0        0      958 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/pagination.html
--rw-r--r--   0        0        0      486 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/components/text_collapsible.html
--rw-r--r--   0        0        0     1053 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/form.html
--rw-r--r--   0        0        0     1900 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/list.html
--rw-r--r--   0        0        0     3099 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base.html
--rw-r--r--   0        0        0     2454 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_print.html
--rw-r--r--   0        0        0     1212 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_simple_print.html
--rw-r--r--   0        0        0      628 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/create.html
--rw-r--r--   0        0        0      635 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
--rw-r--r--   0        0        0      626 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/edit.html
--rw-r--r--   0        0        0      262 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
--rw-r--r--   0        0        0     1349 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/list.html
--rw-r--r--   0        0        0      226 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
--rw-r--r--   0        0        0     3879 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/data_check/list.html
--rw-r--r--   0        0        0     2233 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/edit_dashboard.html
--rw-r--r--   0        0        0        0 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/empty.html
--rw-r--r--   0        0        0     5310 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/child_groups.html
--rw-r--r--   0        0        0      650 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/edit.html
--rw-r--r--   0        0        0     3382 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/full.html
--rw-r--r--   0        0        0     1019 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/list.html
--rw-r--r--   0        0        0     2504 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/index.html
--rw-r--r--   0        0        0      777 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/delete.html
--rw-r--r--   0        0        0     6832 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/system_status.html
--rw-r--r--   0        0        0      603 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/test_pdf.html
--rw-r--r--   0        0        0       93 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/address.html
--rw-r--r--   0        0        0      189 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/admins_list.html
--rw-r--r--   0        0        0     1632 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/announcements.html
--rw-r--r--   0        0        0     1472 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/avatar_content.html
--rw-r--r--   0        0        0      319 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/copy_button.html
--rw-r--r--   0        0        0     1089 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/crud_events.html
--rw-r--r--   0        0        0      389 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/edit_dashboard_widget.html
--rw-r--r--   0        0        0     1624 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/meta.html
--rw-r--r--   0        0        0      414 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/on_page_menu.html
--rw-r--r--   0        0        0      260 2024-04-04 06:54:07.940225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/save_button.html
--rw-r--r--   0        0        0     2358 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/splash_screen.html
--rw-r--r--   0        0        0      325 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/turnable.html
--rw-r--r--   0        0        0      915 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/assign.html
--rw-r--r--   0        0        0     2478 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/list.html
--rw-r--r--   0        0        0      376 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/collection.html
--rw-r--r--   0        0        0      649 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/create.html
--rw-r--r--   0        0        0      645 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/edit.html
--rw-r--r--   0        0        0     1165 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/list.html
--rw-r--r--   0        0        0      927 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/core/vue_index.html
--rw-r--r--   0        0        0     3921 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/django_tables2/materialize.html
--rw-r--r--   0        0        0      981 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/dynamic_preferences/form.html
--rw-r--r--   0        0        0      376 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/dynamic_preferences/sections.html
--rw-r--r--   0        0        0      764 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/disabled.html
--rw-r--r--   0        0        0     1281 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/enter.html
--rw-r--r--   0        0        0     1162 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/forms/_invite.html
--rw-r--r--   0        0        0      102 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/messages/invite_accepted.txt
--rw-r--r--   0        0        0      171 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/field_errors.html
--rw-r--r--   0        0        0     1232 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
--rw-r--r--   0        0        0     1897 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/colorfield_colorwidget.html
--rw-r--r--   0        0        0     1009 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
--rw-r--r--   0        0        0     1009 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_select2widget.html
--rw-r--r--   0        0        0      253 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/material/non_field_errors.html
--rw-r--r--   0        0        0      663 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/create.html
--rw-r--r--   0        0        0     2335 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/detail.html
--rw-r--r--   0        0        0      669 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/edit.html
--rw-r--r--   0        0        0     1074 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/list.html
--rw-r--r--   0        0        0     2686 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/authorize.html
--rw-r--r--   0        0        0      887 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/offline.html
--rw-r--r--   0        0        0       42 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/indexes/core/group_text.txt
--rw-r--r--   0        0        0       69 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/indexes/core/person_text.txt
--rw-r--r--   0        0        0       42 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/indexes/core/room_text.txt
--rw-r--r--   0        0        0     3171 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/search.html
--rw-r--r--   0        0        0      243 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/searchbar_snippet.html
--rw-r--r--   0        0        0      150 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/search/searchbar_snippets.html
--rw-r--r--   0        0        0      169 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/sms/notification.txt
--rw-r--r--   0        0        0      893 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1268 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1289 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login.html
--rw-r--r--   0        0        0      809 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0     1012 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/signup.html
--rw-r--r--   0        0        0     1660 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      630 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/base.email
--rw-r--r--   0        0        0     1527 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/celery_failure.email
--rw-r--r--   0        0        0      994 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/data_checks.email
--rw-r--r--   0        0        0     1014 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/email.css
--rw-r--r--   0        0        0     1102 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/invitation.email
--rw-r--r--   0        0        0     1461 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/notification.email
--rw-r--r--   0        0        0      668 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/person_changed.email
--rw-r--r--   0        0        0      219 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      877 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0      119 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1780 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     6686 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      943 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0      986 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/phone_register.html
--rw-r--r--   0        0        0     3050 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0     2127 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      786 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0        0 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/__init__.py
--rw-r--r--   0        0        0       99 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/apps.py
--rw-r--r--   0        0        0      394 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/dashboard.py
--rw-r--r--   0        0        0     1611 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/data_helpers.py
--rw-r--r--   0        0        0     1543 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/html_helpers.py
--rw-r--r--   0        0        0      206 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/templatetags/msg_box.py
--rw-r--r--   0        0        0     3696 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/browser/test_selenium.py
--rw-r--r--   0        0        0      761 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/managers/test_aleksisbasemanager.py
--rw-r--r--   0        0        0     1607 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/mixins/test_registry_object.py
--rw-r--r--   0        0        0     6596 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test.pdf
--rw-r--r--   0        0        0     1520 2024-04-04 06:54:07.944225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_group_sync.py
--rw-r--r--   0        0        0     3049 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_notification.py
--rw-r--r--   0        0        0     4003 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_pdffile.py
--rw-r--r--   0        0        0      427 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_person.py
--rw-r--r--   0        0        0     5503 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/test_regression.py
--rw-r--r--   0        0        0      683 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/view_oauth.py
--rw-r--r--   0        0        0     1021 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/templatetags/test_data_helpers.py
--rw-r--r--   0        0        0     2292 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/tests/views/test_account.py
--rw-r--r--   0        0        0    17541 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/urls.py
--rw-r--r--   0        0        0        0 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/__init__.py
--rw-r--r--   0        0        0      176 2024-04-04 06:54:54.083692 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14949 2024-04-04 06:54:55.515676 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    10101 2024-04-04 06:54:56.451665 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
--rw-r--r--   0        0        0    29144 2024-04-04 06:54:54.083692 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2024-04-04 06:54:54.495688 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0      771 2024-04-04 06:54:56.463665 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     5811 2024-04-04 06:54:56.455665 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     9909 2024-04-04 06:54:56.691662 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0     2181 2024-04-04 06:54:55.535676 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
--rw-r--r--   0        0        0      657 2024-04-04 06:54:55.535676 aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
--rw-r--r--   0        0        0    11018 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/apps.py
--rw-r--r--   0        0        0     6343 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/auth_helpers.py
--rw-r--r--   0        0        0     7920 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/celery_progress.py
--rw-r--r--   0        0        0      197 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/context_processors.py
--rw-r--r--   0        0        0    18985 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/core_helpers.py
--rw-r--r--   0        0        0      986 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/email.py
--rw-r--r--   0        0        0     1175 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/forms.py
--rw-r--r--   0        0        0     2901 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/frontend_helpers.py
--rw-r--r--   0        0        0     2375 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/ldap.py
--rw-r--r--   0        0        0   192829 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/licenses.json
--rw-r--r--   0        0        0     2255 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/messages.py
--rw-r--r--   0        0        0     2091 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/middlewares.py
--rw-r--r--   0        0        0      850 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/model_helpers.py
--rw-r--r--   0        0        0     3818 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/notifications.py
--rw-r--r--   0        0        0     6131 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/pdf.py
--rw-r--r--   0        0        0     5801 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/predicates.py
--rw-r--r--   0        0        0      936 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/sass_helpers.py
--rw-r--r--   0        0        0      524 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/search.py
--rw-r--r--   0        0        0      125 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/spdx.py
--rw-r--r--   0        0        0     1673 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/util/tables.py
--rw-r--r--   0        0        0    52591 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/views.py
--rw-r--r--   0        0        0    12147 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/vite.config.js
--rw-r--r--   0        0        0      173 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/aleksis/core/wsgi.py
--rw-r--r--   0        0        0       44 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/conftest.py
--rw-r--r--   0        0        0      581 2024-04-04 06:54:07.948225 aleksis_core-4.0.0.dev6/docs/Makefile
--rw-r--r--   0        0        0   127432 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/2fa.png
--rw-r--r--   0        0        0    71362 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/accept_invite.png
--rw-r--r--   0        0        0    72621 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/create_dashboard_widget.png
--rw-r--r--   0        0        0    41935 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/create_social_application.png
--rw-r--r--   0        0        0    72508 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/dashboard.png
--rw-r--r--   0        0        0    87601 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/dashboard_widgets.png
--rw-r--r--   0        0        0   119523 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/data_checks.png
--rw-r--r--   0        0        0    81386 2024-04-04 06:54:07.952225 aleksis_core-4.0.0.dev6/docs/_static/edit_dashboard.png
--rw-r--r--   0        0        0    85722 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/edit_default_dashboard.png
--rw-r--r--   0        0        0   107979 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/invitations.png
--rw-r--r--   0        0        0   177681 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/invite_existing.png
--rw-r--r--   0        0        0    44868 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_desktop_chromium.png
--rw-r--r--   0        0        0    69215 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_chromium.png
--rw-r--r--   0        0        0   128479 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_firefox.png
--rw-r--r--   0        0        0   108973 2024-04-04 06:54:07.956225 aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_safari.png
--rw-r--r--   0        0        0    69804 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/_static/signup.png
--rw-r--r--   0        0        0      132 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/00_index.rst
--rw-r--r--   0        0        0     4231 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/01_core_concepts.rst
--rw-r--r--   0        0        0     8109 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/10_install.rst
--rw-r--r--   0        0        0     1872 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/15_config_files.rst
--rw-r--r--   0        0        0     2086 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/16_config_options.rst
--rw-r--r--   0        0        0     1648 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/17_storage.rst
--rw-r--r--   0        0        0      803 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/18_mail.rst
--rw-r--r--   0        0        0     1509 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/21_ldap.rst
--rw-r--r--   0        0        0     3037 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/22_registration.rst
--rw-r--r--   0        0        0     1467 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/23_socialaccounts.rst
--rw-r--r--   0        0        0     3218 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/31_monitoring.rst
--rw-r--r--   0        0        0     1012 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/32_tasks.rst
--rw-r--r--   0        0        0     1393 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/33_data_checks.rst
--rw-r--r--   0        0        0     4610 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/admin/50_dashboard.rst
--rw-r--r--   0        0        0     6392 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/conf.py
--rw-r--r--   0        0        0      132 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/00_index.rst
--rw-r--r--   0        0        0     4058 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/01_setup.rst
--rw-r--r--   0        0        0     1427 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/02_install_apps.rst
--rw-r--r--   0        0        0     3117 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/03_run_tests.rst
--rw-r--r--   0        0        0     4519 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/04_materialize_templates.rst
--rw-r--r--   0        0        0      289 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/05_extensible_models.rst
--rw-r--r--   0        0        0     1148 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/06_merging_app_settings.rst
--rw-r--r--   0        0        0     1349 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/dev/10_dashboard_widgets.rst
--rw-r--r--   0        0        0      514 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/index.rst
--rw-r--r--   0        0        0      787 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/make.bat
--rw-r--r--   0        0        0       95 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/00_index.rst
--rw-r--r--   0        0        0       69 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/01_checks.rst
--rw-r--r--   0        0        0       70 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/02_managers.rst
--rw-r--r--   0        0        0       64 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/03_mixins.rst
--rw-r--r--   0        0        0       84 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/04_models.rst
--rw-r--r--   0        0        0      108 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/05_registries.rst
--rw-r--r--   0        0        0       93 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/06_search_indexes.rst
--rw-r--r--   0        0        0       79 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/07_tables.rst
--rw-r--r--   0        0        0       90 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/08_tasks.rst
--rw-r--r--   0        0        0     1017 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/09_utils.rst
--rw-r--r--   0        0        0       71 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/10_views.rst
--rw-r--r--   0        0        0       77 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/11_filters.rst
--rw-r--r--   0        0        0      373 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/ref/core/12_template_tags.rst
--rw-r--r--   0        0        0      112 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/00_index.rst
--rw-r--r--   0        0        0     1152 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/01_registration.rst
--rw-r--r--   0        0        0     3465 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/02_personal_account.rst
--rw-r--r--   0        0        0     1770 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/10_dashboard.rst
--rw-r--r--   0        0        0     2607 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/docs/user/20_pwa.rst
--rw-r--r--   0        0        0     5570 2024-04-04 06:54:24.344036 aleksis_core-4.0.0.dev6/pyproject.toml
--rw-r--r--   0        0        0     2180 2024-04-04 06:54:07.960225 aleksis_core-4.0.0.dev6/tox.ini
--rw-r--r--   0        0        0     8737 1970-01-01 00:00:00.000000 aleksis_core-4.0.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0    42631 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/CHANGELOG.rst
+-rw-r--r--   0        0        0    14353 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/LICENCE.rst
+-rw-r--r--   0        0        0     3786 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/README.rst
+-rw-r--r--   0        0        0      194 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/__main__.py
+-rw-r--r--   0        0        0      510 2024-04-23 15:02:13.078757 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2024-04-23 15:02:13.890748 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0     2168 2024-04-23 15:02:16.178721 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0    11656 2024-04-23 15:02:14.866737 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     2533 2024-04-23 15:02:13.114757 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0        0        0     3716 2024-04-23 15:02:16.266720 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/checks.cpython-311.pyc
+-rw-r--r--   0        0        0    23254 2024-04-23 15:02:15.890725 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     5154 2024-04-23 15:02:16.274720 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/health_checks.cpython-311.pyc
+-rw-r--r--   0        0        0    10749 2024-04-23 15:02:15.930724 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0    40416 2024-04-23 15:02:15.910724 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0   103996 2024-04-23 15:02:15.494729 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    25279 2024-04-23 15:02:16.474718 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1144 2024-04-23 15:02:14.882736 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/registries.cpython-311.pyc
+-rw-r--r--   0        0        0    18563 2024-04-23 15:02:16.206721 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0    44148 2024-04-23 15:02:13.902747 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     3825 2024-04-23 15:02:15.934724 aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0     1002 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/admin.py
+-rw-r--r--   0        0        0     8751 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/apps.py
+-rw-r--r--   0        0        0     1338 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/celery.py
+-rw-r--r--   0        0        0     2759 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/checks.py
+-rw-r--r--   0        0        0    14836 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/data_checks.py
+-rw-r--r--   0        0        0      741 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/decorators.py
+-rw-r--r--   0        0        0     5506 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/filters.py
+-rw-r--r--   0        0        0    30667 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/forms.py
+-rw-r--r--   0        0        0     3178 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/apollo.js
+-rw-r--r--   0        0        0     1757 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/dateTimeFormats.js
+-rw-r--r--   0        0        0      197 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/i18n.js
+-rw-r--r--   0        0        0      157 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/router.js
+-rw-r--r--   0        0        0      133 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/sentry.js
+-rw-r--r--   0        0        0     1091 2024-04-23 15:01:16.515413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/vuetify.js
+-rw-r--r--   0        0        0     4682 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/LegacyBaseTemplate.vue
+-rw-r--r--   0        0        0      158 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/Parent.vue
+-rw-r--r--   0        0        0      335 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/About.vue
+-rw-r--r--   0        0        0     1971 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/AboutAleksis.vue
+-rw-r--r--   0        0        0     3831 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/InstalledAppCard.vue
+-rw-r--r--   0        0        0     1003 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/InstalledAppsList.vue
+-rw-r--r--   0        0        0      351 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/installedApps.graphql
+-rw-r--r--   0        0        0     2412 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/AccountMenu.vue
+-rw-r--r--   0        0        0    10484 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/App.vue
+-rw-r--r--   0        0        0      314 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/BrandLogo.vue
+-rw-r--r--   0        0        0     1064 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/ErrorPage.vue
+-rw-r--r--   0        0        0     1471 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/LanguageForm.vue
+-rw-r--r--   0        0        0     4635 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/SideNav.vue
+-rw-r--r--   0        0        0     1454 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/SidenavSearch.vue
+-rw-r--r--   0        0        0      748 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/SnackbarItem.vue
+-rw-r--r--   0        0        0     1932 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/Splash.vue
+-rw-r--r--   0        0        0      124 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/customMenu.graphql
+-rw-r--r--   0        0        0      205 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/dynamicRoutes.graphql
+-rw-r--r--   0        0        0       42 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/messages.graphql
+-rw-r--r--   0        0        0       59 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/ping.graphql
+-rw-r--r--   0        0        0      139 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/searchSnippets.graphql
+-rw-r--r--   0        0        0      412 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/systemProperties.graphql
+-rw-r--r--   0        0        0      329 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/whoAmI.graphql
+-rw-r--r--   0        0        0     2568 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
+-rw-r--r--   0        0        0     1894 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
+-rw-r--r--   0        0        0      220 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
+-rw-r--r--   0        0        0       84 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
+-rw-r--r--   0        0        0     3564 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue
+-rw-r--r--   0        0        0     1190 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue
+-rw-r--r--   0        0        0    13721 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/Calendar.vue
+-rw-r--r--   0        0        0      624 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarControlBar.vue
+-rw-r--r--   0        0        0      309 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarDownloadAllButton.vue
+-rw-r--r--   0        0        0     5903 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarOverview.vue
+-rw-r--r--   0        0        0     2072 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarSelect.vue
+-rw-r--r--   0        0        0      364 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarStatusChip.vue
+-rw-r--r--   0        0        0     1521 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue
+-rw-r--r--   0        0        0     1560 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarWithControls.vue
+-rw-r--r--   0        0        0      318 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CancelledCalendarStatusChip.vue
+-rw-r--r--   0        0        0      405 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/GenericCalendarFeedDetails.vue
+-rw-r--r--   0        0        0      386 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/GenericCalendarFeedEventBar.vue
+-rw-r--r--   0        0        0      426 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/calendar.graphql
+-rw-r--r--   0        0        0      154 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/calendarFeeds.graphql
+-rw-r--r--   0        0        0      561 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/calendarMixin.js
+-rw-r--r--   0        0        0     1096 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js
+-rw-r--r--   0        0        0     9850 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue
+-rw-r--r--   0        0        0     1021 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql
+-rw-r--r--   0        0        0       93 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/setCalendarStatus.graphql
+-rw-r--r--   0        0        0      715 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue
+-rw-r--r--   0        0        0     5242 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue
+-rw-r--r--   0        0        0      434 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar_feeds/event_bar/BirthdaysEventBar.vue
+-rw-r--r--   0        0        0     3611 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
+-rw-r--r--   0        0        0     2806 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
+-rw-r--r--   0        0        0      925 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
+-rw-r--r--   0        0        0      432 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
+-rw-r--r--   0        0        0      191 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
+-rw-r--r--   0        0        0      118 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
+-rw-r--r--   0        0        0     3009 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/ActionSelect.vue
+-rw-r--r--   0        0        0      655 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/AvatarClickbox.vue
+-rw-r--r--   0        0        0      212 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/BackButton.vue
+-rw-r--r--   0        0        0      823 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/ButtonMenu.vue
+-rw-r--r--   0        0        0    13623 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CRUDBar.vue
+-rw-r--r--   0        0        0     5044 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CRUDIterator.vue
+-rw-r--r--   0        0        0     7047 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CRUDList.vue
+-rw-r--r--   0        0        0     1559 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue
+-rw-r--r--   0        0        0     1359 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/DateSelectFooter.vue
+-rw-r--r--   0        0        0      981 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/DetailView.vue
+-rw-r--r--   0        0        0     1483 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/FilterBar.vue
+-rw-r--r--   0        0        0     5289 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/InlineCRUDList.vue
+-rw-r--r--   0        0        0      435 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/ListView.vue
+-rw-r--r--   0        0        0      268 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/MessageBox.vue
+-rw-r--r--   0        0        0     1914 2024-04-23 15:01:16.519413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/ObjectOverview.vue
+-rw-r--r--   0        0        0      269 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/SmallContainer.vue
+-rw-r--r--   0        0        0      292 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/TableLink.vue
+-rw-r--r--   0        0        0     2017 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/UpdateIndicator.vue
+-rw-r--r--   0        0        0      716 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/BaseButton.vue
+-rw-r--r--   0        0        0      456 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/CancelButton.vue
+-rw-r--r--   0        0        0     1229 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue
+-rw-r--r--   0        0        0      361 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/CreateButton.vue
+-rw-r--r--   0        0        0      370 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/DeleteButton.vue
+-rw-r--r--   0        0        0      357 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/EditButton.vue
+-rw-r--r--   0        0        0     1139 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/FilterButton.vue
+-rw-r--r--   0        0        0      335 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/PrimaryActionButton.vue
+-rw-r--r--   0        0        0      357 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/SaveButton.vue
+-rw-r--r--   0        0        0      427 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/SecondaryActionButton.vue
+-rw-r--r--   0        0        0      440 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/ClosableSnackbar.vue
+-rw-r--r--   0        0        0     1273 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue
+-rw-r--r--   0        0        0     3269 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
+-rw-r--r--   0        0        0     5971 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue
+-rw-r--r--   0        0        0     2244 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue
+-rw-r--r--   0        0        0     1038 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue
+-rw-r--r--   0        0        0     1360 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/ColorField.vue
+-rw-r--r--   0        0        0     2622 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/DateField.vue
+-rw-r--r--   0        0        0     2401 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/DateTimeField.vue
+-rw-r--r--   0        0        0     3229 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue
+-rw-r--r--   0        0        0     1006 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue
+-rw-r--r--   0        0        0     4834 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue
+-rw-r--r--   0        0        0      695 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/SexSelect.vue
+-rw-r--r--   0        0        0     2390 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/TimeField.vue
+-rw-r--r--   0        0        0     1267 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/WeekDayField.vue
+-rw-r--r--   0        0        0      355 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/group/GroupChip.vue
+-rw-r--r--   0        0        0      706 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/group/GroupCollection.vue
+-rw-r--r--   0        0        0     2125 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/group_type/GroupType.vue
+-rw-r--r--   0        0        0      696 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/group_type/groupType.graphql
+-rw-r--r--   0        0        0     2697 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/holiday/HolidayInlineList.vue
+-rw-r--r--   0        0        0      742 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/holiday/holiday.graphql
+-rw-r--r--   0        0        0     2966 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/notifications/NotificationItem.vue
+-rw-r--r--   0        0        0     2616 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/notifications/NotificationList.vue
+-rw-r--r--   0        0        0      107 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
+-rw-r--r--   0        0        0      207 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/notifications/myNotifications.graphql
+-rw-r--r--   0        0        0     1017 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/pdf/DownloadPDF.vue
+-rw-r--r--   0        0        0       78 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/pdf/pdf.graphql
+-rw-r--r--   0        0        0     1410 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/AdditionalImage.vue
+-rw-r--r--   0        0        0     1252 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/AvatarContent.vue
+-rw-r--r--   0        0        0     3389 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonActions.vue
+-rw-r--r--   0        0        0      527 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
+-rw-r--r--   0        0        0      862 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonChip.vue
+-rw-r--r--   0        0        0      759 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonCollection.vue
+-rw-r--r--   0        0        0     2482 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonList.vue
+-rw-r--r--   0        0        0     9873 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonOverview.vue
+-rw-r--r--   0        0        0      108 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/avatarContent.graphql
+-rw-r--r--   0        0        0      301 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/personActions.graphql
+-rw-r--r--   0        0        0      345 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/personList.graphql
+-rw-r--r--   0        0        0      589 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/personOverview.graphql
+-rw-r--r--   0        0        0     1488 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/room/RoomInlineList.vue
+-rw-r--r--   0        0        0      630 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/room/room.graphql
+-rw-r--r--   0        0        0     2516 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/school_term/SchoolTermField.vue
+-rw-r--r--   0        0        0     2952 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue
+-rw-r--r--   0        0        0      742 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/school_term/schoolTerm.graphql
+-rw-r--r--   0        0        0     3859 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/two_factor/TwoFactor.vue
+-rw-r--r--   0        0        0     1490 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
+-rw-r--r--   0        0        0      589 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
+-rw-r--r--   0        0        0      385 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/two_factor/twoFactor.graphql
+-rw-r--r--   0        0        0      422 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/css/global.scss
+-rw-r--r--   0        0        0     2841 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/index.js
+-rw-r--r--   0        0        0    15236 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/de.json
+-rw-r--r--   0        0        0    14328 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/en.json
+-rw-r--r--   0        0        0    18225 2024-04-23 15:01:16.523413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/ru.json
+-rw-r--r--   0        0        0    17582 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/uk.json
+-rw-r--r--   0        0        0     3052 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/aleksis.js
+-rw-r--r--   0        0        0     1060 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/calendarFeedDetails.js
+-rw-r--r--   0        0        0      386 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/calendarFeedEventBar.js
+-rw-r--r--   0        0        0     2695 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/createOrPatchMixin.js
+-rw-r--r--   0        0        0      938 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/deepSearchMixin.js
+-rw-r--r--   0        0        0     1540 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/deleteMixin.js
+-rw-r--r--   0        0        0      538 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/error404.js
+-rw-r--r--   0        0        0     2419 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/formRulesMixin.js
+-rw-r--r--   0        0        0      490 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/loadingMixin.js
+-rw-r--r--   0        0        0     3450 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/menus.js
+-rw-r--r--   0        0        0     3296 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/mutateMixin.js
+-rw-r--r--   0        0        0     2256 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/offline.js
+-rw-r--r--   0        0        0      762 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/permissions.js
+-rw-r--r--   0        0        0     3060 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/queryMixin.js
+-rw-r--r--   0        0        0     2154 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/routes.js
+-rw-r--r--   0        0        0      524 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/sexChoiceMixin.js
+-rw-r--r--   0        0        0      766 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/syncSortMixin.js
+-rw-r--r--   0        0        0     1684 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/useRegisterSW.js
+-rw-r--r--   0        0        0     7148 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/plugins/aleksis.js
+-rw-r--r--   0        0        0      450 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/routeValidators.js
+-rw-r--r--   0        0        0    34409 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/frontend/routes.js
+-rw-r--r--   0        0        0     2642 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/health_checks.py
+-rw-r--r--   0        0        0      487 2024-04-23 15:02:16.734715 aleksis_core-4.0.0.dev7/aleksis/core/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74550 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2024-04-23 15:02:16.730715 aleksis_core-4.0.0.dev7/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      894 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    64425 2024-04-23 15:02:16.718715 aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   127576 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2024-04-23 15:02:16.706715 aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1118 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      942 2024-04-23 15:02:16.726715 aleksis_core-4.0.0.dev7/aleksis/core/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    78337 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2024-04-23 15:02:16.718715 aleksis_core-4.0.0.dev7/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      810 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2510 2024-04-23 15:02:16.742715 aleksis_core-4.0.0.dev7/aleksis/core/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    84014 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-04-23 15:02:16.734715 aleksis_core-4.0.0.dev7/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-04-23 15:01:16.527413 aleksis_core-4.0.0.dev7/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2024-04-23 15:02:16.722715 aleksis_core-4.0.0.dev7/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74480 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-04-23 15:02:16.710715 aleksis_core-4.0.0.dev7/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    79209 2024-04-23 15:02:16.746715 aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   137668 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2024-04-23 15:02:16.734715 aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1321 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2024-04-23 15:02:16.706715 aleksis_core-4.0.0.dev7/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74420 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-04-23 15:02:16.702715 aleksis_core-4.0.0.dev7/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    78198 2024-04-23 15:02:16.734715 aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   135337 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2024-04-23 15:02:16.718715 aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2024-04-23 15:01:16.615412 aleksis_core-4.0.0.dev7/aleksis/core/management/__init__.py
+-rw-r--r--   0        0        0     3957 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/management/commands/convert_urls_to_routes.py
+-rw-r--r--   0        0        0     1082 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/management/commands/vite.py
+-rw-r--r--   0        0        0      439 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/management/commands/webpack_bundle.py
+-rw-r--r--   0        0        0     5688 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/managers.py
+-rw-r--r--   0        0        0    49187 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2198 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0002_school_term.py
+-rw-r--r--   0        0        0      531 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0003_drop_image_cropping.py
+-rw-r--r--   0        0        0      796 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
+-rw-r--r--   0        0        0     1252 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0005_timestamped_activity_notification.py
+-rw-r--r--   0        0        0     1567 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0006_dashboard_widget_size.py
+-rw-r--r--   0        0        0     1207 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0007_dashboard_widget_order.py
+-rw-r--r--   0        0        0     1936 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0008_data_check_result.py
+-rw-r--r--   0        0        0     1052 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0009_default_dashboard.py
+-rw-r--r--   0        0        0      952 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0010_external_link_widget.py
+-rw-r--r--   0        0        0      829 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0011_globalpermissions_options.py
+-rw-r--r--   0        0        0      501 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0012_valid_from_announcement.py
+-rw-r--r--   0        0        0     2073 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0013_pdf_file.py
+-rw-r--r--   0        0        0      533 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0014_alter_pdffile_file.py
+-rw-r--r--   0        0        0     1174 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0015_oauth_permissions.py
+-rw-r--r--   0        0        0     1341 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0016_taskuserassignment.py
+-rw-r--r--   0        0        0      426 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0017_dashboardwidget_broken.py
+-rw-r--r--   0        0        0      897 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0018_pdffile_html_file.py
+-rw-r--r--   0        0        0     2116 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      542 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0020_pdf_file_person_optional.py
+-rw-r--r--   0        0        0     1084 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
+-rw-r--r--   0        0        0      923 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0022_public_favicon.py
+-rw-r--r--   0        0        0     6340 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0023_oauth_application_model.py
+-rw-r--r--   0        0        0      714 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0024_oauth_grant_types_optional.py
+-rw-r--r--   0        0        0     1717 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0025_oauth_align_user_fk.py
+-rw-r--r--   0        0        0      582 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
+-rw-r--r--   0        0        0      457 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0027_person_place_of_birth.py
+-rw-r--r--   0        0        0      947 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0028_char_field_not_null.py
+-rw-r--r--   0        0        0     1465 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0029_invitations.py
+-rw-r--r--   0        0        0     1776 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0030_user_attributes.py
+-rw-r--r--   0        0        0      526 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0031_oauthapplication_icon.py
+-rw-r--r--   0        0        0      340 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0032_remove_person_is_active.py
+-rw-r--r--   0        0        0     2416 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0033_update_photo_avatar.py
+-rw-r--r--   0        0        0      816 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0034_invite_permission.py
+-rw-r--r--   0        0        0     1924 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0035_preference_model_unique.py
+-rw-r--r--   0        0        0      626 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0036_additionalfields_helptext_required.py
+-rw-r--r--   0        0        0      917 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0037_add_static_content_widget.py
+-rw-r--r--   0        0        0      522 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0038_notification_send_at.py
+-rw-r--r--   0        0        0     1029 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0039_personal_ical_url.py
+-rw-r--r--   0        0        0      613 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
+-rw-r--r--   0        0        0      516 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0041_update_gender_choices.py
+-rw-r--r--   0        0        0      547 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0042_pdffile_empty.py
+-rw-r--r--   0        0        0     2261 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0043_task_assignment_meta.py
+-rw-r--r--   0        0        0      532 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0044_task_assignment_result_fetched.py
+-rw-r--r--   0        0        0      486 2024-04-23 15:01:16.531413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
+-rw-r--r--   0        0        0   290966 2024-04-23 15:01:16.535413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0046_notification_create_field_icon.py
+-rw-r--r--   0        0        0     2510 2024-04-23 15:01:16.535413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0047_add_room_model.py
+-rw-r--r--   0        0        0   893996 2024-04-23 15:01:16.535413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0048_delete_personalicalurl.py
+-rw-r--r--   0        0        0      533 2024-04-23 15:01:16.535413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
+-rw-r--r--   0        0        0     6221 2024-04-23 15:01:16.535413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0050_managed_by_app_label.py
+-rw-r--r--   0        0        0     5606 2024-04-23 15:01:16.535413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0051_calendarevent_and_holiday.py
+-rw-r--r--   0        0        0   909270 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0052_site_related_name.py
+-rw-r--r--   0        0        0      914 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0053_freebusy.py
+-rw-r--r--   0        0        0     1994 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0054_create_organisation_model.py
+-rw-r--r--   0        0        0     1738 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0055_customevent.py
+-rw-r--r--   0        0        0      332 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0056_rename_customevent_personalevent.py
+-rw-r--r--   0        0        0      505 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0057_drop_otp_yubikey.py
+-rw-r--r--   0        0        0      720 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0058_migrate_preferences_to_global.py
+-rw-r--r--   0        0        0     5514 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0059_drop_site.py
+-rw-r--r--   0        0        0     1165 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0060_person_unique_short_name_email.py
+-rw-r--r--   0        0        0      500 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/migrations/0061_remove_group_additional_fields.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:01:16.619412 aleksis_core-4.0.0.dev7/aleksis/core/migrations/__init__.py
+-rw-r--r--   0        0        0    25176 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/mixins.py
+-rw-r--r--   0        0        0    64648 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/models.py
+-rw-r--r--   0        0        0    15497 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/preferences.py
+-rw-r--r--   0        0        0      611 2024-04-23 15:01:16.539413 aleksis_core-4.0.0.dev7/aleksis/core/registries.py
+-rw-r--r--   0        0        0    17713 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/rules.py
+-rw-r--r--   0        0        0    11074 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/__init__.py
+-rw-r--r--   0        0        0     7649 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/base.py
+-rw-r--r--   0        0        0     4023 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/calendar.py
+-rw-r--r--   0        0        0     3049 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/celery_progress.py
+-rw-r--r--   0        0        0      585 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/custom_menu.py
+-rw-r--r--   0        0        0      459 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/dynamic_routes.py
+-rw-r--r--   0        0        0     2005 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/group.py
+-rw-r--r--   0        0        0     1309 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/group_type.py
+-rw-r--r--   0        0        0     1430 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/holiday.py
+-rw-r--r--   0        0        0     1743 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/installed_apps.py
+-rw-r--r--   0        0        0      265 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/message.py
+-rw-r--r--   0        0        0     1296 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/notification.py
+-rw-r--r--   0        0        0     1145 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/oauth.py
+-rw-r--r--   0        0        0      554 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/pdf.py
+-rw-r--r--   0        0        0      124 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/permissions.py
+-rw-r--r--   0        0        0    10060 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/person.py
+-rw-r--r--   0        0        0     3382 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/personal_event.py
+-rw-r--r--   0        0        0     1270 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/room.py
+-rw-r--r--   0        0        0     2147 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/school_term.py
+-rw-r--r--   0        0        0      868 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/search.py
+-rw-r--r--   0        0        0     1343 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/site_preferences.py
+-rw-r--r--   0        0        0     1697 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/system_properties.py
+-rw-r--r--   0        0        0     3297 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/two_factor.py
+-rw-r--r--   0        0        0      829 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/schema/user.py
+-rw-r--r--   0        0        0      418 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/search_indexes.py
+-rw-r--r--   0        0        0    39858 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/settings.py
+-rw-r--r--   0        0        0    49621 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-banner.svg
+-rw-r--r--   0        0        0     1862 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-favicon.png
+-rw-r--r--   0        0        0    17172 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon-maskable.png
+-rw-r--r--   0        0        0     7843 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon-maskable.svg
+-rw-r--r--   0        0        0    31902 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon.png
+-rw-r--r--   0        0        0     7346 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon.svg
+-rw-r--r--   0        0        0    19126 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/fallback.png
+-rw-r--r--   0        0        0     2237 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/img/hero.svg
+-rw-r--r--   0        0        0      490 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/copy_button.js
+-rw-r--r--   0        0        0      521 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/edit_dashboard.js
+-rw-r--r--   0        0        0      618 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/helper.js
+-rw-r--r--   0        0        0      984 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/include_ajax_live.js
+-rw-r--r--   0        0        0     4351 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/main.js
+-rw-r--r--   0        0        0     1654 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/multi_select.js
+-rw-r--r--   0        0        0     3495 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/search.js
+-rw-r--r--   0        0        0     2581 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/js/serviceworker.js
+-rw-r--r--   0        0        0      271 2024-04-23 15:01:16.543413 aleksis_core-4.0.0.dev7/aleksis/core/static/print-simple.css
+-rw-r--r--   0        0        0     1627 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/static/print.css
+-rw-r--r--   0        0        0      187 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/static/print_landscape.css
+-rw-r--r--   0        0        0     1064 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/static/public/materialize-custom.scss
+-rw-r--r--   0        0        0    15749 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/static/public/style.scss
+-rw-r--r--   0        0        0    11345 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/static/public/theme.scss
+-rw-r--r--   0        0        0     5408 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/tables.py
+-rw-r--r--   0        0        0     2330 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/tasks.py
+-rw-r--r--   0        0        0      838 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/403.html
+-rw-r--r--   0        0        0      789 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/404.html
+-rw-r--r--   0        0        0      918 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/500.html
+-rw-r--r--   0        0        0       76 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/503.html
+-rw-r--r--   0        0        0      851 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      169 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0      525 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0        0        0     1255 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     1182 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_change.html
+-rw-r--r--   0        0        0     1377 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset.html
+-rw-r--r--   0        0        0      825 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     2305 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      649 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      500 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_set.html
+-rw-r--r--   0        0        0      888 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/signup.html
+-rw-r--r--   0        0        0      838 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      820 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/verification_email_required.html
+-rw-r--r--   0        0        0     1160 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      979 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/components/chips.html
+-rw-r--r--   0        0        0      350 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/components/materialize-chips.html
+-rw-r--r--   0        0        0      225 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/components/msgbox.html
+-rw-r--r--   0        0        0      958 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/components/pagination.html
+-rw-r--r--   0        0        0      486 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/components/text_collapsible.html
+-rw-r--r--   0        0        0     1053 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/announcement/form.html
+-rw-r--r--   0        0        0     1900 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/announcement/list.html
+-rw-r--r--   0        0        0     3099 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/base.html
+-rw-r--r--   0        0        0     2454 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/base_print.html
+-rw-r--r--   0        0        0     1212 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/base_simple_print.html
+-rw-r--r--   0        0        0      628 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/create.html
+-rw-r--r--   0        0        0      635 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
+-rw-r--r--   0        0        0      626 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/edit.html
+-rw-r--r--   0        0        0      262 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
+-rw-r--r--   0        0        0     1349 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/list.html
+-rw-r--r--   0        0        0      226 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
+-rw-r--r--   0        0        0     3879 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/data_check/list.html
+-rw-r--r--   0        0        0     2233 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/edit_dashboard.html
+-rw-r--r--   0        0        0        0 2024-04-23 15:01:16.623412 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/empty.html
+-rw-r--r--   0        0        0     5310 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/child_groups.html
+-rw-r--r--   0        0        0      650 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/edit.html
+-rw-r--r--   0        0        0     3382 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/full.html
+-rw-r--r--   0        0        0     1019 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/list.html
+-rw-r--r--   0        0        0     2504 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/index.html
+-rw-r--r--   0        0        0      777 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/pages/delete.html
+-rw-r--r--   0        0        0     6832 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/pages/system_status.html
+-rw-r--r--   0        0        0      603 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/pages/test_pdf.html
+-rw-r--r--   0        0        0       93 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/address.html
+-rw-r--r--   0        0        0      189 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/admins_list.html
+-rw-r--r--   0        0        0     1632 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/announcements.html
+-rw-r--r--   0        0        0     1472 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/avatar_content.html
+-rw-r--r--   0        0        0      319 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/copy_button.html
+-rw-r--r--   0        0        0     1089 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/crud_events.html
+-rw-r--r--   0        0        0      389 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/edit_dashboard_widget.html
+-rw-r--r--   0        0        0     1624 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/meta.html
+-rw-r--r--   0        0        0      414 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/on_page_menu.html
+-rw-r--r--   0        0        0      260 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/save_button.html
+-rw-r--r--   0        0        0     2358 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/splash_screen.html
+-rw-r--r--   0        0        0      325 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/turnable.html
+-rw-r--r--   0        0        0      915 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/perms/assign.html
+-rw-r--r--   0        0        0     2478 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/perms/list.html
+-rw-r--r--   0        0        0      376 2024-04-23 15:01:16.547413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/person/collection.html
+-rw-r--r--   0        0        0      649 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/person/create.html
+-rw-r--r--   0        0        0      645 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/person/edit.html
+-rw-r--r--   0        0        0     1165 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/person/list.html
+-rw-r--r--   0        0        0      927 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/core/vue_index.html
+-rw-r--r--   0        0        0     3921 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/django_tables2/materialize.html
+-rw-r--r--   0        0        0      981 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/dynamic_preferences/form.html
+-rw-r--r--   0        0        0      376 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/dynamic_preferences/sections.html
+-rw-r--r--   0        0        0      764 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/invitations/disabled.html
+-rw-r--r--   0        0        0     1281 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/invitations/enter.html
+-rw-r--r--   0        0        0     1162 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/invitations/forms/_invite.html
+-rw-r--r--   0        0        0      102 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/invitations/messages/invite_accepted.txt
+-rw-r--r--   0        0        0      171 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/material/field_errors.html
+-rw-r--r--   0        0        0     1232 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
+-rw-r--r--   0        0        0     1897 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/colorfield_colorwidget.html
+-rw-r--r--   0        0        0     1009 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
+-rw-r--r--   0        0        0     1009 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/django_select2_select2widget.html
+-rw-r--r--   0        0        0      253 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/material/non_field_errors.html
+-rw-r--r--   0        0        0      663 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/create.html
+-rw-r--r--   0        0        0     2335 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/detail.html
+-rw-r--r--   0        0        0      669 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/edit.html
+-rw-r--r--   0        0        0     1074 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/list.html
+-rw-r--r--   0        0        0     2686 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/authorize.html
+-rw-r--r--   0        0        0      887 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/offline.html
+-rw-r--r--   0        0        0       42 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/search/indexes/core/group_text.txt
+-rw-r--r--   0        0        0       69 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/search/indexes/core/person_text.txt
+-rw-r--r--   0        0        0       42 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/search/indexes/core/room_text.txt
+-rw-r--r--   0        0        0     3171 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/search/search.html
+-rw-r--r--   0        0        0      243 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/search/searchbar_snippet.html
+-rw-r--r--   0        0        0      150 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/search/searchbar_snippets.html
+-rw-r--r--   0        0        0      169 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/sms/notification.txt
+-rw-r--r--   0        0        0      893 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1268 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1289 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      809 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0     1012 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0     1660 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      630 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/base.email
+-rw-r--r--   0        0        0     1527 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/celery_failure.email
+-rw-r--r--   0        0        0      994 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/data_checks.email
+-rw-r--r--   0        0        0     1014 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/email.css
+-rw-r--r--   0        0        0     1102 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/invitation.email
+-rw-r--r--   0        0        0     1461 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/notification.email
+-rw-r--r--   0        0        0      668 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/person_changed.email
+-rw-r--r--   0        0        0      219 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      877 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0      119 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1780 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     6686 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      943 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0      986 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/phone_register.html
+-rw-r--r--   0        0        0     3050 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0     2127 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      786 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0        0 2024-04-23 15:01:16.627412 aleksis_core-4.0.0.dev7/aleksis/core/templatetags/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templatetags/apps.py
+-rw-r--r--   0        0        0      394 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templatetags/dashboard.py
+-rw-r--r--   0        0        0     1611 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templatetags/data_helpers.py
+-rw-r--r--   0        0        0     1543 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templatetags/html_helpers.py
+-rw-r--r--   0        0        0      206 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/templatetags/msg_box.py
+-rw-r--r--   0        0        0     3696 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/browser/test_selenium.py
+-rw-r--r--   0        0        0      761 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/managers/test_aleksisbasemanager.py
+-rw-r--r--   0        0        0     1607 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/mixins/test_registry_object.py
+-rw-r--r--   0        0        0     6596 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test.pdf
+-rw-r--r--   0        0        0     1520 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test_group_sync.py
+-rw-r--r--   0        0        0     3049 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test_notification.py
+-rw-r--r--   0        0        0     4003 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test_pdffile.py
+-rw-r--r--   0        0        0      427 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test_person.py
+-rw-r--r--   0        0        0     5503 2024-04-23 15:01:16.551413 aleksis_core-4.0.0.dev7/aleksis/core/tests/regression/test_regression.py
+-rw-r--r--   0        0        0      683 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/tests/regression/view_oauth.py
+-rw-r--r--   0        0        0     1021 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/tests/templatetags/test_data_helpers.py
+-rw-r--r--   0        0        0     2292 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/tests/views/test_account.py
+-rw-r--r--   0        0        0    17541 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/urls.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:01:16.627412 aleksis_core-4.0.0.dev7/aleksis/core/util/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-23 15:02:13.418753 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14949 2024-04-23 15:02:14.886736 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    10101 2024-04-23 15:02:15.934724 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
+-rw-r--r--   0        0        0    29144 2024-04-23 15:02:13.422753 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     1500 2024-04-23 15:02:13.846748 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/email.cpython-311.pyc
+-rw-r--r--   0        0        0      771 2024-04-23 15:02:15.946724 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     5811 2024-04-23 15:02:15.934724 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0     9909 2024-04-23 15:02:16.206721 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0     2181 2024-04-23 15:02:14.914736 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0      657 2024-04-23 15:02:14.910736 aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
+-rw-r--r--   0        0        0    11018 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/apps.py
+-rw-r--r--   0        0        0     6617 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/auth_helpers.py
+-rw-r--r--   0        0        0     7920 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/celery_progress.py
+-rw-r--r--   0        0        0      197 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/context_processors.py
+-rw-r--r--   0        0        0    18985 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/core_helpers.py
+-rw-r--r--   0        0        0      986 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/email.py
+-rw-r--r--   0        0        0     1175 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/forms.py
+-rw-r--r--   0        0        0     2901 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/frontend_helpers.py
+-rw-r--r--   0        0        0     2375 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/ldap.py
+-rw-r--r--   0        0        0   192829 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/licenses.json
+-rw-r--r--   0        0        0     2255 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/messages.py
+-rw-r--r--   0        0        0     2091 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/middlewares.py
+-rw-r--r--   0        0        0      850 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/model_helpers.py
+-rw-r--r--   0        0        0     3818 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/notifications.py
+-rw-r--r--   0        0        0     6131 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/pdf.py
+-rw-r--r--   0        0        0     5801 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/predicates.py
+-rw-r--r--   0        0        0      936 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/sass_helpers.py
+-rw-r--r--   0        0        0      524 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/search.py
+-rw-r--r--   0        0        0      125 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/spdx.py
+-rw-r--r--   0        0        0     1673 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/util/tables.py
+-rw-r--r--   0        0        0    52591 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/views.py
+-rw-r--r--   0        0        0    12147 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/vite.config.js
+-rw-r--r--   0        0        0      173 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/aleksis/core/wsgi.py
+-rw-r--r--   0        0        0       44 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/conftest.py
+-rw-r--r--   0        0        0      581 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/docs/Makefile
+-rw-r--r--   0        0        0   127432 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/docs/_static/2fa.png
+-rw-r--r--   0        0        0    71362 2024-04-23 15:01:16.555413 aleksis_core-4.0.0.dev7/docs/_static/accept_invite.png
+-rw-r--r--   0        0        0    72621 2024-04-23 15:01:16.559413 aleksis_core-4.0.0.dev7/docs/_static/create_dashboard_widget.png
+-rw-r--r--   0        0        0    41935 2024-04-23 15:01:16.559413 aleksis_core-4.0.0.dev7/docs/_static/create_social_application.png
+-rw-r--r--   0        0        0    72508 2024-04-23 15:01:16.559413 aleksis_core-4.0.0.dev7/docs/_static/dashboard.png
+-rw-r--r--   0        0        0    87601 2024-04-23 15:01:16.559413 aleksis_core-4.0.0.dev7/docs/_static/dashboard_widgets.png
+-rw-r--r--   0        0        0   119523 2024-04-23 15:01:16.559413 aleksis_core-4.0.0.dev7/docs/_static/data_checks.png
+-rw-r--r--   0        0        0    81386 2024-04-23 15:01:16.559413 aleksis_core-4.0.0.dev7/docs/_static/edit_dashboard.png
+-rw-r--r--   0        0        0    85722 2024-04-23 15:01:16.559413 aleksis_core-4.0.0.dev7/docs/_static/edit_default_dashboard.png
+-rw-r--r--   0        0        0   107979 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/_static/invitations.png
+-rw-r--r--   0        0        0   177681 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/_static/invite_existing.png
+-rw-r--r--   0        0        0    44868 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/_static/pwa_desktop_chromium.png
+-rw-r--r--   0        0        0    69215 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/_static/pwa_mobile_chromium.png
+-rw-r--r--   0        0        0   128479 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/_static/pwa_mobile_firefox.png
+-rw-r--r--   0        0        0   108973 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/_static/pwa_mobile_safari.png
+-rw-r--r--   0        0        0    69804 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/_static/signup.png
+-rw-r--r--   0        0        0      132 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     4231 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/01_core_concepts.rst
+-rw-r--r--   0        0        0     8109 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/10_install.rst
+-rw-r--r--   0        0        0     1872 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/15_config_files.rst
+-rw-r--r--   0        0        0     2086 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/16_config_options.rst
+-rw-r--r--   0        0        0     1648 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/17_storage.rst
+-rw-r--r--   0        0        0      803 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/18_mail.rst
+-rw-r--r--   0        0        0     1509 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/21_ldap.rst
+-rw-r--r--   0        0        0     3037 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/22_registration.rst
+-rw-r--r--   0        0        0     1467 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/23_socialaccounts.rst
+-rw-r--r--   0        0        0     3218 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/31_monitoring.rst
+-rw-r--r--   0        0        0     1012 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/32_tasks.rst
+-rw-r--r--   0        0        0     1393 2024-04-23 15:01:16.563413 aleksis_core-4.0.0.dev7/docs/admin/33_data_checks.rst
+-rw-r--r--   0        0        0     4610 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/admin/50_dashboard.rst
+-rw-r--r--   0        0        0     6392 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/conf.py
+-rw-r--r--   0        0        0      132 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     4058 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/01_setup.rst
+-rw-r--r--   0        0        0     1427 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/02_install_apps.rst
+-rw-r--r--   0        0        0     3117 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/03_run_tests.rst
+-rw-r--r--   0        0        0     4519 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/04_materialize_templates.rst
+-rw-r--r--   0        0        0      289 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/05_extensible_models.rst
+-rw-r--r--   0        0        0     1148 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/06_merging_app_settings.rst
+-rw-r--r--   0        0        0     1349 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/dev/10_dashboard_widgets.rst
+-rw-r--r--   0        0        0      514 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/index.rst
+-rw-r--r--   0        0        0      787 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/make.bat
+-rw-r--r--   0        0        0       95 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/00_index.rst
+-rw-r--r--   0        0        0       69 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/01_checks.rst
+-rw-r--r--   0        0        0       70 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/02_managers.rst
+-rw-r--r--   0        0        0       64 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/03_mixins.rst
+-rw-r--r--   0        0        0       84 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/04_models.rst
+-rw-r--r--   0        0        0      108 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/05_registries.rst
+-rw-r--r--   0        0        0       93 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/06_search_indexes.rst
+-rw-r--r--   0        0        0       79 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/07_tables.rst
+-rw-r--r--   0        0        0       90 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/08_tasks.rst
+-rw-r--r--   0        0        0     1017 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/09_utils.rst
+-rw-r--r--   0        0        0       71 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/10_views.rst
+-rw-r--r--   0        0        0       77 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/11_filters.rst
+-rw-r--r--   0        0        0      373 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/ref/core/12_template_tags.rst
+-rw-r--r--   0        0        0      112 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1152 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/user/01_registration.rst
+-rw-r--r--   0        0        0     3465 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/user/02_personal_account.rst
+-rw-r--r--   0        0        0     1770 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/user/10_dashboard.rst
+-rw-r--r--   0        0        0     2607 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/docs/user/20_pwa.rst
+-rw-r--r--   0        0        0     5570 2024-04-23 15:01:33.611215 aleksis_core-4.0.0.dev7/pyproject.toml
+-rw-r--r--   0        0        0     2180 2024-04-23 15:01:16.567412 aleksis_core-4.0.0.dev7/tox.ini
+-rw-r--r--   0        0        0     8737 1970-01-01 00:00:00.000000 aleksis_core-4.0.0.dev7/PKG-INFO
```

### Comparing `aleksis_core-4.0.0.dev6/CHANGELOG.rst` & `aleksis_core-4.0.0.dev7/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 * Generic endpoint for retrieving objects as JSON
 * [Dev] Base model for organisational entities (external companies, associations,…)
 * Management of personal calendar events.
 * [Dev] Support running of data checks before/after migrations.
 * Views can request to span the entire screen width.
 * Add option to disallow reserved usernames.
 * Error message when loading in incompatible browser
+* Tooltips for every information in the person page
 
 Changed
 ~~~~~~~
 
 * Management of school terms was migrated to new frontend.
 * [Dev] Child groups are exposed in the GraphQL type for groups.
 * Content width on different screen sizes is more consistent.
@@ -54,14 +55,16 @@
 * Persons could not be edited by non-superusers with global person editing permission.
 * GraphQL mutations did not return errors in case of exceptions.
 * Make email field unique over all persons.
 * Third-party login buttons now directly open external login page.
 * Opening group details wasn't possible without permissions for all person details.
 * [Dev] Foreign keys to ExtensiblePolymorphicModel types were using the wrong manager.
 * [Dev] Allow activating more frequent polling for Celery task progress.
+* [OIDC] Custom additional claims were not present in userinfo 
+* Synchronisation of AlekSIS and Django groups caused permissions issues
 
 Removed
 ~~~~~~~
 
 * Yubikey support (not WebAuthn) was removed
 * [Dev] `_recursive` methods for groups have been removed.
   Developers relying on parent groups need to account for recursion themselves.
```

### Comparing `aleksis_core-4.0.0.dev6/LICENCE.rst` & `aleksis_core-4.0.0.dev7/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/README.rst` & `aleksis_core-4.0.0.dev7/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/__main__.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/__main__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 464
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/admin.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/admin.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 1002
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/apps.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/apps.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 8751
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/celery.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/celery.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 1338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/checks.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 2759
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/data_checks.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/data_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 14836
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/health_checks.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/health_checks.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 2642
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/managers.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/managers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 5688
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/mixins.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/mixins.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 25176
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/models.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
-files sz: 64469
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
+files sz: 64648
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d015a016d035a0301
@@ -656,430 +656,430 @@
                1140 MAKE_FUNCTION            0
                1142 LOAD_CONST              85 ('Group')
                1144 LOAD_NAME              122 (SchoolTermRelatedExtensibleModel)
                1146 PRECALL                  3
                1150 CALL                     3
                1160 STORE_NAME              20 (Group)
    
-    597        1162 PUSH_NULL
+    602        1162 PUSH_NULL
                1164 LOAD_BUILD_CLASS
-               1166 LOAD_CONST              86 (<code object PersonGroupThrough, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 597>)
+               1166 LOAD_CONST              86 (<code object PersonGroupThrough, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 602>)
                1168 MAKE_FUNCTION            0
                1170 LOAD_CONST              87 ('PersonGroupThrough')
                1172 LOAD_NAME              117 (ExtensibleModel)
                1174 PRECALL                  3
                1178 CALL                     3
                1188 STORE_NAME             138 (PersonGroupThrough)
    
-    608        1190 PUSH_NULL
+    613        1190 PUSH_NULL
                1192 LOAD_NAME               38 (receiver)
                1194 LOAD_NAME               33 (models)
                1196 LOAD_ATTR               81 (signals)
                1206 LOAD_ATTR              139 (m2m_changed)
                1216 LOAD_NAME              138 (PersonGroupThrough)
                1218 KW_NAMES                88
                1220 PRECALL                  2
                1224 CALL                     2
    
-    609        1234 PUSH_NULL
+    614        1234 PUSH_NULL
                1236 LOAD_NAME               38 (receiver)
                1238 LOAD_NAME               33 (models)
                1240 LOAD_ATTR               81 (signals)
                1250 LOAD_ATTR              139 (m2m_changed)
                1260 LOAD_NAME               20 (Group)
                1262 LOAD_ATTR              140 (owners)
                1272 LOAD_ATTR              141 (through)
                1282 KW_NAMES                88
                1284 PRECALL                  2
                1288 CALL                     2
    
-    610        1298 LOAD_CONST              89 ('sender')
+    615        1298 LOAD_CONST              89 ('sender')
    
-    611        1300 LOAD_NAME               12 (Union)
+    616        1300 LOAD_NAME               12 (Union)
                1302 LOAD_NAME              138 (PersonGroupThrough)
                1304 LOAD_NAME               20 (Group)
                1306 LOAD_ATTR              140 (owners)
                1316 LOAD_ATTR              141 (through)
                1326 BUILD_TUPLE              2
                1328 BINARY_SUBSCR
    
-    610        1338 LOAD_CONST              90 ('instance')
+    615        1338 LOAD_CONST              90 ('instance')
    
-    612        1340 LOAD_NAME               33 (models)
+    617        1340 LOAD_NAME               33 (models)
                1342 LOAD_ATTR              142 (Model)
    
-    610        1352 LOAD_CONST              91 ('action')
+    615        1352 LOAD_CONST              91 ('action')
    
-    613        1354 LOAD_NAME              143 (str)
+    618        1354 LOAD_NAME              143 (str)
    
-    610        1356 LOAD_CONST              92 ('reverse')
+    615        1356 LOAD_CONST              92 ('reverse')
    
-    614        1358 LOAD_NAME              144 (bool)
+    619        1358 LOAD_NAME              144 (bool)
    
-    610        1360 LOAD_CONST              93 ('model')
+    615        1360 LOAD_CONST              93 ('model')
    
-    615        1362 LOAD_NAME               33 (models)
+    620        1362 LOAD_NAME               33 (models)
                1364 LOAD_ATTR              142 (Model)
    
-    610        1374 LOAD_CONST              94 ('pk_set')
+    615        1374 LOAD_CONST              94 ('pk_set')
    
-    616        1376 LOAD_NAME               10 (Optional)
+    621        1376 LOAD_NAME               10 (Optional)
                1378 LOAD_NAME              145 (set)
                1380 BINARY_SUBSCR
    
-    610        1390 LOAD_CONST              95 ('return')
+    615        1390 LOAD_CONST              95 ('return')
    
-    618        1392 LOAD_CONST               1 (None)
+    623        1392 LOAD_CONST               1 (None)
    
-    610        1394 BUILD_TUPLE             14
-               1396 LOAD_CONST              96 (<code object save_group_on_m2m_changed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 608>)
+    615        1394 BUILD_TUPLE             14
+               1396 LOAD_CONST              96 (<code object save_group_on_m2m_changed, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 613>)
                1398 MAKE_FUNCTION            4 (annotations)
    
-    609        1400 PRECALL                  0
+    614        1400 PRECALL                  0
                1404 CALL                     0
    
-    608        1414 PRECALL                  0
+    613        1414 PRECALL                  0
                1418 CALL                     0
    
-    610        1428 STORE_NAME             146 (save_group_on_m2m_changed)
+    615        1428 STORE_NAME             146 (save_group_on_m2m_changed)
    
-    643        1430 PUSH_NULL
+    648        1430 PUSH_NULL
                1432 LOAD_BUILD_CLASS
-               1434 LOAD_CONST              97 (<code object Activity, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 643>)
+               1434 LOAD_CONST              97 (<code object Activity, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 648>)
                1436 MAKE_FUNCTION            0
                1438 LOAD_CONST              98 ('Activity')
                1440 LOAD_NAME              117 (ExtensibleModel)
                1442 LOAD_NAME               89 (TimeStampedModel)
                1444 PRECALL                  4
                1448 CALL                     4
                1458 STORE_NAME             147 (Activity)
    
-    663        1460 PUSH_NULL
+    668        1460 PUSH_NULL
                1462 LOAD_BUILD_CLASS
-               1464 LOAD_CONST              99 (<code object Notification, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 663>)
+               1464 LOAD_CONST              99 (<code object Notification, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 668>)
                1466 MAKE_FUNCTION            0
                1468 LOAD_CONST             100 ('Notification')
                1470 LOAD_NAME              117 (ExtensibleModel)
                1472 LOAD_NAME               89 (TimeStampedModel)
                1474 PRECALL                  4
                1478 CALL                     4
                1488 STORE_NAME             148 (Notification)
    
-    706        1490 PUSH_NULL
+    711        1490 PUSH_NULL
                1492 LOAD_BUILD_CLASS
-               1494 LOAD_CONST             101 (<code object AnnouncementQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 706>)
+               1494 LOAD_CONST             101 (<code object AnnouncementQuerySet, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 711>)
                1496 MAKE_FUNCTION            0
                1498 LOAD_CONST             102 ('AnnouncementQuerySet')
                1500 LOAD_NAME               33 (models)
                1502 LOAD_ATTR               36 (QuerySet)
                1512 PRECALL                  3
                1516 CALL                     3
                1526 STORE_NAME             149 (AnnouncementQuerySet)
    
-    760        1528 PUSH_NULL
+    765        1528 PUSH_NULL
                1530 LOAD_BUILD_CLASS
-               1532 LOAD_CONST             103 (<code object Announcement, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 760>)
+               1532 LOAD_CONST             103 (<code object Announcement, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 765>)
                1534 MAKE_FUNCTION            0
                1536 LOAD_CONST             104 ('Announcement')
                1538 LOAD_NAME              117 (ExtensibleModel)
                1540 PRECALL                  3
                1544 CALL                     3
                1554 STORE_NAME             150 (Announcement)
    
-    806        1556 PUSH_NULL
+    811        1556 PUSH_NULL
                1558 LOAD_BUILD_CLASS
-               1560 LOAD_CONST             105 (<code object AnnouncementRecipient, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 806>)
+               1560 LOAD_CONST             105 (<code object AnnouncementRecipient, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 811>)
                1562 MAKE_FUNCTION            0
                1564 LOAD_CONST             106 ('AnnouncementRecipient')
                1566 LOAD_NAME              117 (ExtensibleModel)
                1568 PRECALL                  3
                1572 CALL                     3
                1582 STORE_NAME             151 (AnnouncementRecipient)
    
-    844        1584 PUSH_NULL
+    849        1584 PUSH_NULL
                1586 LOAD_BUILD_CLASS
-               1588 LOAD_CONST             107 (<code object DashboardWidget, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 844>)
+               1588 LOAD_CONST             107 (<code object DashboardWidget, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 849>)
                1590 MAKE_FUNCTION            0
                1592 LOAD_CONST             108 ('DashboardWidget')
                1594 LOAD_NAME              121 (RegistryObject)
                1596 LOAD_NAME               99 (PolymorphicModel)
                1598 LOAD_NAME              120 (PureDjangoModel)
                1600 PRECALL                  5
                1604 CALL                     5
                1614 STORE_NAME             152 (DashboardWidget)
    
-    921        1616 PUSH_NULL
+    926        1616 PUSH_NULL
                1618 LOAD_BUILD_CLASS
-               1620 LOAD_CONST             109 (<code object ExternalLinkWidget, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 921>)
+               1620 LOAD_CONST             109 (<code object ExternalLinkWidget, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 926>)
                1622 MAKE_FUNCTION            0
                1624 LOAD_CONST             110 ('ExternalLinkWidget')
                1626 LOAD_NAME              152 (DashboardWidget)
                1628 PRECALL                  3
                1632 CALL                     3
                1642 STORE_NAME             153 (ExternalLinkWidget)
    
-    935        1644 PUSH_NULL
+    940        1644 PUSH_NULL
                1646 LOAD_BUILD_CLASS
-               1648 LOAD_CONST             111 (<code object StaticContentWidget, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 935>)
+               1648 LOAD_CONST             111 (<code object StaticContentWidget, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 940>)
                1650 MAKE_FUNCTION            0
                1652 LOAD_CONST             112 ('StaticContentWidget')
                1654 LOAD_NAME              152 (DashboardWidget)
                1656 PRECALL                  3
                1660 CALL                     3
                1670 STORE_NAME             154 (StaticContentWidget)
    
-    948        1672 PUSH_NULL
+    953        1672 PUSH_NULL
                1674 LOAD_BUILD_CLASS
-               1676 LOAD_CONST             113 (<code object DashboardWidgetOrder, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 948>)
+               1676 LOAD_CONST             113 (<code object DashboardWidgetOrder, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 953>)
                1678 MAKE_FUNCTION            0
                1680 LOAD_CONST             114 ('DashboardWidgetOrder')
                1682 LOAD_NAME              117 (ExtensibleModel)
                1684 PRECALL                  3
                1688 CALL                     3
                1698 STORE_NAME             155 (DashboardWidgetOrder)
    
-    975        1700 PUSH_NULL
+    980        1700 PUSH_NULL
                1702 LOAD_BUILD_CLASS
-               1704 LOAD_CONST             115 (<code object CustomMenu, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 975>)
+               1704 LOAD_CONST             115 (<code object CustomMenu, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 980>)
                1706 MAKE_FUNCTION            0
                1708 LOAD_CONST             116 ('CustomMenu')
                1710 LOAD_NAME              117 (ExtensibleModel)
                1712 PRECALL                  3
                1716 CALL                     3
                1726 STORE_NAME             156 (CustomMenu)
    
-    998        1728 PUSH_NULL
+   1003        1728 PUSH_NULL
                1730 LOAD_BUILD_CLASS
-               1732 LOAD_CONST             117 (<code object CustomMenuItem, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 998>)
+               1732 LOAD_CONST             117 (<code object CustomMenuItem, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1003>)
                1734 MAKE_FUNCTION            0
                1736 LOAD_CONST             118 ('CustomMenuItem')
                1738 LOAD_NAME              117 (ExtensibleModel)
                1740 PRECALL                  3
                1744 CALL                     3
                1754 STORE_NAME             157 (CustomMenuItem)
    
-   1022        1756 PUSH_NULL
+   1027        1756 PUSH_NULL
                1758 LOAD_BUILD_CLASS
-               1760 LOAD_CONST             119 (<code object DynamicRoute, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1022>)
+               1760 LOAD_CONST             119 (<code object DynamicRoute, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1027>)
                1762 MAKE_FUNCTION            0
                1764 LOAD_CONST             120 ('DynamicRoute')
                1766 LOAD_NAME              121 (RegistryObject)
                1768 PRECALL                  3
                1772 CALL                     3
                1782 STORE_NAME             158 (DynamicRoute)
    
-   1030        1784 PUSH_NULL
+   1035        1784 PUSH_NULL
                1786 LOAD_BUILD_CLASS
-               1788 LOAD_CONST             121 (<code object GroupType, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1030>)
+               1788 LOAD_CONST             121 (<code object GroupType, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1035>)
                1790 MAKE_FUNCTION            0
                1792 LOAD_CONST             122 ('GroupType')
                1794 LOAD_NAME              117 (ExtensibleModel)
                1796 PRECALL                  3
                1800 CALL                     3
                1810 STORE_NAME             159 (GroupType)
    
-   1051        1812 PUSH_NULL
+   1056        1812 PUSH_NULL
                1814 LOAD_BUILD_CLASS
-               1816 LOAD_CONST             123 (<code object GlobalPermissions, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1051>)
+               1816 LOAD_CONST             123 (<code object GlobalPermissions, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1056>)
                1818 MAKE_FUNCTION            0
                1820 LOAD_CONST             124 ('GlobalPermissions')
                1822 LOAD_NAME              119 (GlobalPermissionModel)
                1824 PRECALL                  3
                1828 CALL                     3
                1838 STORE_NAME             160 (GlobalPermissions)
    
-   1069        1840 PUSH_NULL
+   1074        1840 PUSH_NULL
                1842 LOAD_BUILD_CLASS
-               1844 LOAD_CONST             125 (<code object PersonPreferenceModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1069>)
+               1844 LOAD_CONST             125 (<code object PersonPreferenceModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1074>)
                1846 MAKE_FUNCTION            0
                1848 LOAD_CONST             126 ('PersonPreferenceModel')
                1850 LOAD_NAME               72 (PerInstancePreferenceModel)
                1852 LOAD_NAME              120 (PureDjangoModel)
                1854 PRECALL                  4
                1858 CALL                     4
                1868 STORE_NAME             161 (PersonPreferenceModel)
    
-   1078        1870 PUSH_NULL
+   1083        1870 PUSH_NULL
                1872 LOAD_BUILD_CLASS
-               1874 LOAD_CONST             127 (<code object GroupPreferenceModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1078>)
+               1874 LOAD_CONST             127 (<code object GroupPreferenceModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1083>)
                1876 MAKE_FUNCTION            0
                1878 LOAD_CONST             128 ('GroupPreferenceModel')
                1880 LOAD_NAME               72 (PerInstancePreferenceModel)
                1882 LOAD_NAME              120 (PureDjangoModel)
                1884 PRECALL                  4
                1888 CALL                     4
                1898 STORE_NAME             162 (GroupPreferenceModel)
    
-   1087        1900 PUSH_NULL
+   1092        1900 PUSH_NULL
                1902 LOAD_BUILD_CLASS
-               1904 LOAD_CONST             129 (<code object DataCheckResult, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1087>)
+               1904 LOAD_CONST             129 (<code object DataCheckResult, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1092>)
                1906 MAKE_FUNCTION            0
                1908 LOAD_CONST             130 ('DataCheckResult')
                1910 LOAD_NAME              117 (ExtensibleModel)
                1912 PRECALL                  3
                1916 CALL                     3
                1926 STORE_NAME             163 (DataCheckResult)
    
-   1122        1928 PUSH_NULL
+   1127        1928 PUSH_NULL
                1930 LOAD_BUILD_CLASS
-               1932 LOAD_CONST             131 (<code object PersonInvitation, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1122>)
+               1932 LOAD_CONST             131 (<code object PersonInvitation, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1127>)
                1934 MAKE_FUNCTION            0
                1936 LOAD_CONST             132 ('PersonInvitation')
                1938 LOAD_NAME               83 (AbstractBaseInvitation)
                1940 LOAD_NAME              120 (PureDjangoModel)
                1942 PRECALL                  4
                1946 CALL                     4
                1956 STORE_NAME             164 (PersonInvitation)
    
-   1173        1958 PUSH_NULL
+   1178        1958 PUSH_NULL
                1960 LOAD_BUILD_CLASS
-               1962 LOAD_CONST             133 (<code object PDFFile, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1173>)
+               1962 LOAD_CONST             133 (<code object PDFFile, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1178>)
                1964 MAKE_FUNCTION            0
                1966 LOAD_CONST             134 ('PDFFile')
                1968 LOAD_NAME              117 (ExtensibleModel)
                1970 PRECALL                  3
                1974 CALL                     3
                1984 STORE_NAME             165 (PDFFile)
    
-   1205        1986 PUSH_NULL
+   1210        1986 PUSH_NULL
                1988 LOAD_BUILD_CLASS
-               1990 LOAD_CONST             135 (<code object TaskUserAssignment, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1205>)
+               1990 LOAD_CONST             135 (<code object TaskUserAssignment, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1210>)
                1992 MAKE_FUNCTION            0
                1994 LOAD_CONST             136 ('TaskUserAssignment')
                1996 LOAD_NAME              117 (ExtensibleModel)
                1998 PRECALL                  3
                2002 CALL                     3
                2012 STORE_NAME             166 (TaskUserAssignment)
    
-   1286        2014 PUSH_NULL
+   1291        2014 PUSH_NULL
                2016 LOAD_BUILD_CLASS
-               2018 LOAD_CONST             137 (<code object UserAdditionalAttributes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1286>)
+               2018 LOAD_CONST             137 (<code object UserAdditionalAttributes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1291>)
                2020 MAKE_FUNCTION            0
                2022 LOAD_CONST             138 ('UserAdditionalAttributes')
                2024 LOAD_NAME               33 (models)
                2026 LOAD_ATTR              142 (Model)
                2036 LOAD_NAME              120 (PureDjangoModel)
                2038 PRECALL                  4
                2042 CALL                     4
                2052 STORE_NAME             167 (UserAdditionalAttributes)
    
-   1329        2054 PUSH_NULL
+   1334        2054 PUSH_NULL
                2056 LOAD_BUILD_CLASS
-               2058 LOAD_CONST             139 (<code object OAuthApplication, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1329>)
+               2058 LOAD_CONST             139 (<code object OAuthApplication, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1334>)
                2060 MAKE_FUNCTION            0
                2062 LOAD_CONST             140 ('OAuthApplication')
                2064 LOAD_NAME               92 (AbstractApplication)
                2066 PRECALL                  3
                2070 CALL                     3
                2080 STORE_NAME             168 (OAuthApplication)
    
-   1363        2082 PUSH_NULL
+   1368        2082 PUSH_NULL
                2084 LOAD_BUILD_CLASS
-               2086 LOAD_CONST             141 (<code object OAuthGrant, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1363>)
+               2086 LOAD_CONST             141 (<code object OAuthGrant, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1368>)
                2088 MAKE_FUNCTION            0
                2090 LOAD_CONST             142 ('OAuthGrant')
                2092 LOAD_NAME               93 (AbstractGrant)
                2094 PRECALL                  3
                2098 CALL                     3
                2108 STORE_NAME             169 (OAuthGrant)
    
-   1369        2110 PUSH_NULL
+   1374        2110 PUSH_NULL
                2112 LOAD_BUILD_CLASS
-               2114 LOAD_CONST             143 (<code object OAuthAccessToken, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1369>)
+               2114 LOAD_CONST             143 (<code object OAuthAccessToken, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1374>)
                2116 MAKE_FUNCTION            0
                2118 LOAD_CONST             144 ('OAuthAccessToken')
                2120 LOAD_NAME               91 (AbstractAccessToken)
                2122 PRECALL                  3
                2126 CALL                     3
                2136 STORE_NAME             170 (OAuthAccessToken)
    
-   1375        2138 PUSH_NULL
+   1380        2138 PUSH_NULL
                2140 LOAD_BUILD_CLASS
-               2142 LOAD_CONST             145 (<code object OAuthIDToken, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1375>)
+               2142 LOAD_CONST             145 (<code object OAuthIDToken, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1380>)
                2144 MAKE_FUNCTION            0
                2146 LOAD_CONST             146 ('OAuthIDToken')
                2148 LOAD_NAME               94 (AbstractIDToken)
                2150 PRECALL                  3
                2154 CALL                     3
                2164 STORE_NAME             171 (OAuthIDToken)
    
-   1381        2166 PUSH_NULL
+   1386        2166 PUSH_NULL
                2168 LOAD_BUILD_CLASS
-               2170 LOAD_CONST             147 (<code object OAuthRefreshToken, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1381>)
+               2170 LOAD_CONST             147 (<code object OAuthRefreshToken, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1386>)
                2172 MAKE_FUNCTION            0
                2174 LOAD_CONST             148 ('OAuthRefreshToken')
                2176 LOAD_NAME               95 (AbstractRefreshToken)
                2178 PRECALL                  3
                2182 CALL                     3
                2192 STORE_NAME             172 (OAuthRefreshToken)
    
-   1387        2194 PUSH_NULL
+   1392        2194 PUSH_NULL
                2196 LOAD_BUILD_CLASS
-               2198 LOAD_CONST             149 (<code object Room, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1387>)
+               2198 LOAD_CONST             149 (<code object Room, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1392>)
                2200 MAKE_FUNCTION            0
                2202 LOAD_CONST             150 ('Room')
                2204 LOAD_NAME              117 (ExtensibleModel)
                2206 PRECALL                  3
                2210 CALL                     3
                2220 STORE_NAME             173 (Room)
    
-   1409        2222 PUSH_NULL
+   1414        2222 PUSH_NULL
                2224 LOAD_BUILD_CLASS
-               2226 LOAD_CONST             151 (<code object CalendarEvent, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1409>)
+               2226 LOAD_CONST             151 (<code object CalendarEvent, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1414>)
                2228 MAKE_FUNCTION            0
                2230 LOAD_CONST             152 ('CalendarEvent')
                2232 LOAD_NAME              116 (CalendarEventMixin)
                2234 LOAD_NAME              118 (ExtensiblePolymorphicModel)
                2236 PRECALL                  4
                2240 CALL                     4
                2250 STORE_NAME             174 (CalendarEvent)
    
-   1586        2252 PUSH_NULL
+   1591        2252 PUSH_NULL
                2254 LOAD_BUILD_CLASS
-               2256 LOAD_CONST             153 (<code object FreeBusy, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1586>)
+               2256 LOAD_CONST             153 (<code object FreeBusy, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1591>)
                2258 MAKE_FUNCTION            0
                2260 LOAD_CONST             154 ('FreeBusy')
                2262 LOAD_NAME              174 (CalendarEvent)
                2264 PRECALL                  3
                2268 CALL                     3
                2278 STORE_NAME             175 (FreeBusy)
    
-   1590        2280 PUSH_NULL
+   1595        2280 PUSH_NULL
                2282 LOAD_BUILD_CLASS
-               2284 LOAD_CONST             155 (<code object BirthdayEvent, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1590>)
+               2284 LOAD_CONST             155 (<code object BirthdayEvent, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1595>)
                2286 MAKE_FUNCTION            0
                2288 LOAD_CONST             156 ('BirthdayEvent')
                2290 LOAD_NAME              116 (CalendarEventMixin)
                2292 PRECALL                  3
                2296 CALL                     3
                2306 STORE_NAME             176 (BirthdayEvent)
    
-   1646        2308 PUSH_NULL
+   1651        2308 PUSH_NULL
                2310 LOAD_BUILD_CLASS
-               2312 LOAD_CONST             157 (<code object Holiday, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1646>)
+               2312 LOAD_CONST             157 (<code object Holiday, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1651>)
                2314 MAKE_FUNCTION            0
                2316 LOAD_CONST             158 ('Holiday')
                2318 LOAD_NAME              174 (CalendarEvent)
                2320 PRECALL                  3
                2324 CALL                     3
                2334 STORE_NAME             177 (Holiday)
    
-   1720        2336 PUSH_NULL
+   1725        2336 PUSH_NULL
                2338 LOAD_BUILD_CLASS
-               2340 LOAD_CONST             159 (<code object PersonalEvent, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1720>)
+               2340 LOAD_CONST             159 (<code object PersonalEvent, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1725>)
                2342 MAKE_FUNCTION            0
                2344 LOAD_CONST             160 ('PersonalEvent')
                2346 LOAD_NAME              174 (CalendarEvent)
                2348 PRECALL                  3
                2352 CALL                     3
                2362 STORE_NAME             178 (PersonalEvent)
    
-   1807        2364 PUSH_NULL
+   1812        2364 PUSH_NULL
                2366 LOAD_BUILD_CLASS
-               2368 LOAD_CONST             161 (<code object Organisation, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1807>)
+               2368 LOAD_CONST             161 (<code object Organisation, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1812>)
                2370 MAKE_FUNCTION            0
                2372 LOAD_CONST             162 ('Organisation')
                2374 LOAD_NAME              117 (ExtensibleModel)
                2376 PRECALL                  3
                2380 CALL                     3
                2390 STORE_NAME             179 (Organisation)
                2392 LOAD_CONST               1 (None)
@@ -4182,23 +4182,23 @@
                      712 BUILD_TUPLE              2
                      714 LOAD_CLOSURE             0 (__class__)
                      716 BUILD_TUPLE              1
                      718 LOAD_CONST              41 (<code object save, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 572>)
                      720 MAKE_FUNCTION           13 (defaults, annotations, closure)
                      722 STORE_NAME              35 (save)
          
-         590         724 LOAD_NAME               27 (property)
+         593         724 LOAD_NAME               27 (property)
          
-         591         726 LOAD_CONST              42 (<code object django_group, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 590>)
+         594         726 LOAD_CONST              42 (<code object django_group, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 593>)
                      728 MAKE_FUNCTION            0
          
-         590         730 PRECALL                  0
+         593         730 PRECALL                  0
                      734 CALL                     0
          
-         591         744 STORE_NAME              36 (django_group)
+         594         744 STORE_NAME              36 (django_group)
                      746 LOAD_CLOSURE             0 (__class__)
                      748 COPY                     1
                      750 STORE_NAME              37 (__classcell__)
                      752 RETURN_VALUE
          consts
             'Group'
             'Group model.\n\n    Any kind of group of persons in a school, including, but not limited\n    classes, clubs, and the like.\n    '
@@ -4594,38 +4594,36 @@
                firstlineno 564
                lnotab 0x02010e013402
             ('name', 'short_name')
             ('fields',)
             'force'
             code
                argcount  : 2
-               nlocals   : 7
+               nlocals   : 6
                stacksize : 10
                flags     : 15
                code
                   0x950197007c006a00000000000000000064007500702574030000000000
                   00000000007c006a020000000000000000a0030000000000000000000000
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   000000000000007d040200740900000000000000000000a6000000ab0000
                   000000000000006a0500000000000000007c0269007c03a4018e0101007c
-                  0173027c0472d4740c000000000000000000006a070000000000000000a0
-                  0800000000000000000000000000000000000000007c006a090000000000
-                  000000ac01a6010000ab0100000000000000005c0200007d057d067c056a
-                  0a0000000000000000a00b00000000000000000000000000000000000000
-                  007419000000000000000000007c006a0d0000000000000000a00e000000
-                  00000000000000000000000000000000006402ac03a6010000ab01000000
-                  0000000000a00f0000000000000000000000000000000000000000640464
-                  05ac06a6020000ab020000000000000000a0100000000000000000000000
-                  0000000000000000007c006a110000000000000000a00e00000000000000
-                  000000000000000000000000006402ac03a6010000ab0100000000000000
-                  00a00f000000000000000000000000000000000000000064046405ac06a6
-                  020000ab020000000000000000a6010000ab010000000000000000a60100
-                  00ab010000000000000000a6010000ab01000000000000000001007c05a0
-                  050000000000000000000000000000000000000000a6000000ab00000000
-                  000000000001006400530064005300
+                  0173027c0472b77c006a0600000000000000007d057c0572ac7c056a0700
+                  00000000000000a008000000000000000000000000000000000000000074
+                  13000000000000000000007c006a0a0000000000000000a00b0000000000
+                  0000000000000000000000000000006401ac02a6010000ab010000000000
+                  000000a00c000000000000000000000000000000000000000064036404ac
+                  05a6020000ab020000000000000000a00d00000000000000000000000000
+                  000000000000007c006a0e0000000000000000a00b000000000000000000
+                  00000000000000000000006401ac02a6010000ab010000000000000000a0
+                  0c000000000000000000000000000000000000000064036404ac05a60200
+                  00ab020000000000000000a6010000ab010000000000000000a6010000ab
+                  010000000000000000a6010000ab01000000000000000001007c05a00500
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  0000000100640053006400530064005300
                              0 COPY_FREE_VARS           1
                
                572           2 RESUME                   0
                
                574           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (pk)
                             16 LOAD_CONST               0 (None)
@@ -4652,181 +4650,198 @@
                            142 DICT_MERGE               1
                            144 CALL_FUNCTION_EX         1
                            146 POP_TOP
                
                578         148 LOAD_FAST                1 (force)
                            150 POP_JUMP_FORWARD_IF_TRUE     2 (to 156)
                            152 LOAD_FAST                4 (dirty)
-                           154 POP_JUMP_FORWARD_IF_FALSE   212 (to 580)
+                           154 POP_JUMP_FORWARD_IF_FALSE   183 (to 522)
                
-               580     >>  156 LOAD_GLOBAL             12 (DjangoGroup)
-                           168 LOAD_ATTR                7 (objects)
-                           178 LOAD_METHOD              8 (get_or_create)
-                           200 LOAD_FAST                0 (self)
-                           202 LOAD_ATTR                9 (name)
-                           212 KW_NAMES                 1
-                           214 PRECALL                  1
-                           218 CALL                     1
-                           228 UNPACK_SEQUENCE          2
-                           232 STORE_FAST               5 (dj_group)
-                           234 STORE_FAST               6 (_)
-               
-               581         236 LOAD_FAST                5 (dj_group)
-                           238 LOAD_ATTR               10 (user_set)
-                           248 LOAD_METHOD             11 (set)
-               
-               582         270 LOAD_GLOBAL             25 (NULL + list)
-               
-               583         282 LOAD_FAST                0 (self)
-                           284 LOAD_ATTR               13 (members)
-                           294 LOAD_METHOD             14 (filter)
-                           316 LOAD_CONST               2 (False)
-                           318 KW_NAMES                 3
-                           320 PRECALL                  1
-                           324 CALL                     1
-               
-               584         334 LOAD_METHOD             15 (values_list)
-                           356 LOAD_CONST               4 ('user')
-                           358 LOAD_CONST               5 (True)
-                           360 KW_NAMES                 6
-                           362 PRECALL                  2
-                           366 CALL                     2
-               
-               585         376 LOAD_METHOD             16 (union)
-                           398 LOAD_FAST                0 (self)
-                           400 LOAD_ATTR               17 (owners)
-                           410 LOAD_METHOD             14 (filter)
-                           432 LOAD_CONST               2 (False)
-                           434 KW_NAMES                 3
-                           436 PRECALL                  1
-                           440 CALL                     1
-                           450 LOAD_METHOD             15 (values_list)
-                           472 LOAD_CONST               4 ('user')
-                           474 LOAD_CONST               5 (True)
-                           476 KW_NAMES                 6
-                           478 PRECALL                  2
-                           482 CALL                     2
-                           492 PRECALL                  1
-                           496 CALL                     1
-               
-               582         506 PRECALL                  1
-                           510 CALL                     1
-               
-               581         520 PRECALL                  1
-                           524 CALL                     1
-                           534 POP_TOP
-               
-               588         536 LOAD_FAST                5 (dj_group)
-                           538 LOAD_METHOD              5 (save)
-                           560 PRECALL                  0
-                           564 CALL                     0
-                           574 POP_TOP
-                           576 LOAD_CONST               0 (None)
-                           578 RETURN_VALUE
+               580     >>  156 LOAD_FAST                0 (self)
+                           158 LOAD_ATTR                6 (django_group)
+                           168 STORE_FAST               5 (dj_group)
+               
+               581         170 LOAD_FAST                5 (dj_group)
+                           172 POP_JUMP_FORWARD_IF_FALSE   172 (to 518)
+               
+               582         174 LOAD_FAST                5 (dj_group)
+                           176 LOAD_ATTR                7 (user_set)
+                           186 LOAD_METHOD              8 (set)
+               
+               583         208 LOAD_GLOBAL             19 (NULL + list)
+               
+               584         220 LOAD_FAST                0 (self)
+                           222 LOAD_ATTR               10 (members)
+                           232 LOAD_METHOD             11 (filter)
+                           254 LOAD_CONST               1 (False)
+                           256 KW_NAMES                 2
+                           258 PRECALL                  1
+                           262 CALL                     1
+               
+               585         272 LOAD_METHOD             12 (values_list)
+                           294 LOAD_CONST               3 ('user')
+                           296 LOAD_CONST               4 (True)
+                           298 KW_NAMES                 5
+                           300 PRECALL                  2
+                           304 CALL                     2
+               
+               586         314 LOAD_METHOD             13 (union)
+               
+               587         336 LOAD_FAST                0 (self)
+                           338 LOAD_ATTR               14 (owners)
+                           348 LOAD_METHOD             11 (filter)
+                           370 LOAD_CONST               1 (False)
+                           372 KW_NAMES                 2
+                           374 PRECALL                  1
+                           378 CALL                     1
+                           388 LOAD_METHOD             12 (values_list)
+                           410 LOAD_CONST               3 ('user')
+                           412 LOAD_CONST               4 (True)
+                           414 KW_NAMES                 5
+                           416 PRECALL                  2
+                           420 CALL                     2
+               
+               586         430 PRECALL                  1
+                           434 CALL                     1
+               
+               583         444 PRECALL                  1
+                           448 CALL                     1
+               
+               582         458 PRECALL                  1
+                           462 CALL                     1
+                           472 POP_TOP
+               
+               591         474 LOAD_FAST                5 (dj_group)
+                           476 LOAD_METHOD              5 (save)
+                           498 PRECALL                  0
+                           502 CALL                     0
+                           512 POP_TOP
+                           514 LOAD_CONST               0 (None)
+                           516 RETURN_VALUE
                
-               578     >>  580 LOAD_CONST               0 (None)
-                           582 RETURN_VALUE
+               581     >>  518 LOAD_CONST               0 (None)
+                           520 RETURN_VALUE
+               
+               578     >>  522 LOAD_CONST               0 (None)
+                           524 RETURN_VALUE
                consts
                   None
-                  ('name',)
                   False
                   ('user__isnull',)
                   'user'
                   True
                   ('flat',)
-               names      ('pk', 'bool', 'group_info_tracker', 'changed', 'super', 'save', 'DjangoGroup', 'objects', 'get_or_create', 'name', 'user_set', 'set', 'list', 'members', 'filter', 'values_list', 'union', 'owners')
-               varnames   ('self', 'force', 'args', 'kwargs', 'dirty', 'dj_group', '_')
+               names      ('pk', 'bool', 'group_info_tracker', 'changed', 'super', 'save', 'django_group', 'user_set', 'set', 'list', 'members', 'filter', 'values_list', 'union', 'owners')
+               varnames   ('self', 'force', 'args', 'kwargs', 'dirty', 'dj_group')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'save'
                firstlineno 572
-               lnotab 0x04025e0232020802500122010c0134012a0182fd0eff10072cf6
+               lnotab
+                  0x04025e02320208020e01040122010c0134012a0116015eff0efd0eff10
+                  092cf604fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
-                  0x97007400000000000000000000006a010000000000000000a002000000
-                  00000000000000000000000000000000007c006a030000000000000000ac
-                  01a6010000ab0100000000000000005c0200007d017d027c015300
-               590           0 RESUME                   0
-               
-               593           2 LOAD_GLOBAL              0 (DjangoGroup)
-                            14 LOAD_ATTR                1 (objects)
-                            24 LOAD_METHOD              2 (get_or_create)
-                            46 LOAD_FAST                0 (self)
-                            48 LOAD_ATTR                3 (name)
-                            58 KW_NAMES                 1
-                            60 PRECALL                  1
-                            64 CALL                     1
-                            74 UNPACK_SEQUENCE          2
-                            78 STORE_FAST               1 (dj_group)
-                            80 STORE_FAST               2 (_)
+                  0x970064017d017c006a00000000000000000072157c006a000000000000
+                  0000007402000000000000000000006a0200000000000000006b02000000
+                  0072287406000000000000000000006a040000000000000000a005000000
+                  00000000000000000000000000000000007c006a060000000000000000ac
+                  02a6010000ab0100000000000000005c0200007d017d027c015300
+               593           0 RESUME                   0
+               
+               596           2 LOAD_CONST               1 (None)
+                             4 STORE_FAST               1 (dj_group)
+               
+               597           6 LOAD_FAST                0 (self)
+                             8 LOAD_ATTR                0 (school_term)
+                            18 POP_JUMP_FORWARD_IF_FALSE    21 (to 62)
+                            20 LOAD_FAST                0 (self)
+                            22 LOAD_ATTR                0 (school_term)
+                            32 LOAD_GLOBAL              2 (SchoolTerm)
+                            44 LOAD_ATTR                2 (current)
+                            54 COMPARE_OP               2 (==)
+                            60 POP_JUMP_FORWARD_IF_FALSE    40 (to 142)
+               
+               598     >>   62 LOAD_GLOBAL              6 (DjangoGroup)
+                            74 LOAD_ATTR                4 (objects)
+                            84 LOAD_METHOD              5 (get_or_create)
+                           106 LOAD_FAST                0 (self)
+                           108 LOAD_ATTR                6 (name)
+                           118 KW_NAMES                 2
+                           120 PRECALL                  1
+                           124 CALL                     1
+                           134 UNPACK_SEQUENCE          2
+                           138 STORE_FAST               1 (dj_group)
+                           140 STORE_FAST               2 (_)
                
-               594          82 LOAD_FAST                1 (dj_group)
-                            84 RETURN_VALUE
+               599     >>  142 LOAD_FAST                1 (dj_group)
+                           144 RETURN_VALUE
                consts
                   'Get Django group for this group.'
+                  None
                   ('name',)
-               names      ('DjangoGroup', 'objects', 'get_or_create', 'name')
+               names      ('school_term', 'SchoolTerm', 'current', 'DjangoGroup', 'objects', 'get_or_create', 'name')
                varnames   ('self', 'dj_group', '_')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'django_group'
-               firstlineno 590
-               lnotab 0x02035001
+               firstlineno 593
+               lnotab 0x0203040138015001
             (False,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'GroupManager', 'from_queryset', 'GroupQuerySet', 'objects', 'Meta', 'icon_', 'models', 'CharField', '_', 'name', 'short_name', 'ManyToManyField', 'members', 'owners', 'parent_groups', 'ForeignKey', 'SET_NULL', 'group_type', 'ImageField', 'photo', 'avatar', 'str', 'get_absolute_url', 'property', 'announcement_recipients', 'dict', 'get_group_stats', '__str__', 'FieldTracker', 'group_info_tracker', 'bool', 'save', 'django_group', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'Group'
          firstlineno 461
          lnotab
             0x0c01040630021a11040236010e0114010201020102fc12070e01020102
             010201020114fb12070e011aff12040e01020102010201140102fb12080e
             0102010c0102011401020102fa12090e01140102010201040102ff0efc12
             080e0114010201020114fc12070c03020104ff0e01020402010aff0e0102
-            0f0c0618021212020104ff0e01
+            0f0c0618021215020104ff0e01
       'Group'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000065
             0665046a070000000000000000ac02a6020000ab0200000000000000005a
             08020065046a050000000000000000650965046a070000000000000000ac
             02a6020000ab0200000000000000005a0a64035300
-         597           0 RESUME                   0
+         602           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PersonGroupThrough')
                        8 STORE_NAME               2 (__qualname__)
          
-         598          10 LOAD_CONST               1 ('Through table for many-to-many relationship of group members.\n\n    It does not have any fields on its own; these are generated upon instantiation\n    by inspecting the additional fields selected for the linked group.\n    ')
+         603          10 LOAD_CONST               1 ('Through table for many-to-many relationship of group members.\n\n    It does not have any fields on its own; these are generated upon instantiation\n    by inspecting the additional fields selected for the linked group.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         604          14 PUSH_NULL
+         609          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (ForeignKey)
                       28 LOAD_NAME                6 (Group)
                       30 LOAD_NAME                4 (models)
                       32 LOAD_ATTR                7 (CASCADE)
                       42 KW_NAMES                 2
                       44 PRECALL                  2
                       48 CALL                     2
                       58 STORE_NAME               8 (group)
          
-         605          60 PUSH_NULL
+         610          60 PUSH_NULL
                       62 LOAD_NAME                4 (models)
                       64 LOAD_ATTR                5 (ForeignKey)
                       74 LOAD_NAME                9 (Person)
                       76 LOAD_NAME                4 (models)
                       78 LOAD_ATTR                7 (CASCADE)
                       88 KW_NAMES                 2
                       90 PRECALL                  2
@@ -4841,15 +4856,15 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'Group', 'CASCADE', 'group', 'Person', 'person')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'PersonGroupThrough'
-         firstlineno 597
+         firstlineno 602
          lnotab 0x0a0104062e01
       'PersonGroupThrough'
       ('sender',)
       'sender'
       'instance'
       'action'
       'reverse'
@@ -4864,51 +4879,51 @@
          code
             0x97007c02640176017202640253007c0372367c046a0000000000000000
             00a00100000000000000000000000000000000000000007c05ac03a60100
             00ab01000000000000000044005d187d077c07a002000000000000000000
             00000000000000000000006404ac05a6010000ab01000000000000000001
             008c19640253007c01a00200000000000000000000000000000000000000
             006404ac05a6010000ab010000000000000000010064025300
-         608           0 RESUME                   0
+         613           0 RESUME                   0
          
-         629           2 LOAD_FAST                2 (action)
+         634           2 LOAD_FAST                2 (action)
                        4 LOAD_CONST               1 (('post_add', 'post_remove', 'post_clear'))
                        6 CONTAINS_OP              1
                        8 POP_JUMP_FORWARD_IF_FALSE     2 (to 14)
          
-         631          10 LOAD_CONST               2 (None)
+         636          10 LOAD_CONST               2 (None)
                       12 RETURN_VALUE
          
-         633     >>   14 LOAD_FAST                3 (reverse)
+         638     >>   14 LOAD_FAST                3 (reverse)
                       16 POP_JUMP_FORWARD_IF_FALSE    54 (to 126)
          
-         636          18 LOAD_FAST                4 (model)
+         641          18 LOAD_FAST                4 (model)
                       20 LOAD_ATTR                0 (objects)
                       30 LOAD_METHOD              1 (filter)
                       52 LOAD_FAST                5 (pk_set)
                       54 KW_NAMES                 3
                       56 PRECALL                  1
                       60 CALL                     1
                       70 GET_ITER
                  >>   72 FOR_ITER                24 (to 122)
                       74 STORE_FAST               7 (group)
          
-         637          76 LOAD_FAST                7 (group)
+         642          76 LOAD_FAST                7 (group)
                       78 LOAD_METHOD              2 (save)
                      100 LOAD_CONST               4 (True)
                      102 KW_NAMES                 5
                      104 PRECALL                  1
                      108 CALL                     1
                      118 POP_TOP
                      120 JUMP_BACKWARD           25 (to 72)
          
-         636     >>  122 LOAD_CONST               2 (None)
+         641     >>  122 LOAD_CONST               2 (None)
                      124 RETURN_VALUE
          
-         640     >>  126 LOAD_FAST                1 (instance)
+         645     >>  126 LOAD_FAST                1 (instance)
                      128 LOAD_METHOD              2 (save)
                      150 LOAD_CONST               4 (True)
                      152 KW_NAMES                 5
                      154 PRECALL                  1
                      158 CALL                     1
                      168 POP_TOP
                      170 LOAD_CONST               2 (None)
@@ -4922,15 +4937,15 @@
             ('force',)
          names      ('objects', 'filter', 'save')
          varnames   ('sender', 'instance', 'action', 'reverse', 'model', 'pk_set', 'kwargs', 'group')
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'save_group_on_m2m_changed'
-         firstlineno 608
+         firstlineno 613
          lnotab 0x02150802040204033a012eff0404
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
          code
@@ -4940,91 +4955,91 @@
             000000000000006406020065076407a6010000ab010000000000000000ac
             08a6020000ab0200000000000000005a0a020065046a0b00000000000000
             00640902006507640aa6010000ab010000000000000000ac08a6020000ab
             0200000000000000005a0c020065046a090000000000000000640b020065
             07640ca6010000ab010000000000000000ac08a6020000ab020000000000
             0000005a0d640d84005a0e02004700640e8400640fa6020000ab02000000
             00000000005a0f64105300
-         643           0 RESUME                   0
+         648           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Activity')
                        8 STORE_NAME               2 (__qualname__)
          
-         644          10 LOAD_CONST               1 ('Activity of a user to trace some actions done in AlekSIS in displayable form.')
+         649          10 LOAD_CONST               1 ('Activity of a user to trace some actions done in AlekSIS in displayable form.')
                       12 STORE_NAME               3 (__doc__)
          
-         646          14 PUSH_NULL
+         651          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (ForeignKey)
          
-         647          28 LOAD_CONST               2 ('Person')
+         652          28 LOAD_CONST               2 ('Person')
                       30 LOAD_NAME                4 (models)
                       32 LOAD_ATTR                6 (CASCADE)
                       42 LOAD_CONST               3 ('activities')
                       44 PUSH_NULL
                       46 LOAD_NAME                7 (_)
                       48 LOAD_CONST               4 ('User')
                       50 PRECALL                  1
                       54 CALL                     1
          
-         646          64 KW_NAMES                 5
+         651          64 KW_NAMES                 5
                       66 PRECALL                  4
                       70 CALL                     4
                       80 STORE_NAME               8 (user)
          
-         650          82 PUSH_NULL
+         655          82 PUSH_NULL
                       84 LOAD_NAME                4 (models)
                       86 LOAD_ATTR                9 (CharField)
                       96 LOAD_CONST               6 (150)
                       98 PUSH_NULL
                      100 LOAD_NAME                7 (_)
                      102 LOAD_CONST               7 ('Title')
                      104 PRECALL                  1
                      108 CALL                     1
                      118 KW_NAMES                 8
                      120 PRECALL                  2
                      124 CALL                     2
                      134 STORE_NAME              10 (title)
          
-         651         136 PUSH_NULL
+         656         136 PUSH_NULL
                      138 LOAD_NAME                4 (models)
                      140 LOAD_ATTR               11 (TextField)
                      150 LOAD_CONST               9 (500)
                      152 PUSH_NULL
                      154 LOAD_NAME                7 (_)
                      156 LOAD_CONST              10 ('Description')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 KW_NAMES                 8
                      174 PRECALL                  2
                      178 CALL                     2
                      188 STORE_NAME              12 (description)
          
-         653         190 PUSH_NULL
+         658         190 PUSH_NULL
                      192 LOAD_NAME                4 (models)
                      194 LOAD_ATTR                9 (CharField)
                      204 LOAD_CONST              11 (100)
                      206 PUSH_NULL
                      208 LOAD_NAME                7 (_)
                      210 LOAD_CONST              12 ('Application')
                      212 PRECALL                  1
                      216 CALL                     1
                      226 KW_NAMES                 8
                      228 PRECALL                  2
                      232 CALL                     2
                      242 STORE_NAME              13 (app)
          
-         655         244 LOAD_CONST              13 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 655>)
+         660         244 LOAD_CONST              13 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 660>)
                      246 MAKE_FUNCTION            0
                      248 STORE_NAME              14 (__str__)
          
-         658         250 PUSH_NULL
+         663         250 PUSH_NULL
                      252 LOAD_BUILD_CLASS
-                     254 LOAD_CONST              14 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 658>)
+                     254 LOAD_CONST              14 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 663>)
                      256 MAKE_FUNCTION            0
                      258 LOAD_CONST              15 ('Meta')
                      260 PRECALL                  2
                      264 CALL                     2
                      274 STORE_NAME              15 (Meta)
                      276 LOAD_CONST              16 (None)
                      278 RETURN_VALUE
@@ -5044,51 +5059,51 @@
             'Application'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               655           0 RESUME                   0
+               660           0 RESUME                   0
                
-               656           2 LOAD_FAST                0 (self)
+               661           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 655
+               firstlineno 660
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               658           0 RESUME                   0
+               663           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Activity.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               659          10 PUSH_NULL
+               664          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Activity')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               660          32 PUSH_NULL
+               665          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Activities')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -5099,25 +5114,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 658
+               firstlineno 663
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'CASCADE', '_', 'user', 'CharField', 'title', 'TextField', 'description', 'app', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'Activity'
-         firstlineno 643
+         firstlineno 648
          lnotab 0x0a0104020e0124ff12043601360236020603
       'Activity'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
@@ -5141,187 +5156,187 @@
             046a1600000000000000006416020065066418a6010000ab010000000000
             000000ac15a6020000ab0200000000000000005a18641984005a19880066
             01641a84085a1a6420641b651b641c651c651d1900000000000000000066
             04641d84055a1e02004700641e8400641fa6020000ab0200000000000000
             005a1f880078015a205300
                        0 MAKE_CELL                0 (__class__)
          
-         663           2 RESUME                   0
+         668           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Notification')
                       10 STORE_NAME               2 (__qualname__)
          
-         664          12 LOAD_CONST               1 ('Notification to submit to a user.')
+         669          12 LOAD_CONST               1 ('Notification to submit to a user.')
                       14 STORE_NAME               3 (__doc__)
          
-         666          16 PUSH_NULL
+         671          16 PUSH_NULL
                       18 LOAD_NAME                4 (models)
                       20 LOAD_ATTR                5 (CharField)
                       30 LOAD_CONST               2 (100)
                       32 PUSH_NULL
                       34 LOAD_NAME                6 (_)
                       36 LOAD_CONST               3 ('Sender')
                       38 PRECALL                  1
                       42 CALL                     1
                       52 KW_NAMES                 4
                       54 PRECALL                  2
                       58 CALL                     2
                       68 STORE_NAME               7 (sender)
          
-         667          70 PUSH_NULL
+         672          70 PUSH_NULL
                       72 LOAD_NAME                4 (models)
                       74 LOAD_ATTR                8 (ForeignKey)
          
-         668          84 LOAD_CONST               5 ('Person')
+         673          84 LOAD_CONST               5 ('Person')
          
-         669          86 LOAD_NAME                4 (models)
+         674          86 LOAD_NAME                4 (models)
                       88 LOAD_ATTR                9 (CASCADE)
          
-         670          98 LOAD_CONST               6 ('notifications')
+         675          98 LOAD_CONST               6 ('notifications')
          
-         671         100 PUSH_NULL
+         676         100 PUSH_NULL
                      102 LOAD_NAME                6 (_)
                      104 LOAD_CONST               7 ('Recipient')
                      106 PRECALL                  1
                      110 CALL                     1
          
-         667         120 KW_NAMES                 8
+         672         120 KW_NAMES                 8
                      122 PRECALL                  4
                      126 CALL                     4
                      136 STORE_NAME              10 (recipient)
          
-         674         138 PUSH_NULL
+         679         138 PUSH_NULL
                      140 LOAD_NAME                4 (models)
                      142 LOAD_ATTR                5 (CharField)
                      152 LOAD_CONST               9 (150)
                      154 PUSH_NULL
                      156 LOAD_NAME                6 (_)
                      158 LOAD_CONST              10 ('Title')
                      160 PRECALL                  1
                      164 CALL                     1
                      174 KW_NAMES                 4
                      176 PRECALL                  2
                      180 CALL                     2
                      190 STORE_NAME              11 (title)
          
-         675         192 PUSH_NULL
+         680         192 PUSH_NULL
                      194 LOAD_NAME                4 (models)
                      196 LOAD_ATTR               12 (TextField)
                      206 LOAD_CONST              11 (500)
                      208 PUSH_NULL
                      210 LOAD_NAME                6 (_)
                      212 LOAD_CONST              12 ('Description')
                      214 PRECALL                  1
                      218 CALL                     1
                      228 KW_NAMES                 4
                      230 PRECALL                  2
                      234 CALL                     2
                      244 STORE_NAME              13 (description)
          
-         676         246 PUSH_NULL
+         681         246 PUSH_NULL
                      248 LOAD_NAME                4 (models)
                      250 LOAD_ATTR               14 (URLField)
                      260 LOAD_CONST              13 (True)
                      262 PUSH_NULL
                      264 LOAD_NAME                6 (_)
                      266 LOAD_CONST              14 ('Link')
                      268 PRECALL                  1
                      272 CALL                     1
                      282 KW_NAMES                15
                      284 PRECALL                  2
                      288 CALL                     2
                      298 STORE_NAME              15 (link)
          
-         678         300 PUSH_NULL
+         683         300 PUSH_NULL
                      302 LOAD_NAME                4 (models)
                      304 LOAD_ATTR                5 (CharField)
          
-         679         314 LOAD_CONST              16 (50)
+         684         314 LOAD_CONST              16 (50)
                      316 LOAD_NAME               16 (ICONS)
                      318 PUSH_NULL
                      320 LOAD_NAME                6 (_)
                      322 LOAD_CONST              17 ('Icon')
                      324 PRECALL                  1
                      328 CALL                     1
                      338 LOAD_CONST              18 ('information-outline')
          
-         678         340 KW_NAMES                19
+         683         340 KW_NAMES                19
                      342 PRECALL                  4
                      346 CALL                     4
                      356 STORE_NAME              17 (icon)
          
-         682         358 PUSH_NULL
+         687         358 PUSH_NULL
                      360 LOAD_NAME                4 (models)
                      362 LOAD_ATTR               18 (DateTimeField)
                      372 LOAD_NAME               19 (timezone)
                      374 LOAD_ATTR               20 (now)
                      384 PUSH_NULL
                      386 LOAD_NAME                6 (_)
                      388 LOAD_CONST              20 ('Send notification at')
                      390 PRECALL                  1
                      394 CALL                     1
                      404 KW_NAMES                21
                      406 PRECALL                  2
                      410 CALL                     2
                      420 STORE_NAME              21 (send_at)
          
-         684         422 PUSH_NULL
+         689         422 PUSH_NULL
                      424 LOAD_NAME                4 (models)
                      426 LOAD_ATTR               22 (BooleanField)
                      436 LOAD_CONST              22 (False)
                      438 PUSH_NULL
                      440 LOAD_NAME                6 (_)
                      442 LOAD_CONST              23 ('Read')
                      444 PRECALL                  1
                      448 CALL                     1
                      458 KW_NAMES                21
                      460 PRECALL                  2
                      464 CALL                     2
                      474 STORE_NAME              23 (read)
          
-         685         476 PUSH_NULL
+         690         476 PUSH_NULL
                      478 LOAD_NAME                4 (models)
                      480 LOAD_ATTR               22 (BooleanField)
                      490 LOAD_CONST              22 (False)
                      492 PUSH_NULL
                      494 LOAD_NAME                6 (_)
                      496 LOAD_CONST              24 ('Sent')
                      498 PRECALL                  1
                      502 CALL                     1
                      512 KW_NAMES                21
                      514 PRECALL                  2
                      518 CALL                     2
                      528 STORE_NAME              24 (sent)
          
-         687         530 LOAD_CONST              25 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 687>)
+         692         530 LOAD_CONST              25 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 692>)
                      532 MAKE_FUNCTION            0
                      534 STORE_NAME              25 (__str__)
          
-         690         536 LOAD_CLOSURE             0 (__class__)
+         695         536 LOAD_CLOSURE             0 (__class__)
                      538 BUILD_TUPLE              1
-                     540 LOAD_CONST              26 (<code object save, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 690>)
+                     540 LOAD_CONST              26 (<code object save, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 695>)
                      542 MAKE_FUNCTION            8 (closure)
                      544 STORE_NAME              26 (save)
          
-         696         546 LOAD_CONST              32 ((False,))
+         701         546 LOAD_CONST              32 ((False,))
                      548 LOAD_CONST              27 ('resend')
                      550 LOAD_NAME               27 (bool)
                      552 LOAD_CONST              28 ('return')
                      554 LOAD_NAME               28 (Optional)
                      556 LOAD_NAME               29 (AsyncResult)
                      558 BINARY_SUBSCR
                      568 BUILD_TUPLE              4
-                     570 LOAD_CONST              29 (<code object send, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 696>)
+                     570 LOAD_CONST              29 (<code object send, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 701>)
                      572 MAKE_FUNCTION            5 (defaults, annotations)
                      574 STORE_NAME              30 (send)
          
-         701         576 PUSH_NULL
+         706         576 PUSH_NULL
                      578 LOAD_BUILD_CLASS
-                     580 LOAD_CONST              30 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 701>)
+                     580 LOAD_CONST              30 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 706>)
                      582 MAKE_FUNCTION            0
                      584 LOAD_CONST              31 ('Meta')
                      586 PRECALL                  2
                      590 CALL                     2
                      600 STORE_NAME              31 (Meta)
                      602 LOAD_CLOSURE             0 (__class__)
                      604 COPY                     1
@@ -5357,31 +5372,31 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-               687           0 RESUME                   0
+               692           0 RESUME                   0
                
-               688           2 LOAD_GLOBAL              1 (NULL + str)
+               693           2 LOAD_GLOBAL              1 (NULL + str)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (title)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('str', 'title')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 687
+               firstlineno 692
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 11
                code
@@ -5391,140 +5406,140 @@
                   0000006a050000000000000000a6000000ab0000000000000000006b0100
                   00000072317c00a0060000000000000000000000000000000000000000a6
                   000000ab00000000000000000001000200740100000000000000000000a6
                   000000ab0000000000000000006a010000000000000000640169007c01a4
                   018e010100640053006400530064005300
                              0 COPY_FREE_VARS           1
                
-               690           2 RESUME                   0
+               695           2 RESUME                   0
                
-               691           4 PUSH_NULL
+               696           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (save)
                             42 LOAD_CONST               1 (())
                             44 BUILD_MAP                0
                             46 LOAD_FAST                1 (kwargs)
                             48 DICT_MERGE               1
                             50 CALL_FUNCTION_EX         1
                             52 POP_TOP
                
-               692          54 LOAD_FAST                0 (self)
+               697          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (sent)
                             66 POP_JUMP_FORWARD_IF_TRUE    75 (to 218)
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                3 (send_at)
                             80 LOAD_GLOBAL              9 (NULL + timezone)
                             92 LOAD_ATTR                5 (now)
                            102 PRECALL                  0
                            106 CALL                     0
                            116 COMPARE_OP               1 (<=)
                            122 POP_JUMP_FORWARD_IF_FALSE    49 (to 222)
                
-               693         124 LOAD_FAST                0 (self)
+               698         124 LOAD_FAST                0 (self)
                            126 LOAD_METHOD              6 (send)
                            148 PRECALL                  0
                            152 CALL                     0
                            162 POP_TOP
                
-               694         164 PUSH_NULL
+               699         164 PUSH_NULL
                            166 LOAD_GLOBAL              1 (NULL + super)
                            178 PRECALL                  0
                            182 CALL                     0
                            192 LOAD_ATTR                1 (save)
                            202 LOAD_CONST               1 (())
                            204 BUILD_MAP                0
                            206 LOAD_FAST                1 (kwargs)
                            208 DICT_MERGE               1
                            210 CALL_FUNCTION_EX         1
                            212 POP_TOP
                            214 LOAD_CONST               0 (None)
                            216 RETURN_VALUE
                
-               692     >>  218 LOAD_CONST               0 (None)
+               697     >>  218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                        >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   ()
                names      ('super', 'save', 'sent', 'send_at', 'timezone', 'now', 'send')
                varnames   ('self', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'save'
-               firstlineno 690
+               firstlineno 695
                lnotab 0x040132014601280136fe
             'resend'
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000072027c01721b740300000000000000
                   0000006a0200000000000000007c006a0300000000000000007c01ac01a6
                   020000ab020000000000000000530064025300
-               696           0 RESUME                   0
+               701           0 RESUME                   0
                
-               698           2 LOAD_FAST                0 (self)
+               703           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sent)
                             14 POP_JUMP_FORWARD_IF_FALSE     2 (to 20)
                             16 LOAD_FAST                1 (resend)
                             18 POP_JUMP_FORWARD_IF_FALSE    27 (to 74)
                
-               699     >>   20 LOAD_GLOBAL              3 (NULL + send_notification)
+               704     >>   20 LOAD_GLOBAL              3 (NULL + send_notification)
                             32 LOAD_ATTR                2 (delay)
                             42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                3 (pk)
                             54 LOAD_FAST                1 (resend)
                             56 KW_NAMES                 1
                             58 PRECALL                  2
                             62 CALL                     2
                             72 RETURN_VALUE
                
-               698     >>   74 LOAD_CONST               2 (None)
+               703     >>   74 LOAD_CONST               2 (None)
                             76 RETURN_VALUE
                consts
                   'Send the notification to the recipient.'
                   ('resend',)
                   None
                names      ('sent', 'send_notification', 'delay', 'pk')
                varnames   ('self', 'resend')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'send'
-               firstlineno 696
+               firstlineno 701
                lnotab 0x0202120136ff
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               701           0 RESUME                   0
+               706           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Notification.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               702          10 PUSH_NULL
+               707          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Notification')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               703          32 PUSH_NULL
+               708          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Notifications')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -5535,25 +5550,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 701
+               firstlineno 706
                lnotab 0x0a011601
             'Meta'
             (False,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'CharField', '_', 'sender', 'ForeignKey', 'CASCADE', 'recipient', 'title', 'TextField', 'description', 'URLField', 'link', 'ICONS', 'icon', 'DateTimeField', 'timezone', 'now', 'send_at', 'BooleanField', 'read', 'sent', '__str__', 'save', 'bool', 'Optional', 'AsyncResult', 'send', 'Meta', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'Notification'
-         firstlineno 663
+         firstlineno 668
          lnotab
             0x0c01040236010e0102010c01020114fc12073601360136020e011aff12
             0440023601360206030a061e05
       'Notification'
       code
          argcount  : 0
          nlocals   : 0
@@ -5563,83 +5578,83 @@
             0x970065005a0164005a0264015a036402650465056a0600000000000000
             0065056a070000000000000000660219000000000000000000640365056a
             0700000000000000006604640484045a08640e64066509650a1900000000
             0000000000640365056a0700000000000000006604640784055a0b640e64
             066509650c19000000000000000000640365056a07000000000000000066
             04640884055a0d6409650c640a650c640365056a07000000000000000066
             06640b84045a0e640c650f640365106604640d84045a1164055300
-         706           0 RESUME                   0
+         711           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AnnouncementQuerySet')
                        8 STORE_NAME               2 (__qualname__)
          
-         707          10 LOAD_CONST               1 ('Queryset for announcements providing time-based utility functions.')
+         712          10 LOAD_CONST               1 ('Queryset for announcements providing time-based utility functions.')
                       12 STORE_NAME               3 (__doc__)
          
-         709          14 LOAD_CONST               2 ('obj')
+         714          14 LOAD_CONST               2 ('obj')
                       16 LOAD_NAME                4 (Union)
                       18 LOAD_NAME                5 (models)
                       20 LOAD_ATTR                6 (Model)
                       30 LOAD_NAME                5 (models)
                       32 LOAD_ATTR                7 (QuerySet)
                       42 BUILD_TUPLE              2
                       44 BINARY_SUBSCR
                       54 LOAD_CONST               3 ('return')
                       56 LOAD_NAME                5 (models)
                       58 LOAD_ATTR                7 (QuerySet)
                       68 BUILD_TUPLE              4
-                      70 LOAD_CONST               4 (<code object relevant_for, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 709>)
+                      70 LOAD_CONST               4 (<code object relevant_for, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 714>)
                       72 MAKE_FUNCTION            4 (annotations)
                       74 STORE_NAME               8 (relevant_for)
          
-         724          76 LOAD_CONST              14 ((None,))
+         729          76 LOAD_CONST              14 ((None,))
                       78 LOAD_CONST               6 ('when')
                       80 LOAD_NAME                9 (Optional)
                       82 LOAD_NAME               10 (datetime)
                       84 BINARY_SUBSCR
                       94 LOAD_CONST               3 ('return')
                       96 LOAD_NAME                5 (models)
                       98 LOAD_ATTR                7 (QuerySet)
                      108 BUILD_TUPLE              4
-                     110 LOAD_CONST               7 (<code object at_time, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 724>)
+                     110 LOAD_CONST               7 (<code object at_time, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 729>)
                      112 MAKE_FUNCTION            5 (defaults, annotations)
                      114 STORE_NAME              11 (at_time)
          
-         733         116 LOAD_CONST              14 ((None,))
+         738         116 LOAD_CONST              14 ((None,))
                      118 LOAD_CONST               6 ('when')
                      120 LOAD_NAME                9 (Optional)
                      122 LOAD_NAME               12 (date)
                      124 BINARY_SUBSCR
                      134 LOAD_CONST               3 ('return')
                      136 LOAD_NAME                5 (models)
                      138 LOAD_ATTR                7 (QuerySet)
                      148 BUILD_TUPLE              4
-                     150 LOAD_CONST               8 (<code object on_date, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 733>)
+                     150 LOAD_CONST               8 (<code object on_date, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 738>)
                      152 MAKE_FUNCTION            5 (defaults, annotations)
                      154 STORE_NAME              13 (on_date)
          
-         742         156 LOAD_CONST               9 ('start')
+         747         156 LOAD_CONST               9 ('start')
                      158 LOAD_NAME               12 (date)
                      160 LOAD_CONST              10 ('stop')
                      162 LOAD_NAME               12 (date)
                      164 LOAD_CONST               3 ('return')
                      166 LOAD_NAME                5 (models)
                      168 LOAD_ATTR                7 (QuerySet)
                      178 BUILD_TUPLE              6
-                     180 LOAD_CONST              11 (<code object within_days, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 742>)
+                     180 LOAD_CONST              11 (<code object within_days, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 747>)
                      182 MAKE_FUNCTION            4 (annotations)
                      184 STORE_NAME              14 (within_days)
          
-         749         186 LOAD_CONST              12 ('person')
+         754         186 LOAD_CONST              12 ('person')
                      188 LOAD_NAME               15 (Person)
                      190 LOAD_CONST               3 ('return')
                      192 LOAD_NAME               16 (List)
                      194 BUILD_TUPLE              4
-                     196 LOAD_CONST              13 (<code object for_person, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 749>)
+                     196 LOAD_CONST              13 (<code object for_person, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 754>)
                      198 MAKE_FUNCTION            4 (annotations)
                      200 STORE_NAME              17 (for_person)
                      202 LOAD_CONST               5 (None)
                      204 RETURN_VALUE
          consts
             'AnnouncementQuerySet'
             'Queryset for announcements providing time-based utility functions.'
@@ -5658,60 +5673,60 @@
                   00000000007d02740f000000000000000000007c01a00800000000000000
                   0000000000000000000000000064016402ac03a6020000ab020000000000
                   000000a6010000ab0100000000000000007d036e27740600000000000000
                   0000006a040000000000000000a005000000000000000000000000000000
                   00000000007c01a6010000ab0100000000000000007d027c016a09000000
                   000000000067017d037c00a00a0000000000000000000000000000000000
                   0000007c027c03ac04a6020000ab0200000000000000005300
-               709           0 RESUME                   0
+               714           0 RESUME                   0
                
-               715           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               720           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                1 (obj)
                             16 LOAD_GLOBAL              2 (models)
                             28 LOAD_ATTR                2 (QuerySet)
                             38 PRECALL                  2
                             42 CALL                     2
                             52 POP_JUMP_FORWARD_IF_FALSE    73 (to 200)
                
-               716          54 LOAD_GLOBAL              6 (ContentType)
+               721          54 LOAD_GLOBAL              6 (ContentType)
                             66 LOAD_ATTR                4 (objects)
                             76 LOAD_METHOD              5 (get_for_model)
                             98 LOAD_FAST                1 (obj)
                            100 LOAD_ATTR                6 (model)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               2 (ct)
                
-               717         126 LOAD_GLOBAL             15 (NULL + list)
+               722         126 LOAD_GLOBAL             15 (NULL + list)
                            138 LOAD_FAST                1 (obj)
                            140 LOAD_METHOD              8 (values_list)
                            162 LOAD_CONST               1 ('pk')
                            164 LOAD_CONST               2 (True)
                            166 KW_NAMES                 3
                            168 PRECALL                  2
                            172 CALL                     2
                            182 PRECALL                  1
                            186 CALL                     1
                            196 STORE_FAST               3 (pks)
                            198 JUMP_FORWARD            39 (to 278)
                
-               719     >>  200 LOAD_GLOBAL              6 (ContentType)
+               724     >>  200 LOAD_GLOBAL              6 (ContentType)
                            212 LOAD_ATTR                4 (objects)
                            222 LOAD_METHOD              5 (get_for_model)
                            244 LOAD_FAST                1 (obj)
                            246 PRECALL                  1
                            250 CALL                     1
                            260 STORE_FAST               2 (ct)
                
-               720         262 LOAD_FAST                1 (obj)
+               725         262 LOAD_FAST                1 (obj)
                            264 LOAD_ATTR                9 (pk)
                            274 BUILD_LIST               1
                            276 STORE_FAST               3 (pks)
                
-               722     >>  278 LOAD_FAST                0 (self)
+               727     >>  278 LOAD_FAST                0 (self)
                            280 LOAD_METHOD             10 (filter)
                            302 LOAD_FAST                2 (ct)
                            304 LOAD_FAST                3 (pks)
                            306 KW_NAMES                 4
                            308 PRECALL                  2
                            312 CALL                     2
                            322 RETURN_VALUE
@@ -5723,194 +5738,194 @@
                   ('recipients__content_type', 'recipients__recipient_id__in')
                names      ('isinstance', 'models', 'QuerySet', 'ContentType', 'objects', 'get_for_model', 'model', 'list', 'values_list', 'pk', 'filter')
                varnames   ('self', 'obj', 'ct', 'pks')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'relevant_for'
-               firstlineno 709
+               firstlineno 714
                lnotab 0x0206340148014a023e011002
             None
             'when'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c0170127401000000000000000000006a010000000000000000a6
                   000000ab0000000000000000007d017c00a0020000000000000000000000
                   0000000000000000007c017c01ac01a6020000ab0200000000000000007d
                   027c025300
-               724           0 RESUME                   0
+               729           0 RESUME                   0
                
-               726           2 LOAD_FAST                1 (when)
+               731           2 LOAD_FAST                1 (when)
                              4 JUMP_IF_TRUE_OR_POP     18 (to 42)
                              6 LOAD_GLOBAL              1 (NULL + timezone)
                             18 LOAD_ATTR                1 (now)
                             28 PRECALL                  0
                             32 CALL                     0
                        >>   42 STORE_FAST               1 (when)
                
-               729          44 LOAD_FAST                0 (self)
+               734          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              2 (filter)
                             68 LOAD_FAST                1 (when)
                             70 LOAD_FAST                1 (when)
                             72 KW_NAMES                 1
                             74 PRECALL                  2
                             78 CALL                     2
                             88 STORE_FAST               2 (announcements)
                
-               731          90 LOAD_FAST                2 (announcements)
+               736          90 LOAD_FAST                2 (announcements)
                             92 RETURN_VALUE
                consts
                   'Get all announcements at a certain time.'
                   ('valid_from__lte', 'valid_until__gte')
                names      ('timezone', 'now', 'filter')
                varnames   ('self', 'when', 'announcements')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'at_time'
-               firstlineno 724
+               firstlineno 729
                lnotab 0x02022a032e02
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c0170247401000000000000000000006a010000000000000000a6
                   000000ab000000000000000000a002000000000000000000000000000000
                   0000000000a6000000ab0000000000000000007d017c00a0030000000000
                   0000000000000000000000000000007c017c01ac01a6020000ab02000000
                   00000000007d027c025300
-               733           0 RESUME                   0
+               738           0 RESUME                   0
                
-               735           2 LOAD_FAST                1 (when)
+               740           2 LOAD_FAST                1 (when)
                              4 JUMP_IF_TRUE_OR_POP     36 (to 78)
                              6 LOAD_GLOBAL              1 (NULL + timezone)
                             18 LOAD_ATTR                1 (now)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 LOAD_METHOD              2 (date)
                             64 PRECALL                  0
                             68 CALL                     0
                        >>   78 STORE_FAST               1 (when)
                
-               738          80 LOAD_FAST                0 (self)
+               743          80 LOAD_FAST                0 (self)
                             82 LOAD_METHOD              3 (filter)
                            104 LOAD_FAST                1 (when)
                            106 LOAD_FAST                1 (when)
                            108 KW_NAMES                 1
                            110 PRECALL                  2
                            114 CALL                     2
                            124 STORE_FAST               2 (announcements)
                
-               740         126 LOAD_FAST                2 (announcements)
+               745         126 LOAD_FAST                2 (announcements)
                            128 RETURN_VALUE
                consts
                   'Get all announcements at a certain date.'
                   ('valid_from__date__lte', 'valid_until__date__gte')
                names      ('timezone', 'now', 'date', 'filter')
                varnames   ('self', 'when', 'announcements')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'on_date'
-               firstlineno 733
+               firstlineno 738
                lnotab 0x02024e032e02
             'start'
             'stop'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c027c
                   01ac01a6020000ab0200000000000000007d037c035300
-               742           0 RESUME                   0
+               747           0 RESUME                   0
                
-               745           2 LOAD_FAST                0 (self)
+               750           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (filter)
                             26 LOAD_FAST                2 (stop)
                             28 LOAD_FAST                1 (start)
                             30 KW_NAMES                 1
                             32 PRECALL                  2
                             36 CALL                     2
                             46 STORE_FAST               3 (announcements)
                
-               747          48 LOAD_FAST                3 (announcements)
+               752          48 LOAD_FAST                3 (announcements)
                             50 RETURN_VALUE
                consts
                   'Get all announcements valid for a set of days.'
                   ('valid_from__date__lte', 'valid_until__date__gte')
                names      ('filter',)
                varnames   ('self', 'start', 'stop', 'announcements')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'within_days'
-               firstlineno 742
+               firstlineno 747
                lnotab 0x02032e02
             'person'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x970067007d027c0044005d207d037c017c036a00000000000000000076
                   0072157c02a00100000000000000000000000000000000000000007c03a6
                   010000ab01000000000000000001008c217c025300
-               749           0 RESUME                   0
+               754           0 RESUME                   0
                
-               752           2 BUILD_LIST               0
+               757           2 BUILD_LIST               0
                              4 STORE_FAST               2 (announcements_for_person)
                
-               753           6 LOAD_FAST                0 (self)
+               758           6 LOAD_FAST                0 (self)
                              8 GET_ITER
                        >>   10 FOR_ITER                32 (to 76)
                             12 STORE_FAST               3 (announcement)
                
-               754          14 LOAD_FAST                1 (person)
+               759          14 LOAD_FAST                1 (person)
                             16 LOAD_FAST                3 (announcement)
                             18 LOAD_ATTR                0 (recipient_persons)
                             28 CONTAINS_OP              0
                             30 POP_JUMP_FORWARD_IF_FALSE    21 (to 74)
                
-               755          32 LOAD_FAST                2 (announcements_for_person)
+               760          32 LOAD_FAST                2 (announcements_for_person)
                             34 LOAD_METHOD              1 (append)
                             56 LOAD_FAST                3 (announcement)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                        >>   74 JUMP_BACKWARD           33 (to 10)
                
-               757     >>   76 LOAD_FAST                2 (announcements_for_person)
+               762     >>   76 LOAD_FAST                2 (announcements_for_person)
                             78 RETURN_VALUE
                consts
                   'Get all announcements for one person.'
                names      ('recipient_persons', 'append')
                varnames   ('self', 'person', 'announcements_for_person', 'announcement')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'for_person'
-               firstlineno 749
+               firstlineno 754
                lnotab 0x02030401080112012c02
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Union', 'models', 'Model', 'QuerySet', 'relevant_for', 'Optional', 'datetime', 'at_time', 'date', 'on_date', 'within_days', 'Person', 'List', 'for_person')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'AnnouncementQuerySet'
-         firstlineno 706
+         firstlineno 711
          lnotab 0x0a0104023e0f280928091e07
       'AnnouncementQuerySet'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
@@ -5928,148 +5943,148 @@
             0200000000000000005a13020065046a1000000000000000000200650a64
             0da6010000ab0100000000000000006514ac0ca6020000ab020000000000
             0000005a156516640e65176518190000000000000000006602640f8404a6
             000000ab0000000000000000005a196410651a65046a1b00000000000000
             0019000000000000000000640e651765046a1b0000000000000000190000
             000000000000006604641184045a1c641284005a1d020047006413840064
             14a6020000ab0200000000000000005a1e64155300
-         760           0 RESUME                   0
+         765           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Announcement')
                        8 STORE_NAME               2 (__qualname__)
          
-         761          10 LOAD_CONST               1 ('Announcement model.\n\n    Persistent announcement to display to groups or persons in various places during a\n    specific time range.\n    ')
+         766          10 LOAD_CONST               1 ('Announcement model.\n\n    Persistent announcement to display to groups or persons in various places during a\n    specific time range.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         767          14 PUSH_NULL
+         772          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (Manager)
                       28 LOAD_METHOD              6 (from_queryset)
                       50 LOAD_NAME                7 (AnnouncementQuerySet)
                       52 PRECALL                  1
                       56 CALL                     1
                       66 PRECALL                  0
                       70 CALL                     0
                       80 STORE_NAME               8 (objects)
          
-         769          82 PUSH_NULL
+         774          82 PUSH_NULL
                       84 LOAD_NAME                4 (models)
                       86 LOAD_ATTR                9 (CharField)
                       96 LOAD_CONST               2 (150)
                       98 PUSH_NULL
                      100 LOAD_NAME               10 (_)
                      102 LOAD_CONST               3 ('Title')
                      104 PRECALL                  1
                      108 CALL                     1
                      118 KW_NAMES                 4
                      120 PRECALL                  2
                      124 CALL                     2
                      134 STORE_NAME              11 (title)
          
-         770         136 PUSH_NULL
+         775         136 PUSH_NULL
                      138 LOAD_NAME                4 (models)
                      140 LOAD_ATTR               12 (TextField)
                      150 LOAD_CONST               5 (500)
                      152 PUSH_NULL
                      154 LOAD_NAME               10 (_)
                      156 LOAD_CONST               6 ('Description')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 LOAD_CONST               7 (True)
                      174 KW_NAMES                 8
                      176 PRECALL                  3
                      180 CALL                     3
                      190 STORE_NAME              13 (description)
          
-         771         192 PUSH_NULL
+         776         192 PUSH_NULL
                      194 LOAD_NAME                4 (models)
                      196 LOAD_ATTR               14 (URLField)
                      206 LOAD_CONST               7 (True)
                      208 PUSH_NULL
                      210 LOAD_NAME               10 (_)
                      212 LOAD_CONST               9 ('Link to detailed view')
                      214 PRECALL                  1
                      218 CALL                     1
                      228 KW_NAMES                10
                      230 PRECALL                  2
                      234 CALL                     2
                      244 STORE_NAME              15 (link)
          
-         773         246 PUSH_NULL
+         778         246 PUSH_NULL
                      248 LOAD_NAME                4 (models)
                      250 LOAD_ATTR               16 (DateTimeField)
          
-         774         260 PUSH_NULL
+         779         260 PUSH_NULL
                      262 LOAD_NAME               10 (_)
                      264 LOAD_CONST              11 ('Date and time from when to show')
                      266 PRECALL                  1
                      270 CALL                     1
                      280 LOAD_NAME               17 (timezone)
                      282 LOAD_ATTR               18 (now)
          
-         773         292 KW_NAMES                12
+         778         292 KW_NAMES                12
                      294 PRECALL                  2
                      298 CALL                     2
                      308 STORE_NAME              19 (valid_from)
          
-         776         310 PUSH_NULL
+         781         310 PUSH_NULL
                      312 LOAD_NAME                4 (models)
                      314 LOAD_ATTR               16 (DateTimeField)
          
-         777         324 PUSH_NULL
+         782         324 PUSH_NULL
                      326 LOAD_NAME               10 (_)
                      328 LOAD_CONST              13 ('Date and time until when to show')
                      330 PRECALL                  1
                      334 CALL                     1
          
-         778         344 LOAD_NAME               20 (now_tomorrow)
+         783         344 LOAD_NAME               20 (now_tomorrow)
          
-         776         346 KW_NAMES                12
+         781         346 KW_NAMES                12
                      348 PRECALL                  2
                      352 CALL                     2
                      362 STORE_NAME              21 (valid_until)
          
-         781         364 LOAD_NAME               22 (property)
+         786         364 LOAD_NAME               22 (property)
          
-         782         366 LOAD_CONST              14 ('return')
+         787         366 LOAD_CONST              14 ('return')
                      368 LOAD_NAME               23 (Sequence)
                      370 LOAD_NAME               24 (Person)
                      372 BINARY_SUBSCR
                      382 BUILD_TUPLE              2
-                     384 LOAD_CONST              15 (<code object recipient_persons, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 781>)
+                     384 LOAD_CONST              15 (<code object recipient_persons, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 786>)
                      386 MAKE_FUNCTION            4 (annotations)
          
-         781         388 PRECALL                  0
+         786         388 PRECALL                  0
                      392 CALL                     0
          
-         782         402 STORE_NAME              25 (recipient_persons)
+         787         402 STORE_NAME              25 (recipient_persons)
          
-         789         404 LOAD_CONST              16 ('obj')
+         794         404 LOAD_CONST              16 ('obj')
                      406 LOAD_NAME               26 (Union)
                      408 LOAD_NAME                4 (models)
                      410 LOAD_ATTR               27 (Model)
                      420 BINARY_SUBSCR
                      430 LOAD_CONST              14 ('return')
                      432 LOAD_NAME               23 (Sequence)
                      434 LOAD_NAME                4 (models)
                      436 LOAD_ATTR               27 (Model)
                      446 BINARY_SUBSCR
                      456 BUILD_TUPLE              4
-                     458 LOAD_CONST              17 (<code object get_recipients_for_model, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 789>)
+                     458 LOAD_CONST              17 (<code object get_recipients_for_model, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 794>)
                      460 MAKE_FUNCTION            4 (annotations)
                      462 STORE_NAME              28 (get_recipients_for_model)
          
-         798         464 LOAD_CONST              18 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 798>)
+         803         464 LOAD_CONST              18 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 803>)
                      466 MAKE_FUNCTION            0
                      468 STORE_NAME              29 (__str__)
          
-         801         470 PUSH_NULL
+         806         470 PUSH_NULL
                      472 LOAD_BUILD_CLASS
-                     474 LOAD_CONST              19 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 801>)
+                     474 LOAD_CONST              19 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 806>)
                      476 MAKE_FUNCTION            0
                      478 LOAD_CONST              20 ('Meta')
                      480 PRECALL                  2
                      484 CALL                     2
                      494 STORE_NAME              30 (Meta)
                      496 LOAD_CONST              21 (None)
                      498 RETURN_VALUE
@@ -6094,70 +6109,70 @@
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x970067007d017c006a000000000000000000a001000000000000000000
                   0000000000000000000000a6000000ab00000000000000000044005d0c7d
                   027c017c026a0200000000000000007a0d00007d018c0d7c015300
-               781           0 RESUME                   0
+               786           0 RESUME                   0
                
-               784           2 BUILD_LIST               0
+               789           2 BUILD_LIST               0
                              4 STORE_FAST               1 (persons)
                
-               785           6 LOAD_FAST                0 (self)
+               790           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (recipients)
                             18 LOAD_METHOD              1 (all)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 GET_ITER
                        >>   56 FOR_ITER                12 (to 82)
                             58 STORE_FAST               2 (recipient)
                
-               786          60 LOAD_FAST                1 (persons)
+               791          60 LOAD_FAST                1 (persons)
                             62 LOAD_FAST                2 (recipient)
                             64 LOAD_ATTR                2 (persons)
                             74 BINARY_OP               13 (+=)
                             78 STORE_FAST               1 (persons)
                             80 JUMP_BACKWARD           13 (to 56)
                
-               787     >>   82 LOAD_FAST                1 (persons)
+               792     >>   82 LOAD_FAST                1 (persons)
                             84 RETURN_VALUE
                consts
                   'Return a list of Persons this announcement is relevant for.'
                names      ('recipients', 'all', 'persons')
                varnames   ('self', 'persons', 'recipient')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'recipient_persons'
-               firstlineno 781
+               firstlineno 786
                lnotab 0x0203040136011601
             'obj'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c01a6010000ab010000000000
                   0000007d02640184007c006a030000000000000000a00400000000000000
                   000000000000000000000000007c02ac02a6010000ab0100000000000000
                   004400a6000000ab0000000000000000005300
-               789           0 RESUME                   0
+               794           0 RESUME                   0
                
-               795           2 LOAD_GLOBAL              0 (ContentType)
+               800           2 LOAD_GLOBAL              0 (ContentType)
                             14 LOAD_ATTR                1 (objects)
                             24 LOAD_METHOD              2 (get_for_model)
                             46 LOAD_FAST                1 (obj)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               2 (ct)
                
-               796          64 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 796>)
+               801          64 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 801>)
                             66 MAKE_FUNCTION            0
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                3 (recipients)
                             80 LOAD_METHOD              4 (filter)
                            102 LOAD_FAST                2 (ct)
                            104 KW_NAMES                 2
                            106 PRECALL                  1
@@ -6170,15 +6185,15 @@
                   'Get all recipients.\n\n        Get all recipients for this announcement\n        with a special content type (provided through model)\n        '
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     796           0 RESUME                   0
+                     801           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (r)
                                   10 LOAD_FAST                1 (r)
                                   12 LOAD_ATTR                0 (recipient)
                                   22 LIST_APPEND              2
@@ -6187,68 +6202,68 @@
                      consts
                      names      ('recipient',)
                      varnames   ('.0', 'r')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 796
+                     firstlineno 801
                      lnotab 0x
                   ('content_type',)
                names      ('ContentType', 'objects', 'get_for_model', 'recipients', 'filter')
                varnames   ('self', 'obj', 'ct')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_recipients_for_model'
-               firstlineno 789
+               firstlineno 794
                lnotab 0x02063e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               798           0 RESUME                   0
+               803           0 RESUME                   0
                
-               799           2 LOAD_FAST                0 (self)
+               804           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 798
+               firstlineno 803
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               801           0 RESUME                   0
+               806           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Announcement.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               802          10 PUSH_NULL
+               807          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Announcement')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               803          32 PUSH_NULL
+               808          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Announcements')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -6259,25 +6274,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 801
+               firstlineno 806
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'Manager', 'from_queryset', 'AnnouncementQuerySet', 'objects', 'CharField', '_', 'title', 'TextField', 'description', 'URLField', 'link', 'DateTimeField', 'timezone', 'now', 'valid_from', 'now_tomorrow', 'valid_until', 'property', 'Sequence', 'Person', 'recipient_persons', 'Union', 'Model', 'get_recipients_for_model', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'Announcement'
-         firstlineno 760
+         firstlineno 765
          lnotab
             0x0a01040644023601380136020e0120ff12030e01140102fe1205020116
             ff0e0102073c090603
       'Announcement'
       code
          argcount  : 0
          nlocals   : 0
@@ -6288,85 +6303,85 @@
             0665046a0700000000000000006402ac03a6030000ab0300000000000000
             005a08020065046a050000000000000000650965046a0700000000000000
             00ac04a6020000ab0200000000000000005a0a020065046a0b0000000000
             000000a6000000ab0000000000000000005a0c0200650d64056406a60200
             00ab0200000000000000005a0e650f640765106511190000000000000000
             00660264088404a6000000ab0000000000000000005a12640984005a1302
             004700640a8400640ba6020000ab0200000000000000005a14640c5300
-         806           0 RESUME                   0
+         811           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AnnouncementRecipient')
                        8 STORE_NAME               2 (__qualname__)
          
-         807          10 LOAD_CONST               1 ('Announcement recipient model.\n\n    Generalisation of a recipient for an announcement, used to wrap arbitrary\n    objects that can receive announcements.\n\n    Contract: Objects to serve as recipient have a property announcement_recipients\n    returning a flat list of Person objects.\n    ')
+         812          10 LOAD_CONST               1 ('Announcement recipient model.\n\n    Generalisation of a recipient for an announcement, used to wrap arbitrary\n    objects that can receive announcements.\n\n    Contract: Objects to serve as recipient have a property announcement_recipients\n    returning a flat list of Person objects.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         816          14 PUSH_NULL
+         821          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (ForeignKey)
          
-         817          28 LOAD_NAME                6 (Announcement)
+         822          28 LOAD_NAME                6 (Announcement)
                       30 LOAD_NAME                4 (models)
                       32 LOAD_ATTR                7 (CASCADE)
                       42 LOAD_CONST               2 ('recipients')
          
-         816          44 KW_NAMES                 3
+         821          44 KW_NAMES                 3
                       46 PRECALL                  3
                       50 CALL                     3
                       60 STORE_NAME               8 (announcement)
          
-         820          62 PUSH_NULL
+         825          62 PUSH_NULL
                       64 LOAD_NAME                4 (models)
                       66 LOAD_ATTR                5 (ForeignKey)
                       76 LOAD_NAME                9 (ContentType)
                       78 LOAD_NAME                4 (models)
                       80 LOAD_ATTR                7 (CASCADE)
                       90 KW_NAMES                 4
                       92 PRECALL                  2
                       96 CALL                     2
                      106 STORE_NAME              10 (content_type)
          
-         821         108 PUSH_NULL
+         826         108 PUSH_NULL
                      110 LOAD_NAME                4 (models)
                      112 LOAD_ATTR               11 (PositiveIntegerField)
                      122 PRECALL                  0
                      126 CALL                     0
                      136 STORE_NAME              12 (recipient_id)
          
-         822         138 PUSH_NULL
+         827         138 PUSH_NULL
                      140 LOAD_NAME               13 (GenericForeignKey)
                      142 LOAD_CONST               5 ('content_type')
                      144 LOAD_CONST               6 ('recipient_id')
                      146 PRECALL                  2
                      150 CALL                     2
                      160 STORE_NAME              14 (recipient)
          
-         824         162 LOAD_NAME               15 (property)
+         829         162 LOAD_NAME               15 (property)
          
-         825         164 LOAD_CONST               7 ('return')
+         830         164 LOAD_CONST               7 ('return')
                      166 LOAD_NAME               16 (Sequence)
                      168 LOAD_NAME               17 (Person)
                      170 BINARY_SUBSCR
                      180 BUILD_TUPLE              2
-                     182 LOAD_CONST               8 (<code object persons, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 824>)
+                     182 LOAD_CONST               8 (<code object persons, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 829>)
                      184 MAKE_FUNCTION            4 (annotations)
          
-         824         186 PRECALL                  0
+         829         186 PRECALL                  0
                      190 CALL                     0
          
-         825         200 STORE_NAME              18 (persons)
+         830         200 STORE_NAME              18 (persons)
          
-         836         202 LOAD_CONST               9 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 836>)
+         841         202 LOAD_CONST               9 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 841>)
                      204 MAKE_FUNCTION            0
                      206 STORE_NAME              19 (__str__)
          
-         839         208 PUSH_NULL
+         844         208 PUSH_NULL
                      210 LOAD_BUILD_CLASS
-                     212 LOAD_CONST              10 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 839>)
+                     212 LOAD_CONST              10 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 844>)
                      214 MAKE_FUNCTION            0
                      216 LOAD_CONST              11 ('Meta')
                      218 PRECALL                  2
                      222 CALL                     2
                      232 STORE_NAME              20 (Meta)
                      234 LOAD_CONST              12 (None)
                      236 RETURN_VALUE
@@ -6385,30 +6400,30 @@
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000740400
                   000000000000000000a6020000ab02000000000000000072087c006a0100
                   00000000000000670153007407000000000000000000007c006a01000000
                   000000000064016700a6030000ab0300000000000000005300
-               824           0 RESUME                   0
+               829           0 RESUME                   0
                
-               831           2 LOAD_GLOBAL              1 (NULL + isinstance)
+               836           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (recipient)
                             26 LOAD_GLOBAL              4 (Person)
                             38 PRECALL                  2
                             42 CALL                     2
                             52 POP_JUMP_FORWARD_IF_FALSE     8 (to 70)
                
-               832          54 LOAD_FAST                0 (self)
+               837          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                1 (recipient)
                             66 BUILD_LIST               1
                             68 RETURN_VALUE
                
-               834     >>   70 LOAD_GLOBAL              7 (NULL + getattr)
+               839     >>   70 LOAD_GLOBAL              7 (NULL + getattr)
                             82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                1 (recipient)
                             94 LOAD_CONST               1 ('announcement_recipients')
                             96 BUILD_LIST               0
                             98 PRECALL                  3
                            102 CALL                     3
                            112 RETURN_VALUE
@@ -6417,64 +6432,64 @@
                   'announcement_recipients'
                names      ('isinstance', 'recipient', 'Person', 'getattr')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'persons'
-               firstlineno 824
+               firstlineno 829
                lnotab 0x020734011002
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-               836           0 RESUME                   0
+               841           0 RESUME                   0
                
-               837           2 LOAD_GLOBAL              1 (NULL + str)
+               842           2 LOAD_GLOBAL              1 (NULL + str)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (recipient)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('str', 'recipient')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 836
+               firstlineno 841
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               839           0 RESUME                   0
+               844           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('AnnouncementRecipient.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               840          10 PUSH_NULL
+               845          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Announcement recipient')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               841          32 PUSH_NULL
+               846          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Announcement recipients')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -6485,25 +6500,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 839
+               firstlineno 844
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'Announcement', 'CASCADE', 'announcement', 'ContentType', 'content_type', 'PositiveIntegerField', 'recipient_id', 'GenericForeignKey', 'recipient', 'property', 'Sequence', 'Person', 'persons', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'AnnouncementRecipient'
-         firstlineno 806
+         firstlineno 811
          lnotab 0x0a0104090e0110ff12042e011e011802020116ff0e01020b0603
       'AnnouncementRecipient'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
@@ -6528,238 +6543,238 @@
             000000020065176410a6010000ab01000000000000000067016416ac11a6
             040000ab0400000000000000005a1a0200650f6a16000000000000000002
             0065116417a6010000ab010000000000000000020065116418a6010000ab
             010000000000000000020065176410a6010000ab01000000000000000067
             016419ac11a6040000ab0400000000000000005a1b641a84005a1c641b84
             005a1d641c84005a1e641d84005a1f02004700641e8400641fa6020000ab
             0200000000000000005a2064045300
-         844           0 RESUME                   0
+         849           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DashboardWidget')
                        8 STORE_NAME               2 (__qualname__)
          
-         845          10 LOAD_CONST               1 ('Base class for dashboard widgets on the index page.')
+         850          10 LOAD_CONST               1 ('Base class for dashboard widgets on the index page.')
                       12 STORE_NAME               3 (__doc__)
          
-         847          14 PUSH_NULL
+         852          14 PUSH_NULL
                       16 LOAD_NAME                4 (UninstallRenitentPolymorphicManager)
                       18 PRECALL                  0
                       22 CALL                     0
                       32 STORE_NAME               5 (objects)
          
-         849          34 LOAD_NAME                6 (staticmethod)
+         854          34 LOAD_NAME                6 (staticmethod)
          
-         850          36 LOAD_CONST               2 ('widgets')
+         855          36 LOAD_CONST               2 ('widgets')
                       38 LOAD_NAME                7 (Union)
                       40 LOAD_NAME                8 (QuerySet)
                       42 LOAD_NAME                9 (Iterable)
                       44 BUILD_TUPLE              2
                       46 BINARY_SUBSCR
                       56 BUILD_TUPLE              2
-                      58 LOAD_CONST               3 (<code object get_media, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 849>)
+                      58 LOAD_CONST               3 (<code object get_media, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 854>)
                       60 MAKE_FUNCTION            4 (annotations)
          
-         849          62 PRECALL                  0
+         854          62 PRECALL                  0
                       66 CALL                     0
          
-         850          76 STORE_NAME              10 (get_media)
+         855          76 STORE_NAME              10 (get_media)
          
-         857          78 LOAD_CONST               4 (None)
+         862          78 LOAD_CONST               4 (None)
                       80 STORE_NAME              11 (template)
          
-         858          82 LOAD_CONST               5 ('core/dashboard_widget/dashboardwidget_broken.html')
+         863          82 LOAD_CONST               5 ('core/dashboard_widget/dashboardwidget_broken.html')
                       84 STORE_NAME              12 (template_broken)
          
-         859          86 PUSH_NULL
+         864          86 PUSH_NULL
                       88 LOAD_NAME               13 (Media)
                       90 PRECALL                  0
                       94 CALL                     0
                      104 STORE_NAME              14 (media)
          
-         861         106 PUSH_NULL
+         866         106 PUSH_NULL
                      108 LOAD_NAME               15 (models)
                      110 LOAD_ATTR               16 (CharField)
                      120 LOAD_CONST               6 (150)
                      122 PUSH_NULL
                      124 LOAD_NAME               17 (_)
                      126 LOAD_CONST               7 ('Widget Title')
                      128 PRECALL                  1
                      132 CALL                     1
                      142 KW_NAMES                 8
                      144 PRECALL                  2
                      148 CALL                     2
                      158 STORE_NAME              18 (title)
          
-         862         160 PUSH_NULL
+         867         160 PUSH_NULL
                      162 LOAD_NAME               15 (models)
                      164 LOAD_ATTR               19 (BooleanField)
                      174 PUSH_NULL
                      176 LOAD_NAME               17 (_)
                      178 LOAD_CONST               9 ('Activate Widget')
                      180 PRECALL                  1
                      184 CALL                     1
                      194 KW_NAMES                10
                      196 PRECALL                  1
                      200 CALL                     1
                      210 STORE_NAME              20 (active)
          
-         863         212 PUSH_NULL
+         868         212 PUSH_NULL
                      214 LOAD_NAME               15 (models)
                      216 LOAD_ATTR               19 (BooleanField)
                      226 PUSH_NULL
                      228 LOAD_NAME               17 (_)
                      230 LOAD_CONST              11 ('Widget is broken')
                      232 PRECALL                  1
                      236 CALL                     1
                      246 LOAD_CONST              12 (False)
                      248 KW_NAMES                13
                      250 PRECALL                  2
                      254 CALL                     2
                      264 STORE_NAME              21 (broken)
          
-         865         266 PUSH_NULL
+         870         266 PUSH_NULL
                      268 LOAD_NAME               15 (models)
                      270 LOAD_ATTR               22 (PositiveSmallIntegerField)
          
-         866         280 PUSH_NULL
+         871         280 PUSH_NULL
                      282 LOAD_NAME               17 (_)
                      284 LOAD_CONST              14 ('Size on mobile devices')
                      286 PRECALL                  1
                      290 CALL                     1
          
-         867         300 PUSH_NULL
+         872         300 PUSH_NULL
                      302 LOAD_NAME               17 (_)
                      304 LOAD_CONST              15 ('<= 600 px, 12 columns')
                      306 PRECALL                  1
                      310 CALL                     1
          
-         868         320 PUSH_NULL
+         873         320 PUSH_NULL
                      322 LOAD_NAME               23 (MaxValueValidator)
                      324 LOAD_CONST              16 (12)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 BUILD_LIST               1
          
-         869         342 LOAD_CONST              16 (12)
+         874         342 LOAD_CONST              16 (12)
          
-         865         344 KW_NAMES                17
+         870         344 KW_NAMES                17
                      346 PRECALL                  4
                      350 CALL                     4
                      360 STORE_NAME              24 (size_s)
          
-         871         362 PUSH_NULL
+         876         362 PUSH_NULL
                      364 LOAD_NAME               15 (models)
                      366 LOAD_ATTR               22 (PositiveSmallIntegerField)
          
-         872         376 PUSH_NULL
+         877         376 PUSH_NULL
                      378 LOAD_NAME               17 (_)
                      380 LOAD_CONST              18 ('Size on tablet devices')
                      382 PRECALL                  1
                      386 CALL                     1
          
-         873         396 PUSH_NULL
+         878         396 PUSH_NULL
                      398 LOAD_NAME               17 (_)
                      400 LOAD_CONST              19 ('> 600 px, 12 columns')
                      402 PRECALL                  1
                      406 CALL                     1
          
-         874         416 PUSH_NULL
+         879         416 PUSH_NULL
                      418 LOAD_NAME               23 (MaxValueValidator)
                      420 LOAD_CONST              16 (12)
                      422 PRECALL                  1
                      426 CALL                     1
                      436 BUILD_LIST               1
          
-         875         438 LOAD_CONST              16 (12)
+         880         438 LOAD_CONST              16 (12)
          
-         871         440 KW_NAMES                17
+         876         440 KW_NAMES                17
                      442 PRECALL                  4
                      446 CALL                     4
                      456 STORE_NAME              25 (size_m)
          
-         877         458 PUSH_NULL
+         882         458 PUSH_NULL
                      460 LOAD_NAME               15 (models)
                      462 LOAD_ATTR               22 (PositiveSmallIntegerField)
          
-         878         472 PUSH_NULL
+         883         472 PUSH_NULL
                      474 LOAD_NAME               17 (_)
                      476 LOAD_CONST              20 ('Size on desktop devices')
                      478 PRECALL                  1
                      482 CALL                     1
          
-         879         492 PUSH_NULL
+         884         492 PUSH_NULL
                      494 LOAD_NAME               17 (_)
                      496 LOAD_CONST              21 ('> 992 px, 12 columns')
                      498 PRECALL                  1
                      502 CALL                     1
          
-         880         512 PUSH_NULL
+         885         512 PUSH_NULL
                      514 LOAD_NAME               23 (MaxValueValidator)
                      516 LOAD_CONST              16 (12)
                      518 PRECALL                  1
                      522 CALL                     1
                      532 BUILD_LIST               1
          
-         881         534 LOAD_CONST              22 (6)
+         886         534 LOAD_CONST              22 (6)
          
-         877         536 KW_NAMES                17
+         882         536 KW_NAMES                17
                      538 PRECALL                  4
                      542 CALL                     4
                      552 STORE_NAME              26 (size_l)
          
-         883         554 PUSH_NULL
+         888         554 PUSH_NULL
                      556 LOAD_NAME               15 (models)
                      558 LOAD_ATTR               22 (PositiveSmallIntegerField)
          
-         884         568 PUSH_NULL
+         889         568 PUSH_NULL
                      570 LOAD_NAME               17 (_)
                      572 LOAD_CONST              23 ('Size on large desktop devices')
                      574 PRECALL                  1
                      578 CALL                     1
          
-         885         588 PUSH_NULL
+         890         588 PUSH_NULL
                      590 LOAD_NAME               17 (_)
                      592 LOAD_CONST              24 ('> 1200 px>, 12 columns')
                      594 PRECALL                  1
                      598 CALL                     1
          
-         886         608 PUSH_NULL
+         891         608 PUSH_NULL
                      610 LOAD_NAME               23 (MaxValueValidator)
                      612 LOAD_CONST              16 (12)
                      614 PRECALL                  1
                      618 CALL                     1
                      628 BUILD_LIST               1
          
-         887         630 LOAD_CONST              25 (4)
+         892         630 LOAD_CONST              25 (4)
          
-         883         632 KW_NAMES                17
+         888         632 KW_NAMES                17
                      634 PRECALL                  4
                      638 CALL                     4
                      648 STORE_NAME              27 (size_xl)
          
-         890         650 LOAD_CONST              26 (<code object _get_context_safe, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 890>)
+         895         650 LOAD_CONST              26 (<code object _get_context_safe, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 895>)
                      652 MAKE_FUNCTION            0
                      654 STORE_NAME              28 (_get_context_safe)
          
-         895         656 LOAD_CONST              27 (<code object get_context, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 895>)
+         900         656 LOAD_CONST              27 (<code object get_context, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 900>)
                      658 MAKE_FUNCTION            0
                      660 STORE_NAME              29 (get_context)
          
-         899         662 LOAD_CONST              28 (<code object get_template, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 899>)
+         904         662 LOAD_CONST              28 (<code object get_template, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 904>)
                      664 MAKE_FUNCTION            0
                      666 STORE_NAME              30 (get_template)
          
-         912         668 LOAD_CONST              29 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 912>)
+         917         668 LOAD_CONST              29 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 917>)
                      670 MAKE_FUNCTION            0
                      672 STORE_NAME              31 (__str__)
          
-         915         674 PUSH_NULL
+         920         674 PUSH_NULL
                      676 LOAD_BUILD_CLASS
-                     678 LOAD_CONST              30 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 915>)
+                     678 LOAD_CONST              30 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 920>)
                      680 MAKE_FUNCTION            0
                      682 LOAD_CONST              31 ('Meta')
                      684 PRECALL                  2
                      688 CALL                     2
                      698 STORE_NAME              32 (Meta)
                      700 LOAD_CONST               4 (None)
                      702 RETURN_VALUE
@@ -6772,44 +6787,44 @@
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007d
                   017c0044005d0c7d027c017c026a0100000000000000007a0000007d018c
                   0d7c015300
-               849           0 RESUME                   0
+               854           0 RESUME                   0
                
-               852           2 LOAD_GLOBAL              1 (NULL + Media)
+               857           2 LOAD_GLOBAL              1 (NULL + Media)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 STORE_FAST               1 (media)
                
-               853          30 LOAD_FAST                0 (widgets)
+               858          30 LOAD_FAST                0 (widgets)
                             32 GET_ITER
                        >>   34 FOR_ITER                12 (to 60)
                             36 STORE_FAST               2 (widget)
                
-               854          38 LOAD_FAST                1 (media)
+               859          38 LOAD_FAST                1 (media)
                             40 LOAD_FAST                2 (widget)
                             42 LOAD_ATTR                1 (media)
                             52 BINARY_OP                0 (+)
                             56 STORE_FAST               1 (media)
                             58 JUMP_BACKWARD           13 (to 34)
                
-               855     >>   60 LOAD_FAST                1 (media)
+               860     >>   60 LOAD_FAST                1 (media)
                             62 RETURN_VALUE
                consts
                   'Return all media required to render the selected widgets.'
                names      ('Media', 'media')
                varnames   ('widgets', 'media', 'widget')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_media'
-               firstlineno 849
+               firstlineno 854
                lnotab 0x02031c0108011601
             None
             'core/dashboard_widget/dashboardwidget_broken.html'
             150
             'Widget Title'
             ('max_length', 'verbose_name')
             'Activate Widget'
@@ -6834,166 +6849,166 @@
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000720964017c006a0100000000000000
                   00690153007c00a00200000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000005300
-               890           0 RESUME                   0
+               895           0 RESUME                   0
                
-               891           2 LOAD_FAST                0 (self)
+               896           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (broken)
                             14 POP_JUMP_FORWARD_IF_FALSE     9 (to 34)
                
-               892          16 LOAD_CONST               1 ('title')
+               897          16 LOAD_CONST               1 ('title')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (title)
                             30 BUILD_MAP                1
                             32 RETURN_VALUE
                
-               893     >>   34 LOAD_FAST                0 (self)
+               898     >>   34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              2 (get_context)
                             58 LOAD_FAST                1 (request)
                             60 PRECALL                  1
                             64 CALL                     1
                             74 RETURN_VALUE
                consts
                   None
                   'title'
                names      ('broken', 'title', 'get_context')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '_get_context_safe'
-               firstlineno 890
+               firstlineno 895
                lnotab 0x02010e011201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   008201
-               895           0 RESUME                   0
+               900           0 RESUME                   0
                
-               897           2 LOAD_GLOBAL              1 (NULL + NotImplementedError)
+               902           2 LOAD_GLOBAL              1 (NULL + NotImplementedError)
                             14 LOAD_CONST               1 ('A widget subclass needs to implement the get_context method.')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RAISE_VARARGS            1
                consts
                   'Get the context dictionary to pass to the widget template.'
                   'A widget subclass needs to implement the get_context method.'
                names      ('NotImplementedError',)
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_context'
-               firstlineno 895
+               firstlineno 900
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a00000000000000000072077c006a01000000000000000053
                   007c006a020000000000000000730f7407000000000000000000006401a6
                   010000ab01000000000000000082017c006a0200000000000000005300
-               899           0 RESUME                   0
+               904           0 RESUME                   0
                
-               906           2 LOAD_FAST                0 (self)
+               911           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (broken)
                             14 POP_JUMP_FORWARD_IF_FALSE     7 (to 30)
                
-               907          16 LOAD_FAST                0 (self)
+               912          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (template_broken)
                             28 RETURN_VALUE
                
-               908     >>   30 LOAD_FAST                0 (self)
+               913     >>   30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (template)
                             42 POP_JUMP_FORWARD_IF_TRUE    15 (to 74)
                
-               909          44 LOAD_GLOBAL              7 (NULL + NotImplementedError)
+               914          44 LOAD_GLOBAL              7 (NULL + NotImplementedError)
                             56 LOAD_CONST               1 ('A widget subclass needs to define a template.')
                             58 PRECALL                  1
                             62 CALL                     1
                             72 RAISE_VARARGS            1
                
-               910     >>   74 LOAD_FAST                0 (self)
+               915     >>   74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                2 (template)
                             86 RETURN_VALUE
                consts
                   'Get template.\n\n        Get the template to render the widget with. Defaults to the template attribute,\n        but can be overridden to allow more complex template generation scenarios. If\n        the widget is marked as broken, the template_broken attribute will be returned.\n        '
                   'A widget subclass needs to define a template.'
                names      ('broken', 'template_broken', 'template', 'NotImplementedError')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_template'
-               firstlineno 899
+               firstlineno 904
                lnotab 0x02070e010e010e011e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               912           0 RESUME                   0
+               917           0 RESUME                   0
                
-               913           2 LOAD_FAST                0 (self)
+               918           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 912
+               firstlineno 917
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x970065005a0164005a026401020065036402a6010000ab010000000000
                   000000660266015a04020065036403a6010000ab0100000000000000005a
                   05020065036404a6010000ab0100000000000000005a0664055300
-               915           0 RESUME                   0
+               920           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('DashboardWidget.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               916          10 LOAD_CONST               1 ('edit_default_dashboard')
+               921          10 LOAD_CONST               1 ('edit_default_dashboard')
                             12 PUSH_NULL
                             14 LOAD_NAME                3 (_)
                             16 LOAD_CONST               2 ('Can edit default dashboard')
                             18 PRECALL                  1
                             22 CALL                     1
                             32 BUILD_TUPLE              2
                             34 BUILD_TUPLE              1
                             36 STORE_NAME               4 (permissions)
                
-               917          38 PUSH_NULL
+               922          38 PUSH_NULL
                             40 LOAD_NAME                3 (_)
                             42 LOAD_CONST               3 ('Dashboard Widget')
                             44 PRECALL                  1
                             48 CALL                     1
                             58 STORE_NAME               5 (verbose_name)
                
-               918          60 PUSH_NULL
+               923          60 PUSH_NULL
                             62 LOAD_NAME                3 (_)
                             64 LOAD_CONST               4 ('Dashboard Widgets')
                             66 PRECALL                  1
                             70 CALL                     1
                             80 STORE_NAME               6 (verbose_name_plural)
                             82 LOAD_CONST               5 (None)
                             84 RETURN_VALUE
@@ -7006,24 +7021,24 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'permissions', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 915
+               firstlineno 920
                lnotab 0x0a011c011601
             'Meta'
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'UninstallRenitentPolymorphicManager', 'objects', 'staticmethod', 'Union', 'QuerySet', 'Iterable', 'get_media', 'template', 'template_broken', 'Media', 'media', 'models', 'CharField', '_', 'title', 'BooleanField', 'active', 'broken', 'PositiveSmallIntegerField', 'MaxValueValidator', 'size_s', 'size_m', 'size_l', 'size_xl', '_get_context_safe', 'get_context', 'get_template', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'DashboardWidget'
-         firstlineno 844
+         firstlineno 849
          lnotab
             0x0a010402140202011aff0e0102070401040114023601340136020e0114
             011401160102fc12060e0114011401160102fc12060e0114011401160102
             fc12060e0114011401160102fc120706050604060d0603
       'DashboardWidget'
       code
          argcount  : 0
@@ -7033,56 +7048,56 @@
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000002
             0065066402a6010000ab010000000000000000ac03a6010000ab01000000
             00000000005a07020065046a050000000000000000020065066404a60100
             00ab010000000000000000ac03a6010000ab0100000000000000005a0864
             0584005a0902004700640684006407a6020000ab0200000000000000005a
             0a64085300
-         921           0 RESUME                   0
+         926           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ExternalLinkWidget')
                        8 STORE_NAME               2 (__qualname__)
          
-         922          10 LOAD_CONST               1 ('core/dashboard_widget/external_link_widget.html')
+         927          10 LOAD_CONST               1 ('core/dashboard_widget/external_link_widget.html')
                       12 STORE_NAME               3 (template)
          
-         924          14 PUSH_NULL
+         929          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (URLField)
                       28 PUSH_NULL
                       30 LOAD_NAME                6 (_)
                       32 LOAD_CONST               2 ('URL')
                       34 PRECALL                  1
                       38 CALL                     1
                       48 KW_NAMES                 3
                       50 PRECALL                  1
                       54 CALL                     1
                       64 STORE_NAME               7 (url)
          
-         925          66 PUSH_NULL
+         930          66 PUSH_NULL
                       68 LOAD_NAME                4 (models)
                       70 LOAD_ATTR                5 (URLField)
                       80 PUSH_NULL
                       82 LOAD_NAME                6 (_)
                       84 LOAD_CONST               4 ('Icon URL')
                       86 PRECALL                  1
                       90 CALL                     1
                      100 KW_NAMES                 3
                      102 PRECALL                  1
                      106 CALL                     1
                      116 STORE_NAME               8 (icon_url)
          
-         927         118 LOAD_CONST               5 (<code object get_context, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 927>)
+         932         118 LOAD_CONST               5 (<code object get_context, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 932>)
                      120 MAKE_FUNCTION            0
                      122 STORE_NAME               9 (get_context)
          
-         930         124 PUSH_NULL
+         935         124 PUSH_NULL
                      126 LOAD_BUILD_CLASS
-                     128 LOAD_CONST               6 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 930>)
+                     128 LOAD_CONST               6 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 935>)
                      130 MAKE_FUNCTION            0
                      132 LOAD_CONST               7 ('Meta')
                      134 PRECALL                  2
                      138 CALL                     2
                      148 STORE_NAME              10 (Meta)
                      150 LOAD_CONST               8 (None)
                      152 RETURN_VALUE
@@ -7096,17 +7111,17 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a0100000000000000007c006a
                   02000000000000000064019c035300
-               927           0 RESUME                   0
+               932           0 RESUME                   0
                
-               928           2 LOAD_FAST                0 (self)
+               933           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (url)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (icon_url)
                             38 LOAD_CONST               1 (('title', 'url', 'icon_url'))
                             40 BUILD_CONST_KEY_MAP      3
@@ -7116,38 +7131,38 @@
                   ('title', 'url', 'icon_url')
                names      ('title', 'url', 'icon_url')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_context'
-               firstlineno 927
+               firstlineno 932
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               930           0 RESUME                   0
+               935           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('ExternalLinkWidget.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               931          10 PUSH_NULL
+               936          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('External link widget')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               932          32 PUSH_NULL
+               937          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('External link widgets')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -7158,65 +7173,65 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 930
+               firstlineno 935
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'template', 'models', 'URLField', '_', 'url', 'icon_url', 'get_context', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'ExternalLinkWidget'
-         firstlineno 921
+         firstlineno 926
          lnotab 0x0a010402340134020603
       'ExternalLinkWidget'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a0302006504020065056402a6010000ab
             010000000000000000ac03a6010000ab0100000000000000005a06640484
             005a0702004700640584006406a6020000ab0200000000000000005a0864
             075300
-         935           0 RESUME                   0
+         940           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('StaticContentWidget')
                        8 STORE_NAME               2 (__qualname__)
          
-         936          10 LOAD_CONST               1 ('core/dashboard_widget/static_content_widget.html')
+         941          10 LOAD_CONST               1 ('core/dashboard_widget/static_content_widget.html')
                       12 STORE_NAME               3 (template)
          
-         938          14 PUSH_NULL
+         943          14 PUSH_NULL
                       16 LOAD_NAME                4 (RichTextField)
                       18 PUSH_NULL
                       20 LOAD_NAME                5 (_)
                       22 LOAD_CONST               2 ('Content')
                       24 PRECALL                  1
                       28 CALL                     1
                       38 KW_NAMES                 3
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_NAME               6 (content)
          
-         940          56 LOAD_CONST               4 (<code object get_context, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 940>)
+         945          56 LOAD_CONST               4 (<code object get_context, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 945>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME               7 (get_context)
          
-         943          62 PUSH_NULL
+         948          62 PUSH_NULL
                       64 LOAD_BUILD_CLASS
-                      66 LOAD_CONST               5 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 943>)
+                      66 LOAD_CONST               5 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 948>)
                       68 MAKE_FUNCTION            0
                       70 LOAD_CONST               6 ('Meta')
                       72 PRECALL                  2
                       76 CALL                     2
                       86 STORE_NAME               8 (Meta)
                       88 LOAD_CONST               7 (None)
                       90 RETURN_VALUE
@@ -7229,17 +7244,17 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c006a01000000000000000064019c
                   025300
-               940           0 RESUME                   0
+               945           0 RESUME                   0
                
-               941           2 LOAD_FAST                0 (self)
+               946           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (content)
                             26 LOAD_CONST               1 (('title', 'content'))
                             28 BUILD_CONST_KEY_MAP      2
                             30 RETURN_VALUE
                consts
@@ -7247,38 +7262,38 @@
                   ('title', 'content')
                names      ('title', 'content')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_context'
-               firstlineno 940
+               firstlineno 945
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               943           0 RESUME                   0
+               948           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('StaticContentWidget.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               944          10 PUSH_NULL
+               949          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Static content widget')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               945          32 PUSH_NULL
+               950          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Static content widgets')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -7289,25 +7304,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 943
+               firstlineno 948
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'template', 'RichTextField', '_', 'content', 'get_context', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'StaticContentWidget'
-         firstlineno 935
+         firstlineno 940
          lnotab 0x0a0104022a020603
       'StaticContentWidget'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
@@ -7319,104 +7334,104 @@
             000000000064046404ac05a6050000ab0500000000000000005a0a020065
             036a0b0000000000000000020065076406a6010000ab0100000000000000
             00ac07a6010000ab0100000000000000005a0c020065036a0d0000000000
             0000006408020065076409a6010000ab010000000000000000ac0aa60200
             00ab0200000000000000005a0e0200650fa6000000ab0000000000000000
             005a106511640b8400a6000000ab0000000000000000005a120200470064
             0c8400640da6020000ab0200000000000000005a13640e5300
-         948           0 RESUME                   0
+         953           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DashboardWidgetOrder')
                        8 STORE_NAME               2 (__qualname__)
          
-         949          10 PUSH_NULL
+         954          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-         950          24 LOAD_NAME                5 (DashboardWidget)
+         955          24 LOAD_NAME                5 (DashboardWidget)
                       26 LOAD_NAME                3 (models)
                       28 LOAD_ATTR                6 (CASCADE)
                       38 PUSH_NULL
                       40 LOAD_NAME                7 (_)
                       42 LOAD_CONST               1 ('Dashboard widget')
                       44 PRECALL                  1
                       48 CALL                     1
          
-         949          58 KW_NAMES                 2
+         954          58 KW_NAMES                 2
                       60 PRECALL                  3
                       64 CALL                     3
                       74 STORE_NAME               8 (widget)
          
-         952          76 PUSH_NULL
+         957          76 PUSH_NULL
                       78 LOAD_NAME                3 (models)
                       80 LOAD_ATTR                4 (ForeignKey)
          
-         953          90 LOAD_NAME                9 (Person)
+         958          90 LOAD_NAME                9 (Person)
                       92 LOAD_NAME                3 (models)
                       94 LOAD_ATTR                6 (CASCADE)
                      104 PUSH_NULL
                      106 LOAD_NAME                7 (_)
                      108 LOAD_CONST               3 ('Person')
                      110 PRECALL                  1
                      114 CALL                     1
                      124 LOAD_CONST               4 (True)
                      126 LOAD_CONST               4 (True)
          
-         952         128 KW_NAMES                 5
+         957         128 KW_NAMES                 5
                      130 PRECALL                  5
                      134 CALL                     5
                      144 STORE_NAME              10 (person)
          
-         955         146 PUSH_NULL
+         960         146 PUSH_NULL
                      148 LOAD_NAME                3 (models)
                      150 LOAD_ATTR               11 (PositiveIntegerField)
                      160 PUSH_NULL
                      162 LOAD_NAME                7 (_)
                      164 LOAD_CONST               6 ('Order')
                      166 PRECALL                  1
                      170 CALL                     1
                      180 KW_NAMES                 7
                      182 PRECALL                  1
                      186 CALL                     1
                      196 STORE_NAME              12 (order)
          
-         956         198 PUSH_NULL
+         961         198 PUSH_NULL
                      200 LOAD_NAME                3 (models)
                      202 LOAD_ATTR               13 (BooleanField)
                      212 LOAD_CONST               8 (False)
                      214 PUSH_NULL
                      216 LOAD_NAME                7 (_)
                      218 LOAD_CONST               9 ('Part of the default dashboard')
                      220 PRECALL                  1
                      224 CALL                     1
                      234 KW_NAMES                10
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_NAME              14 (default)
          
-         958         252 PUSH_NULL
+         963         252 PUSH_NULL
                      254 LOAD_NAME               15 (InstalledWidgetsDashboardWidgetOrderManager)
                      256 PRECALL                  0
                      260 CALL                     0
                      270 STORE_NAME              16 (objects)
          
-         960         272 LOAD_NAME               17 (classproperty)
+         965         272 LOAD_NAME               17 (classproperty)
          
-         961         274 LOAD_CONST              11 (<code object default_dashboard_widgets, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 960>)
+         966         274 LOAD_CONST              11 (<code object default_dashboard_widgets, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 965>)
                      276 MAKE_FUNCTION            0
          
-         960         278 PRECALL                  0
+         965         278 PRECALL                  0
                      282 CALL                     0
          
-         961         292 STORE_NAME              18 (default_dashboard_widgets)
+         966         292 STORE_NAME              18 (default_dashboard_widgets)
          
-         970         294 PUSH_NULL
+         975         294 PUSH_NULL
                      296 LOAD_BUILD_CLASS
-                     298 LOAD_CONST              12 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 970>)
+                     298 LOAD_CONST              12 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 975>)
                      300 MAKE_FUNCTION            0
                      302 LOAD_CONST              13 ('Meta')
                      304 PRECALL                  2
                      308 CALL                     2
                      318 STORE_NAME              19 (Meta)
                      320 LOAD_CONST              14 (None)
                      322 RETURN_VALUE
@@ -7438,103 +7453,103 @@
                stacksize : 6
                flags     : 3
                code
                   0x9700640184007c006a000000000000000000a001000000000000000000
                   0000000000000000000000640264036403ac04a6030000ab030000000000
                   000000a00200000000000000000000000000000000000000006405a60100
                   00ab0100000000000000004400a6000000ab0000000000000000005300
-               960           0 RESUME                   0
+               965           0 RESUME                   0
                
-               963           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 963>)
+               968           2 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 968>)
                              4 MAKE_FUNCTION            0
                
-               965           6 LOAD_FAST                0 (cls)
+               970           6 LOAD_FAST                0 (cls)
                              8 LOAD_ATTR                0 (objects)
                             18 LOAD_METHOD              1 (filter)
                             40 LOAD_CONST               2 (None)
                             42 LOAD_CONST               3 (True)
                             44 LOAD_CONST               3 (True)
                             46 KW_NAMES                 4
                             48 PRECALL                  3
                             52 CALL                     3
                             62 LOAD_METHOD              2 (order_by)
                
-               966          84 LOAD_CONST               5 ('order')
+               971          84 LOAD_CONST               5 ('order')
                
-               965          86 PRECALL                  1
+               970          86 PRECALL                  1
                             90 CALL                     1
                
-               963         100 GET_ITER
+               968         100 GET_ITER
                            102 PRECALL                  0
                            106 CALL                     0
                            116 RETURN_VALUE
                consts
                   'Get default order for dashboard widgets.'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     963           0 RESUME                   0
+                     968           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                      
-                     965           8 STORE_FAST               1 (w)
+                     970           8 STORE_FAST               1 (w)
                      
-                     964          10 LOAD_FAST                1 (w)
+                     969          10 LOAD_FAST                1 (w)
                                   12 LOAD_ATTR                0 (widget)
                      
-                     963          22 LIST_APPEND              2
+                     968          22 LIST_APPEND              2
                                   24 JUMP_BACKWARD           10 (to 6)
                              >>   26 RETURN_VALUE
                      consts
                      names      ('widget',)
                      varnames   ('.0', 'w')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 963
+                     firstlineno 968
                      lnotab 0x080202ff0cff
                   None
                   True
                   ('person', 'default', 'widget__active')
                   'order'
                names      ('objects', 'filter', 'order_by')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'default_dashboard_widgets'
-               firstlineno 960
+               firstlineno 965
                lnotab 0x020304024e0102ff0efe
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               970           0 RESUME                   0
+               975           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('DashboardWidgetOrder.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               971          10 PUSH_NULL
+               976          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Dashboard widget order')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               972          32 PUSH_NULL
+               977          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Dashboard widget orders')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                             54 LOAD_CONST               3 (None)
                             56 RETURN_VALUE
@@ -7545,88 +7560,88 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 970
+               firstlineno 975
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'DashboardWidget', 'CASCADE', '_', 'widget', 'Person', 'person', 'PositiveIntegerField', 'order', 'BooleanField', 'default', 'InstalledWidgetsDashboardWidgetOrderManager', 'objects', 'classproperty', 'default_dashboard_widgets', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'DashboardWidgetOrder'
-         firstlineno 948
+         firstlineno 953
          lnotab 0x0a010e0122ff12030e0126ff1203340136021402020104ff0e010209
       'DashboardWidgetOrder'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000064
             02020065066403a6010000ab010000000000000000ac04a6020000ab0200
             000000000000005a07640584005a0865090200650a6406a6010000ab0100
             0000000000000064078400a6000000ab000000000000000000a6000000ab
             0000000000000000005a0b02004700640884006409a6020000ab02000000
             00000000005a0c640a5300
-         975           0 RESUME                   0
+         980           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CustomMenu')
                        8 STORE_NAME               2 (__qualname__)
          
-         976          10 LOAD_CONST               1 ('A custom menu to display in the footer.')
+         981          10 LOAD_CONST               1 ('A custom menu to display in the footer.')
                       12 STORE_NAME               3 (__doc__)
          
-         978          14 PUSH_NULL
+         983          14 PUSH_NULL
                       16 LOAD_NAME                4 (models)
                       18 LOAD_ATTR                5 (CharField)
                       28 LOAD_CONST               2 (100)
                       30 PUSH_NULL
                       32 LOAD_NAME                6 (_)
                       34 LOAD_CONST               3 ('Menu ID')
                       36 PRECALL                  1
                       40 CALL                     1
                       50 KW_NAMES                 4
                       52 PRECALL                  2
                       56 CALL                     2
                       66 STORE_NAME               7 (name)
          
-         980          68 LOAD_CONST               5 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 980>)
+         985          68 LOAD_CONST               5 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 985>)
                       70 MAKE_FUNCTION            0
                       72 STORE_NAME               8 (__str__)
          
-         983          74 LOAD_NAME                9 (classmethod)
+         988          74 LOAD_NAME                9 (classmethod)
          
-         984          76 PUSH_NULL
+         989          76 PUSH_NULL
                       78 LOAD_NAME               10 (cache_memoize)
                       80 LOAD_CONST               6 (3600)
                       82 PRECALL                  1
                       86 CALL                     1
          
-         985          96 LOAD_CONST               7 (<code object get_default, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 983>)
+         990          96 LOAD_CONST               7 (<code object get_default, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 988>)
                       98 MAKE_FUNCTION            0
          
-         984         100 PRECALL                  0
+         989         100 PRECALL                  0
                      104 CALL                     0
          
-         983         114 PRECALL                  0
+         988         114 PRECALL                  0
                      118 CALL                     0
          
-         985         128 STORE_NAME              11 (get_default)
+         990         128 STORE_NAME              11 (get_default)
          
-         990         130 PUSH_NULL
+         995         130 PUSH_NULL
                      132 LOAD_BUILD_CLASS
-                     134 LOAD_CONST               8 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 990>)
+                     134 LOAD_CONST               8 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 995>)
                      136 MAKE_FUNCTION            0
                      138 LOAD_CONST               9 ('Meta')
                      140 PRECALL                  2
                      144 CALL                     2
                      154 STORE_NAME              12 (Meta)
                      156 LOAD_CONST              10 (None)
                      158 RETURN_VALUE
@@ -7640,17 +7655,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b030000000072077c006a0000
                   000000000000006e067c006a0100000000000000005300
-               980           0 RESUME                   0
+               985           0 RESUME                   0
                
-               981           2 LOAD_FAST                0 (self)
+               986           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (name)
                             14 LOAD_CONST               1 ('')
                             16 COMPARE_OP               3 (!=)
                             22 POP_JUMP_FORWARD_IF_FALSE     7 (to 38)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                0 (name)
                             36 JUMP_FORWARD             6 (to 50)
@@ -7662,99 +7677,99 @@
                   ''
                names      ('name', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 980
+               firstlineno 985
                lnotab 0x0201
             3600
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   0000000000000000000000000000007c01ac02a6010000ab010000000000
                   0000005c0200007d027d037c025300
-               983           0 RESUME                   0
+               988           0 RESUME                   0
                
-               987           2 LOAD_FAST                0 (cls)
+               992           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (objects)
                             14 LOAD_METHOD              1 (prefetch_related)
                             36 LOAD_CONST               1 ('items')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (get_or_create)
                             74 LOAD_FAST                1 (name)
                             76 KW_NAMES                 2
                             78 PRECALL                  1
                             82 CALL                     1
                             92 UNPACK_SEQUENCE          2
                             96 STORE_FAST               2 (menu)
                             98 STORE_FAST               3 (_)
                
-               988         100 LOAD_FAST                2 (menu)
+               993         100 LOAD_FAST                2 (menu)
                            102 RETURN_VALUE
                consts
                   'Get a menu by name or create if it does not exist.'
                   'items'
                   ('name',)
                names      ('objects', 'prefetch_related', 'get_or_create')
                varnames   ('cls', 'name', 'menu', '_')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_default'
-               firstlineno 983
+               firstlineno 988
                lnotab 0x02046201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a05020065066a
                   070000000000000000640367016404ac05a6020000ab0200000000000000
                   0067015a0864065300
-               990           0 RESUME                   0
+               995           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('CustomMenu.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               991          10 PUSH_NULL
+               996          10 PUSH_NULL
                             12 LOAD_NAME                3 (_)
                             14 LOAD_CONST               1 ('Custom menu')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 STORE_NAME               4 (verbose_name)
                
-               992          32 PUSH_NULL
+               997          32 PUSH_NULL
                             34 LOAD_NAME                3 (_)
                             36 LOAD_CONST               2 ('Custom menus')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_NAME               5 (verbose_name_plural)
                
-               994          54 PUSH_NULL
+               999          54 PUSH_NULL
                             56 LOAD_NAME                6 (models)
                             58 LOAD_ATTR                7 (UniqueConstraint)
                             68 LOAD_CONST               3 ('name')
                             70 BUILD_LIST               1
                             72 LOAD_CONST               4 ('unique_menu_name')
                             74 KW_NAMES                 5
                             76 PRECALL                  2
                             80 CALL                     2
                
-               993          90 BUILD_LIST               1
+               998          90 BUILD_LIST               1
                             92 STORE_NAME               8 (constraints)
                             94 LOAD_CONST               6 (None)
                             96 RETURN_VALUE
                consts
                   'CustomMenu.Meta'
                   'Custom menu'
                   'Custom menus'
@@ -7764,25 +7779,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural', 'models', 'UniqueConstraint', 'constraints')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 990
+               firstlineno 995
                lnotab 0x0a011601160224ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'CharField', '_', 'name', '__str__', 'classmethod', 'cache_memoize', 'get_default', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'CustomMenu'
-         firstlineno 975
+         firstlineno 980
          lnotab 0x0a010402360206030201140104ff0eff0e020205
       'CustomMenu'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
@@ -7793,70 +7808,70 @@
             000000000000006405020065086406a6010000ab010000000000000000ac
             07a6020000ab0200000000000000005a0b020065046a0c00000000000000
             00020065086408a6010000ab010000000000000000ac09a6010000ab0100
             000000000000005a0d020065046a0a0000000000000000640a640b650e02
             006508640ca6010000ab010000000000000000ac0da6040000ab04000000
             00000000005a0f640e84005a1002004700640f84006410a6020000ab0200
             000000000000005a11641184005a1264125300
-          998           0 RESUME                   0
+         1003           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('CustomMenuItem')
                         8 STORE_NAME               2 (__qualname__)
          
-          999          10 LOAD_CONST               1 ('Single item in a custom menu.')
+         1004          10 LOAD_CONST               1 ('Single item in a custom menu.')
                        12 STORE_NAME               3 (__doc__)
          
-         1001          14 PUSH_NULL
+         1006          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (ForeignKey)
          
-         1002          28 LOAD_NAME                6 (CustomMenu)
+         1007          28 LOAD_NAME                6 (CustomMenu)
                        30 LOAD_NAME                4 (models)
                        32 LOAD_ATTR                7 (CASCADE)
                        42 PUSH_NULL
                        44 LOAD_NAME                8 (_)
                        46 LOAD_CONST               2 ('Menu')
                        48 PRECALL                  1
                        52 CALL                     1
                        62 LOAD_CONST               3 ('items')
          
-         1001          64 KW_NAMES                 4
+         1006          64 KW_NAMES                 4
                        66 PRECALL                  4
                        70 CALL                     4
                        80 STORE_NAME               9 (menu)
          
-         1004          82 PUSH_NULL
+         1009          82 PUSH_NULL
                        84 LOAD_NAME                4 (models)
                        86 LOAD_ATTR               10 (CharField)
                        96 LOAD_CONST               5 (150)
                        98 PUSH_NULL
                       100 LOAD_NAME                8 (_)
                       102 LOAD_CONST               6 ('Name')
                       104 PRECALL                  1
                       108 CALL                     1
                       118 KW_NAMES                 7
                       120 PRECALL                  2
                       124 CALL                     2
                       134 STORE_NAME              11 (name)
          
-         1005         136 PUSH_NULL
+         1010         136 PUSH_NULL
                       138 LOAD_NAME                4 (models)
                       140 LOAD_ATTR               12 (URLField)
                       150 PUSH_NULL
                       152 LOAD_NAME                8 (_)
                       154 LOAD_CONST               8 ('Link')
                       156 PRECALL                  1
                       160 CALL                     1
                       170 KW_NAMES                 9
                       172 PRECALL                  1
                       176 CALL                     1
                       186 STORE_NAME              13 (url)
          
-         1006         188 PUSH_NULL
+         1011         188 PUSH_NULL
                       190 LOAD_NAME                4 (models)
                       192 LOAD_ATTR               10 (CharField)
                       202 LOAD_CONST              10 (50)
                       204 LOAD_CONST              11 (True)
                       206 LOAD_NAME               14 (ICONS)
                       208 PUSH_NULL
                       210 LOAD_NAME                8 (_)
@@ -7864,28 +7879,28 @@
                       214 PRECALL                  1
                       218 CALL                     1
                       228 KW_NAMES                13
                       230 PRECALL                  4
                       234 CALL                     4
                       244 STORE_NAME              15 (icon)
          
-         1008         246 LOAD_CONST              14 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1008>)
+         1013         246 LOAD_CONST              14 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1013>)
                       248 MAKE_FUNCTION            0
                       250 STORE_NAME              16 (__str__)
          
-         1011         252 PUSH_NULL
+         1016         252 PUSH_NULL
                       254 LOAD_BUILD_CLASS
-                      256 LOAD_CONST              15 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1011>)
+                      256 LOAD_CONST              15 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1016>)
                       258 MAKE_FUNCTION            0
                       260 LOAD_CONST              16 ('Meta')
                       262 PRECALL                  2
                       266 CALL                     2
                       276 STORE_NAME              17 (Meta)
          
-         1018         278 LOAD_CONST              17 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1018>)
+         1023         278 LOAD_CONST              17 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1023>)
                       280 MAKE_FUNCTION            0
                       282 STORE_NAME              18 (get_absolute_url)
                       284 LOAD_CONST              18 (None)
                       286 RETURN_VALUE
          consts
             'CustomMenuItem'
             'Single item in a custom menu.'
@@ -7905,17 +7920,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970064017c006a0000000000000000009b0064027c006a010000000000
                   0000009b009d045300
-               1008           0 RESUME                   0
+               1013           0 RESUME                   0
                
-               1009           2 LOAD_CONST               1 ('[')
+               1014           2 LOAD_CONST               1 ('[')
                               4 LOAD_FAST                0 (self)
                               6 LOAD_ATTR                0 (menu)
                              16 FORMAT_VALUE             0
                              18 LOAD_CONST               2 ('] ')
                              20 LOAD_FAST                0 (self)
                              22 LOAD_ATTR                1 (name)
                              32 FORMAT_VALUE             0
@@ -7927,58 +7942,58 @@
                   '] '
                names      ('menu', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1008
+               firstlineno 1013
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a05020065066a
                   0700000000000000006403640467026405ac06a6020000ab020000000000
                   00000067015a0864075300
-               1011           0 RESUME                   0
+               1016           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('CustomMenuItem.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1012          10 PUSH_NULL
+               1017          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('Custom menu item')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1013          32 PUSH_NULL
+               1018          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('Custom menu items')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                
-               1015          54 PUSH_NULL
+               1020          54 PUSH_NULL
                              56 LOAD_NAME                6 (models)
                              58 LOAD_ATTR                7 (UniqueConstraint)
                              68 LOAD_CONST               3 ('menu')
                              70 LOAD_CONST               4 ('name')
                              72 BUILD_LIST               2
                              74 LOAD_CONST               5 ('unique_name_per_menu')
                              76 KW_NAMES                 6
                              78 PRECALL                  2
                              82 CALL                     2
                
-               1014          92 BUILD_LIST               1
+               1019          92 BUILD_LIST               1
                              94 STORE_NAME               8 (constraints)
                              96 LOAD_CONST               7 (None)
                              98 RETURN_VALUE
                consts
                   'CustomMenuItem.Meta'
                   'Custom menu item'
                   'Custom menu items'
@@ -7989,28 +8004,28 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural', 'models', 'UniqueConstraint', 'constraints')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1011
+               firstlineno 1016
                lnotab 0x0a011601160226ff
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               1018           0 RESUME                   0
+               1023           0 RESUME                   0
                
-               1019           2 LOAD_GLOBAL              1 (NULL + reverse)
+               1024           2 LOAD_GLOBAL              1 (NULL + reverse)
                              14 LOAD_CONST               1 ('admin:core_custommenuitem_change')
                              16 LOAD_FAST                0 (self)
                              18 LOAD_ATTR                1 (id)
                              28 BUILD_LIST               1
                              30 KW_NAMES                 2
                              32 PRECALL                  2
                              36 CALL                     2
@@ -8021,114 +8036,114 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_absolute_url'
-               firstlineno 1018
+               firstlineno 1023
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'CustomMenu', 'CASCADE', '_', 'menu', 'CharField', 'name', 'URLField', 'url', 'ICONS', 'icon', '__str__', 'Meta', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'CustomMenuItem'
-         firstlineno 998
+         firstlineno 1003
          lnotab 0x0a0104020e0124ff1203360134013a0206031a07
       'CustomMenuItem'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         1022           0 RESUME                   0
+         1027           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('DynamicRoute')
                         8 STORE_NAME               2 (__qualname__)
          
-         1023          10 LOAD_CONST               1 ('Define a dynamic route.\n\n    Dynamic routes should be used to register Vue routes dynamically, e. g.\n    when an app is supposed to show menu items for dynamically creatable objects.\n    ')
+         1028          10 LOAD_CONST               1 ('Define a dynamic route.\n\n    Dynamic routes should be used to register Vue routes dynamically, e. g.\n    when an app is supposed to show menu items for dynamically creatable objects.\n    ')
                        12 STORE_NAME               3 (__doc__)
                        14 LOAD_CONST               2 (None)
                        16 RETURN_VALUE
          consts
             'DynamicRoute'
             'Define a dynamic route.\n\n    Dynamic routes should be used to register Vue routes dynamically, e. g.\n    when an app is supposed to show menu items for dynamically creatable objects.\n    '
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'DynamicRoute'
-         firstlineno 1022
+         firstlineno 1027
          lnotab 0x0a01
       'DynamicRoute'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000002
             0065066402a6010000ab0100000000000000006403ac04a6020000ab0200
             000000000000005a07020065046a050000000000000000020065066405a6
             010000ab0100000000000000006406ac04a6020000ab0200000000000000
             005a08640765096602640884045a0a0200470064098400640aa6020000ab
             0200000000000000005a0b640b5300
-         1030           0 RESUME                   0
+         1035           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('GroupType')
                         8 STORE_NAME               2 (__qualname__)
          
-         1031          10 LOAD_CONST               1 ('Group type model.\n\n    Descriptive type of a group; used to tag groups and for apps to distinguish\n    how to display or handle a certain group.\n    ')
+         1036          10 LOAD_CONST               1 ('Group type model.\n\n    Descriptive type of a group; used to tag groups and for apps to distinguish\n    how to display or handle a certain group.\n    ')
                        12 STORE_NAME               3 (__doc__)
          
-         1037          14 PUSH_NULL
+         1042          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (CharField)
                        28 PUSH_NULL
                        30 LOAD_NAME                6 (_)
                        32 LOAD_CONST               2 ('Title of type')
                        34 PRECALL                  1
                        38 CALL                     1
                        48 LOAD_CONST               3 (50)
                        50 KW_NAMES                 4
                        52 PRECALL                  2
                        56 CALL                     2
                        66 STORE_NAME               7 (name)
          
-         1038          68 PUSH_NULL
+         1043          68 PUSH_NULL
                        70 LOAD_NAME                4 (models)
                        72 LOAD_ATTR                5 (CharField)
                        82 PUSH_NULL
                        84 LOAD_NAME                6 (_)
                        86 LOAD_CONST               5 ('Description')
                        88 PRECALL                  1
                        92 CALL                     1
                       102 LOAD_CONST               6 (500)
                       104 KW_NAMES                 4
                       106 PRECALL                  2
                       110 CALL                     2
                       120 STORE_NAME               8 (description)
          
-         1040         122 LOAD_CONST               7 ('return')
+         1045         122 LOAD_CONST               7 ('return')
                       124 LOAD_NAME                9 (str)
                       126 BUILD_TUPLE              2
-                      128 LOAD_CONST               8 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1040>)
+                      128 LOAD_CONST               8 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1045>)
                       130 MAKE_FUNCTION            4 (annotations)
                       132 STORE_NAME              10 (__str__)
          
-         1043         134 PUSH_NULL
+         1048         134 PUSH_NULL
                       136 LOAD_BUILD_CLASS
-                      138 LOAD_CONST               9 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1043>)
+                      138 LOAD_CONST               9 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1048>)
                       140 MAKE_FUNCTION            0
                       142 LOAD_CONST              10 ('Meta')
                       144 PRECALL                  2
                       148 CALL                     2
                       158 STORE_NAME              11 (Meta)
                       160 LOAD_CONST              11 (None)
                       162 RETURN_VALUE
@@ -8143,70 +8158,70 @@
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               1040           0 RESUME                   0
+               1045           0 RESUME                   0
                
-               1041           2 LOAD_FAST                0 (self)
+               1046           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (name)
                              14 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1040
+               firstlineno 1045
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a05020065066a
                   070000000000000000640367016404ac05a6020000ab0200000000000000
                   0067015a0864065300
-               1043           0 RESUME                   0
+               1048           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('GroupType.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1044          10 PUSH_NULL
+               1049          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('Group type')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1045          32 PUSH_NULL
+               1050          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('Group types')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                
-               1047          54 PUSH_NULL
+               1052          54 PUSH_NULL
                              56 LOAD_NAME                6 (models)
                              58 LOAD_ATTR                7 (UniqueConstraint)
                              68 LOAD_CONST               3 ('name')
                              70 BUILD_LIST               1
                              72 LOAD_CONST               4 ('unique_group_type_name')
                              74 KW_NAMES                 5
                              76 PRECALL                  2
                              80 CALL                     2
                
-               1046          90 BUILD_LIST               1
+               1051          90 BUILD_LIST               1
                              92 STORE_NAME               8 (constraints)
                              94 LOAD_CONST               6 (None)
                              96 RETURN_VALUE
                consts
                   'GroupType.Meta'
                   'Group type'
                   'Group types'
@@ -8216,47 +8231,47 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural', 'models', 'UniqueConstraint', 'constraints')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1043
+               firstlineno 1048
                lnotab 0x0a011601160224ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'CharField', '_', 'name', 'description', 'str', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'GroupType'
-         firstlineno 1030
+         firstlineno 1035
          lnotab 0x0a010406360136020c03
       'GroupType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a030200470064028400640365046a0500
             00000000000000a6030000ab0300000000000000005a0564045300
-         1051           0 RESUME                   0
+         1056           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('GlobalPermissions')
                         8 STORE_NAME               2 (__qualname__)
          
-         1052          10 LOAD_CONST               1 ('Container for global permissions.')
+         1057          10 LOAD_CONST               1 ('Container for global permissions.')
                        12 STORE_NAME               3 (__doc__)
          
-         1054          14 PUSH_NULL
+         1059          14 PUSH_NULL
                        16 LOAD_BUILD_CLASS
-                       18 LOAD_CONST               2 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1054>)
+                       18 LOAD_CONST               2 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1059>)
                        20 MAKE_FUNCTION            0
                        22 LOAD_CONST               3 ('Meta')
                        24 LOAD_NAME                4 (GlobalPermissionModel)
                        26 LOAD_ATTR                5 (Meta)
                        36 PRECALL                  3
                        40 CALL                     3
                        50 STORE_NAME               5 (Meta)
@@ -8276,101 +8291,101 @@
                   05020065036406a6010000ab010000000000000000660264070200650364
                   08a6010000ab0100000000000000006602640902006503640aa6010000ab
                   0100000000000000006602640b02006503640ca6010000ab010000000000
                   0000006602640d02006503640ea6010000ab010000000000000000660264
                   0f020065036410a6010000ab010000000000000000660264110200650364
                   12a6010000ab01000000000000000066026413020065036414a6010000ab
                   0100000000000000006602660a5a0464155300
-               1054           0 RESUME                   0
+               1059           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('GlobalPermissions.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1056          10 LOAD_CONST               1 ('view_system_status')
+               1061          10 LOAD_CONST               1 ('view_system_status')
                              12 PUSH_NULL
                              14 LOAD_NAME                3 (_)
                              16 LOAD_CONST               2 ('Can view system status')
                              18 PRECALL                  1
                              22 CALL                     1
                              32 BUILD_TUPLE              2
                
-               1057          34 LOAD_CONST               3 ('manage_data')
+               1062          34 LOAD_CONST               3 ('manage_data')
                              36 PUSH_NULL
                              38 LOAD_NAME                3 (_)
                              40 LOAD_CONST               4 ('Can manage data')
                              42 PRECALL                  1
                              46 CALL                     1
                              56 BUILD_TUPLE              2
                
-               1058          58 LOAD_CONST               5 ('impersonate')
+               1063          58 LOAD_CONST               5 ('impersonate')
                              60 PUSH_NULL
                              62 LOAD_NAME                3 (_)
                              64 LOAD_CONST               6 ('Can impersonate')
                              66 PRECALL                  1
                              70 CALL                     1
                              80 BUILD_TUPLE              2
                
-               1059          82 LOAD_CONST               7 ('search')
+               1064          82 LOAD_CONST               7 ('search')
                              84 PUSH_NULL
                              86 LOAD_NAME                3 (_)
                              88 LOAD_CONST               8 ('Can use search')
                              90 PRECALL                  1
                              94 CALL                     1
                             104 BUILD_TUPLE              2
                
-               1060         106 LOAD_CONST               9 ('change_site_preferences')
+               1065         106 LOAD_CONST               9 ('change_site_preferences')
                             108 PUSH_NULL
                             110 LOAD_NAME                3 (_)
                             112 LOAD_CONST              10 ('Can change site preferences')
                             114 PRECALL                  1
                             118 CALL                     1
                             128 BUILD_TUPLE              2
                
-               1061         130 LOAD_CONST              11 ('change_person_preferences')
+               1066         130 LOAD_CONST              11 ('change_person_preferences')
                             132 PUSH_NULL
                             134 LOAD_NAME                3 (_)
                             136 LOAD_CONST              12 ('Can change person preferences')
                             138 PRECALL                  1
                             142 CALL                     1
                             152 BUILD_TUPLE              2
                
-               1062         154 LOAD_CONST              13 ('change_group_preferences')
+               1067         154 LOAD_CONST              13 ('change_group_preferences')
                             156 PUSH_NULL
                             158 LOAD_NAME                3 (_)
                             160 LOAD_CONST              14 ('Can change group preferences')
                             162 PRECALL                  1
                             166 CALL                     1
                             176 BUILD_TUPLE              2
                
-               1063         178 LOAD_CONST              15 ('test_pdf')
+               1068         178 LOAD_CONST              15 ('test_pdf')
                             180 PUSH_NULL
                             182 LOAD_NAME                3 (_)
                             184 LOAD_CONST              16 ('Can test PDF generation')
                             186 PRECALL                  1
                             190 CALL                     1
                             200 BUILD_TUPLE              2
                
-               1064         202 LOAD_CONST              17 ('invite')
+               1069         202 LOAD_CONST              17 ('invite')
                             204 PUSH_NULL
                             206 LOAD_NAME                3 (_)
                             208 LOAD_CONST              18 ('Can invite persons')
                             210 PRECALL                  1
                             214 CALL                     1
                             224 BUILD_TUPLE              2
                
-               1065         226 LOAD_CONST              19 ('view_birthday_calendar')
+               1070         226 LOAD_CONST              19 ('view_birthday_calendar')
                             228 PUSH_NULL
                             230 LOAD_NAME                3 (_)
                             232 LOAD_CONST              20 ('Can view birthday calendar')
                             234 PRECALL                  1
                             238 CALL                     1
                             248 BUILD_TUPLE              2
                
-               1055         250 BUILD_TUPLE             10
+               1060         250 BUILD_TUPLE             10
                             252 STORE_NAME               4 (permissions)
                             254 LOAD_CONST              21 (None)
                             256 RETURN_VALUE
                consts
                   'GlobalPermissions.Meta'
                   'view_system_status'
                   'Can view system status'
@@ -8395,60 +8410,60 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'permissions')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1054
+               firstlineno 1059
                lnotab 0x0a0218011801180118011801180118011801180118f6
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'GlobalPermissionModel', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'GlobalPermissions'
-         firstlineno 1051
+         firstlineno 1056
          lnotab 0x0a010402
       'GlobalPermissions'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000065
             0665046a070000000000000000ac02a6020000ab0200000000000000005a
             080200470064038400640465096a0a0000000000000000a6030000ab0300
             000000000000005a0a64055300
-         1069           0 RESUME                   0
+         1074           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('PersonPreferenceModel')
                         8 STORE_NAME               2 (__qualname__)
          
-         1070          10 LOAD_CONST               1 ('Preference model to hold pereferences valid for a person.')
+         1075          10 LOAD_CONST               1 ('Preference model to hold pereferences valid for a person.')
                        12 STORE_NAME               3 (__doc__)
          
-         1072          14 PUSH_NULL
+         1077          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (ForeignKey)
                        28 LOAD_NAME                6 (Person)
                        30 LOAD_NAME                4 (models)
                        32 LOAD_ATTR                7 (CASCADE)
                        42 KW_NAMES                 2
                        44 PRECALL                  2
                        48 CALL                     2
                        58 STORE_NAME               8 (instance)
          
-         1074          60 PUSH_NULL
+         1079          60 PUSH_NULL
                        62 LOAD_BUILD_CLASS
-                       64 LOAD_CONST               3 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1074>)
+                       64 LOAD_CONST               3 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1079>)
                        66 MAKE_FUNCTION            0
                        68 LOAD_CONST               4 ('Meta')
                        70 LOAD_NAME                9 (PerInstancePreferenceModel)
                        72 LOAD_ATTR               10 (Meta)
                        82 PRECALL                  3
                        86 CALL                     3
                        96 STORE_NAME              10 (Meta)
@@ -8460,80 +8475,80 @@
             ('on_delete',)
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               1074           0 RESUME                   0
+               1079           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('PersonPreferenceModel.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1075          10 LOAD_CONST               1 ('core')
+               1080          10 LOAD_CONST               1 ('core')
                              12 STORE_NAME               3 (app_label)
                              14 LOAD_CONST               2 (None)
                              16 RETURN_VALUE
                consts
                   'PersonPreferenceModel.Meta'
                   'core'
                   None
                names      ('__name__', '__module__', '__qualname__', 'app_label')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1074
+               firstlineno 1079
                lnotab 0x0a01
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'Person', 'CASCADE', 'instance', 'PerInstancePreferenceModel', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'PersonPreferenceModel'
-         firstlineno 1069
+         firstlineno 1074
          lnotab 0x0a0104022e02
       'PersonPreferenceModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0264015a03020065046a05000000000000000065
             0665046a070000000000000000ac02a6020000ab0200000000000000005a
             080200470064038400640465096a0a0000000000000000a6030000ab0300
             000000000000005a0a64055300
-         1078           0 RESUME                   0
+         1083           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('GroupPreferenceModel')
                         8 STORE_NAME               2 (__qualname__)
          
-         1079          10 LOAD_CONST               1 ('Preference model to hold pereferences valid for members of a group.')
+         1084          10 LOAD_CONST               1 ('Preference model to hold pereferences valid for members of a group.')
                        12 STORE_NAME               3 (__doc__)
          
-         1081          14 PUSH_NULL
+         1086          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (ForeignKey)
                        28 LOAD_NAME                6 (Group)
                        30 LOAD_NAME                4 (models)
                        32 LOAD_ATTR                7 (CASCADE)
                        42 KW_NAMES                 2
                        44 PRECALL                  2
                        48 CALL                     2
                        58 STORE_NAME               8 (instance)
          
-         1083          60 PUSH_NULL
+         1088          60 PUSH_NULL
                        62 LOAD_BUILD_CLASS
-                       64 LOAD_CONST               3 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1083>)
+                       64 LOAD_CONST               3 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1088>)
                        66 MAKE_FUNCTION            0
                        68 LOAD_CONST               4 ('Meta')
                        70 LOAD_NAME                9 (PerInstancePreferenceModel)
                        72 LOAD_ATTR               10 (Meta)
                        82 PRECALL                  3
                        86 CALL                     3
                        96 STORE_NAME              10 (Meta)
@@ -8545,45 +8560,45 @@
             ('on_delete',)
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               1083           0 RESUME                   0
+               1088           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('GroupPreferenceModel.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1084          10 LOAD_CONST               1 ('core')
+               1089          10 LOAD_CONST               1 ('core')
                              12 STORE_NAME               3 (app_label)
                              14 LOAD_CONST               2 (None)
                              16 RETURN_VALUE
                consts
                   'GroupPreferenceModel.Meta'
                   'core'
                   None
                names      ('__name__', '__module__', '__qualname__', 'app_label')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1083
+               firstlineno 1088
                lnotab 0x0a01
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'ForeignKey', 'Group', 'CASCADE', 'instance', 'PerInstancePreferenceModel', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'GroupPreferenceModel'
-         firstlineno 1078
+         firstlineno 1083
          lnotab 0x0a0104022e02
       'GroupPreferenceModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
@@ -8597,127 +8612,127 @@
             0000005a10020065046a110000000000000000640902006506640aa60100
             00ab010000000000000000ac0ba6020000ab0200000000000000005a1202
             0065046a110000000000000000640902006506640ca6010000ab01000000
             0000000000ac0ba6020000ab0200000000000000005a136514640d650766
             02640e8404a6000000ab0000000000000000005a15641664106516660264
             1184055a17641284005a1802004700641384006414a6020000ab02000000
             00000000005a1964155300
-         1087           0 RESUME                   0
+         1092           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('DataCheckResult')
                         8 STORE_NAME               2 (__qualname__)
          
-         1088          10 LOAD_CONST               1 ('Save the result of a data check for a specific object.')
+         1093          10 LOAD_CONST               1 ('Save the result of a data check for a specific object.')
                        12 STORE_NAME               3 (__doc__)
          
-         1090          14 PUSH_NULL
+         1095          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (CharField)
          
-         1091          28 LOAD_CONST               2 (255)
+         1096          28 LOAD_CONST               2 (255)
          
-         1092          30 PUSH_NULL
+         1097          30 PUSH_NULL
                        32 LOAD_NAME                6 (_)
                        34 LOAD_CONST               3 ('Related data check task')
                        36 PRECALL                  1
                        40 CALL                     1
          
-         1093          50 LOAD_NAME                7 (DataCheck)
+         1098          50 LOAD_NAME                7 (DataCheck)
                        52 LOAD_ATTR                8 (data_checks_choices)
          
-         1090          62 KW_NAMES                 4
+         1095          62 KW_NAMES                 4
                        64 PRECALL                  3
                        68 CALL                     3
                        78 STORE_NAME               9 (data_check)
          
-         1096          80 PUSH_NULL
+         1101          80 PUSH_NULL
                        82 LOAD_NAME                4 (models)
                        84 LOAD_ATTR               10 (ForeignKey)
                        94 LOAD_NAME               11 (ContentType)
                        96 LOAD_NAME                4 (models)
                        98 LOAD_ATTR               12 (CASCADE)
                       108 KW_NAMES                 5
                       110 PRECALL                  2
                       114 CALL                     2
                       124 STORE_NAME              13 (content_type)
          
-         1097         126 PUSH_NULL
+         1102         126 PUSH_NULL
                       128 LOAD_NAME                4 (models)
                       130 LOAD_ATTR                5 (CharField)
                       140 LOAD_CONST               2 (255)
                       142 KW_NAMES                 6
                       144 PRECALL                  1
                       148 CALL                     1
                       158 STORE_NAME              14 (object_id)
          
-         1098         160 PUSH_NULL
+         1103         160 PUSH_NULL
                       162 LOAD_NAME               15 (GenericForeignKey)
                       164 LOAD_CONST               7 ('content_type')
                       166 LOAD_CONST               8 ('object_id')
                       168 PRECALL                  2
                       172 CALL                     2
                       182 STORE_NAME              16 (related_object)
          
-         1100         184 PUSH_NULL
+         1105         184 PUSH_NULL
                       186 LOAD_NAME                4 (models)
                       188 LOAD_ATTR               17 (BooleanField)
                       198 LOAD_CONST               9 (False)
                       200 PUSH_NULL
                       202 LOAD_NAME                6 (_)
                       204 LOAD_CONST              10 ('Issue solved')
                       206 PRECALL                  1
                       210 CALL                     1
                       220 KW_NAMES                11
                       222 PRECALL                  2
                       226 CALL                     2
                       236 STORE_NAME              18 (solved)
          
-         1101         238 PUSH_NULL
+         1106         238 PUSH_NULL
                       240 LOAD_NAME                4 (models)
                       242 LOAD_ATTR               17 (BooleanField)
                       252 LOAD_CONST               9 (False)
                       254 PUSH_NULL
                       256 LOAD_NAME                6 (_)
                       258 LOAD_CONST              12 ('Notification sent')
                       260 PRECALL                  1
                       264 CALL                     1
                       274 KW_NAMES                11
                       276 PRECALL                  2
                       280 CALL                     2
                       290 STORE_NAME              19 (sent)
          
-         1103         292 LOAD_NAME               20 (property)
+         1108         292 LOAD_NAME               20 (property)
          
-         1104         294 LOAD_CONST              13 ('return')
+         1109         294 LOAD_CONST              13 ('return')
                       296 LOAD_NAME                7 (DataCheck)
                       298 BUILD_TUPLE              2
-                      300 LOAD_CONST              14 (<code object related_check, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1103>)
+                      300 LOAD_CONST              14 (<code object related_check, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1108>)
                       302 MAKE_FUNCTION            4 (annotations)
          
-         1103         304 PRECALL                  0
+         1108         304 PRECALL                  0
                       308 CALL                     0
          
-         1104         318 STORE_NAME              21 (related_check)
+         1109         318 STORE_NAME              21 (related_check)
          
-         1107         320 LOAD_CONST              22 (('default',))
+         1112         320 LOAD_CONST              22 (('default',))
                       322 LOAD_CONST              16 ('solve_option')
                       324 LOAD_NAME               22 (str)
                       326 BUILD_TUPLE              2
-                      328 LOAD_CONST              17 (<code object solve, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1107>)
+                      328 LOAD_CONST              17 (<code object solve, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1112>)
                       330 MAKE_FUNCTION            5 (defaults, annotations)
                       332 STORE_NAME              23 (solve)
          
-         1110         334 LOAD_CONST              18 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1110>)
+         1115         334 LOAD_CONST              18 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1115>)
                       336 MAKE_FUNCTION            0
                       338 STORE_NAME              24 (__str__)
          
-         1113         340 PUSH_NULL
+         1118         340 PUSH_NULL
                       342 LOAD_BUILD_CLASS
-                      344 LOAD_CONST              19 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1113>)
+                      344 LOAD_CONST              19 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1118>)
                       346 MAKE_FUNCTION            0
                       348 LOAD_CONST              20 ('Meta')
                       350 PRECALL                  2
                       354 CALL                     2
                       364 STORE_NAME              25 (Meta)
                       366 LOAD_CONST              21 (None)
                       368 RETURN_VALUE
@@ -8740,46 +8755,46 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007400000000000000000000006a0100000000000000007c006a0200
                   00000000000000190000000000000000005300
-               1103           0 RESUME                   0
+               1108           0 RESUME                   0
                
-               1105           2 LOAD_GLOBAL              0 (DataCheck)
+               1110           2 LOAD_GLOBAL              0 (DataCheck)
                              14 LOAD_ATTR                1 (registered_objects_dict)
                              24 LOAD_FAST                0 (self)
                              26 LOAD_ATTR                2 (data_check)
                              36 BINARY_SUBSCR
                              46 RETURN_VALUE
                consts
                   None
                names      ('DataCheck', 'registered_objects_dict', 'data_check')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'related_check'
-               firstlineno 1103
+               firstlineno 1108
                lnotab 0x0202
             'default'
             'solve_option'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c007c01a6020000ab0200000000000000000100640053
                   00
-               1107           0 RESUME                   0
+               1112           0 RESUME                   0
                
-               1108           2 LOAD_FAST                0 (self)
+               1113           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (related_check)
                              14 LOAD_METHOD              1 (solve)
                              36 LOAD_FAST                0 (self)
                              38 LOAD_FAST                1 (solve_option)
                              40 PRECALL                  2
                              44 CALL                     2
                              54 POP_TOP
@@ -8789,27 +8804,27 @@
                   None
                names      ('related_check', 'solve')
                varnames   ('self', 'solve_option')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'solve'
-               firstlineno 1107
+               firstlineno 1112
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   006a0200000000000000009b009d035300
-               1110           0 RESUME                   0
+               1115           0 RESUME                   0
                
-               1111           2 LOAD_FAST                0 (self)
+               1116           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (related_object)
                              14 FORMAT_VALUE             0
                              16 LOAD_CONST               1 (': ')
                              18 LOAD_FAST                0 (self)
                              20 LOAD_ATTR                1 (related_check)
                              30 LOAD_ATTR                2 (problem_name)
                              40 FORMAT_VALUE             0
@@ -8820,63 +8835,63 @@
                   ': '
                names      ('related_object', 'related_check', 'problem_name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1110
+               firstlineno 1115
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 5
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a056403020065
                   036404a6010000ab01000000000000000066026405020065036406a60100
                   00ab010000000000000000660266025a0664075300
-               1113           0 RESUME                   0
+               1118           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('DataCheckResult.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1114          10 PUSH_NULL
+               1119          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('Data check result')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1115          32 PUSH_NULL
+               1120          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('Data check results')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                
-               1117          54 LOAD_CONST               3 ('run_data_checks')
+               1122          54 LOAD_CONST               3 ('run_data_checks')
                              56 PUSH_NULL
                              58 LOAD_NAME                3 (_)
                              60 LOAD_CONST               4 ('Can run data checks')
                              62 PRECALL                  1
                              66 CALL                     1
                              76 BUILD_TUPLE              2
                
-               1118          78 LOAD_CONST               5 ('solve_data_problem')
+               1123          78 LOAD_CONST               5 ('solve_data_problem')
                              80 PUSH_NULL
                              82 LOAD_NAME                3 (_)
                              84 LOAD_CONST               6 ('Can solve data check problems')
                              86 PRECALL                  1
                              90 CALL                     1
                             100 BUILD_TUPLE              2
                
-               1116         102 BUILD_TUPLE              2
+               1121         102 BUILD_TUPLE              2
                             104 STORE_NAME               6 (permissions)
                             106 LOAD_CONST               7 (None)
                             108 RETURN_VALUE
                consts
                   'DataCheckResult.Meta'
                   'Data check result'
                   'Data check results'
@@ -8887,26 +8902,26 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural', 'permissions')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1113
+               firstlineno 1118
                lnotab 0x0a0116011602180118fe
             'Meta'
             None
             ('default',)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'CharField', '_', 'DataCheck', 'data_checks_choices', 'data_check', 'ForeignKey', 'ContentType', 'CASCADE', 'content_type', 'object_id', 'GenericForeignKey', 'related_object', 'BooleanField', 'solved', 'sent', 'property', 'related_check', 'str', 'solve', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'DataCheckResult'
-         firstlineno 1087
+         firstlineno 1092
          lnotab
             0x0a0104020e01020114010cfd12062e01220118023601360202010aff0e
             0102030e030603
       'DataCheckResult'
       code
          argcount  : 0
          nlocals   : 0
@@ -8916,80 +8931,80 @@
             0x970065005a0164005a0264015a03020065046a05000000000000000002
             0065066402a6010000ab0100000000000000006403ac04a6020000ab0200
             000000000000005a07020065046a080000000000000000650965046a0a00
             00000000000000640364056403ac06a6050000ab0500000000000000005a
             0b6407650c6602640884045a0d650e640c640a8401a6000000ab00000000
             00000000005a0f640b84005a1065116a1200000000000000005a1265105a
             1064095300
-         1122           0 RESUME                   0
+         1127           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('PersonInvitation')
                         8 STORE_NAME               2 (__qualname__)
          
-         1123          10 LOAD_CONST               1 ('Custom model for invitations to allow to generate invitations codes without email address.')
+         1128          10 LOAD_CONST               1 ('Custom model for invitations to allow to generate invitations codes without email address.')
                        12 STORE_NAME               3 (__doc__)
          
-         1125          14 PUSH_NULL
+         1130          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (EmailField)
                        28 PUSH_NULL
                        30 LOAD_NAME                6 (_)
                        32 LOAD_CONST               2 ('E-Mail address')
                        34 PRECALL                  1
                        38 CALL                     1
                        48 LOAD_CONST               3 (True)
                        50 KW_NAMES                 4
                        52 PRECALL                  2
                        56 CALL                     2
                        66 STORE_NAME               7 (email)
          
-         1126          68 PUSH_NULL
+         1131          68 PUSH_NULL
                        70 LOAD_NAME                4 (models)
                        72 LOAD_ATTR                8 (ForeignKey)
          
-         1127          82 LOAD_NAME                9 (Person)
+         1132          82 LOAD_NAME                9 (Person)
                        84 LOAD_NAME                4 (models)
                        86 LOAD_ATTR               10 (CASCADE)
                        96 LOAD_CONST               3 (True)
                        98 LOAD_CONST               5 ('invitation')
                       100 LOAD_CONST               3 (True)
          
-         1126         102 KW_NAMES                 6
+         1131         102 KW_NAMES                 6
                       104 PRECALL                  5
                       108 CALL                     5
                       118 STORE_NAME              11 (person)
          
-         1130         120 LOAD_CONST               7 ('return')
+         1135         120 LOAD_CONST               7 ('return')
                       122 LOAD_NAME               12 (str)
                       124 BUILD_TUPLE              2
-                      126 LOAD_CONST               8 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1130>)
+                      126 LOAD_CONST               8 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1135>)
                       128 MAKE_FUNCTION            4 (annotations)
                       130 STORE_NAME              13 (__str__)
          
-         1133         132 LOAD_NAME               14 (classmethod)
+         1138         132 LOAD_NAME               14 (classmethod)
          
-         1134         134 LOAD_CONST              12 ((None,))
-                      136 LOAD_CONST              10 (<code object create, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1133>)
+         1139         134 LOAD_CONST              12 ((None,))
+                      136 LOAD_CONST              10 (<code object create, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1138>)
                       138 MAKE_FUNCTION            1 (defaults)
          
-         1133         140 PRECALL                  0
+         1138         140 PRECALL                  0
                       144 CALL                     0
          
-         1134         154 STORE_NAME              15 (create)
+         1139         154 STORE_NAME              15 (create)
          
-         1142         156 LOAD_CONST              11 (<code object send_invitation, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1142>)
+         1147         156 LOAD_CONST              11 (<code object send_invitation, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1147>)
                       158 MAKE_FUNCTION            0
                       160 STORE_NAME              16 (send_invitation)
          
-         1169         162 LOAD_NAME               17 (Invitation)
+         1174         162 LOAD_NAME               17 (Invitation)
                       164 LOAD_ATTR               18 (key_expired)
                       174 STORE_NAME              18 (key_expired)
          
-         1170         176 LOAD_NAME               16 (send_invitation)
+         1175         176 LOAD_NAME               16 (send_invitation)
                       178 STORE_NAME              16 (send_invitation)
                       180 LOAD_CONST               9 (None)
                       182 RETURN_VALUE
          consts
             'PersonInvitation'
             'Custom model for invitations to allow to generate invitations codes without email address.'
             'E-Mail address'
@@ -9002,17 +9017,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064029d045300
-               1130           0 RESUME                   0
+               1135           0 RESUME                   0
                
-               1131           2 LOAD_FAST                0 (self)
+               1136           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (email)
                              14 FORMAT_VALUE             0
                              16 LOAD_CONST               1 (' (')
                              18 LOAD_FAST                0 (self)
                              20 LOAD_ATTR                1 (inviter)
                              30 FORMAT_VALUE             0
                              32 LOAD_CONST               2 (')')
@@ -9024,82 +9039,82 @@
                   ')'
                names      ('email', 'inviter')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1130
+               firstlineno 1135
                lnotab 0x0201
             None
             code
                argcount  : 3
                nlocals   : 8
                stacksize : 7
                flags     : 11
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000064
                   01190000000000000000007d04740100000000000000000000a6000000ab
                   0000000000000000006402190000000000000000007d0574030000000000
                   00000000007c047c05a6020000ab0200000000000000007d0602007c006a
                   0200000000000000006a03000000000000000064047c017c027c0664039c
                   037c03a4018e017d077c075300
-               1133           0 RESUME                   0
+               1138           0 RESUME                   0
                
-               1135           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+               1140           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 LOAD_CONST               1 ('auth__invite_code_length')
                              30 BINARY_SUBSCR
                              40 STORE_FAST               4 (length)
                
-               1136          42 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+               1141          42 LOAD_GLOBAL              1 (NULL + get_site_preferences)
                              54 PRECALL                  0
                              58 CALL                     0
                              68 LOAD_CONST               2 ('auth__invite_code_packet_size')
                              70 BINARY_SUBSCR
                              80 STORE_FAST               5 (packet_size)
                
-               1137          82 LOAD_GLOBAL              3 (NULL + generate_random_code)
+               1142          82 LOAD_GLOBAL              3 (NULL + generate_random_code)
                              94 LOAD_FAST                4 (length)
                              96 LOAD_FAST                5 (packet_size)
                              98 PRECALL                  2
                             102 CALL                     2
                             112 STORE_FAST               6 (code)
                
-               1139         114 PUSH_NULL
+               1144         114 PUSH_NULL
                             116 LOAD_FAST                0 (cls)
                             118 LOAD_ATTR                2 (objects)
                             128 LOAD_ATTR                3 (create)
                             138 LOAD_CONST               4 (())
                             140 LOAD_FAST                1 (email)
                             142 LOAD_FAST                2 (inviter)
                             144 LOAD_FAST                6 (code)
                             146 LOAD_CONST               3 (('email', 'inviter', 'key'))
                             148 BUILD_CONST_KEY_MAP      3
                             150 LOAD_FAST                3 (kwargs)
                             152 DICT_MERGE               1
                             154 CALL_FUNCTION_EX         1
                             156 STORE_FAST               7 (instance)
                
-               1140         158 LOAD_FAST                7 (instance)
+               1145         158 LOAD_FAST                7 (instance)
                             160 RETURN_VALUE
                consts
                   None
                   'auth__invite_code_length'
                   'auth__invite_code_packet_size'
                   ('email', 'inviter', 'key')
                   ()
                names      ('get_site_preferences', 'generate_random_code', 'objects', 'create')
                varnames   ('cls', 'email', 'inviter', 'kwargs', 'length', 'packet_size', 'code', 'instance')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'create'
-               firstlineno 1133
+               firstlineno 1138
                lnotab 0x02022801280120022c01
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 8
                flags     : 11
                code
@@ -9116,107 +9131,107 @@
                   0001007415000000000000000000006a0b0000000000000000a6000000ab
                   0000000000000000007c005f0c00000000000000007c00a00d0000000000
                   000000000000000000000000000000a6000000ab00000000000000000001
                   00741c000000000000000000006a0f0000000000000000a0100000000000
                   0000000000000000000000000000007c006a1100000000000000007c007c
                   037c006a070000000000000000ac09a6040000ab04000000000000000001
                   00640a5300
-               1142           0 RESUME                   0
+               1147           0 RESUME                   0
                
-               1144           2 LOAD_GLOBAL              1 (NULL + reverse)
+               1149           2 LOAD_GLOBAL              1 (NULL + reverse)
                              14 LOAD_CONST               1 ('invitations:accept-invite')
                              16 LOAD_FAST                0 (self)
                              18 LOAD_ATTR                1 (key)
                              28 BUILD_LIST               1
                              30 KW_NAMES                 2
                              32 PRECALL                  2
                              36 CALL                     2
                              46 STORE_FAST               3 (invite_url)
                
-               1145          48 LOAD_FAST                1 (request)
+               1150          48 LOAD_FAST                1 (request)
                              50 LOAD_METHOD              2 (build_absolute_uri)
                              72 LOAD_FAST                3 (invite_url)
                              74 PRECALL                  1
                              78 CALL                     1
                              88 LOAD_METHOD              3 (replace)
                             110 LOAD_CONST               3 ('/django')
                             112 LOAD_CONST               4 ('')
                             114 PRECALL                  2
                             118 CALL                     2
                             128 STORE_FAST               3 (invite_url)
                
-               1146         130 LOAD_FAST                2 (kwargs)
+               1151         130 LOAD_FAST                2 (kwargs)
                             132 STORE_FAST               4 (context)
                
-               1147         134 LOAD_FAST                4 (context)
+               1152         134 LOAD_FAST                4 (context)
                             136 LOAD_METHOD              4 (update)
                
-               1149         158 LOAD_FAST                3 (invite_url)
+               1154         158 LOAD_FAST                3 (invite_url)
                
-               1150         160 LOAD_GLOBAL             11 (NULL + get_site_preferences)
+               1155         160 LOAD_GLOBAL             11 (NULL + get_site_preferences)
                             172 PRECALL                  0
                             176 CALL                     0
                             186 LOAD_CONST               5 ('general__title')
                             188 BINARY_SUBSCR
                
-               1151         198 LOAD_FAST                0 (self)
+               1156         198 LOAD_FAST                0 (self)
                             200 LOAD_ATTR                6 (email)
                
-               1152         210 LOAD_FAST                0 (self)
+               1157         210 LOAD_FAST                0 (self)
                             212 LOAD_ATTR                7 (inviter)
                
-               1153         222 LOAD_FAST                0 (self)
+               1158         222 LOAD_FAST                0 (self)
                             224 LOAD_ATTR                8 (person)
                
-               1148         234 LOAD_CONST               6 (('invite_url', 'site_name', 'email', 'inviter', 'person'))
+               1153         234 LOAD_CONST               6 (('invite_url', 'site_name', 'email', 'inviter', 'person'))
                             236 BUILD_CONST_KEY_MAP      5
                
-               1147         238 PRECALL                  1
+               1152         238 PRECALL                  1
                             242 CALL                     1
                             252 POP_TOP
                
-               1157         254 LOAD_GLOBAL             19 (NULL + send_email)
+               1162         254 LOAD_GLOBAL             19 (NULL + send_email)
                             266 LOAD_CONST               7 ('invitation')
                             268 LOAD_FAST                0 (self)
                             270 LOAD_ATTR                6 (email)
                             280 BUILD_LIST               1
                             282 LOAD_FAST                4 (context)
                             284 KW_NAMES                 8
                             286 PRECALL                  3
                             290 CALL                     3
                             300 POP_TOP
                
-               1159         302 LOAD_GLOBAL             21 (NULL + timezone)
+               1164         302 LOAD_GLOBAL             21 (NULL + timezone)
                             314 LOAD_ATTR               11 (now)
                             324 PRECALL                  0
                             328 CALL                     0
                             338 LOAD_FAST                0 (self)
                             340 STORE_ATTR              12 (sent)
                
-               1160         350 LOAD_FAST                0 (self)
+               1165         350 LOAD_FAST                0 (self)
                             352 LOAD_METHOD             13 (save)
                             374 PRECALL                  0
                             378 CALL                     0
                             388 POP_TOP
                
-               1162         390 LOAD_GLOBAL             28 (signals)
+               1167         390 LOAD_GLOBAL             28 (signals)
                             402 LOAD_ATTR               15 (invite_url_sent)
                             412 LOAD_METHOD             16 (send)
                
-               1163         434 LOAD_FAST                0 (self)
+               1168         434 LOAD_FAST                0 (self)
                             436 LOAD_ATTR               17 (__class__)
                
-               1164         446 LOAD_FAST                0 (self)
+               1169         446 LOAD_FAST                0 (self)
                
-               1165         448 LOAD_FAST                3 (invite_url)
+               1170         448 LOAD_FAST                3 (invite_url)
                
-               1166         450 LOAD_FAST                0 (self)
+               1171         450 LOAD_FAST                0 (self)
                             452 LOAD_ATTR                7 (inviter)
                
-               1162         462 KW_NAMES                 9
+               1167         462 KW_NAMES                 9
                             464 PRECALL                  4
                             468 CALL                     4
                             478 POP_TOP
                             480 LOAD_CONST              10 (None)
                             482 RETURN_VALUE
                consts
                   'Send the invitation email to the person.'
@@ -9232,26 +9247,26 @@
                   None
                names      ('reverse', 'key', 'build_absolute_uri', 'replace', 'update', 'get_site_preferences', 'email', 'inviter', 'person', 'send_email', 'timezone', 'now', 'sent', 'save', 'signals', 'invite_url_sent', 'send', '__class__')
                varnames   ('self', 'request', 'kwargs', 'invite_url', 'context')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'send_invitation'
-               firstlineno 1142
+               firstlineno 1147
                lnotab
                   0x02022e01520104011802020126010c010c010cfb04ff100a3002300128
                   022c010c01020102010cfc
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'EmailField', '_', 'email', 'ForeignKey', 'Person', 'CASCADE', 'person', 'str', '__str__', 'classmethod', 'create', 'send_invitation', 'Invitation', 'key_expired')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'PersonInvitation'
-         firstlineno 1122
+         firstlineno 1127
          lnotab 0x0a01040236010e0114ff12040c03020106ff0e010208061b0e01
       'PersonInvitation'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
@@ -9262,112 +9277,112 @@
             005a0a020065056a0b0000000000000000020065096407a6010000ab0100
             000000000000006504ac08a6020000ab0200000000000000005a0c020065
             056a0d0000000000000000640902006509640aa6010000ab010000000000
             00000064036403ac0ba6040000ab0400000000000000005a0e020065056a
             0d000000000000000064096403640302006509640ca6010000ab01000000
             0000000000ac0da6040000ab0400000000000000005a0f640e84005a1002
             004700640f84006410a6020000ab0200000000000000005a1164115300
-         1173           0 RESUME                   0
+         1178           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('PDFFile')
                         8 STORE_NAME               2 (__qualname__)
          
-         1174          10 LOAD_CONST               1 ('Link to a rendered PDF file.')
+         1179          10 LOAD_CONST               1 ('Link to a rendered PDF file.')
                        12 STORE_NAME               3 (__doc__)
          
-         1176          14 LOAD_CONST               2 (<code object _get_default_expiration, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1176>)
+         1181          14 LOAD_CONST               2 (<code object _get_default_expiration, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1181>)
                        16 MAKE_FUNCTION            0
                        18 STORE_NAME               4 (_get_default_expiration)
          
-         1179          20 PUSH_NULL
+         1184          20 PUSH_NULL
                        22 LOAD_NAME                5 (models)
                        24 LOAD_ATTR                6 (ForeignKey)
          
-         1180          34 LOAD_NAME                7 (Person)
+         1185          34 LOAD_NAME                7 (Person)
          
-         1181          36 LOAD_NAME                5 (models)
+         1186          36 LOAD_NAME                5 (models)
                        38 LOAD_ATTR                8 (CASCADE)
          
-         1182          48 LOAD_CONST               3 (True)
+         1187          48 LOAD_CONST               3 (True)
          
-         1183          50 LOAD_CONST               3 (True)
+         1188          50 LOAD_CONST               3 (True)
          
-         1184          52 PUSH_NULL
+         1189          52 PUSH_NULL
                        54 LOAD_NAME                9 (_)
                        56 LOAD_CONST               4 ('Owner')
                        58 PRECALL                  1
                        62 CALL                     1
          
-         1185          72 LOAD_CONST               5 ('pdf_files')
+         1190          72 LOAD_CONST               5 ('pdf_files')
          
-         1179          74 KW_NAMES                 6
+         1184          74 KW_NAMES                 6
                        76 PRECALL                  6
                        80 CALL                     6
                        90 STORE_NAME              10 (person)
          
-         1187          92 PUSH_NULL
+         1192          92 PUSH_NULL
                        94 LOAD_NAME                5 (models)
                        96 LOAD_ATTR               11 (DateTimeField)
          
-         1188         106 PUSH_NULL
+         1193         106 PUSH_NULL
                       108 LOAD_NAME                9 (_)
                       110 LOAD_CONST               7 ('File expires at')
                       112 PRECALL                  1
                       116 CALL                     1
                       126 LOAD_NAME                4 (_get_default_expiration)
          
-         1187         128 KW_NAMES                 8
+         1192         128 KW_NAMES                 8
                       130 PRECALL                  2
                       134 CALL                     2
                       144 STORE_NAME              12 (expires_at)
          
-         1190         146 PUSH_NULL
+         1195         146 PUSH_NULL
                       148 LOAD_NAME                5 (models)
                       150 LOAD_ATTR               13 (FileField)
          
-         1191         160 LOAD_CONST               9 ('pdfs/')
+         1196         160 LOAD_CONST               9 ('pdfs/')
                       162 PUSH_NULL
                       164 LOAD_NAME                9 (_)
                       166 LOAD_CONST              10 ('Generated HTML file')
                       168 PRECALL                  1
                       172 CALL                     1
                       182 LOAD_CONST               3 (True)
                       184 LOAD_CONST               3 (True)
          
-         1190         186 KW_NAMES                11
+         1195         186 KW_NAMES                11
                       188 PRECALL                  4
                       192 CALL                     4
                       202 STORE_NAME              14 (html_file)
          
-         1193         204 PUSH_NULL
+         1198         204 PUSH_NULL
                       206 LOAD_NAME                5 (models)
                       208 LOAD_ATTR               13 (FileField)
          
-         1194         218 LOAD_CONST               9 ('pdfs/')
+         1199         218 LOAD_CONST               9 ('pdfs/')
                       220 LOAD_CONST               3 (True)
                       222 LOAD_CONST               3 (True)
                       224 PUSH_NULL
                       226 LOAD_NAME                9 (_)
                       228 LOAD_CONST              12 ('Generated PDF file')
                       230 PRECALL                  1
                       234 CALL                     1
          
-         1193         244 KW_NAMES                13
+         1198         244 KW_NAMES                13
                       246 PRECALL                  4
                       250 CALL                     4
                       260 STORE_NAME              15 (file)
          
-         1197         262 LOAD_CONST              14 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1197>)
+         1202         262 LOAD_CONST              14 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1202>)
                       264 MAKE_FUNCTION            0
                       266 STORE_NAME              16 (__str__)
          
-         1200         268 PUSH_NULL
+         1205         268 PUSH_NULL
                       270 LOAD_BUILD_CLASS
-                      272 LOAD_CONST              15 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1200>)
+                      272 LOAD_CONST              15 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1205>)
                       274 MAKE_FUNCTION            0
                       276 LOAD_CONST              16 ('Meta')
                       278 PRECALL                  2
                       282 CALL                     2
                       292 STORE_NAME              17 (Meta)
                       294 LOAD_CONST              17 (None)
                       296 RETURN_VALUE
@@ -9380,17 +9395,17 @@
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a010000000000000000a6000000ab
                   000000000000000000740500000000000000000000740700000000000000
                   000000a6000000ab000000000000000000640119000000000000000000ac
                   02a6010000ab0100000000000000007a0000005300
-               1176           0 RESUME                   0
+               1181           0 RESUME                   0
                
-               1177           2 LOAD_GLOBAL              1 (NULL + timezone)
+               1182           2 LOAD_GLOBAL              1 (NULL + timezone)
                              14 LOAD_ATTR                1 (now)
                              24 PRECALL                  0
                              28 CALL                     0
                              38 LOAD_GLOBAL              5 (NULL + timedelta)
                              50 LOAD_GLOBAL              7 (NULL + get_site_preferences)
                              62 PRECALL                  0
                              66 CALL                     0
@@ -9407,15 +9422,15 @@
                   ('minutes',)
                names      ('timezone', 'now', 'timedelta', 'get_site_preferences')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '_get_default_expiration'
-               firstlineno 1176
+               firstlineno 1181
                lnotab 0x0201
             True
             'Owner'
             'pdf_files'
             ('to', 'on_delete', 'blank', 'null', 'verbose_name', 'related_name')
             'File expires at'
             ('verbose_name', 'default')
@@ -9428,17 +9443,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064029d045300
-               1197           0 RESUME                   0
+               1202           0 RESUME                   0
                
-               1198           2 LOAD_FAST                0 (self)
+               1203           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (person)
                              14 FORMAT_VALUE             0
                              16 LOAD_CONST               1 (' (')
                              18 LOAD_FAST                0 (self)
                              20 LOAD_ATTR                1 (pk)
                              30 FORMAT_VALUE             0
                              32 LOAD_CONST               2 (')')
@@ -9450,38 +9465,38 @@
                   ')'
                names      ('person', 'pk')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1197
+               firstlineno 1202
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               1200           0 RESUME                   0
+               1205           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('PDFFile.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1201          10 PUSH_NULL
+               1206          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('PDF file')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1202          32 PUSH_NULL
+               1207          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('PDF files')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                              54 LOAD_CONST               3 (None)
                              56 RETURN_VALUE
@@ -9492,25 +9507,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1200
+               firstlineno 1205
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', '_get_default_expiration', 'models', 'ForeignKey', 'Person', 'CASCADE', '_', 'person', 'DateTimeField', 'expires_at', 'FileField', 'html_file', 'file', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'PDFFile'
-         firstlineno 1173
+         firstlineno 1178
          lnotab
             0x0a01040206030e0102010c0102010201140102fa12080e0116ff12030e
             011aff12030e011aff12040603
       'PDFFile'
       code
          argcount  : 0
          nlocals   : 0
@@ -9542,264 +9557,264 @@
             00000000006412020065076413a6010000ab010000000000000000ac14a6
             020000ab0200000000000000005a1865196415651a641664176418640066
             0664198404a6000000ab0000000000000000005a1b6418651c651a651d66
             02190000000000000000006602641a84045a1e6418651c651a651d660219
             0000000000000000006602641b84045a1f64186520652119000000000000
             0000006602641c84045a226418651a6602641d84045a2302004700641e84
             00641fa6020000ab0200000000000000005a2464205300
-         1205           0 RESUME                   0
+         1210           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('TaskUserAssignment')
                         8 STORE_NAME               2 (__qualname__)
          
-         1206          10 PUSH_NULL
+         1211          10 PUSH_NULL
                        12 LOAD_NAME                3 (models)
                        14 LOAD_ATTR                4 (ForeignKey)
          
-         1207          24 LOAD_NAME                5 (TaskResult)
+         1212          24 LOAD_NAME                5 (TaskResult)
                        26 LOAD_NAME                3 (models)
                        28 LOAD_ATTR                6 (CASCADE)
                        38 PUSH_NULL
                        40 LOAD_NAME                7 (_)
                        42 LOAD_CONST               1 ('Task result')
                        44 PRECALL                  1
                        48 CALL                     1
          
-         1206          58 KW_NAMES                 2
+         1211          58 KW_NAMES                 2
                        60 PRECALL                  3
                        64 CALL                     3
                        74 STORE_NAME               8 (task_result)
          
-         1209          76 PUSH_NULL
+         1214          76 PUSH_NULL
                        78 LOAD_NAME                3 (models)
                        80 LOAD_ATTR                4 (ForeignKey)
          
-         1210          90 PUSH_NULL
+         1215          90 PUSH_NULL
                        92 LOAD_NAME                9 (get_user_model)
                        94 PRECALL                  0
                        98 CALL                     0
                       108 LOAD_NAME                3 (models)
                       110 LOAD_ATTR                6 (CASCADE)
                       120 PUSH_NULL
                       122 LOAD_NAME                7 (_)
                       124 LOAD_CONST               3 ('Task user')
                       126 PRECALL                  1
                       130 CALL                     1
          
-         1209         140 KW_NAMES                 2
+         1214         140 KW_NAMES                 2
                       142 PRECALL                  3
                       146 CALL                     3
                       156 STORE_NAME              10 (user)
          
-         1213         158 PUSH_NULL
+         1218         158 PUSH_NULL
                       160 LOAD_NAME                3 (models)
                       162 LOAD_ATTR               11 (CharField)
                       172 LOAD_CONST               4 (255)
                       174 PUSH_NULL
                       176 LOAD_NAME                7 (_)
                       178 LOAD_CONST               5 ('Title')
                       180 PRECALL                  1
                       184 CALL                     1
                       194 KW_NAMES                 6
                       196 PRECALL                  2
                       200 CALL                     2
                       210 STORE_NAME              12 (title)
          
-         1214         212 PUSH_NULL
+         1219         212 PUSH_NULL
                       214 LOAD_NAME                3 (models)
                       216 LOAD_ATTR               13 (URLField)
                       226 PUSH_NULL
                       228 LOAD_NAME                7 (_)
                       230 LOAD_CONST               7 ('Back URL')
                       232 PRECALL                  1
                       236 CALL                     1
                       246 LOAD_CONST               8 (True)
                       248 KW_NAMES                 9
                       250 PRECALL                  2
                       254 CALL                     2
                       264 STORE_NAME              14 (back_url)
          
-         1215         266 PUSH_NULL
+         1220         266 PUSH_NULL
                       268 LOAD_NAME                3 (models)
                       270 LOAD_ATTR               11 (CharField)
                       280 LOAD_CONST               4 (255)
                       282 PUSH_NULL
                       284 LOAD_NAME                7 (_)
                       286 LOAD_CONST              10 ('Progress title')
                       288 PRECALL                  1
                       292 CALL                     1
                       302 LOAD_CONST               8 (True)
                       304 KW_NAMES                11
                       306 PRECALL                  3
                       310 CALL                     3
                       320 STORE_NAME              15 (progress_title)
          
-         1216         322 PUSH_NULL
+         1221         322 PUSH_NULL
                       324 LOAD_NAME                3 (models)
                       326 LOAD_ATTR               16 (TextField)
                       336 PUSH_NULL
                       338 LOAD_NAME                7 (_)
                       340 LOAD_CONST              12 ('Error message')
                       342 PRECALL                  1
                       346 CALL                     1
                       356 LOAD_CONST               8 (True)
                       358 KW_NAMES                 9
                       360 PRECALL                  2
                       364 CALL                     2
                       374 STORE_NAME              17 (error_message)
          
-         1217         376 PUSH_NULL
+         1222         376 PUSH_NULL
                       378 LOAD_NAME                3 (models)
                       380 LOAD_ATTR               16 (TextField)
                       390 PUSH_NULL
                       392 LOAD_NAME                7 (_)
                       394 LOAD_CONST              13 ('Success message')
                       396 PRECALL                  1
                       400 CALL                     1
                       410 LOAD_CONST               8 (True)
                       412 KW_NAMES                 9
                       414 PRECALL                  2
                       418 CALL                     2
                       428 STORE_NAME              18 (success_message)
          
-         1218         430 PUSH_NULL
+         1223         430 PUSH_NULL
                       432 LOAD_NAME                3 (models)
                       434 LOAD_ATTR               13 (URLField)
                       444 PUSH_NULL
                       446 LOAD_NAME                7 (_)
                       448 LOAD_CONST              14 ('Redirect on success URL')
                       450 PRECALL                  1
                       454 CALL                     1
                       464 LOAD_CONST               8 (True)
                       466 KW_NAMES                 9
                       468 PRECALL                  2
                       472 CALL                     2
                       482 STORE_NAME              19 (redirect_on_success_url)
          
-         1219         484 PUSH_NULL
+         1224         484 PUSH_NULL
                       486 LOAD_NAME                3 (models)
                       488 LOAD_ATTR               11 (CharField)
          
-         1220         498 LOAD_CONST               4 (255)
+         1225         498 LOAD_CONST               4 (255)
                       500 PUSH_NULL
                       502 LOAD_NAME                7 (_)
                       504 LOAD_CONST              15 ('Additional button title')
                       506 PRECALL                  1
                       510 CALL                     1
                       520 LOAD_CONST               8 (True)
          
-         1219         522 KW_NAMES                11
+         1224         522 KW_NAMES                11
                       524 PRECALL                  3
                       528 CALL                     3
                       538 STORE_NAME              20 (additional_button_title)
          
-         1222         540 PUSH_NULL
+         1227         540 PUSH_NULL
                       542 LOAD_NAME                3 (models)
                       544 LOAD_ATTR               13 (URLField)
                       554 PUSH_NULL
                       556 LOAD_NAME                7 (_)
                       558 LOAD_CONST              16 ('Additional button URL')
                       560 PRECALL                  1
                       564 CALL                     1
                       574 LOAD_CONST               8 (True)
                       576 KW_NAMES                 9
                       578 PRECALL                  2
                       582 CALL                     2
                       592 STORE_NAME              21 (additional_button_url)
          
-         1223         594 PUSH_NULL
+         1228         594 PUSH_NULL
                       596 LOAD_NAME                3 (models)
                       598 LOAD_ATTR               11 (CharField)
          
-         1224         608 LOAD_CONST               4 (255)
+         1229         608 LOAD_CONST               4 (255)
                       610 PUSH_NULL
                       612 LOAD_NAME                7 (_)
                       614 LOAD_CONST              17 ('Additional button icon')
                       616 PRECALL                  1
                       620 CALL                     1
                       630 LOAD_CONST               8 (True)
          
-         1223         632 KW_NAMES                11
+         1228         632 KW_NAMES                11
                       634 PRECALL                  3
                       638 CALL                     3
                       648 STORE_NAME              22 (additional_button_icon)
          
-         1226         650 PUSH_NULL
+         1231         650 PUSH_NULL
                       652 LOAD_NAME                3 (models)
                       654 LOAD_ATTR               23 (BooleanField)
                       664 LOAD_CONST              18 (False)
                       666 PUSH_NULL
                       668 LOAD_NAME                7 (_)
                       670 LOAD_CONST              19 ('Result fetched')
                       672 PRECALL                  1
                       676 CALL                     1
                       686 KW_NAMES                20
                       688 PRECALL                  2
                       692 CALL                     2
                       702 STORE_NAME              24 (result_fetched)
          
-         1228         704 LOAD_NAME               25 (classmethod)
+         1233         704 LOAD_NAME               25 (classmethod)
          
-         1229         706 LOAD_CONST              21 ('task_id')
+         1234         706 LOAD_CONST              21 ('task_id')
                       708 LOAD_NAME               26 (str)
                       710 LOAD_CONST              22 ('user')
                       712 LOAD_CONST              23 ('User')
                       714 LOAD_CONST              24 ('return')
                       716 LOAD_CONST               0 ('TaskUserAssignment')
                       718 BUILD_TUPLE              6
-                      720 LOAD_CONST              25 (<code object create_for_task_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1228>)
+                      720 LOAD_CONST              25 (<code object create_for_task_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1233>)
                       722 MAKE_FUNCTION            4 (annotations)
          
-         1228         724 PRECALL                  0
+         1233         724 PRECALL                  0
                       728 CALL                     0
          
-         1229         738 STORE_NAME              27 (create_for_task_id)
+         1234         738 STORE_NAME              27 (create_for_task_id)
          
-         1236         740 LOAD_CONST              24 ('return')
+         1241         740 LOAD_CONST              24 ('return')
                       742 LOAD_NAME               28 (dict)
                       744 LOAD_NAME               26 (str)
                       746 LOAD_NAME               29 (any)
                       748 BUILD_TUPLE              2
                       750 BINARY_SUBSCR
                       760 BUILD_TUPLE              2
-                      762 LOAD_CONST              26 (<code object get_progress, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1236>)
+                      762 LOAD_CONST              26 (<code object get_progress, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1241>)
                       764 MAKE_FUNCTION            4 (annotations)
                       766 STORE_NAME              30 (get_progress)
          
-         1241         768 LOAD_CONST              24 ('return')
+         1246         768 LOAD_CONST              24 ('return')
                       770 LOAD_NAME               28 (dict)
                       772 LOAD_NAME               26 (str)
                       774 LOAD_NAME               29 (any)
                       776 BUILD_TUPLE              2
                       778 BINARY_SUBSCR
                       788 BUILD_TUPLE              2
-                      790 LOAD_CONST              27 (<code object get_progress_with_meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1241>)
+                      790 LOAD_CONST              27 (<code object get_progress_with_meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1246>)
                       792 MAKE_FUNCTION            4 (annotations)
                       794 STORE_NAME              31 (get_progress_with_meta)
          
-         1247         796 LOAD_CONST              24 ('return')
+         1252         796 LOAD_CONST              24 ('return')
                       798 LOAD_NAME               32 (Optional)
                       800 LOAD_NAME               33 (Notification)
                       802 BINARY_SUBSCR
                       812 BUILD_TUPLE              2
-                      814 LOAD_CONST              28 (<code object create_notification, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1247>)
+                      814 LOAD_CONST              28 (<code object create_notification, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1252>)
                       816 MAKE_FUNCTION            4 (annotations)
                       818 STORE_NAME              34 (create_notification)
          
-         1278         820 LOAD_CONST              24 ('return')
+         1283         820 LOAD_CONST              24 ('return')
                       822 LOAD_NAME               26 (str)
                       824 BUILD_TUPLE              2
-                      826 LOAD_CONST              29 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1278>)
+                      826 LOAD_CONST              29 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1283>)
                       828 MAKE_FUNCTION            4 (annotations)
                       830 STORE_NAME              35 (get_absolute_url)
          
-         1281         832 PUSH_NULL
+         1286         832 PUSH_NULL
                       834 LOAD_BUILD_CLASS
-                      836 LOAD_CONST              30 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1281>)
+                      836 LOAD_CONST              30 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1286>)
                       838 MAKE_FUNCTION            0
                       840 LOAD_CONST              31 ('Meta')
                       842 PRECALL                  2
                       846 CALL                     2
                       856 STORE_NAME              36 (Meta)
                       858 LOAD_CONST              32 (None)
                       860 RETURN_VALUE
@@ -9838,34 +9853,34 @@
                   0x9700740100000000000000000000a6000000ab00000000000000000035
                   0001007402000000000000000000006a020000000000000000a003000000
                   00000000000000000000000000000000007c01ac01a6010000ab01000000
                   00000000005c0200007d037d04640064006400a6020000ab020000000000
                   00000001006e0b230031007304770278035900770101005900010001007c
                   006a020000000000000000a0040000000000000000000000000000000000
                   0000007c037c02ac02a6020000ab0200000000000000005300
-               1228           0 RESUME                   0
+               1233           0 RESUME                   0
                
-               1232           2 LOAD_GLOBAL              1 (NULL + cachalot_disabled)
+               1237           2 LOAD_GLOBAL              1 (NULL + cachalot_disabled)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 BEFORE_WITH
                              30 POP_TOP
                
-               1233          32 LOAD_GLOBAL              2 (TaskResult)
+               1238          32 LOAD_GLOBAL              2 (TaskResult)
                              44 LOAD_ATTR                2 (objects)
                              54 LOAD_METHOD              3 (get_or_create)
                              76 LOAD_FAST                1 (task_id)
                              78 KW_NAMES                 1
                              80 PRECALL                  1
                              84 CALL                     1
                              94 UNPACK_SEQUENCE          2
                              98 STORE_FAST               3 (result)
                             100 STORE_FAST               4 (__)
                
-               1232         102 LOAD_CONST               0 (None)
+               1237         102 LOAD_CONST               0 (None)
                             104 LOAD_CONST               0 (None)
                             106 LOAD_CONST               0 (None)
                             108 PRECALL                  2
                             112 CALL                     2
                             122 POP_TOP
                             124 JUMP_FORWARD            11 (to 148)
                         >>  126 PUSH_EXC_INFO
@@ -9876,15 +9891,15 @@
                             136 POP_EXCEPT
                             138 RERAISE                  1
                         >>  140 POP_TOP
                             142 POP_EXCEPT
                             144 POP_TOP
                             146 POP_TOP
                
-               1234     >>  148 LOAD_FAST                0 (cls)
+               1239     >>  148 LOAD_FAST                0 (cls)
                             150 LOAD_ATTR                2 (objects)
                             160 LOAD_METHOD              4 (create)
                             182 LOAD_FAST                3 (result)
                             184 LOAD_FAST                2 (user)
                             186 KW_NAMES                 2
                             188 PRECALL                  2
                             192 CALL                     2
@@ -9899,87 +9914,87 @@
                   ('task_result', 'user')
                names      ('cachalot_disabled', 'TaskResult', 'objects', 'get_or_create', 'create')
                varnames   ('cls', 'task_id', 'user', 'result', '__')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'create_for_task_id'
-               firstlineno 1228
+               firstlineno 1233
                lnotab 0x02041e0146ff2e02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007403000000000000000000007c006a
                   0200000000000000006a030000000000000000a6010000ab010000000000
                   000000a6010000ab0100000000000000007d017c01a00400000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-               1236           0 RESUME                   0
+               1241           0 RESUME                   0
                
-               1238           2 LOAD_GLOBAL              1 (NULL + Progress)
+               1243           2 LOAD_GLOBAL              1 (NULL + Progress)
                              14 LOAD_GLOBAL              3 (NULL + AsyncResult)
                              26 LOAD_FAST                0 (self)
                              28 LOAD_ATTR                2 (task_result)
                              38 LOAD_ATTR                3 (task_id)
                              48 PRECALL                  1
                              52 CALL                     1
                              62 PRECALL                  1
                              66 CALL                     1
                              76 STORE_FAST               1 (progress)
                
-               1239          78 LOAD_FAST                1 (progress)
+               1244          78 LOAD_FAST                1 (progress)
                              80 LOAD_METHOD              4 (get_info)
                             102 PRECALL                  0
                             106 CALL                     0
                             116 RETURN_VALUE
                consts
                   'Get progress information for this task.'
                names      ('Progress', 'AsyncResult', 'task_result', 'task_id', 'get_info')
                varnames   ('self', 'progress')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_progress'
-               firstlineno 1236
+               firstlineno 1241
                lnotab 0x02024c01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d017c007c0164013c0000007c015300
-               1241           0 RESUME                   0
+               1246           0 RESUME                   0
                
-               1243           2 LOAD_FAST                0 (self)
+               1248           2 LOAD_FAST                0 (self)
                               4 LOAD_METHOD              0 (get_progress)
                              26 PRECALL                  0
                              30 CALL                     0
                              40 STORE_FAST               1 (progress)
                
-               1244          42 LOAD_FAST                0 (self)
+               1249          42 LOAD_FAST                0 (self)
                              44 LOAD_FAST                1 (progress)
                              46 LOAD_CONST               1 ('meta')
                              48 STORE_SUBSCR
                
-               1245          52 LOAD_FAST                1 (progress)
+               1250          52 LOAD_FAST                1 (progress)
                              54 RETURN_VALUE
                consts
                   'Get progress information for this task.'
                   'meta'
                names      ('get_progress',)
                varnames   ('self', 'progress')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_progress_with_meta'
-               firstlineno 1241
+               firstlineno 1246
                lnotab 0x020228010a01
             code
                argcount  : 1
                nlocals   : 7
                stacksize : 8
                flags     : 3
                code
@@ -9998,125 +10013,125 @@
                   070000000000000000000000000000000000000000a6000000ab00000000
                   0000000000a6020000ab0200000000000000007d05741100000000000000
                   000000740300000000000000000000640ba6010000ab0100000000000000
                   007c006a0900000000000000006a0a00000000000000007c027c037c057c
                   04ac0ca6060000ab0600000000000000007d067c06a00b00000000000000
                   00000000000000000000000000a6000000ab00000000000000000001007c
                   065300
-               1247           0 RESUME                   0
+               1252           0 RESUME                   0
                
-               1249           2 LOAD_FAST                0 (self)
+               1254           2 LOAD_FAST                0 (self)
                               4 LOAD_METHOD              0 (get_progress)
                              26 PRECALL                  0
                              30 CALL                     0
                              40 STORE_FAST               1 (progress)
                
-               1250          42 LOAD_FAST                1 (progress)
+               1255          42 LOAD_FAST                1 (progress)
                              44 LOAD_CONST               1 ('state')
                              46 BINARY_SUBSCR
                              56 LOAD_CONST               2 ('SUCCESS')
                              58 COMPARE_OP               2 (==)
                              64 POP_JUMP_FORWARD_IF_FALSE    57 (to 180)
                
-               1251          66 LOAD_GLOBAL              3 (NULL + _)
+               1256          66 LOAD_GLOBAL              3 (NULL + _)
                              78 LOAD_CONST               3 ('Background task completed successfully')
                              80 PRECALL                  1
                              84 CALL                     1
                              94 STORE_FAST               2 (title)
                
-               1252          96 LOAD_GLOBAL              3 (NULL + _)
+               1257          96 LOAD_GLOBAL              3 (NULL + _)
                             108 LOAD_CONST               4 ("The background task '{}' has been completed successfully.")
                             110 PRECALL                  1
                             114 CALL                     1
                             124 LOAD_METHOD              2 (format)
                
-               1253         146 LOAD_FAST                0 (self)
+               1258         146 LOAD_FAST                0 (self)
                             148 LOAD_ATTR                3 (title)
                
-               1252         158 PRECALL                  1
+               1257         158 PRECALL                  1
                             162 CALL                     1
                             172 STORE_FAST               3 (description)
                
-               1255         174 LOAD_CONST               5 ('check-circle-outline')
+               1260         174 LOAD_CONST               5 ('check-circle-outline')
                             176 STORE_FAST               4 (icon)
                             178 JUMP_FORWARD            71 (to 322)
                
-               1257     >>  180 LOAD_FAST                1 (progress)
+               1262     >>  180 LOAD_FAST                1 (progress)
                             182 LOAD_CONST               1 ('state')
                             184 BINARY_SUBSCR
                             194 LOAD_CONST               6 ('FAILURE')
                             196 COMPARE_OP               2 (==)
                             202 POP_JUMP_FORWARD_IF_FALSE    57 (to 318)
                
-               1258         204 LOAD_GLOBAL              3 (NULL + _)
+               1263         204 LOAD_GLOBAL              3 (NULL + _)
                             216 LOAD_CONST               7 ('Background task failed')
                             218 PRECALL                  1
                             222 CALL                     1
                             232 STORE_FAST               2 (title)
                
-               1259         234 LOAD_GLOBAL              3 (NULL + _)
+               1264         234 LOAD_GLOBAL              3 (NULL + _)
                             246 LOAD_CONST               8 ("The background task '{}' has failed.")
                             248 PRECALL                  1
                             252 CALL                     1
                             262 LOAD_METHOD              2 (format)
                             284 LOAD_FAST                0 (self)
                             286 LOAD_ATTR                3 (title)
                             296 PRECALL                  1
                             300 CALL                     1
                             310 STORE_FAST               3 (description)
                
-               1260         312 LOAD_CONST               9 ('alert-octagon-outline')
+               1265         312 LOAD_CONST               9 ('alert-octagon-outline')
                             314 STORE_FAST               4 (icon)
                             316 JUMP_FORWARD             2 (to 322)
                
-               1263     >>  318 LOAD_CONST              10 (None)
+               1268     >>  318 LOAD_CONST              10 (None)
                             320 RETURN_VALUE
                
-               1265     >>  322 LOAD_GLOBAL              9 (NULL + urljoin)
+               1270     >>  322 LOAD_GLOBAL              9 (NULL + urljoin)
                             334 LOAD_GLOBAL             10 (settings)
                             346 LOAD_ATTR                6 (BASE_URL)
                             356 LOAD_FAST                0 (self)
                             358 LOAD_METHOD              7 (get_absolute_url)
                             380 PRECALL                  0
                             384 CALL                     0
                             394 PRECALL                  2
                             398 CALL                     2
                             408 STORE_FAST               5 (link)
                
-               1267         410 LOAD_GLOBAL             17 (NULL + Notification)
+               1272         410 LOAD_GLOBAL             17 (NULL + Notification)
                
-               1268         422 LOAD_GLOBAL              3 (NULL + _)
+               1273         422 LOAD_GLOBAL              3 (NULL + _)
                             434 LOAD_CONST              11 ('Background task')
                             436 PRECALL                  1
                             440 CALL                     1
                
-               1269         450 LOAD_FAST                0 (self)
+               1274         450 LOAD_FAST                0 (self)
                             452 LOAD_ATTR                9 (user)
                             462 LOAD_ATTR               10 (person)
                
-               1270         472 LOAD_FAST                2 (title)
+               1275         472 LOAD_FAST                2 (title)
                
-               1271         474 LOAD_FAST                3 (description)
+               1276         474 LOAD_FAST                3 (description)
                
-               1272         476 LOAD_FAST                5 (link)
+               1277         476 LOAD_FAST                5 (link)
                
-               1273         478 LOAD_FAST                4 (icon)
+               1278         478 LOAD_FAST                4 (icon)
                
-               1267         480 KW_NAMES                12
+               1272         480 KW_NAMES                12
                             482 PRECALL                  6
                             486 CALL                     6
                             496 STORE_FAST               6 (notification)
                
-               1275         498 LOAD_FAST                6 (notification)
+               1280         498 LOAD_FAST                6 (notification)
                             500 LOAD_METHOD             11 (save)
                             522 PRECALL                  0
                             526 CALL                     0
                             536 POP_TOP
                
-               1276         538 LOAD_FAST                6 (notification)
+               1281         538 LOAD_FAST                6 (notification)
                             540 RETURN_VALUE
                consts
                   'Create a notification for this task.'
                   'state'
                   'SUCCESS'
                   'Background task completed successfully'
                   "The background task '{}' has been completed successfully."
@@ -10130,29 +10145,29 @@
                   ('sender', 'recipient', 'title', 'description', 'link', 'icon')
                names      ('get_progress', '_', 'format', 'title', 'urljoin', 'settings', 'BASE_URL', 'get_absolute_url', 'Notification', 'user', 'person', 'save')
                varnames   ('self', 'progress', 'title', 'description', 'icon', 'link', 'notification')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'create_notification'
-               firstlineno 1247
+               firstlineno 1252
                lnotab
                   0x0202280118011e0132010cff1003060218011e014e010603040258020c
                   011c01160102010201020102fa12082801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x970064017c006a0000000000000000006a0100000000000000009b009d
                   025300
-               1278           0 RESUME                   0
+               1283           0 RESUME                   0
                
-               1279           2 LOAD_CONST               1 ('/celery_progress/')
+               1284           2 LOAD_CONST               1 ('/celery_progress/')
                               4 LOAD_FAST                0 (self)
                               6 LOAD_ATTR                0 (task_result)
                              16 LOAD_ATTR                1 (task_id)
                              26 FORMAT_VALUE             0
                              28 BUILD_STRING             2
                              30 RETURN_VALUE
                consts
@@ -10160,38 +10175,38 @@
                   '/celery_progress/'
                names      ('task_result', 'task_id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_absolute_url'
-               firstlineno 1278
+               firstlineno 1283
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               1281           0 RESUME                   0
+               1286           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('TaskUserAssignment.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1282          10 PUSH_NULL
+               1287          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('Task user assignment')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1283          32 PUSH_NULL
+               1288          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('Task user assignments')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                              54 LOAD_CONST               3 (None)
                              56 RETURN_VALUE
@@ -10202,25 +10217,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1281
+               firstlineno 1286
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'TaskResult', 'CASCADE', '_', 'task_result', 'get_user_model', 'user', 'CharField', 'title', 'URLField', 'back_url', 'progress_title', 'TextField', 'error_message', 'success_message', 'redirect_on_success_url', 'additional_button_title', 'additional_button_url', 'additional_button_icon', 'BooleanField', 'result_fetched', 'classmethod', 'str', 'create_for_task_id', 'dict', 'any', 'get_progress', 'get_progress_with_meta', 'Optional', 'Notification', 'create_notification', 'get_absolute_url', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'TaskUserAssignment'
-         firstlineno 1205
+         firstlineno 1210
          lnotab
             0x0a010e0122ff12030e0132ff12043601360138013601360136010e0118
             ff120336010e0118ff12033602020112ff0e0102071c051c06181f0c03
       'TaskUserAssignment'
       code
          argcount  : 0
          nlocals   : 0
@@ -10232,114 +10247,114 @@
             02020065086403a6010000ab010000000000000000ac04a6040000ab0400
             000000000000005a09020065046a0a0000000000000000020065086405a6
             010000ab010000000000000000650bac06a6020000ab0200000000000000
             005a0c640784005a0d650e090064106409650f640a650f640b6510651119
             000000000000000000640c65116608640d8405a6000000ab000000000000
             0000005a12650e6409650f640a650f640e65116606640f8404a6000000ab
             0000000000000000005a1364085300
-         1286           0 RESUME                   0
+         1291           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('UserAdditionalAttributes')
                         8 STORE_NAME               2 (__qualname__)
          
-         1287          10 LOAD_CONST               1 ('Additional attributes for Django user accounts.\n\n    These attributes are explicitly linked to a User, not to a Person.\n    ')
+         1292          10 LOAD_CONST               1 ('Additional attributes for Django user accounts.\n\n    These attributes are explicitly linked to a User, not to a Person.\n    ')
                        12 STORE_NAME               3 (__doc__)
          
-         1292          14 PUSH_NULL
+         1297          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (OneToOneField)
          
-         1293          28 PUSH_NULL
+         1298          28 PUSH_NULL
                        30 LOAD_NAME                6 (get_user_model)
                        32 PRECALL                  0
                        36 CALL                     0
          
-         1294          46 LOAD_NAME                4 (models)
+         1299          46 LOAD_NAME                4 (models)
                        48 LOAD_ATTR                7 (CASCADE)
          
-         1295          58 LOAD_CONST               2 ('additional_attributes')
+         1300          58 LOAD_CONST               2 ('additional_attributes')
          
-         1296          60 PUSH_NULL
+         1301          60 PUSH_NULL
                        62 LOAD_NAME                8 (_)
                        64 LOAD_CONST               3 ('Linked user')
                        66 PRECALL                  1
                        70 CALL                     1
          
-         1292          80 KW_NAMES                 4
+         1297          80 KW_NAMES                 4
                        82 PRECALL                  4
                        86 CALL                     4
                        96 STORE_NAME               9 (user)
          
-         1299          98 PUSH_NULL
+         1304          98 PUSH_NULL
                       100 LOAD_NAME                4 (models)
                       102 LOAD_ATTR               10 (JSONField)
                       112 PUSH_NULL
                       114 LOAD_NAME                8 (_)
                       116 LOAD_CONST               5 ('Additional attributes')
                       118 PRECALL                  1
                       122 CALL                     1
                       132 LOAD_NAME               11 (dict)
                       134 KW_NAMES                 6
                       136 PRECALL                  2
                       140 CALL                     2
                       150 STORE_NAME              12 (attributes)
          
-         1301         152 LOAD_CONST               7 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1301>)
+         1306         152 LOAD_CONST               7 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1306>)
                       154 MAKE_FUNCTION            0
                       156 STORE_NAME              13 (__str__)
          
-         1304         158 LOAD_NAME               14 (classmethod)
+         1309         158 LOAD_NAME               14 (classmethod)
          
-         1306         160 NOP
+         1311         160 NOP
          
-         1305         162 LOAD_CONST              16 ((None,))
+         1310         162 LOAD_CONST              16 ((None,))
                       164 LOAD_CONST               9 ('username')
          
-         1306         166 LOAD_NAME               15 (str)
+         1311         166 LOAD_NAME               15 (str)
          
-         1305         168 LOAD_CONST              10 ('attribute')
+         1310         168 LOAD_CONST              10 ('attribute')
          
-         1306         170 LOAD_NAME               15 (str)
+         1311         170 LOAD_NAME               15 (str)
          
-         1305         172 LOAD_CONST              11 ('default')
+         1310         172 LOAD_CONST              11 ('default')
          
-         1306         174 LOAD_NAME               16 (Optional)
+         1311         174 LOAD_NAME               16 (Optional)
                       176 LOAD_NAME               17 (Any)
                       178 BINARY_SUBSCR
          
-         1305         188 LOAD_CONST              12 ('return')
+         1310         188 LOAD_CONST              12 ('return')
          
-         1307         190 LOAD_NAME               17 (Any)
+         1312         190 LOAD_NAME               17 (Any)
          
-         1305         192 BUILD_TUPLE              8
-                      194 LOAD_CONST              13 (<code object get_user_attribute, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1304>)
+         1310         192 BUILD_TUPLE              8
+                      194 LOAD_CONST              13 (<code object get_user_attribute, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1309>)
                       196 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1304         198 PRECALL                  0
+         1309         198 PRECALL                  0
                       202 CALL                     0
          
-         1305         212 STORE_NAME              18 (get_user_attribute)
+         1310         212 STORE_NAME              18 (get_user_attribute)
          
-         1316         214 LOAD_NAME               14 (classmethod)
+         1321         214 LOAD_NAME               14 (classmethod)
          
-         1317         216 LOAD_CONST               9 ('username')
+         1322         216 LOAD_CONST               9 ('username')
                       218 LOAD_NAME               15 (str)
                       220 LOAD_CONST              10 ('attribute')
                       222 LOAD_NAME               15 (str)
                       224 LOAD_CONST              14 ('value')
                       226 LOAD_NAME               17 (Any)
                       228 BUILD_TUPLE              6
-                      230 LOAD_CONST              15 (<code object set_user_attribute, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1316>)
+                      230 LOAD_CONST              15 (<code object set_user_attribute, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1321>)
                       232 MAKE_FUNCTION            4 (annotations)
          
-         1316         234 PRECALL                  0
+         1321         234 PRECALL                  0
                       238 CALL                     0
          
-         1317         248 STORE_NAME              19 (set_user_attribute)
+         1322         248 STORE_NAME              19 (set_user_attribute)
                       250 LOAD_CONST               8 (None)
                       252 RETURN_VALUE
          consts
             'UserAdditionalAttributes'
             'Additional attributes for Django user accounts.\n\n    These attributes are explicitly linked to a User, not to a Person.\n    '
             'additional_attributes'
             'Linked user'
@@ -10350,31 +10365,31 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-               1301           0 RESUME                   0
+               1306           0 RESUME                   0
                
-               1302           2 LOAD_GLOBAL              1 (NULL + str)
+               1307           2 LOAD_GLOBAL              1 (NULL + str)
                              14 LOAD_FAST                0 (self)
                              16 LOAD_ATTR                1 (user)
                              26 PRECALL                  1
                              30 CALL                     1
                              40 RETURN_VALUE
                consts
                   None
                names      ('str', 'user')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1301
+               firstlineno 1306
                lnotab 0x0201
             None
             'username'
             'attribute'
             'default'
             'return'
             code
@@ -10385,46 +10400,46 @@
                code
                   0x970009007c006a000000000000000000a0010000000000000000000000
                   0000000000000000007c01ac01a6010000ab0100000000000000007d046e
                   1223007c006a0200000000000000002400720501007c0363025900530077
                   007803590077017c046a030000000000000000a001000000000000000000
                   00000000000000000000007c027c03a6020000ab02000000000000000053
                   00
-               1304           0 RESUME                   0
+               1309           0 RESUME                   0
                
-               1309           2 NOP
+               1314           2 NOP
                
-               1310           4 LOAD_FAST                0 (cls)
+               1315           4 LOAD_FAST                0 (cls)
                               6 LOAD_ATTR                0 (objects)
                              16 LOAD_METHOD              1 (get)
                              38 LOAD_FAST                1 (username)
                              40 KW_NAMES                 1
                              42 PRECALL                  1
                              46 CALL                     1
                              56 STORE_FAST               4 (attributes)
                              58 JUMP_FORWARD            18 (to 96)
                         >>   60 PUSH_EXC_INFO
                
-               1311          62 LOAD_FAST                0 (cls)
+               1316          62 LOAD_FAST                0 (cls)
                              64 LOAD_ATTR                2 (DoesNotExist)
                              74 CHECK_EXC_MATCH
                              76 POP_JUMP_FORWARD_IF_FALSE     5 (to 88)
                              78 POP_TOP
                
-               1312          80 LOAD_FAST                3 (default)
+               1317          80 LOAD_FAST                3 (default)
                              82 SWAP                     2
                              84 POP_EXCEPT
                              86 RETURN_VALUE
                
-               1311     >>   88 RERAISE                  0
+               1316     >>   88 RERAISE                  0
                         >>   90 COPY                     3
                              92 POP_EXCEPT
                              94 RERAISE                  1
                
-               1314     >>   96 LOAD_FAST                4 (attributes)
+               1319     >>   96 LOAD_FAST                4 (attributes)
                              98 LOAD_ATTR                3 (attributes)
                             108 LOAD_METHOD              1 (get)
                             130 LOAD_FAST                2 (attribute)
                             132 LOAD_FAST                3 (default)
                             134 PRECALL                  2
                             138 CALL                     2
                             148 RETURN_VALUE
@@ -10437,15 +10452,15 @@
                   ('user__username',)
                names      ('objects', 'get', 'DoesNotExist', 'attributes')
                varnames   ('cls', 'username', 'attribute', 'default', 'attributes')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_user_attribute'
-               firstlineno 1304
+               firstlineno 1309
                lnotab 0x020502013a01120108ff0803
             'value'
             code
                argcount  : 4
                nlocals   : 7
                stacksize : 3
                flags     : 3
@@ -10453,45 +10468,45 @@
                   0x9700740100000000000000000000a6000000ab0000000000000000006a
                   010000000000000000a00200000000000000000000000000000000000000
                   007c01ac01a6010000ab0100000000000000007d047c006a010000000000
                   000000a00300000000000000000000000000000000000000007c04ac02a6
                   010000ab0100000000000000005c0200007d057d067c037c056a04000000
                   00000000007c023c0000007c05a005000000000000000000000000000000
                   0000000000a6000000ab000000000000000000010064035300
-               1316           0 RESUME                   0
+               1321           0 RESUME                   0
                
-               1322           2 LOAD_GLOBAL              1 (NULL + get_user_model)
+               1327           2 LOAD_GLOBAL              1 (NULL + get_user_model)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 LOAD_ATTR                1 (objects)
                              38 LOAD_METHOD              2 (get)
                              60 LOAD_FAST                1 (username)
                              62 KW_NAMES                 1
                              64 PRECALL                  1
                              68 CALL                     1
                              78 STORE_FAST               4 (user)
                
-               1323          80 LOAD_FAST                0 (cls)
+               1328          80 LOAD_FAST                0 (cls)
                              82 LOAD_ATTR                1 (objects)
                              92 LOAD_METHOD              3 (update_or_create)
                             114 LOAD_FAST                4 (user)
                             116 KW_NAMES                 2
                             118 PRECALL                  1
                             122 CALL                     1
                             132 UNPACK_SEQUENCE          2
                             136 STORE_FAST               5 (attributes)
                             138 STORE_FAST               6 (__)
                
-               1325         140 LOAD_FAST                3 (value)
+               1330         140 LOAD_FAST                3 (value)
                             142 LOAD_FAST                5 (attributes)
                             144 LOAD_ATTR                4 (attributes)
                             154 LOAD_FAST                2 (attribute)
                             156 STORE_SUBSCR
                
-               1326         160 LOAD_FAST                5 (attributes)
+               1331         160 LOAD_FAST                5 (attributes)
                             162 LOAD_METHOD              5 (save)
                             184 PRECALL                  0
                             188 CALL                     0
                             198 POP_TOP
                             200 LOAD_CONST               3 (None)
                             202 RETURN_VALUE
                consts
@@ -10501,24 +10516,24 @@
                   None
                names      ('get_user_model', 'objects', 'get', 'update_or_create', 'attributes', 'save')
                varnames   ('cls', 'username', 'attribute', 'value', 'user', 'attributes', '__')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'set_user_attribute'
-               firstlineno 1316
+               firstlineno 1321
                lnotab 0x02064e013c021401
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'OneToOneField', 'get_user_model', 'CASCADE', '_', 'user', 'JSONField', 'dict', 'attributes', '__str__', 'classmethod', 'str', 'Optional', 'Any', 'get_user_attribute', 'set_user_attribute')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'UserAdditionalAttributes'
-         firstlineno 1286
+         firstlineno 1291
          lnotab
             0x0a0104050e0112010c01020114fc120736020603020202ff040102ff02
             0102ff02010eff020202fe06ff0e01020b020112ff0e01
       'UserAdditionalAttributes'
       code
          argcount  : 0
          nlocals   : 0
@@ -10530,102 +10545,102 @@
             005a0802006509020065046a0500000000000000006405ac06a6010000ab
             0100000000000000000200650a6407a6010000ab01000000000000000064
             036403ac08a6040000ab0400000000000000005a0b020065046a0c000000
             00000000000200650a6409a6010000ab0100000000000000006403640302
             00650a640aa6010000ab010000000000000000ac0ba6040000ab04000000
             00000000005a0d640c650e650f19000000000000000000640d6510660464
             0e84045a11640f84005a1264105300
-         1329           0 RESUME                   0
+         1334           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('OAuthApplication')
                         8 STORE_NAME               2 (__qualname__)
          
-         1330          10 LOAD_CONST               1 ('Modified OAuth application class that supports Grant Flows configured in preferences.')
+         1335          10 LOAD_CONST               1 ('Modified OAuth application class that supports Grant Flows configured in preferences.')
                        12 STORE_NAME               3 (__doc__)
          
-         1333          14 PUSH_NULL
+         1338          14 PUSH_NULL
                        16 LOAD_NAME                4 (models)
                        18 LOAD_ATTR                5 (CharField)
          
-         1334          28 LOAD_CONST               2 (32)
+         1339          28 LOAD_CONST               2 (32)
                        30 LOAD_NAME                6 (AbstractApplication)
                        32 LOAD_ATTR                7 (GRANT_TYPES)
                        42 LOAD_CONST               3 (True)
          
-         1333          44 KW_NAMES                 4
+         1338          44 KW_NAMES                 4
                        46 PRECALL                  3
                        50 CALL                     3
                        60 STORE_NAME               8 (authorization_grant_type)
          
-         1338          62 PUSH_NULL
+         1343          62 PUSH_NULL
                        64 LOAD_NAME                9 (ArrayField)
          
-         1339          66 PUSH_NULL
+         1344          66 PUSH_NULL
                        68 LOAD_NAME                4 (models)
                        70 LOAD_ATTR                5 (CharField)
                        80 LOAD_CONST               5 (255)
                        82 KW_NAMES                 6
                        84 PRECALL                  1
                        88 CALL                     1
          
-         1340          98 PUSH_NULL
+         1345          98 PUSH_NULL
                       100 LOAD_NAME               10 (_)
                       102 LOAD_CONST               7 ('Allowed scopes that clients can request')
                       104 PRECALL                  1
                       108 CALL                     1
          
-         1341         118 LOAD_CONST               3 (True)
+         1346         118 LOAD_CONST               3 (True)
          
-         1342         120 LOAD_CONST               3 (True)
+         1347         120 LOAD_CONST               3 (True)
          
-         1338         122 KW_NAMES                 8
+         1343         122 KW_NAMES                 8
                       124 PRECALL                  4
                       128 CALL                     4
                       138 STORE_NAME              11 (allowed_scopes)
          
-         1345         140 PUSH_NULL
+         1350         140 PUSH_NULL
                       142 LOAD_NAME                4 (models)
                       144 LOAD_ATTR               12 (ImageField)
          
-         1346         154 PUSH_NULL
+         1351         154 PUSH_NULL
                       156 LOAD_NAME               10 (_)
                       158 LOAD_CONST               9 ('Icon')
                       160 PRECALL                  1
                       164 CALL                     1
          
-         1347         174 LOAD_CONST               3 (True)
+         1352         174 LOAD_CONST               3 (True)
          
-         1348         176 LOAD_CONST               3 (True)
+         1353         176 LOAD_CONST               3 (True)
          
-         1349         178 PUSH_NULL
+         1354         178 PUSH_NULL
                       180 LOAD_NAME               10 (_)
          
-         1350         182 LOAD_CONST              10 ('This image will be shown as icon in the authorization flow. It should be squared.')
+         1355         182 LOAD_CONST              10 ('This image will be shown as icon in the authorization flow. It should be squared.')
          
-         1349         184 PRECALL                  1
+         1354         184 PRECALL                  1
                       188 CALL                     1
          
-         1345         198 KW_NAMES                11
+         1350         198 KW_NAMES                11
                       200 PRECALL                  4
                       204 CALL                     4
                       214 STORE_NAME              13 (icon)
          
-         1354         216 LOAD_CONST              12 ('grant_types')
+         1359         216 LOAD_CONST              12 ('grant_types')
                       218 LOAD_NAME               14 (set)
                       220 LOAD_NAME               15 (str)
                       222 BINARY_SUBSCR
                       232 LOAD_CONST              13 ('return')
                       234 LOAD_NAME               16 (bool)
                       236 BUILD_TUPLE              4
-                      238 LOAD_CONST              14 (<code object allows_grant_type, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1354>)
+                      238 LOAD_CONST              14 (<code object allows_grant_type, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1359>)
                       240 MAKE_FUNCTION            4 (annotations)
                       242 STORE_NAME              17 (allows_grant_type)
          
-         1359         244 LOAD_CONST              15 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1359>)
+         1364         244 LOAD_CONST              15 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1364>)
                       246 MAKE_FUNCTION            0
                       248 STORE_NAME              18 (get_absolute_url)
                       250 LOAD_CONST              16 (None)
                       252 RETURN_VALUE
          consts
             'OAuthApplication'
             'Modified OAuth application class that supports Grant Flows configured in preferences.'
@@ -10648,24 +10663,24 @@
                flags     : 7
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000064
                   01190000000000000000007d027403000000000000000000007405000000
                   000000000000007c02a6010000ab01000000000000000074050000000000
                   00000000007c01a6010000ab0100000000000000007a010000a6010000ab
                   0100000000000000005300
-               1354           0 RESUME                   0
+               1359           0 RESUME                   0
                
-               1355           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+               1360           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 LOAD_CONST               1 ('auth__oauth_allowed_grants')
                              30 BINARY_SUBSCR
                              40 STORE_FAST               2 (allowed_grants)
                
-               1357          42 LOAD_GLOBAL              3 (NULL + bool)
+               1362          42 LOAD_GLOBAL              3 (NULL + bool)
                              54 LOAD_GLOBAL              5 (NULL + set)
                              66 LOAD_FAST                2 (allowed_grants)
                              68 PRECALL                  1
                              72 CALL                     1
                              82 LOAD_GLOBAL              5 (NULL + set)
                              94 LOAD_FAST                1 (grant_types)
                              96 PRECALL                  1
@@ -10679,27 +10694,27 @@
                   'auth__oauth_allowed_grants'
                names      ('get_site_preferences', 'bool', 'set')
                varnames   ('self', 'grant_types', 'allowed_grants')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'allows_grant_type'
-               firstlineno 1354
+               firstlineno 1359
                lnotab 0x02012802
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               1359           0 RESUME                   0
+               1364           0 RESUME                   0
                
-               1360           2 LOAD_GLOBAL              1 (NULL + reverse)
+               1365           2 LOAD_GLOBAL              1 (NULL + reverse)
                              14 LOAD_CONST               1 ('oauth2_application')
                              16 LOAD_FAST                0 (self)
                              18 LOAD_ATTR                1 (id)
                              28 BUILD_LIST               1
                              30 KW_NAMES                 2
                              32 PRECALL                  2
                              36 CALL                     2
@@ -10710,214 +10725,214 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_absolute_url'
-               firstlineno 1359
+               firstlineno 1364
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'CharField', 'AbstractApplication', 'GRANT_TYPES', 'authorization_grant_type', 'ArrayField', '_', 'allowed_scopes', 'ImageField', 'icon', 'set', 'str', 'bool', 'allows_grant_type', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'OAuthApplication'
-         firstlineno 1329
+         firstlineno 1334
          lnotab
             0x0a0104030e0110ff1205040120011401020102fc12070e011401020102
             01040102ff0efc12091c05
       'OAuthApplication'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         1363           0 RESUME                   0
+         1368           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('OAuthGrant')
                         8 STORE_NAME               2 (__qualname__)
          
-         1364          10 LOAD_CONST               1 ('Placeholder for customising the Grant model.')
+         1369          10 LOAD_CONST               1 ('Placeholder for customising the Grant model.')
                        12 STORE_NAME               3 (__doc__)
          
-         1366          14 LOAD_CONST               2 (None)
+         1371          14 LOAD_CONST               2 (None)
                        16 RETURN_VALUE
          consts
             'OAuthGrant'
             'Placeholder for customising the Grant model.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'OAuthGrant'
-         firstlineno 1363
+         firstlineno 1368
          lnotab 0x0a010402
       'OAuthGrant'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         1369           0 RESUME                   0
+         1374           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('OAuthAccessToken')
                         8 STORE_NAME               2 (__qualname__)
          
-         1370          10 LOAD_CONST               1 ('Placeholder for customising the AccessToken model.')
+         1375          10 LOAD_CONST               1 ('Placeholder for customising the AccessToken model.')
                        12 STORE_NAME               3 (__doc__)
          
-         1372          14 LOAD_CONST               2 (None)
+         1377          14 LOAD_CONST               2 (None)
                        16 RETURN_VALUE
          consts
             'OAuthAccessToken'
             'Placeholder for customising the AccessToken model.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'OAuthAccessToken'
-         firstlineno 1369
+         firstlineno 1374
          lnotab 0x0a010402
       'OAuthAccessToken'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         1375           0 RESUME                   0
+         1380           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('OAuthIDToken')
                         8 STORE_NAME               2 (__qualname__)
          
-         1376          10 LOAD_CONST               1 ('Placeholder for customising the IDToken model.')
+         1381          10 LOAD_CONST               1 ('Placeholder for customising the IDToken model.')
                        12 STORE_NAME               3 (__doc__)
          
-         1378          14 LOAD_CONST               2 (None)
+         1383          14 LOAD_CONST               2 (None)
                        16 RETURN_VALUE
          consts
             'OAuthIDToken'
             'Placeholder for customising the IDToken model.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'OAuthIDToken'
-         firstlineno 1375
+         firstlineno 1380
          lnotab 0x0a010402
       'OAuthIDToken'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         1381           0 RESUME                   0
+         1386           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('OAuthRefreshToken')
                         8 STORE_NAME               2 (__qualname__)
          
-         1382          10 LOAD_CONST               1 ('Placeholder for customising the RefreshToken model.')
+         1387          10 LOAD_CONST               1 ('Placeholder for customising the RefreshToken model.')
                        12 STORE_NAME               3 (__doc__)
          
-         1384          14 LOAD_CONST               2 (None)
+         1389          14 LOAD_CONST               2 (None)
                        16 RETURN_VALUE
          consts
             'OAuthRefreshToken'
             'Placeholder for customising the RefreshToken model.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'OAuthRefreshToken'
-         firstlineno 1381
+         firstlineno 1386
          lnotab 0x0a010402
       'OAuthRefreshToken'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000000200650564
             01a6010000ab0100000000000000006402ac03a6020000ab020000000000
             0000005a06020065036a040000000000000000020065056404a6010000ab
             0100000000000000006402ac03a6020000ab0200000000000000005a0764
             055a08640665096602640784045a0a640665096602640884045a0b020047
             0064098400640aa6020000ab0200000000000000005a0c640b5300
-         1387           0 RESUME                   0
+         1392           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('Room')
                         8 STORE_NAME               2 (__qualname__)
          
-         1388          10 PUSH_NULL
+         1393          10 PUSH_NULL
                        12 LOAD_NAME                3 (models)
                        14 LOAD_ATTR                4 (CharField)
                        24 PUSH_NULL
                        26 LOAD_NAME                5 (_)
                        28 LOAD_CONST               1 ('Short name')
                        30 PRECALL                  1
                        34 CALL                     1
                        44 LOAD_CONST               2 (255)
                        46 KW_NAMES                 3
                        48 PRECALL                  2
                        52 CALL                     2
                        62 STORE_NAME               6 (short_name)
          
-         1389          64 PUSH_NULL
+         1394          64 PUSH_NULL
                        66 LOAD_NAME                3 (models)
                        68 LOAD_ATTR                4 (CharField)
                        78 PUSH_NULL
                        80 LOAD_NAME                5 (_)
                        82 LOAD_CONST               4 ('Long name')
                        84 PRECALL                  1
                        88 CALL                     1
                        98 LOAD_CONST               2 (255)
                       100 KW_NAMES                 3
                       102 PRECALL                  2
                       106 CALL                     2
                       116 STORE_NAME               7 (name)
          
-         1391         118 LOAD_CONST               5 ('door')
+         1396         118 LOAD_CONST               5 ('door')
                       120 STORE_NAME               8 (icon_)
          
-         1393         122 LOAD_CONST               6 ('return')
+         1398         122 LOAD_CONST               6 ('return')
                       124 LOAD_NAME                9 (str)
                       126 BUILD_TUPLE              2
-                      128 LOAD_CONST               7 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1393>)
+                      128 LOAD_CONST               7 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1398>)
                       130 MAKE_FUNCTION            4 (annotations)
                       132 STORE_NAME              10 (__str__)
          
-         1396         134 LOAD_CONST               6 ('return')
+         1401         134 LOAD_CONST               6 ('return')
                       136 LOAD_NAME                9 (str)
                       138 BUILD_TUPLE              2
-                      140 LOAD_CONST               8 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1396>)
+                      140 LOAD_CONST               8 (<code object get_absolute_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1401>)
                       142 MAKE_FUNCTION            4 (annotations)
                       144 STORE_NAME              11 (get_absolute_url)
          
-         1399         146 PUSH_NULL
+         1404         146 PUSH_NULL
                       148 LOAD_BUILD_CLASS
-                      150 LOAD_CONST               9 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1399>)
+                      150 LOAD_CONST               9 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1404>)
                       152 MAKE_FUNCTION            0
                       154 LOAD_CONST              10 ('Meta')
                       156 PRECALL                  2
                       160 CALL                     2
                       170 STORE_NAME              12 (Meta)
                       172 LOAD_CONST              11 (None)
                       174 RETURN_VALUE
@@ -10933,17 +10948,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064029d045300
-               1393           0 RESUME                   0
+               1398           0 RESUME                   0
                
-               1394           2 LOAD_FAST                0 (self)
+               1399           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (name)
                              14 FORMAT_VALUE             0
                              16 LOAD_CONST               1 (' (')
                              18 LOAD_FAST                0 (self)
                              20 LOAD_ATTR                1 (short_name)
                              30 FORMAT_VALUE             0
                              32 LOAD_CONST               2 (')')
@@ -10955,27 +10970,27 @@
                   ')'
                names      ('name', 'short_name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1393
+               firstlineno 1398
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000640164027c006a0100000000000000
                   006702ac03a6020000ab0200000000000000005300
-               1396           0 RESUME                   0
+               1401           0 RESUME                   0
                
-               1397           2 LOAD_GLOBAL              1 (NULL + reverse)
+               1402           2 LOAD_GLOBAL              1 (NULL + reverse)
                              14 LOAD_CONST               1 ('timetable')
                              16 LOAD_CONST               2 ('room')
                              18 LOAD_FAST                0 (self)
                              20 LOAD_ATTR                1 (id)
                              30 BUILD_LIST               2
                              32 KW_NAMES                 3
                              34 PRECALL                  2
@@ -10988,73 +11003,73 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_absolute_url'
-               firstlineno 1396
+               firstlineno 1401
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x970065005a0164005a026401020065036402a6010000ab010000000000
                   000000660266015a046403640467025a05020065036405a6010000ab0100
                   000000000000005a06020065036406a6010000ab0100000000000000005a
                   07020065086a090000000000000000640467016407ac08a6020000ab0200
                   0000000000000067015a0a64095300
-               1399           0 RESUME                   0
+               1404           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('Room.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1400          10 LOAD_CONST               1 ('view_room_timetable')
+               1405          10 LOAD_CONST               1 ('view_room_timetable')
                              12 PUSH_NULL
                              14 LOAD_NAME                3 (_)
                              16 LOAD_CONST               2 ('Can view room timetable')
                              18 PRECALL                  1
                              22 CALL                     1
                              32 BUILD_TUPLE              2
                              34 BUILD_TUPLE              1
                              36 STORE_NAME               4 (permissions)
                
-               1401          38 LOAD_CONST               3 ('name')
+               1406          38 LOAD_CONST               3 ('name')
                              40 LOAD_CONST               4 ('short_name')
                              42 BUILD_LIST               2
                              44 STORE_NAME               5 (ordering)
                
-               1402          46 PUSH_NULL
+               1407          46 PUSH_NULL
                              48 LOAD_NAME                3 (_)
                              50 LOAD_CONST               5 ('Room')
                              52 PRECALL                  1
                              56 CALL                     1
                              66 STORE_NAME               6 (verbose_name)
                
-               1403          68 PUSH_NULL
+               1408          68 PUSH_NULL
                              70 LOAD_NAME                3 (_)
                              72 LOAD_CONST               6 ('Rooms')
                              74 PRECALL                  1
                              78 CALL                     1
                              88 STORE_NAME               7 (verbose_name_plural)
                
-               1405          90 PUSH_NULL
+               1410          90 PUSH_NULL
                              92 LOAD_NAME                8 (models)
                              94 LOAD_ATTR                9 (UniqueConstraint)
                             104 LOAD_CONST               4 ('short_name')
                             106 BUILD_LIST               1
                             108 LOAD_CONST               7 ('unique_room_short_name')
                             110 KW_NAMES                 8
                             112 PRECALL                  2
                             116 CALL                     2
                
-               1404         126 BUILD_LIST               1
+               1409         126 BUILD_LIST               1
                             128 STORE_NAME              10 (constraints)
                             130 LOAD_CONST               9 (None)
                             132 RETURN_VALUE
                consts
                   'Room.Meta'
                   'view_room_timetable'
                   'Can view room timetable'
@@ -11067,25 +11082,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'permissions', 'ordering', 'verbose_name', 'verbose_name_plural', 'models', 'UniqueConstraint', 'constraints')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1399
+               firstlineno 1404
                lnotab 0x0a011c0108011601160224ff
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', '_', 'short_name', 'name', 'icon_', 'str', '__str__', 'get_absolute_url', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'Room'
-         firstlineno 1387
+         firstlineno 1392
          lnotab 0x0a013601360204020c030c03
       'Room'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
@@ -11128,519 +11143,519 @@
             000000000000005a2765140900642464116515640f7a070000641e652865
             166529660219000000000000000000640f7a0700006412652a6606641f84
             05a6000000ab0000000000000000005a2b88006601642084085a2c020047
             00642184006422a6020000ab0200000000000000005a2d880078015a2e53
             00
                         0 MAKE_CELL                0 (__class__)
          
-         1409           2 RESUME                   0
+         1414           2 RESUME                   0
                         4 LOAD_NAME                0 (__name__)
                         6 STORE_NAME               1 (__module__)
                         8 LOAD_CONST               0 ('CalendarEvent')
                        10 STORE_NAME               2 (__qualname__)
          
-         1410          12 LOAD_CONST               1 ('A planned event in a calendar.\n\n    To make use of this model, you need to inherit from this model.\n    Every subclass of this model represents a certain calendar (feed).\n    It therefore needs to set the basic attributes of the calendar like\n    described in the documentation of `CalendarEventMixin`.\n\n    Furthermore, every `value_*` method from `CalendarEventMixin`\n    can be implemented to provide additional data (either static or dynamic).\n    Some like start and end date are pre-implemented in this model. Others, like\n    `value_title` need to be implemented in the subclass. Some methods are\n    also optional, like `value_location` or `value_description`.\n    Please refer to the documentation of `CalendarEventMixin` for more information.\n    ')
+         1415          12 LOAD_CONST               1 ('A planned event in a calendar.\n\n    To make use of this model, you need to inherit from this model.\n    Every subclass of this model represents a certain calendar (feed).\n    It therefore needs to set the basic attributes of the calendar like\n    described in the documentation of `CalendarEventMixin`.\n\n    Furthermore, every `value_*` method from `CalendarEventMixin`\n    can be implemented to provide additional data (either static or dynamic).\n    Some like start and end date are pre-implemented in this model. Others, like\n    `value_title` need to be implemented in the subclass. Some methods are\n    also optional, like `value_location` or `value_description`.\n    Please refer to the documentation of `CalendarEventMixin` for more information.\n    ')
                        14 STORE_NAME               3 (__doc__)
          
-         1425          16 PUSH_NULL
+         1430          16 PUSH_NULL
                        18 LOAD_NAME                4 (models)
                        20 LOAD_ATTR                5 (DateTimeField)
          
-         1426          30 PUSH_NULL
+         1431          30 PUSH_NULL
                        32 LOAD_NAME                6 (_)
                        34 LOAD_CONST               2 ('Start date and time')
                        36 PRECALL                  1
                        40 CALL                     1
                        50 LOAD_CONST               3 (True)
                        52 LOAD_CONST               3 (True)
          
-         1425          54 KW_NAMES                 4
+         1430          54 KW_NAMES                 4
                        56 PRECALL                  3
                        60 CALL                     3
                        70 STORE_NAME               7 (datetime_start)
          
-         1428          72 PUSH_NULL
+         1433          72 PUSH_NULL
                        74 LOAD_NAME                4 (models)
                        76 LOAD_ATTR                5 (DateTimeField)
                        86 PUSH_NULL
                        88 LOAD_NAME                6 (_)
                        90 LOAD_CONST               5 ('End date and time')
                        92 PRECALL                  1
                        96 CALL                     1
                       106 LOAD_CONST               3 (True)
                       108 LOAD_CONST               3 (True)
                       110 KW_NAMES                 4
                       112 PRECALL                  3
                       116 CALL                     3
                       126 STORE_NAME               8 (datetime_end)
          
-         1429         128 PUSH_NULL
+         1434         128 PUSH_NULL
                       130 LOAD_NAME                9 (TimeZoneField)
                       132 PUSH_NULL
                       134 LOAD_NAME                6 (_)
                       136 LOAD_CONST               6 ('Timezone')
                       138 PRECALL                  1
                       142 CALL                     1
                       152 LOAD_CONST               3 (True)
                       154 LOAD_CONST               3 (True)
                       156 KW_NAMES                 4
                       158 PRECALL                  3
                       162 CALL                     3
                       172 STORE_NAME              10 (timezone)
          
-         1430         174 PUSH_NULL
+         1435         174 PUSH_NULL
                       176 LOAD_NAME                4 (models)
                       178 LOAD_ATTR               11 (DateField)
                       188 PUSH_NULL
                       190 LOAD_NAME                6 (_)
                       192 LOAD_CONST               7 ('Start date')
                       194 PRECALL                  1
                       198 CALL                     1
                       208 LOAD_CONST               3 (True)
                       210 LOAD_CONST               3 (True)
                       212 KW_NAMES                 4
                       214 PRECALL                  3
                       218 CALL                     3
                       228 STORE_NAME              12 (date_start)
          
-         1431         230 PUSH_NULL
+         1436         230 PUSH_NULL
                       232 LOAD_NAME                4 (models)
                       234 LOAD_ATTR               11 (DateField)
                       244 PUSH_NULL
                       246 LOAD_NAME                6 (_)
                       248 LOAD_CONST               8 ('End date')
                       250 PRECALL                  1
                       254 CALL                     1
                       264 LOAD_CONST               3 (True)
                       266 LOAD_CONST               3 (True)
                       268 KW_NAMES                 4
                       270 PRECALL                  3
                       274 CALL                     3
                       284 STORE_NAME              13 (date_end)
          
-         1432         286 PUSH_NULL
+         1437         286 PUSH_NULL
                       288 LOAD_NAME               14 (RecurrenceField)
                       290 PUSH_NULL
                       292 LOAD_NAME                6 (_)
                       294 LOAD_CONST               9 ('Recurrences')
                       296 PRECALL                  1
                       300 CALL                     1
                       310 LOAD_CONST               3 (True)
                       312 LOAD_CONST               3 (True)
                       314 KW_NAMES                 4
                       316 PRECALL                  3
                       320 CALL                     3
                       330 STORE_NAME              15 (recurrences)
          
-         1433         332 PUSH_NULL
+         1438         332 PUSH_NULL
                       334 LOAD_NAME                4 (models)
                       336 LOAD_ATTR               16 (ForeignKey)
          
-         1434         346 LOAD_CONST              10 ('self')
+         1439         346 LOAD_CONST              10 ('self')
          
-         1435         348 LOAD_NAME                4 (models)
+         1440         348 LOAD_NAME                4 (models)
                       350 LOAD_ATTR               17 (CASCADE)
          
-         1436         360 LOAD_CONST               3 (True)
+         1441         360 LOAD_CONST               3 (True)
          
-         1437         362 LOAD_CONST               3 (True)
+         1442         362 LOAD_CONST               3 (True)
          
-         1438         364 PUSH_NULL
+         1443         364 PUSH_NULL
                       366 LOAD_NAME                6 (_)
                       368 LOAD_CONST              11 ('Amended base event')
                       370 PRECALL                  1
                       374 CALL                     1
          
-         1439         384 LOAD_CONST              12 ('amended_by')
+         1444         384 LOAD_CONST              12 ('amended_by')
          
-         1433         386 KW_NAMES                13
+         1438         386 KW_NAMES                13
                       388 PRECALL                  6
                       392 CALL                     6
                       402 STORE_NAME              18 (amends)
          
-         1442         404 LOAD_CONST              14 (<code object provide_list_in_timezone, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1442>)
+         1447         404 LOAD_CONST              14 (<code object provide_list_in_timezone, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1447>)
                       406 MAKE_FUNCTION            0
                       408 STORE_NAME              19 (provide_list_in_timezone)
          
-         1446         410 LOAD_NAME               20 (classmethod)
+         1451         410 LOAD_NAME               20 (classmethod)
          
-         1448         412 NOP
+         1453         412 NOP
          
-         1447         414 LOAD_CONST              35 ((None,))
+         1452         414 LOAD_CONST              35 ((None,))
                       416 LOAD_CONST              16 ('reference_object')
          
-         1448         418 LOAD_CONST               0 ('CalendarEvent')
+         1453         418 LOAD_CONST               0 ('CalendarEvent')
          
-         1447         420 LOAD_CONST              17 ('request')
+         1452         420 LOAD_CONST              17 ('request')
          
-         1448         422 LOAD_NAME               21 (HttpRequest)
+         1453         422 LOAD_NAME               21 (HttpRequest)
                       424 LOAD_CONST              15 (None)
                       426 BINARY_OP                7 (|)
          
-         1447         430 LOAD_CONST              18 ('return')
+         1452         430 LOAD_CONST              18 ('return')
          
-         1449         432 LOAD_NAME               22 (str)
+         1454         432 LOAD_NAME               22 (str)
          
-         1447         434 BUILD_TUPLE              6
-                      436 LOAD_CONST              19 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1446>)
+         1452         434 BUILD_TUPLE              6
+                      436 LOAD_CONST              19 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1451>)
                       438 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1446         440 PRECALL                  0
+         1451         440 PRECALL                  0
                       444 CALL                     0
          
-         1447         454 STORE_NAME              23 (value_title)
+         1452         454 STORE_NAME              23 (value_title)
          
-         1453         456 LOAD_NAME               20 (classmethod)
+         1458         456 LOAD_NAME               20 (classmethod)
          
-         1455         458 NOP
+         1460         458 NOP
          
-         1454         460 LOAD_CONST              35 ((None,))
+         1459         460 LOAD_CONST              35 ((None,))
                       462 LOAD_CONST              16 ('reference_object')
          
-         1455         464 LOAD_CONST               0 ('CalendarEvent')
+         1460         464 LOAD_CONST               0 ('CalendarEvent')
          
-         1454         466 LOAD_CONST              17 ('request')
+         1459         466 LOAD_CONST              17 ('request')
          
-         1455         468 LOAD_NAME               21 (HttpRequest)
+         1460         468 LOAD_NAME               21 (HttpRequest)
                       470 LOAD_CONST              15 (None)
                       472 BINARY_OP                7 (|)
          
-         1454         476 LOAD_CONST              18 ('return')
+         1459         476 LOAD_CONST              18 ('return')
          
-         1456         478 LOAD_NAME               24 (Union)
+         1461         478 LOAD_NAME               24 (Union)
                       480 LOAD_NAME               25 (datetime)
                       482 LOAD_NAME               26 (date)
                       484 BUILD_TUPLE              2
                       486 BINARY_SUBSCR
          
-         1454         496 BUILD_TUPLE              6
-                      498 LOAD_CONST              20 (<code object value_start_datetime, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1453>)
+         1459         496 BUILD_TUPLE              6
+                      498 LOAD_CONST              20 (<code object value_start_datetime, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1458>)
                       500 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1453         502 PRECALL                  0
+         1458         502 PRECALL                  0
                       506 CALL                     0
          
-         1454         516 STORE_NAME              27 (value_start_datetime)
+         1459         516 STORE_NAME              27 (value_start_datetime)
          
-         1462         518 LOAD_NAME               20 (classmethod)
+         1467         518 LOAD_NAME               20 (classmethod)
          
-         1464         520 NOP
+         1469         520 NOP
          
-         1463         522 LOAD_CONST              35 ((None,))
+         1468         522 LOAD_CONST              35 ((None,))
                       524 LOAD_CONST              16 ('reference_object')
          
-         1464         526 LOAD_CONST               0 ('CalendarEvent')
+         1469         526 LOAD_CONST               0 ('CalendarEvent')
          
-         1463         528 LOAD_CONST              17 ('request')
+         1468         528 LOAD_CONST              17 ('request')
          
-         1464         530 LOAD_NAME               21 (HttpRequest)
+         1469         530 LOAD_NAME               21 (HttpRequest)
                       532 LOAD_CONST              15 (None)
                       534 BINARY_OP                7 (|)
          
-         1463         538 LOAD_CONST              18 ('return')
+         1468         538 LOAD_CONST              18 ('return')
          
-         1465         540 LOAD_NAME               24 (Union)
+         1470         540 LOAD_NAME               24 (Union)
                       542 LOAD_NAME               25 (datetime)
                       544 LOAD_NAME               26 (date)
                       546 LOAD_CONST              15 (None)
                       548 BUILD_TUPLE              3
                       550 BINARY_SUBSCR
          
-         1463         560 BUILD_TUPLE              6
-                      562 LOAD_CONST              21 (<code object value_end_datetime, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1462>)
+         1468         560 BUILD_TUPLE              6
+                      562 LOAD_CONST              21 (<code object value_end_datetime, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1467>)
                       564 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1462         566 PRECALL                  0
+         1467         566 PRECALL                  0
                       570 CALL                     0
          
-         1463         580 STORE_NAME              28 (value_end_datetime)
+         1468         580 STORE_NAME              28 (value_end_datetime)
          
-         1475         582 LOAD_NAME               20 (classmethod)
+         1480         582 LOAD_NAME               20 (classmethod)
          
-         1477         584 NOP
+         1482         584 NOP
          
-         1476         586 LOAD_CONST              35 ((None,))
+         1481         586 LOAD_CONST              35 ((None,))
                       588 LOAD_CONST              16 ('reference_object')
          
-         1477         590 LOAD_CONST               0 ('CalendarEvent')
+         1482         590 LOAD_CONST               0 ('CalendarEvent')
          
-         1476         592 LOAD_CONST              17 ('request')
+         1481         592 LOAD_CONST              17 ('request')
          
-         1477         594 LOAD_NAME               21 (HttpRequest)
+         1482         594 LOAD_NAME               21 (HttpRequest)
                       596 LOAD_CONST              15 (None)
                       598 BINARY_OP                7 (|)
          
-         1476         602 LOAD_CONST              18 ('return')
+         1481         602 LOAD_CONST              18 ('return')
          
-         1478         604 LOAD_NAME               29 (Optional)
+         1483         604 LOAD_NAME               29 (Optional)
                       606 LOAD_NAME               30 (vRecur)
                       608 BINARY_SUBSCR
          
-         1476         618 BUILD_TUPLE              6
-                      620 LOAD_CONST              22 (<code object value_rrule, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1475>)
+         1481         618 BUILD_TUPLE              6
+                      620 LOAD_CONST              22 (<code object value_rrule, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1480>)
                       622 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1475         624 PRECALL                  0
+         1480         624 PRECALL                  0
                       628 CALL                     0
          
-         1476         638 STORE_NAME              31 (value_rrule)
+         1481         638 STORE_NAME              31 (value_rrule)
          
-         1485         640 LOAD_NAME               20 (classmethod)
+         1490         640 LOAD_NAME               20 (classmethod)
          
-         1487         642 NOP
+         1492         642 NOP
          
-         1486         644 LOAD_CONST              35 ((None,))
+         1491         644 LOAD_CONST              35 ((None,))
                       646 LOAD_CONST              16 ('reference_object')
          
-         1487         648 LOAD_CONST               0 ('CalendarEvent')
+         1492         648 LOAD_CONST               0 ('CalendarEvent')
          
-         1486         650 LOAD_CONST              17 ('request')
+         1491         650 LOAD_CONST              17 ('request')
          
-         1487         652 LOAD_NAME               21 (HttpRequest)
+         1492         652 LOAD_NAME               21 (HttpRequest)
                       654 LOAD_CONST              15 (None)
                       656 BINARY_OP                7 (|)
          
-         1486         660 LOAD_CONST              18 ('return')
+         1491         660 LOAD_CONST              18 ('return')
          
-         1488         662 LOAD_NAME               29 (Optional)
+         1493         662 LOAD_NAME               29 (Optional)
                       664 LOAD_NAME               32 (list)
                       666 LOAD_NAME               25 (datetime)
                       668 BINARY_SUBSCR
                       678 BINARY_SUBSCR
          
-         1486         688 BUILD_TUPLE              6
-                      690 LOAD_CONST              23 (<code object value_rdate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1485>)
+         1491         688 BUILD_TUPLE              6
+                      690 LOAD_CONST              23 (<code object value_rdate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1490>)
                       692 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1485         694 PRECALL                  0
+         1490         694 PRECALL                  0
                       698 CALL                     0
          
-         1486         708 STORE_NAME              33 (value_rdate)
+         1491         708 STORE_NAME              33 (value_rdate)
          
-         1494         710 LOAD_NAME               20 (classmethod)
+         1499         710 LOAD_NAME               20 (classmethod)
          
-         1496         712 NOP
+         1501         712 NOP
          
-         1495         714 LOAD_CONST              35 ((None,))
+         1500         714 LOAD_CONST              35 ((None,))
                       716 LOAD_CONST              16 ('reference_object')
          
-         1496         718 LOAD_CONST               0 ('CalendarEvent')
+         1501         718 LOAD_CONST               0 ('CalendarEvent')
          
-         1495         720 LOAD_CONST              17 ('request')
+         1500         720 LOAD_CONST              17 ('request')
          
-         1496         722 LOAD_NAME               21 (HttpRequest)
+         1501         722 LOAD_NAME               21 (HttpRequest)
                       724 LOAD_CONST              15 (None)
                       726 BINARY_OP                7 (|)
          
-         1495         730 LOAD_CONST              18 ('return')
+         1500         730 LOAD_CONST              18 ('return')
          
-         1497         732 LOAD_NAME               29 (Optional)
+         1502         732 LOAD_NAME               29 (Optional)
                       734 LOAD_NAME               32 (list)
                       736 LOAD_NAME               30 (vRecur)
                       738 BINARY_SUBSCR
                       748 BINARY_SUBSCR
          
-         1495         758 BUILD_TUPLE              6
-                      760 LOAD_CONST              24 (<code object value_exrule, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1494>)
+         1500         758 BUILD_TUPLE              6
+                      760 LOAD_CONST              24 (<code object value_exrule, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1499>)
                       762 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1494         764 PRECALL                  0
+         1499         764 PRECALL                  0
                       768 CALL                     0
          
-         1495         778 STORE_NAME              34 (value_exrule)
+         1500         778 STORE_NAME              34 (value_exrule)
          
-         1503         780 LOAD_NAME               20 (classmethod)
+         1508         780 LOAD_NAME               20 (classmethod)
          
-         1505         782 NOP
+         1510         782 NOP
          
-         1504         784 LOAD_CONST              35 ((None,))
+         1509         784 LOAD_CONST              35 ((None,))
                       786 LOAD_CONST              16 ('reference_object')
          
-         1505         788 LOAD_CONST               0 ('CalendarEvent')
+         1510         788 LOAD_CONST               0 ('CalendarEvent')
          
-         1504         790 LOAD_CONST              17 ('request')
+         1509         790 LOAD_CONST              17 ('request')
          
-         1505         792 LOAD_NAME               21 (HttpRequest)
+         1510         792 LOAD_NAME               21 (HttpRequest)
                       794 LOAD_CONST              15 (None)
                       796 BINARY_OP                7 (|)
          
-         1504         800 LOAD_CONST              18 ('return')
+         1509         800 LOAD_CONST              18 ('return')
          
-         1506         802 LOAD_NAME               29 (Optional)
+         1511         802 LOAD_NAME               29 (Optional)
                       804 LOAD_NAME               32 (list)
                       806 LOAD_NAME               25 (datetime)
                       808 BINARY_SUBSCR
                       818 BINARY_SUBSCR
          
-         1504         828 BUILD_TUPLE              6
-                      830 LOAD_CONST              25 (<code object value_exdate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1503>)
+         1509         828 BUILD_TUPLE              6
+                      830 LOAD_CONST              25 (<code object value_exdate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1508>)
                       832 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1503         834 PRECALL                  0
+         1508         834 PRECALL                  0
                       838 CALL                     0
          
-         1504         848 STORE_NAME              35 (value_exdate)
+         1509         848 STORE_NAME              35 (value_exdate)
          
-         1512         850 LOAD_NAME               20 (classmethod)
+         1517         850 LOAD_NAME               20 (classmethod)
          
-         1514         852 NOP
+         1519         852 NOP
          
-         1513         854 LOAD_CONST              35 ((None,))
+         1518         854 LOAD_CONST              35 ((None,))
                       856 LOAD_CONST              16 ('reference_object')
          
-         1514         858 LOAD_CONST               0 ('CalendarEvent')
+         1519         858 LOAD_CONST               0 ('CalendarEvent')
          
-         1513         860 LOAD_CONST              17 ('request')
+         1518         860 LOAD_CONST              17 ('request')
          
-         1514         862 LOAD_NAME               21 (HttpRequest)
+         1519         862 LOAD_NAME               21 (HttpRequest)
                       864 LOAD_CONST              15 (None)
                       866 BINARY_OP                7 (|)
          
-         1513         870 LOAD_CONST              18 ('return')
+         1518         870 LOAD_CONST              18 ('return')
          
-         1515         872 LOAD_NAME               22 (str)
+         1520         872 LOAD_NAME               22 (str)
          
-         1513         874 BUILD_TUPLE              6
-                      876 LOAD_CONST              26 (<code object value_unique_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1512>)
+         1518         874 BUILD_TUPLE              6
+                      876 LOAD_CONST              26 (<code object value_unique_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1517>)
                       878 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1512         880 PRECALL                  0
+         1517         880 PRECALL                  0
                       884 CALL                     0
          
-         1513         894 STORE_NAME              36 (value_unique_id)
+         1518         894 STORE_NAME              36 (value_unique_id)
          
-         1521         896 LOAD_NAME               20 (classmethod)
+         1526         896 LOAD_NAME               20 (classmethod)
          
-         1523         898 NOP
+         1528         898 NOP
          
-         1522         900 LOAD_CONST              35 ((None,))
+         1527         900 LOAD_CONST              35 ((None,))
                       902 LOAD_CONST              16 ('reference_object')
          
-         1523         904 LOAD_CONST               0 ('CalendarEvent')
+         1528         904 LOAD_CONST               0 ('CalendarEvent')
          
-         1522         906 LOAD_CONST              17 ('request')
+         1527         906 LOAD_CONST              17 ('request')
          
-         1523         908 LOAD_NAME               21 (HttpRequest)
+         1528         908 LOAD_NAME               21 (HttpRequest)
                       910 LOAD_CONST              15 (None)
                       912 BINARY_OP                7 (|)
          
-         1522         916 LOAD_CONST              18 ('return')
+         1527         916 LOAD_CONST              18 ('return')
          
-         1524         918 LOAD_NAME               29 (Optional)
+         1529         918 LOAD_NAME               29 (Optional)
                       920 LOAD_NAME               24 (Union)
                       922 LOAD_NAME               25 (datetime)
                       924 LOAD_NAME               26 (date)
                       926 BUILD_TUPLE              2
                       928 BINARY_SUBSCR
                       938 BINARY_SUBSCR
          
-         1522         948 BUILD_TUPLE              6
-                      950 LOAD_CONST              27 (<code object value_recurrence_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1521>)
+         1527         948 BUILD_TUPLE              6
+                      950 LOAD_CONST              27 (<code object value_recurrence_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1526>)
                       952 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1521         954 PRECALL                  0
+         1526         954 PRECALL                  0
                       958 CALL                     0
          
-         1522         968 STORE_NAME              37 (value_recurrence_id)
+         1527         968 STORE_NAME              37 (value_recurrence_id)
          
-         1530         970 LOAD_NAME               20 (classmethod)
+         1535         970 LOAD_NAME               20 (classmethod)
          
-         1532         972 NOP
+         1537         972 NOP
          
-         1531         974 LOAD_CONST              35 ((None,))
+         1536         974 LOAD_CONST              35 ((None,))
                       976 LOAD_CONST              16 ('reference_object')
          
-         1532         978 LOAD_CONST               0 ('CalendarEvent')
+         1537         978 LOAD_CONST               0 ('CalendarEvent')
          
-         1531         980 LOAD_CONST              17 ('request')
+         1536         980 LOAD_CONST              17 ('request')
          
-         1532         982 LOAD_NAME               21 (HttpRequest)
+         1537         982 LOAD_NAME               21 (HttpRequest)
                       984 LOAD_CONST              15 (None)
                       986 BINARY_OP                7 (|)
          
-         1531         990 LOAD_CONST              18 ('return')
+         1536         990 LOAD_CONST              18 ('return')
          
-         1533         992 LOAD_NAME               22 (str)
+         1538         992 LOAD_NAME               22 (str)
          
-         1531         994 BUILD_TUPLE              6
-                      996 LOAD_CONST              28 (<code object value_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1530>)
+         1536         994 BUILD_TUPLE              6
+                      996 LOAD_CONST              28 (<code object value_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1535>)
                       998 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1530        1000 PRECALL                  0
+         1535        1000 PRECALL                  0
                      1004 CALL                     0
          
-         1531        1014 STORE_NAME              38 (value_color)
+         1536        1014 STORE_NAME              38 (value_color)
          
-         1537        1016 LOAD_NAME               20 (classmethod)
+         1542        1016 LOAD_NAME               20 (classmethod)
          
-         1539        1018 NOP
+         1544        1018 NOP
          
-         1538        1020 LOAD_CONST              35 ((None,))
+         1543        1020 LOAD_CONST              35 ((None,))
                      1022 LOAD_CONST              16 ('reference_object')
          
-         1539        1024 LOAD_CONST               0 ('CalendarEvent')
+         1544        1024 LOAD_CONST               0 ('CalendarEvent')
          
-         1538        1026 LOAD_CONST              17 ('request')
+         1543        1026 LOAD_CONST              17 ('request')
          
-         1539        1028 LOAD_NAME               21 (HttpRequest)
+         1544        1028 LOAD_NAME               21 (HttpRequest)
                      1030 LOAD_CONST              15 (None)
                      1032 BINARY_OP                7 (|)
          
-         1538        1036 BUILD_TUPLE              4
-                     1038 LOAD_CONST              29 (<code object value_reference_object, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1537>)
+         1543        1036 BUILD_TUPLE              4
+                     1038 LOAD_CONST              29 (<code object value_reference_object, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1542>)
                      1040 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1537        1042 PRECALL                  0
+         1542        1042 PRECALL                  0
                      1046 CALL                     0
          
-         1538        1056 STORE_NAME              39 (value_reference_object)
+         1543        1056 STORE_NAME              39 (value_reference_object)
          
-         1544        1058 LOAD_NAME               20 (classmethod)
+         1549        1058 LOAD_NAME               20 (classmethod)
          
-         1546        1060 NOP
+         1551        1060 NOP
          
-         1545        1062 LOAD_CONST              36 ((None, None))
+         1550        1062 LOAD_CONST              36 ((None, None))
                      1064 LOAD_CONST              17 ('request')
          
-         1546        1066 LOAD_NAME               21 (HttpRequest)
+         1551        1066 LOAD_NAME               21 (HttpRequest)
                      1068 LOAD_CONST              15 (None)
                      1070 BINARY_OP                7 (|)
          
-         1545        1074 LOAD_CONST              30 ('params')
+         1550        1074 LOAD_CONST              30 ('params')
          
-         1546        1076 LOAD_NAME               40 (dict)
+         1551        1076 LOAD_NAME               40 (dict)
                      1078 LOAD_NAME               22 (str)
                      1080 LOAD_NAME               41 (any)
                      1082 BUILD_TUPLE              2
                      1084 BINARY_SUBSCR
                      1094 LOAD_CONST              15 (None)
                      1096 BINARY_OP                7 (|)
          
-         1545        1100 LOAD_CONST              18 ('return')
+         1550        1100 LOAD_CONST              18 ('return')
          
-         1547        1102 LOAD_NAME               42 (Iterable)
+         1552        1102 LOAD_NAME               42 (Iterable)
          
-         1545        1104 BUILD_TUPLE              6
-                     1106 LOAD_CONST              31 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1544>)
+         1550        1104 BUILD_TUPLE              6
+                     1106 LOAD_CONST              31 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1549>)
                      1108 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1544        1110 PRECALL                  0
+         1549        1110 PRECALL                  0
                      1114 CALL                     0
          
-         1545        1124 STORE_NAME              43 (get_objects)
+         1550        1124 STORE_NAME              43 (get_objects)
          
-         1551        1126 LOAD_CLOSURE             0 (__class__)
+         1556        1126 LOAD_CLOSURE             0 (__class__)
                      1128 BUILD_TUPLE              1
-                     1130 LOAD_CONST              32 (<code object save, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1551>)
+                     1130 LOAD_CONST              32 (<code object save, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1556>)
                      1132 MAKE_FUNCTION            8 (closure)
                      1134 STORE_NAME              44 (save)
          
-         1562        1136 PUSH_NULL
+         1567        1136 PUSH_NULL
                      1138 LOAD_BUILD_CLASS
-                     1140 LOAD_CONST              33 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1562>)
+                     1140 LOAD_CONST              33 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1567>)
                      1142 MAKE_FUNCTION            0
                      1144 LOAD_CONST              34 ('Meta')
                      1146 PRECALL                  2
                      1150 CALL                     2
                      1160 STORE_NAME              45 (Meta)
                      1162 LOAD_CLOSURE             0 (__class__)
                      1164 COPY                     1
@@ -11667,19 +11682,19 @@
                stacksize : 2
                flags     : 3
                code
                   0x8700970088006601640184087c014400a6000000ab0000000000000000
                   005300
                               0 MAKE_CELL                0 (self)
                
-               1442           2 RESUME                   0
+               1447           2 RESUME                   0
                
-               1444           4 LOAD_CLOSURE             0 (self)
+               1449           4 LOAD_CLOSURE             0 (self)
                               6 BUILD_TUPLE              1
-                              8 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1444>)
+                              8 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1449>)
                              10 MAKE_FUNCTION            8 (closure)
                              12 LOAD_FAST                1 (seq)
                              14 GET_ITER
                              16 PRECALL                  0
                              20 CALL                     0
                              30 RETURN_VALUE
                consts
@@ -11692,15 +11707,15 @@
                      code
                         0x9501970067007c005d337d017401000000000000000000007c01740200
                         000000000000000000a6020000ab020000000000000000721a7c01a00200
                         0000000000000000000000000000000000000089026a0300000000000000
                         00a6010000ab0100000000000000006e017c0191028c345300
                                     0 COPY_FREE_VARS           1
                      
-                     1444           2 RESUME                   0
+                     1449           2 RESUME                   0
                                     4 BUILD_LIST               0
                                     6 LOAD_FAST                0 (.0)
                               >>    8 FOR_ITER                51 (to 112)
                                    10 STORE_FAST               1 (dt)
                                    12 LOAD_GLOBAL              1 (NULL + isinstance)
                                    24 LOAD_FAST                1 (dt)
                                    26 LOAD_GLOBAL              2 (datetime)
@@ -11721,164 +11736,164 @@
                      consts
                      names      ('isinstance', 'datetime', 'astimezone', 'timezone')
                      varnames   ('.0', 'dt')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 1444
+                     firstlineno 1449
                      lnotab 0x
                names      ()
                varnames   ('self', 'seq')
                freevars   ()
                cellvars   ('self',)
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'provide_list_in_timezone'
-               firstlineno 1442
+               firstlineno 1447
                lnotab 0x0402
             None
             'reference_object'
             'request'
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000082
                   01
-               1446           0 RESUME                   0
+               1451           0 RESUME                   0
                
-               1451           2 LOAD_GLOBAL              1 (NULL + NotImplementedError)
+               1456           2 LOAD_GLOBAL              1 (NULL + NotImplementedError)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 RAISE_VARARGS            1
                consts
                   'Return the title of the calendar event.'
                names      ('NotImplementedError',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_title'
-               firstlineno 1446
+               firstlineno 1451
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c016a000000000000000000721f7c016a000000000000000000a0
                   0100000000000000000000000000000000000000007c016a020000000000
                   000000a6010000ab01000000000000000053007c016a0300000000000000
                   005300
-               1453           0 RESUME                   0
+               1458           0 RESUME                   0
                
-               1458           2 LOAD_FAST                1 (reference_object)
+               1463           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (datetime_start)
                              14 POP_JUMP_FORWARD_IF_FALSE    31 (to 78)
                
-               1459          16 LOAD_FAST                1 (reference_object)
+               1464          16 LOAD_FAST                1 (reference_object)
                              18 LOAD_ATTR                0 (datetime_start)
                              28 LOAD_METHOD              1 (astimezone)
                              50 LOAD_FAST                1 (reference_object)
                              52 LOAD_ATTR                2 (timezone)
                              62 PRECALL                  1
                              66 CALL                     1
                              76 RETURN_VALUE
                
-               1460     >>   78 LOAD_FAST                1 (reference_object)
+               1465     >>   78 LOAD_FAST                1 (reference_object)
                              80 LOAD_ATTR                3 (date_start)
                              90 RETURN_VALUE
                consts
                   'Return the start datetime of the calendar event.'
                names      ('datetime_start', 'astimezone', 'timezone', 'date_start')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_start_datetime'
-               firstlineno 1453
+               firstlineno 1458
                lnotab 0x02050e013e01
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c016a000000000000000000721f7c016a000000000000000000a0
                   0100000000000000000000000000000000000000007c016a020000000000
                   000000a6010000ab01000000000000000053007c016a0300000000000000
                   007c016a0400000000000000006b02000000007202640153007c016a0300
                   000000000000005300
-               1462           0 RESUME                   0
+               1467           0 RESUME                   0
                
-               1467           2 LOAD_FAST                1 (reference_object)
+               1472           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (datetime_end)
                              14 POP_JUMP_FORWARD_IF_FALSE    31 (to 78)
                
-               1468          16 LOAD_FAST                1 (reference_object)
+               1473          16 LOAD_FAST                1 (reference_object)
                              18 LOAD_ATTR                0 (datetime_end)
                              28 LOAD_METHOD              1 (astimezone)
                              50 LOAD_FAST                1 (reference_object)
                              52 LOAD_ATTR                2 (timezone)
                              62 PRECALL                  1
                              66 CALL                     1
                              76 RETURN_VALUE
                
-               1469     >>   78 LOAD_FAST                1 (reference_object)
+               1474     >>   78 LOAD_FAST                1 (reference_object)
                              80 LOAD_ATTR                3 (date_end)
                              90 LOAD_FAST                1 (reference_object)
                              92 LOAD_ATTR                4 (date_start)
                             102 COMPARE_OP               2 (==)
                             108 POP_JUMP_FORWARD_IF_FALSE     2 (to 114)
                
-               1472         110 LOAD_CONST               1 (None)
+               1477         110 LOAD_CONST               1 (None)
                             112 RETURN_VALUE
                
-               1473     >>  114 LOAD_FAST                1 (reference_object)
+               1478     >>  114 LOAD_FAST                1 (reference_object)
                             116 LOAD_ATTR                3 (date_end)
                             126 RETURN_VALUE
                consts
                   'Return the end datetime of the calendar event.'
                   None
                names      ('datetime_end', 'astimezone', 'timezone', 'date_end', 'date_start')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_end_datetime'
-               firstlineno 1462
+               firstlineno 1467
                lnotab 0x02050e013e0120030401
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c016a000000000000000000720c7c016a0000000000000000006a
                   0100000000000000007302640153007405000000000000000000007c016a
                   0000000000000000006a0100000000000000006402190000000000000000
                   00a6010000ab0100000000000000005300
-               1475           0 RESUME                   0
+               1480           0 RESUME                   0
                
-               1480           2 LOAD_FAST                1 (reference_object)
+               1485           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (recurrences)
                              14 POP_JUMP_FORWARD_IF_FALSE    12 (to 40)
                              16 LOAD_FAST                1 (reference_object)
                              18 LOAD_ATTR                0 (recurrences)
                              28 LOAD_ATTR                1 (rrules)
                              38 POP_JUMP_FORWARD_IF_TRUE     2 (to 44)
                
-               1481     >>   40 LOAD_CONST               1 (None)
+               1486     >>   40 LOAD_CONST               1 (None)
                              42 RETURN_VALUE
                
-               1483     >>   44 LOAD_GLOBAL              5 (NULL + build_rrule_from_recurrences_rrule)
+               1488     >>   44 LOAD_GLOBAL              5 (NULL + build_rrule_from_recurrences_rrule)
                              56 LOAD_FAST                1 (reference_object)
                              58 LOAD_ATTR                0 (recurrences)
                              68 LOAD_ATTR                1 (rrules)
                              78 LOAD_CONST               2 (0)
                              80 BINARY_SUBSCR
                              90 PRECALL                  1
                              94 CALL                     1
@@ -11889,35 +11904,35 @@
                   0
                names      ('recurrences', 'rrules', 'build_rrule_from_recurrences_rrule')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_rrule'
-               firstlineno 1475
+               firstlineno 1480
                lnotab 0x020526010402
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c016a0000000000000000007302640153007c01a0010000000000
                   0000000000000000000000000000007c016a0000000000000000006a0200
                   00000000000000a6010000ab0100000000000000005300
-               1485           0 RESUME                   0
+               1490           0 RESUME                   0
                
-               1490           2 LOAD_FAST                1 (reference_object)
+               1495           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (recurrences)
                              14 POP_JUMP_FORWARD_IF_TRUE     2 (to 20)
                
-               1491          16 LOAD_CONST               1 (None)
+               1496          16 LOAD_CONST               1 (None)
                              18 RETURN_VALUE
                
-               1492     >>   20 LOAD_FAST                1 (reference_object)
+               1497     >>   20 LOAD_FAST                1 (reference_object)
                              22 LOAD_METHOD              1 (provide_list_in_timezone)
                              44 LOAD_FAST                1 (reference_object)
                              46 LOAD_ATTR                0 (recurrences)
                              56 LOAD_ATTR                2 (rdates)
                              66 PRECALL                  1
                              70 CALL                     1
                              80 RETURN_VALUE
@@ -11926,39 +11941,39 @@
                   None
                names      ('recurrences', 'provide_list_in_timezone', 'rdates')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_rdate'
-               firstlineno 1485
+               firstlineno 1490
                lnotab 0x02050e010401
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c016a000000000000000000720c7c016a0000000000000000006a
                   010000000000000000730264015300640284007c016a0000000000000000
                   006a0100000000000000004400a6000000ab0000000000000000005300
-               1494           0 RESUME                   0
+               1499           0 RESUME                   0
                
-               1499           2 LOAD_FAST                1 (reference_object)
+               1504           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (recurrences)
                              14 POP_JUMP_FORWARD_IF_FALSE    12 (to 40)
                              16 LOAD_FAST                1 (reference_object)
                              18 LOAD_ATTR                0 (recurrences)
                              28 LOAD_ATTR                1 (exrules)
                              38 POP_JUMP_FORWARD_IF_TRUE     2 (to 44)
                
-               1500     >>   40 LOAD_CONST               1 (None)
+               1505     >>   40 LOAD_CONST               1 (None)
                              42 RETURN_VALUE
                
-               1501     >>   44 LOAD_CONST               2 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1501>)
+               1506     >>   44 LOAD_CONST               2 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1506>)
                              46 MAKE_FUNCTION            0
                              48 LOAD_FAST                1 (reference_object)
                              50 LOAD_ATTR                0 (recurrences)
                              60 LOAD_ATTR                1 (exrules)
                              70 GET_ITER
                              72 PRECALL                  0
                              76 CALL                     0
@@ -11970,15 +11985,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d117d017401000000000000000000007c01a6010000ab
                         01000000000000000091028c125300
-                     1501           0 RESUME                   0
+                     1506           0 RESUME                   0
                                     2 BUILD_LIST               0
                                     4 LOAD_FAST                0 (.0)
                               >>    6 FOR_ITER                17 (to 42)
                                     8 STORE_FAST               1 (r)
                                    10 LOAD_GLOBAL              1 (NULL + build_rrule_from_recurrences_rrule)
                                    22 LOAD_FAST                1 (r)
                                    24 PRECALL                  1
@@ -11989,43 +12004,43 @@
                      consts
                      names      ('build_rrule_from_recurrences_rrule',)
                      varnames   ('.0', 'r')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 1501
+                     firstlineno 1506
                      lnotab 0x
                names      ('recurrences', 'exrules')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_exrule'
-               firstlineno 1494
+               firstlineno 1499
                lnotab 0x020526010401
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c016a0000000000000000007302640153007c01a0010000000000
                   0000000000000000000000000000007c016a0000000000000000006a0200
                   00000000000000a6010000ab0100000000000000005300
-               1503           0 RESUME                   0
+               1508           0 RESUME                   0
                
-               1508           2 LOAD_FAST                1 (reference_object)
+               1513           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (recurrences)
                              14 POP_JUMP_FORWARD_IF_TRUE     2 (to 20)
                
-               1509          16 LOAD_CONST               1 (None)
+               1514          16 LOAD_CONST               1 (None)
                              18 RETURN_VALUE
                
-               1510     >>   20 LOAD_FAST                1 (reference_object)
+               1515     >>   20 LOAD_FAST                1 (reference_object)
                              22 LOAD_METHOD              1 (provide_list_in_timezone)
                              44 LOAD_FAST                1 (reference_object)
                              46 LOAD_ATTR                0 (recurrences)
                              56 LOAD_ATTR                2 (exdates)
                              66 PRECALL                  1
                              70 CALL                     1
                              80 RETURN_VALUE
@@ -12034,43 +12049,43 @@
                   None
                names      ('recurrences', 'provide_list_in_timezone', 'exdates')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_exdate'
-               firstlineno 1503
+               firstlineno 1508
                lnotab 0x02050e010401
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c016a000000000000000000721c7c00a001000000000000000000
                   00000000000000000000007c016a0000000000000000007c02ac01a60200
                   00ab02000000000000000053007c006a0200000000000000009b0064027c
                   016a0300000000000000009b009d035300
-               1512           0 RESUME                   0
+               1517           0 RESUME                   0
                
-               1517           2 LOAD_FAST                1 (reference_object)
+               1522           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (amends)
                              14 POP_JUMP_FORWARD_IF_FALSE    28 (to 72)
                
-               1518          16 LOAD_FAST                0 (cls)
+               1523          16 LOAD_FAST                0 (cls)
                              18 LOAD_METHOD              1 (value_unique_id)
                              40 LOAD_FAST                1 (reference_object)
                              42 LOAD_ATTR                0 (amends)
                              52 LOAD_FAST                2 (request)
                              54 KW_NAMES                 1
                              56 PRECALL                  2
                              60 CALL                     2
                              70 RETURN_VALUE
                
-               1519     >>   72 LOAD_FAST                0 (cls)
+               1524     >>   72 LOAD_FAST                0 (cls)
                              74 LOAD_ATTR                2 (name)
                              84 FORMAT_VALUE             0
                              86 LOAD_CONST               2 ('-')
                              88 LOAD_FAST                1 (reference_object)
                              90 LOAD_ATTR                3 (id)
                             100 FORMAT_VALUE             0
                             102 BUILD_STRING             3
@@ -12081,128 +12096,128 @@
                   '-'
                names      ('amends', 'value_unique_id', 'name', 'id')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_unique_id'
-               firstlineno 1512
+               firstlineno 1517
                lnotab 0x02050e013801
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c016a000000000000000000721c7c016a000000000000000000a0
                   0100000000000000000000000000000000000000007c017c02ac01a60200
                   00ab020000000000000000530064025300
-               1521           0 RESUME                   0
+               1526           0 RESUME                   0
                
-               1526           2 LOAD_FAST                1 (reference_object)
+               1531           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (amends)
                              14 POP_JUMP_FORWARD_IF_FALSE    28 (to 72)
                
-               1527          16 LOAD_FAST                1 (reference_object)
+               1532          16 LOAD_FAST                1 (reference_object)
                              18 LOAD_ATTR                0 (amends)
                              28 LOAD_METHOD              1 (value_start_datetime)
                              50 LOAD_FAST                1 (reference_object)
                              52 LOAD_FAST                2 (request)
                              54 KW_NAMES                 1
                              56 PRECALL                  2
                              60 CALL                     2
                              70 RETURN_VALUE
                
-               1528     >>   72 LOAD_CONST               2 (None)
+               1533     >>   72 LOAD_CONST               2 (None)
                              74 RETURN_VALUE
                consts
                   'Return the recurrence id of the calendar event.'
                   ('request',)
                   None
                names      ('amends', 'value_start_datetime')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_recurrence_id'
-               firstlineno 1521
+               firstlineno 1526
                lnotab 0x02050e013801
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c02a6
                   010000ab0100000000000000005300
-               1530           0 RESUME                   0
+               1535           0 RESUME                   0
                
-               1535           2 LOAD_FAST                0 (cls)
+               1540           2 LOAD_FAST                0 (cls)
                               4 LOAD_METHOD              0 (get_color)
                              26 LOAD_FAST                2 (request)
                              28 PRECALL                  1
                              32 CALL                     1
                              42 RETURN_VALUE
                consts
                   'Return the color of the calendar.'
                names      ('get_color',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_color'
-               firstlineno 1530
+               firstlineno 1535
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007c015300
-               1537           0 RESUME                   0
+               1542           0 RESUME                   0
                
-               1542           2 LOAD_FAST                1 (reference_object)
+               1547           2 LOAD_FAST                1 (reference_object)
                               4 RETURN_VALUE
                consts
                   'Return the reference object itself.'
                names      ()
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_reference_object'
-               firstlineno 1537
+               firstlineno 1542
                lnotab 0x0205
             'params'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c00a6010000ab0100000000000000005300
-               1544           0 RESUME                   0
+               1549           0 RESUME                   0
                
-               1549           2 LOAD_FAST                0 (cls)
+               1554           2 LOAD_FAST                0 (cls)
                               4 LOAD_ATTR                0 (objects)
                              14 LOAD_METHOD              1 (instance_of)
                              36 LOAD_FAST                0 (cls)
                              38 PRECALL                  1
                              42 CALL                     1
                              52 RETURN_VALUE
                consts
                   'Return all objects that should be included in the calendar.'
                names      ('objects', 'instance_of')
                varnames   ('cls', 'request', 'params')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_objects'
-               firstlineno 1544
+               firstlineno 1549
                lnotab 0x0205
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
@@ -12214,60 +12229,60 @@
                   00000000007c005f0100000000000000007c006a00000000000000000072
                   187c006a01000000000000000072117c006a0000000000000000006a0200
                   000000000000007c005f0400000000000000000200740b00000000000000
                   000000a6000000ab0000000000000000006a0600000000000000007c0169
                   007c02a4018e01010064005300
                               0 COPY_FREE_VARS           1
                
-               1551           2 RESUME                   0
+               1556           2 RESUME                   0
                
-               1553           4 LOAD_FAST                0 (self)
+               1558           4 LOAD_FAST                0 (self)
                               6 LOAD_ATTR                0 (datetime_start)
                
-               1552          16 POP_JUMP_FORWARD_IF_FALSE    74 (to 166)
+               1557          16 POP_JUMP_FORWARD_IF_FALSE    74 (to 166)
                
-               1554          18 LOAD_FAST                0 (self)
+               1559          18 LOAD_FAST                0 (self)
                              20 LOAD_ATTR                1 (datetime_end)
                
-               1552          30 POP_JUMP_FORWARD_IF_FALSE    67 (to 166)
+               1557          30 POP_JUMP_FORWARD_IF_FALSE    67 (to 166)
                
-               1555          32 LOAD_FAST                0 (self)
+               1560          32 LOAD_FAST                0 (self)
                              34 LOAD_ATTR                0 (datetime_start)
                              44 LOAD_ATTR                2 (tzinfo)
                              54 LOAD_FAST                0 (self)
                              56 LOAD_ATTR                1 (datetime_end)
                              66 LOAD_ATTR                2 (tzinfo)
                              76 COMPARE_OP               3 (!=)
                              82 POP_JUMP_FORWARD_IF_FALSE    41 (to 166)
                
-               1557          84 LOAD_FAST                0 (self)
+               1562          84 LOAD_FAST                0 (self)
                              86 LOAD_ATTR                1 (datetime_end)
                              96 LOAD_METHOD              3 (astimezone)
                             118 LOAD_FAST                0 (self)
                             120 LOAD_ATTR                0 (datetime_start)
                             130 LOAD_ATTR                2 (tzinfo)
                             140 PRECALL                  1
                             144 CALL                     1
                             154 LOAD_FAST                0 (self)
                             156 STORE_ATTR               1 (datetime_end)
                
-               1558     >>  166 LOAD_FAST                0 (self)
+               1563     >>  166 LOAD_FAST                0 (self)
                             168 LOAD_ATTR                0 (datetime_start)
                             178 POP_JUMP_FORWARD_IF_FALSE    24 (to 228)
                             180 LOAD_FAST                0 (self)
                             182 LOAD_ATTR                1 (datetime_end)
                             192 POP_JUMP_FORWARD_IF_FALSE    17 (to 228)
                
-               1559         194 LOAD_FAST                0 (self)
+               1564         194 LOAD_FAST                0 (self)
                             196 LOAD_ATTR                0 (datetime_start)
                             206 LOAD_ATTR                2 (tzinfo)
                             216 LOAD_FAST                0 (self)
                             218 STORE_ATTR               4 (timezone)
                
-               1560     >>  228 PUSH_NULL
+               1565     >>  228 PUSH_NULL
                             230 LOAD_GLOBAL             11 (NULL + super)
                             242 PRECALL                  0
                             246 CALL                     0
                             256 LOAD_ATTR                6 (save)
                             266 LOAD_FAST                1 (args)
                             268 BUILD_MAP                0
                             270 LOAD_FAST                2 (kwargs)
@@ -12280,15 +12295,15 @@
                   None
                names      ('datetime_start', 'datetime_end', 'tzinfo', 'astimezone', 'timezone', 'super', 'save')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'save'
-               firstlineno 1551
+               firstlineno 1556
                lnotab 0x04020cff02020cfe0203340252011c012201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 9
                flags     : 0
                code
@@ -12299,114 +12314,114 @@
                   000000000000000200650864036403ac07a6020000ab0200000000000000
                   000f006408ac06a6020000ab020000000000000000020065066a07000000
                   00000000000200650864096403ac0aa6020000ab0200000000000000000f
                   00640bac06a6020000ab020000000000000000020065066a070000000000
                   0000000200650864096403ac0ca6020000ab0200000000000000000f0064
                   0dac06a6020000ab02000000000000000067045a096700640ea2015a0a64
                   0f5300
-               1562           0 RESUME                   0
+               1567           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('CalendarEvent.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1563          10 PUSH_NULL
+               1568          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('Calendar Event')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1564          32 PUSH_NULL
+               1569          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('Calendar Events')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                
-               1566          54 PUSH_NULL
+               1571          54 PUSH_NULL
                              56 LOAD_NAME                6 (models)
                              58 LOAD_ATTR                7 (CheckConstraint)
                
-               1567          68 PUSH_NULL
+               1572          68 PUSH_NULL
                              70 LOAD_NAME                8 (Q)
                              72 LOAD_CONST               3 (True)
                              74 LOAD_CONST               3 (True)
                              76 KW_NAMES                 4
                              78 PRECALL                  2
                              82 CALL                     2
                              92 UNARY_INVERT
                
-               1568          94 LOAD_CONST               5 ('datetime_start_or_date_start')
+               1573          94 LOAD_CONST               5 ('datetime_start_or_date_start')
                
-               1566          96 KW_NAMES                 6
+               1571          96 KW_NAMES                 6
                              98 PRECALL                  2
                             102 CALL                     2
                
-               1570         112 PUSH_NULL
+               1575         112 PUSH_NULL
                             114 LOAD_NAME                6 (models)
                             116 LOAD_ATTR                7 (CheckConstraint)
                
-               1571         126 PUSH_NULL
+               1576         126 PUSH_NULL
                             128 LOAD_NAME                8 (Q)
                             130 LOAD_CONST               3 (True)
                             132 LOAD_CONST               3 (True)
                             134 KW_NAMES                 7
                             136 PRECALL                  2
                             140 CALL                     2
                             150 UNARY_INVERT
                
-               1572         152 LOAD_CONST               8 ('datetime_end_or_date_end')
+               1577         152 LOAD_CONST               8 ('datetime_end_or_date_end')
                
-               1570         154 KW_NAMES                 6
+               1575         154 KW_NAMES                 6
                             156 PRECALL                  2
                             160 CALL                     2
                
-               1574         170 PUSH_NULL
+               1579         170 PUSH_NULL
                             172 LOAD_NAME                6 (models)
                             174 LOAD_ATTR                7 (CheckConstraint)
                
-               1575         184 PUSH_NULL
+               1580         184 PUSH_NULL
                             186 LOAD_NAME                8 (Q)
                             188 LOAD_CONST               9 (False)
                             190 LOAD_CONST               3 (True)
                             192 KW_NAMES                10
                             194 PRECALL                  2
                             198 CALL                     2
                             208 UNARY_INVERT
                
-               1576         210 LOAD_CONST              11 ('timezone_if_datetime_start')
+               1581         210 LOAD_CONST              11 ('timezone_if_datetime_start')
                
-               1574         212 KW_NAMES                 6
+               1579         212 KW_NAMES                 6
                             214 PRECALL                  2
                             218 CALL                     2
                
-               1578         228 PUSH_NULL
+               1583         228 PUSH_NULL
                             230 LOAD_NAME                6 (models)
                             232 LOAD_ATTR                7 (CheckConstraint)
                
-               1579         242 PUSH_NULL
+               1584         242 PUSH_NULL
                             244 LOAD_NAME                8 (Q)
                             246 LOAD_CONST               9 (False)
                             248 LOAD_CONST               3 (True)
                             250 KW_NAMES                12
                             252 PRECALL                  2
                             256 CALL                     2
                             266 UNARY_INVERT
                
-               1580         268 LOAD_CONST              13 ('timezone_if_datetime_end')
+               1585         268 LOAD_CONST              13 ('timezone_if_datetime_end')
                
-               1578         270 KW_NAMES                 6
+               1583         270 KW_NAMES                 6
                             272 PRECALL                  2
                             276 CALL                     2
                
-               1565         286 BUILD_LIST               4
+               1570         286 BUILD_LIST               4
                             288 STORE_NAME               9 (constraints)
                
-               1583         290 BUILD_LIST               0
+               1588         290 BUILD_LIST               0
                             292 LOAD_CONST              14 (('datetime_start', 'date_start', 'datetime_end', 'date_end'))
                             294 LIST_EXTEND              1
                             296 STORE_NAME              10 (ordering)
                             298 LOAD_CONST              15 (None)
                             300 RETURN_VALUE
                consts
                   'CalendarEvent.Meta'
@@ -12427,28 +12442,28 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural', 'models', 'CheckConstraint', 'Q', 'constraints', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1562
+               firstlineno 1567
                lnotab
                   0x0a01160116020e011a0102fe10040e011a0102fe10040e011a0102fe10
                   040e011a0102fe10f30412
             'Meta'
             (None,)
             (None, None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'models', 'DateTimeField', '_', 'datetime_start', 'datetime_end', 'TimeZoneField', 'timezone', 'DateField', 'date_start', 'date_end', 'RecurrenceField', 'recurrences', 'ForeignKey', 'CASCADE', 'amends', 'provide_list_in_timezone', 'classmethod', 'HttpRequest', 'str', 'value_title', 'Union', 'datetime', 'date', 'value_start_datetime', 'value_end_datetime', 'Optional', 'vRecur', 'value_rrule', 'list', 'value_rdate', 'value_exrule', 'value_exdate', 'value_unique_id', 'value_recurrence_id', 'value_color', 'value_reference_object', 'dict', 'any', 'Iterable', 'get_objects', 'save', 'Meta', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'CalendarEvent'
-         firstlineno 1409
+         firstlineno 1414
          lnotab
             0x0c01040f0e0118ff120338012e01380138012e010e0102010c01020102
             01140102fa12090604020202ff040102ff020108ff020202fe06ff0e0102
             06020202ff040102ff020108ff020212fe06ff0e010208020202ff040102
             ff020108ff020214fe06ff0e01020c020202ff040102ff020108ff02020e
             fe06ff0e010209020202ff040102ff020108ff02021afe06ff0e01020802
             0202ff040102ff020108ff02021afe06ff0e010208020202ff040102ff02
@@ -12460,32 +12475,32 @@
       'CalendarEvent'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015300
-         1586           0 RESUME                   0
+         1591           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('FreeBusy')
                         8 STORE_NAME               2 (__qualname__)
          
-         1587          10 LOAD_CONST               1 (None)
+         1592          10 LOAD_CONST               1 (None)
                        12 RETURN_VALUE
          consts
             'FreeBusy'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'FreeBusy'
-         firstlineno 1586
+         firstlineno 1591
          lnotab 0x0a01
       'FreeBusy'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
@@ -12501,215 +12516,215 @@
             006408650b6606640d8405a6000000ab0000000000000000005a12650864
             12640665096407650a64057a070000640865136606640e8405a6000000ab
             0000000000000000005a14650864126407650a64057a0700006408650b66
             04640f8405a6000000ab0000000000000000005a15650809006413640765
             0a64057a07000064106513650b651666021900000000000000000064057a
             07000064086517660664118405a6000000ab0000000000000000005a1864
             055300
-         1590           0 RESUME                   0
+         1595           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('BirthdayEvent')
                         8 STORE_NAME               2 (__qualname__)
          
-         1591          10 LOAD_CONST               1 ('A calendar feed with all birthdays.')
+         1596          10 LOAD_CONST               1 ('A calendar feed with all birthdays.')
                        12 STORE_NAME               3 (__doc__)
          
-         1593          14 LOAD_CONST               2 ('birthdays')
+         1598          14 LOAD_CONST               2 ('birthdays')
                        16 STORE_NAME               4 (name)
          
-         1594          18 PUSH_NULL
+         1599          18 PUSH_NULL
                        20 LOAD_NAME                5 (_)
                        22 LOAD_CONST               3 ('Birthdays')
                        24 PRECALL                  1
                        28 CALL                     1
                        38 STORE_NAME               6 (verbose_name)
          
-         1595          40 LOAD_CONST               4 ('core.view_birthday_calendar')
+         1600          40 LOAD_CONST               4 ('core.view_birthday_calendar')
                        42 STORE_NAME               7 (permission_required)
          
-         1597          44 LOAD_NAME                8 (classmethod)
+         1602          44 LOAD_NAME                8 (classmethod)
          
-         1598          46 LOAD_CONST              18 ((None,))
+         1603          46 LOAD_CONST              18 ((None,))
                        48 LOAD_CONST               6 ('reference_object')
                        50 LOAD_NAME                9 (Person)
                        52 LOAD_CONST               7 ('request')
                        54 LOAD_NAME               10 (HttpRequest)
                        56 LOAD_CONST               5 (None)
                        58 BINARY_OP                7 (|)
                        62 LOAD_CONST               8 ('return')
                        64 LOAD_NAME               11 (str)
                        66 BUILD_TUPLE              6
-                       68 LOAD_CONST               9 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1597>)
+                       68 LOAD_CONST               9 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1602>)
                        70 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1597          72 PRECALL                  0
+         1602          72 PRECALL                  0
                        76 CALL                     0
          
-         1598          86 STORE_NAME              12 (value_title)
+         1603          86 STORE_NAME              12 (value_title)
          
-         1601          88 LOAD_NAME                8 (classmethod)
+         1606          88 LOAD_NAME                8 (classmethod)
          
-         1602          90 LOAD_CONST              18 ((None,))
+         1607          90 LOAD_CONST              18 ((None,))
                        92 LOAD_CONST               6 ('reference_object')
                        94 LOAD_NAME                9 (Person)
                        96 LOAD_CONST               7 ('request')
                        98 LOAD_NAME               10 (HttpRequest)
                       100 LOAD_CONST               5 (None)
                       102 BINARY_OP                7 (|)
                       106 LOAD_CONST               8 ('return')
                       108 LOAD_NAME               11 (str)
                       110 BUILD_TUPLE              6
-                      112 LOAD_CONST              10 (<code object value_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1601>)
+                      112 LOAD_CONST              10 (<code object value_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1606>)
                       114 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1601         116 PRECALL                  0
+         1606         116 PRECALL                  0
                       120 CALL                     0
          
-         1602         130 STORE_NAME              13 (value_description)
+         1607         130 STORE_NAME              13 (value_description)
          
-         1608         132 LOAD_NAME                8 (classmethod)
+         1613         132 LOAD_NAME                8 (classmethod)
          
-         1610         134 NOP
+         1615         134 NOP
          
-         1609         136 LOAD_CONST              18 ((None,))
+         1614         136 LOAD_CONST              18 ((None,))
                       138 LOAD_CONST               6 ('reference_object')
          
-         1610         140 LOAD_NAME                9 (Person)
+         1615         140 LOAD_NAME                9 (Person)
          
-         1609         142 LOAD_CONST               7 ('request')
+         1614         142 LOAD_CONST               7 ('request')
          
-         1610         144 LOAD_NAME               10 (HttpRequest)
+         1615         144 LOAD_NAME               10 (HttpRequest)
                       146 LOAD_CONST               5 (None)
                       148 BINARY_OP                7 (|)
          
-         1609         152 LOAD_CONST               8 ('return')
+         1614         152 LOAD_CONST               8 ('return')
          
-         1611         154 LOAD_NAME               14 (date)
+         1616         154 LOAD_NAME               14 (date)
          
-         1609         156 BUILD_TUPLE              6
-                      158 LOAD_CONST              11 (<code object value_start_datetime, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1608>)
+         1614         156 BUILD_TUPLE              6
+                      158 LOAD_CONST              11 (<code object value_start_datetime, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1613>)
                       160 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1608         162 PRECALL                  0
+         1613         162 PRECALL                  0
                       166 CALL                     0
          
-         1609         176 STORE_NAME              15 (value_start_datetime)
+         1614         176 STORE_NAME              15 (value_start_datetime)
          
-         1614         178 LOAD_NAME                8 (classmethod)
+         1619         178 LOAD_NAME                8 (classmethod)
          
-         1615         180 LOAD_CONST              18 ((None,))
+         1620         180 LOAD_CONST              18 ((None,))
                       182 LOAD_CONST               6 ('reference_object')
                       184 LOAD_NAME                9 (Person)
                       186 LOAD_CONST               7 ('request')
                       188 LOAD_NAME               10 (HttpRequest)
                       190 LOAD_CONST               5 (None)
                       192 BINARY_OP                7 (|)
                       196 LOAD_CONST               8 ('return')
                       198 LOAD_NAME               16 (vRecur)
                       200 BUILD_TUPLE              6
-                      202 LOAD_CONST              12 (<code object value_rrule, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1614>)
+                      202 LOAD_CONST              12 (<code object value_rrule, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1619>)
                       204 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1614         206 PRECALL                  0
+         1619         206 PRECALL                  0
                       210 CALL                     0
          
-         1615         220 STORE_NAME              17 (value_rrule)
+         1620         220 STORE_NAME              17 (value_rrule)
          
-         1618         222 LOAD_NAME                8 (classmethod)
+         1623         222 LOAD_NAME                8 (classmethod)
          
-         1619         224 LOAD_CONST              18 ((None,))
+         1624         224 LOAD_CONST              18 ((None,))
                       226 LOAD_CONST               6 ('reference_object')
                       228 LOAD_NAME                9 (Person)
                       230 LOAD_CONST               7 ('request')
                       232 LOAD_NAME               10 (HttpRequest)
                       234 LOAD_CONST               5 (None)
                       236 BINARY_OP                7 (|)
                       240 LOAD_CONST               8 ('return')
                       242 LOAD_NAME               11 (str)
                       244 BUILD_TUPLE              6
-                      246 LOAD_CONST              13 (<code object value_unique_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1618>)
+                      246 LOAD_CONST              13 (<code object value_unique_id, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1623>)
                       248 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1618         250 PRECALL                  0
+         1623         250 PRECALL                  0
                       254 CALL                     0
          
-         1619         264 STORE_NAME              18 (value_unique_id)
+         1624         264 STORE_NAME              18 (value_unique_id)
          
-         1622         266 LOAD_NAME                8 (classmethod)
+         1627         266 LOAD_NAME                8 (classmethod)
          
-         1623         268 LOAD_CONST              18 ((None,))
+         1628         268 LOAD_CONST              18 ((None,))
                       270 LOAD_CONST               6 ('reference_object')
                       272 LOAD_NAME                9 (Person)
                       274 LOAD_CONST               7 ('request')
                       276 LOAD_NAME               10 (HttpRequest)
                       278 LOAD_CONST               5 (None)
                       280 BINARY_OP                7 (|)
                       284 LOAD_CONST               8 ('return')
                       286 LOAD_NAME               19 (dict)
                       288 BUILD_TUPLE              6
-                      290 LOAD_CONST              14 (<code object value_meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1622>)
+                      290 LOAD_CONST              14 (<code object value_meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1627>)
                       292 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1622         294 PRECALL                  0
+         1627         294 PRECALL                  0
                       298 CALL                     0
          
-         1623         308 STORE_NAME              20 (value_meta)
+         1628         308 STORE_NAME              20 (value_meta)
          
-         1629         310 LOAD_NAME                8 (classmethod)
+         1634         310 LOAD_NAME                8 (classmethod)
          
-         1630         312 LOAD_CONST              18 ((None,))
+         1635         312 LOAD_CONST              18 ((None,))
                       314 LOAD_CONST               7 ('request')
                       316 LOAD_NAME               10 (HttpRequest)
                       318 LOAD_CONST               5 (None)
                       320 BINARY_OP                7 (|)
                       324 LOAD_CONST               8 ('return')
                       326 LOAD_NAME               11 (str)
                       328 BUILD_TUPLE              4
-                      330 LOAD_CONST              15 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1629>)
+                      330 LOAD_CONST              15 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1634>)
                       332 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1629         334 PRECALL                  0
+         1634         334 PRECALL                  0
                       338 CALL                     0
          
-         1630         348 STORE_NAME              21 (get_color)
+         1635         348 STORE_NAME              21 (get_color)
          
-         1633         350 LOAD_NAME                8 (classmethod)
+         1638         350 LOAD_NAME                8 (classmethod)
          
-         1635         352 NOP
+         1640         352 NOP
          
-         1634         354 LOAD_CONST              19 ((None, None))
+         1639         354 LOAD_CONST              19 ((None, None))
                       356 LOAD_CONST               7 ('request')
          
-         1635         358 LOAD_NAME               10 (HttpRequest)
+         1640         358 LOAD_NAME               10 (HttpRequest)
                       360 LOAD_CONST               5 (None)
                       362 BINARY_OP                7 (|)
          
-         1634         366 LOAD_CONST              16 ('params')
+         1639         366 LOAD_CONST              16 ('params')
          
-         1635         368 LOAD_NAME               19 (dict)
+         1640         368 LOAD_NAME               19 (dict)
                       370 LOAD_NAME               11 (str)
                       372 LOAD_NAME               22 (any)
                       374 BUILD_TUPLE              2
                       376 BINARY_SUBSCR
                       386 LOAD_CONST               5 (None)
                       388 BINARY_OP                7 (|)
          
-         1634         392 LOAD_CONST               8 ('return')
+         1639         392 LOAD_CONST               8 ('return')
          
-         1636         394 LOAD_NAME               23 (QuerySet)
+         1641         394 LOAD_NAME               23 (QuerySet)
          
-         1634         396 BUILD_TUPLE              6
-                      398 LOAD_CONST              17 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1633>)
+         1639         396 BUILD_TUPLE              6
+                      398 LOAD_CONST              17 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1638>)
                       400 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1633         402 PRECALL                  0
+         1638         402 PRECALL                  0
                       406 CALL                     0
          
-         1634         416 STORE_NAME              24 (get_objects)
+         1639         416 STORE_NAME              24 (get_objects)
                       418 LOAD_CONST               5 (None)
                       420 RETURN_VALUE
          consts
             'BirthdayEvent'
             'A calendar feed with all birthdays.'
             'birthdays'
             'Birthdays'
@@ -12723,17 +12738,17 @@
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   00a00100000000000000000000000000000000000000007c016a02000000
                   0000000000a6010000ab0100000000000000005300
-               1597           0 RESUME                   0
+               1602           0 RESUME                   0
                
-               1599           2 LOAD_GLOBAL              1 (NULL + _)
+               1604           2 LOAD_GLOBAL              1 (NULL + _)
                              14 LOAD_CONST               1 ("{}'s birthday")
                              16 PRECALL                  1
                              20 CALL                     1
                              30 LOAD_METHOD              1 (format)
                              52 LOAD_FAST                1 (reference_object)
                              54 LOAD_ATTR                2 (addressing_name)
                              64 PRECALL                  1
@@ -12744,188 +12759,188 @@
                   "{}'s birthday"
                names      ('_', 'format', 'addressing_name')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_title'
-               firstlineno 1597
+               firstlineno 1602
                lnotab 0x0202
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97006401a00000000000000000000000000000000000000000007c016a
                   0100000000000000007405000000000000000000007c016a030000000000
                   000000a6010000ab010000000000000000ac02a6020000ab020000000000
                   0000005300
-               1601           0 RESUME                   0
+               1606           0 RESUME                   0
                
-               1603           2 LOAD_CONST               1 ('{name} was born on {birthday}.')
+               1608           2 LOAD_CONST               1 ('{name} was born on {birthday}.')
                               4 LOAD_METHOD              0 (format)
                
-               1604          26 LOAD_FAST                1 (reference_object)
+               1609          26 LOAD_FAST                1 (reference_object)
                              28 LOAD_ATTR                1 (addressing_name)
                
-               1605          38 LOAD_GLOBAL              5 (NULL + date_format)
+               1610          38 LOAD_GLOBAL              5 (NULL + date_format)
                              50 LOAD_FAST                1 (reference_object)
                              52 LOAD_ATTR                3 (date_of_birth)
                              62 PRECALL                  1
                              66 CALL                     1
                
-               1603          76 KW_NAMES                 2
+               1608          76 KW_NAMES                 2
                              78 PRECALL                  2
                              82 CALL                     2
                              92 RETURN_VALUE
                consts
                   None
                   '{name} was born on {birthday}.'
                   ('name', 'birthday')
                names      ('format', 'addressing_name', 'date_format', 'date_of_birth')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_description'
-               firstlineno 1601
+               firstlineno 1606
                lnotab 0x020218010c0126fe
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007c016a0000000000000000005300
-               1608           0 RESUME                   0
+               1613           0 RESUME                   0
                
-               1612           2 LOAD_FAST                1 (reference_object)
+               1617           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (date_of_birth)
                              14 RETURN_VALUE
                consts
                   None
                names      ('date_of_birth',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_start_datetime'
-               firstlineno 1608
+               firstlineno 1613
                lnotab 0x0204
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   005300
-               1614           0 RESUME                   0
+               1619           0 RESUME                   0
                
-               1616           2 LOAD_GLOBAL              1 (NULL + build_rrule_from_text)
+               1621           2 LOAD_GLOBAL              1 (NULL + build_rrule_from_text)
                              14 LOAD_CONST               1 ('FREQ=YEARLY')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 RETURN_VALUE
                consts
                   None
                   'FREQ=YEARLY'
                names      ('build_rrule_from_text',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_rrule'
-               firstlineno 1614
+               firstlineno 1619
                lnotab 0x0202
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code 0x970064017c016a0000000000000000009b009d025300
-               1618           0 RESUME                   0
+               1623           0 RESUME                   0
                
-               1620           2 LOAD_CONST               1 ('birthday-')
+               1625           2 LOAD_CONST               1 ('birthday-')
                               4 LOAD_FAST                1 (reference_object)
                               6 LOAD_ATTR                0 (id)
                              16 FORMAT_VALUE             0
                              18 BUILD_STRING             2
                              20 RETURN_VALUE
                consts
                   None
                   'birthday-'
                names      ('id',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_unique_id'
-               firstlineno 1618
+               firstlineno 1623
                lnotab 0x0202
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c016a0000000000000000007c016a010000000000000000a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000064019c025300
-               1622           0 RESUME                   0
+               1627           0 RESUME                   0
                
-               1625           2 LOAD_FAST                1 (reference_object)
+               1630           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (addressing_name)
                
-               1626          14 LOAD_FAST                1 (reference_object)
+               1631          14 LOAD_FAST                1 (reference_object)
                              16 LOAD_ATTR                1 (date_of_birth)
                              26 LOAD_METHOD              2 (isoformat)
                              48 PRECALL                  0
                              52 CALL                     0
                
-               1624          62 LOAD_CONST               1 (('name', 'date_of_birth'))
+               1629          62 LOAD_CONST               1 (('name', 'date_of_birth'))
                              64 BUILD_CONST_KEY_MAP      2
                              66 RETURN_VALUE
                consts
                   None
                   ('name', 'date_of_birth')
                names      ('addressing_name', 'date_of_birth', 'isoformat')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_meta'
-               firstlineno 1622
+               firstlineno 1627
                lnotab 0x02030c0130fe
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000064
                   01190000000000000000005300
-               1629           0 RESUME                   0
+               1634           0 RESUME                   0
                
-               1631           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+               1636           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 LOAD_CONST               1 ('calendar__birthday_color')
                              30 BINARY_SUBSCR
                              40 RETURN_VALUE
                consts
                   None
                   'calendar__birthday_color'
                names      ('get_site_preferences',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_color'
-               firstlineno 1629
+               firstlineno 1634
                lnotab 0x0202
             'params'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 10
                flags     : 3
@@ -12935,84 +12950,84 @@
                   00000000007d037c0172577c03a002000000000000000000000000000000
                   00000000007407000000000000000000007c016a0400000000000000006a
                   0500000000000000006a060000000000000000ac03a6010000ab01000000
                   0000000000740700000000000000000000740f000000000000000000007c
                   016a04000000000000000064047c03a6030000ab030000000000000000ac
                   05a6010000ab0100000000000000007a070000a6010000ab010000000000
                   0000007d037c035300
-               1633           0 RESUME                   0
+               1638           0 RESUME                   0
                
-               1637           2 LOAD_GLOBAL              0 (Person)
+               1642           2 LOAD_GLOBAL              0 (Person)
                              14 LOAD_ATTR                1 (objects)
                              24 LOAD_METHOD              2 (filter)
                              46 LOAD_CONST               1 (False)
                              48 KW_NAMES                 2
                              50 PRECALL                  1
                              54 CALL                     1
                              64 STORE_FAST               3 (qs)
                
-               1638          66 LOAD_FAST                1 (request)
+               1643          66 LOAD_FAST                1 (request)
                              68 POP_JUMP_FORWARD_IF_FALSE    87 (to 244)
                
-               1639          70 LOAD_FAST                3 (qs)
+               1644          70 LOAD_FAST                3 (qs)
                              72 LOAD_METHOD              2 (filter)
                
-               1640          94 LOAD_GLOBAL              7 (NULL + Q)
+               1645          94 LOAD_GLOBAL              7 (NULL + Q)
                             106 LOAD_FAST                1 (request)
                             108 LOAD_ATTR                4 (user)
                             118 LOAD_ATTR                5 (person)
                             128 LOAD_ATTR                6 (pk)
                             138 KW_NAMES                 3
                             140 PRECALL                  1
                             144 CALL                     1
                
-               1641         154 LOAD_GLOBAL              7 (NULL + Q)
+               1646         154 LOAD_GLOBAL              7 (NULL + Q)
                             166 LOAD_GLOBAL             15 (NULL + get_objects_for_user)
                             178 LOAD_FAST                1 (request)
                             180 LOAD_ATTR                4 (user)
                             190 LOAD_CONST               4 ('core.view_personal_details')
                             192 LOAD_FAST                3 (qs)
                             194 PRECALL                  3
                             198 CALL                     3
                             208 KW_NAMES                 5
                             210 PRECALL                  1
                             214 CALL                     1
                
-               1640         224 BINARY_OP                7 (|)
+               1645         224 BINARY_OP                7 (|)
                
-               1639         228 PRECALL                  1
+               1644         228 PRECALL                  1
                             232 CALL                     1
                             242 STORE_FAST               3 (qs)
                
-               1643     >>  244 LOAD_FAST                3 (qs)
+               1648     >>  244 LOAD_FAST                3 (qs)
                             246 RETURN_VALUE
                consts
                   None
                   False
                   ('date_of_birth__isnull',)
                   ('pk',)
                   'core.view_personal_details'
                   ('pk__in',)
                names      ('Person', 'objects', 'filter', 'Q', 'user', 'person', 'pk', 'get_objects_for_user')
                varnames   ('cls', 'request', 'params', 'qs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_objects'
-               firstlineno 1633
+               firstlineno 1638
                lnotab 0x02044001040118013c0146ff04ff1004
             (None,)
             (None, None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'name', '_', 'verbose_name', 'permission_required', 'classmethod', 'Person', 'HttpRequest', 'str', 'value_title', 'value_description', 'date', 'value_start_datetime', 'vRecur', 'value_rrule', 'value_unique_id', 'dict', 'value_meta', 'get_color', 'any', 'QuerySet', 'get_objects')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'BirthdayEvent'
-         firstlineno 1590
+         firstlineno 1595
          lnotab
             0x0a01040204011601040202011aff0e01020302011aff0e010206020202
             ff040102ff020108ff020202fe06ff0e01020502011aff0e01020302011a
             ff0e01020302011aff0e010206020116ff0e010203020202ff040108ff02
             0118ff020202fe06ff0e01
       'BirthdayEvent'
       code
@@ -13032,177 +13047,177 @@
             05640ca6010000ab010000000000000000640dac0ea6020000ab02000000
             00000000005a14640865156516190000000000000000006602640f84045a
             1765086410651864086519651a651b640019000000000000000000660219
             000000000000000000660464118404a6000000ab0000000000000000005a
             1c650864128400a6000000ab0000000000000000005a1d6408650a660264
             1384045a1e02004700641484006415a6020000ab0200000000000000005a
             1f64055300
-         1646           0 RESUME                   0
+         1651           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('Holiday')
                         8 STORE_NAME               2 (__qualname__)
          
-         1647          10 LOAD_CONST               1 ('Holiday model for keeping track of school holidays.')
+         1652          10 LOAD_CONST               1 ('Holiday model for keeping track of school holidays.')
                        12 STORE_NAME               3 (__doc__)
          
-         1649          14 LOAD_CONST               2 ('holidays')
+         1654          14 LOAD_CONST               2 ('holidays')
                        16 STORE_NAME               4 (name)
          
-         1650          18 PUSH_NULL
+         1655          18 PUSH_NULL
                        20 LOAD_NAME                5 (_)
                        22 LOAD_CONST               3 ('Holidays')
                        24 PRECALL                  1
                        28 CALL                     1
                        38 STORE_NAME               6 (verbose_name)
          
-         1651          40 LOAD_CONST               4 ('core.view_holiday_calendar')
+         1656          40 LOAD_CONST               4 ('core.view_holiday_calendar')
                        42 STORE_NAME               7 (permission_required)
          
-         1653          44 LOAD_NAME                8 (classmethod)
+         1658          44 LOAD_NAME                8 (classmethod)
          
-         1654          46 LOAD_CONST              22 ((None,))
+         1659          46 LOAD_CONST              22 ((None,))
                        48 LOAD_CONST               6 ('reference_object')
                        50 LOAD_CONST               0 ('Holiday')
                        52 LOAD_CONST               7 ('request')
                        54 LOAD_NAME                9 (HttpRequest)
                        56 LOAD_CONST               5 (None)
                        58 BINARY_OP                7 (|)
                        62 LOAD_CONST               8 ('return')
                        64 LOAD_NAME               10 (str)
                        66 BUILD_TUPLE              6
-                       68 LOAD_CONST               9 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1653>)
+                       68 LOAD_CONST               9 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1658>)
                        70 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1653          72 PRECALL                  0
+         1658          72 PRECALL                  0
                        76 CALL                     0
          
-         1654          86 STORE_NAME              11 (value_title)
+         1659          86 STORE_NAME              11 (value_title)
          
-         1657          88 LOAD_NAME                8 (classmethod)
+         1662          88 LOAD_NAME                8 (classmethod)
          
-         1659          90 NOP
+         1664          90 NOP
          
-         1658          92 LOAD_CONST              22 ((None,))
+         1663          92 LOAD_CONST              22 ((None,))
                        94 LOAD_CONST               6 ('reference_object')
          
-         1659          96 LOAD_CONST               0 ('Holiday')
+         1664          96 LOAD_CONST               0 ('Holiday')
          
-         1658          98 LOAD_CONST               7 ('request')
+         1663          98 LOAD_CONST               7 ('request')
          
-         1659         100 LOAD_NAME                9 (HttpRequest)
+         1664         100 LOAD_NAME                9 (HttpRequest)
                       102 LOAD_CONST               5 (None)
                       104 BINARY_OP                7 (|)
          
-         1658         108 LOAD_CONST               8 ('return')
+         1663         108 LOAD_CONST               8 ('return')
          
-         1660         110 LOAD_NAME               10 (str)
+         1665         110 LOAD_NAME               10 (str)
          
-         1658         112 BUILD_TUPLE              6
-                      114 LOAD_CONST              10 (<code object value_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1657>)
+         1663         112 BUILD_TUPLE              6
+                      114 LOAD_CONST              10 (<code object value_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1662>)
                       116 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1657         118 PRECALL                  0
+         1662         118 PRECALL                  0
                       122 CALL                     0
          
-         1658         132 STORE_NAME              12 (value_description)
+         1663         132 STORE_NAME              12 (value_description)
          
-         1663         134 LOAD_NAME                8 (classmethod)
+         1668         134 LOAD_NAME                8 (classmethod)
          
-         1664         136 LOAD_CONST              22 ((None,))
+         1669         136 LOAD_CONST              22 ((None,))
                       138 LOAD_CONST               7 ('request')
                       140 LOAD_NAME                9 (HttpRequest)
                       142 LOAD_CONST               5 (None)
                       144 BINARY_OP                7 (|)
                       148 LOAD_CONST               8 ('return')
                       150 LOAD_NAME               10 (str)
                       152 BUILD_TUPLE              4
-                      154 LOAD_CONST              11 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1663>)
+                      154 LOAD_CONST              11 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1668>)
                       156 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1663         158 PRECALL                  0
+         1668         158 PRECALL                  0
                       162 CALL                     0
          
-         1664         172 STORE_NAME              13 (get_color)
+         1669         172 STORE_NAME              13 (get_color)
          
-         1667         174 PUSH_NULL
+         1672         174 PUSH_NULL
                       176 PUSH_NULL
                       178 LOAD_NAME               14 (PolymorphicBaseManager)
                       180 LOAD_ATTR               15 (from_queryset)
                       190 LOAD_NAME               16 (HolidayQuerySet)
                       192 PRECALL                  1
                       196 CALL                     1
                       206 PRECALL                  0
                       210 CALL                     0
                       220 STORE_NAME              17 (objects)
          
-         1669         222 PUSH_NULL
+         1674         222 PUSH_NULL
                       224 LOAD_NAME               18 (models)
                       226 LOAD_ATTR               19 (CharField)
                       236 PUSH_NULL
                       238 LOAD_NAME                5 (_)
                       240 LOAD_CONST              12 ('Name')
                       242 PRECALL                  1
                       246 CALL                     1
                       256 LOAD_CONST              13 (255)
                       258 KW_NAMES                14
                       260 PRECALL                  2
                       264 CALL                     2
                       274 STORE_NAME              20 (holiday_name)
          
-         1671         276 LOAD_CONST               8 ('return')
+         1676         276 LOAD_CONST               8 ('return')
                       278 LOAD_NAME               21 (Iterator)
                       280 LOAD_NAME               22 (date)
                       282 BINARY_SUBSCR
                       292 BUILD_TUPLE              2
-                      294 LOAD_CONST              15 (<code object get_days, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1671>)
+                      294 LOAD_CONST              15 (<code object get_days, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1676>)
                       296 MAKE_FUNCTION            4 (annotations)
                       298 STORE_NAME              23 (get_days)
          
-         1677         300 LOAD_NAME                8 (classmethod)
+         1682         300 LOAD_NAME                8 (classmethod)
          
-         1678         302 LOAD_CONST              16 ('week')
+         1683         302 LOAD_CONST              16 ('week')
                       304 LOAD_NAME               24 (CalendarWeek)
                       306 LOAD_CONST               8 ('return')
                       308 LOAD_NAME               25 (dict)
                       310 LOAD_NAME               26 (int)
                       312 LOAD_NAME               27 (Optional)
                       314 LOAD_CONST               0 ('Holiday')
                       316 BINARY_SUBSCR
                       326 BUILD_TUPLE              2
                       328 BINARY_SUBSCR
                       338 BUILD_TUPLE              4
-                      340 LOAD_CONST              17 (<code object in_week, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1677>)
+                      340 LOAD_CONST              17 (<code object in_week, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1682>)
                       342 MAKE_FUNCTION            4 (annotations)
          
-         1677         344 PRECALL                  0
+         1682         344 PRECALL                  0
                       348 CALL                     0
          
-         1678         358 STORE_NAME              28 (in_week)
+         1683         358 STORE_NAME              28 (in_week)
          
-         1696         360 LOAD_NAME                8 (classmethod)
+         1701         360 LOAD_NAME                8 (classmethod)
          
-         1697         362 LOAD_CONST              18 (<code object get_ex_dates, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1696>)
+         1702         362 LOAD_CONST              18 (<code object get_ex_dates, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1701>)
                       364 MAKE_FUNCTION            0
          
-         1696         366 PRECALL                  0
+         1701         366 PRECALL                  0
                       370 CALL                     0
          
-         1697         380 STORE_NAME              29 (get_ex_dates)
+         1702         380 STORE_NAME              29 (get_ex_dates)
          
-         1711         382 LOAD_CONST               8 ('return')
+         1716         382 LOAD_CONST               8 ('return')
                       384 LOAD_NAME               10 (str)
                       386 BUILD_TUPLE              2
-                      388 LOAD_CONST              19 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1711>)
+                      388 LOAD_CONST              19 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1716>)
                       390 MAKE_FUNCTION            4 (annotations)
                       392 STORE_NAME              30 (__str__)
          
-         1714         394 PUSH_NULL
+         1719         394 PUSH_NULL
                       396 LOAD_BUILD_CLASS
-                      398 LOAD_CONST              20 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1714>)
+                      398 LOAD_CONST              20 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1719>)
                       400 MAKE_FUNCTION            0
                       402 LOAD_CONST              21 ('Meta')
                       404 PRECALL                  2
                       408 CALL                     2
                       418 STORE_NAME              31 (Meta)
                       420 LOAD_CONST               5 (None)
                       422 RETURN_VALUE
@@ -13218,76 +13233,76 @@
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007c016a0000000000000000005300
-               1653           0 RESUME                   0
+               1658           0 RESUME                   0
                
-               1655           2 LOAD_FAST                1 (reference_object)
+               1660           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (holiday_name)
                              14 RETURN_VALUE
                consts
                   None
                names      ('holiday_name',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_title'
-               firstlineno 1653
+               firstlineno 1658
                lnotab 0x0202
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064015300
-               1657           0 RESUME                   0
+               1662           0 RESUME                   0
                
-               1661           2 LOAD_CONST               1 ('')
+               1666           2 LOAD_CONST               1 ('')
                               4 RETURN_VALUE
                consts
                   None
                   ''
                names      ()
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_description'
-               firstlineno 1657
+               firstlineno 1662
                lnotab 0x0204
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000064
                   01190000000000000000005300
-               1663           0 RESUME                   0
+               1668           0 RESUME                   0
                
-               1665           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+               1670           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 LOAD_CONST               1 ('calendar__holiday_color')
                              30 BINARY_SUBSCR
                              40 RETURN_VALUE
                consts
                   None
                   'calendar__holiday_color'
                names      ('get_site_preferences',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_color'
-               firstlineno 1663
+               firstlineno 1668
                lnotab 0x0202
             'Name'
             255
             ('verbose_name', 'max_length')
             code
                argcount  : 1
                nlocals   : 3
@@ -13295,63 +13310,63 @@
                flags     : 35
                code
                   0x4b00010097007c006a0000000000000000007c006a0100000000000000
                   007a0a00007d017405000000000000000000007c016a0300000000000000
                   0064017a000000a6010000ab01000000000000000044005d1c7d027c006a
                   0100000000000000007409000000000000000000007c02ac02a6010000ab
                   0100000000000000007a0000005600970101008c1d64035300
-               1671           0 RETURN_GENERATOR
+               1676           0 RETURN_GENERATOR
                               2 POP_TOP
                               4 RESUME                   0
                
-               1673           6 LOAD_FAST                0 (self)
+               1678           6 LOAD_FAST                0 (self)
                               8 LOAD_ATTR                0 (date_end)
                              18 LOAD_FAST                0 (self)
                              20 LOAD_ATTR                1 (date_start)
                              30 BINARY_OP               10 (-)
                              34 STORE_FAST               1 (delta)
                
-               1674          36 LOAD_GLOBAL              5 (NULL + range)
+               1679          36 LOAD_GLOBAL              5 (NULL + range)
                              48 LOAD_FAST                1 (delta)
                              50 LOAD_ATTR                3 (days)
                              60 LOAD_CONST               1 (1)
                              62 BINARY_OP                0 (+)
                              66 PRECALL                  1
                              70 CALL                     1
                              80 GET_ITER
                         >>   82 FOR_ITER                28 (to 140)
                              84 STORE_FAST               2 (i)
                
-               1675          86 LOAD_FAST                0 (self)
+               1680          86 LOAD_FAST                0 (self)
                              88 LOAD_ATTR                1 (date_start)
                              98 LOAD_GLOBAL              9 (NULL + timedelta)
                             110 LOAD_FAST                2 (i)
                             112 KW_NAMES                 2
                             114 PRECALL                  1
                             118 CALL                     1
                             128 BINARY_OP                0 (+)
                             132 YIELD_VALUE
                             134 RESUME                   1
                             136 POP_TOP
                             138 JUMP_BACKWARD           29 (to 82)
                
-               1674     >>  140 LOAD_CONST               3 (None)
+               1679     >>  140 LOAD_CONST               3 (None)
                             142 RETURN_VALUE
                consts
                   'Get all days included in the holiday.'
                   1
                   ('days',)
                   None
                names      ('date_end', 'date_start', 'range', 'days', 'timedelta')
                varnames   ('self', 'delta', 'i')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_days'
-               firstlineno 1671
+               firstlineno 1676
                lnotab 0x06021e01320136ff
             'week'
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 7
                flags     : 3
@@ -13362,71 +13377,71 @@
                   00ab02000000000000000044005d377d047c017c04190000000000000000
                   008a06740900000000000000000000740b00000000000000000000880666
                   01640384087c03a6020000ab020000000000000000a6010000ab01000000
                   00000000007d057c05720b7c056401190000000000000000007c027c043c
                   0000008c387c025300
                               0 MAKE_CELL                6 (holiday_date)
                
-               1677           2 RESUME                   0
+               1682           2 RESUME                   0
                
-               1680           4 BUILD_MAP                0
+               1685           4 BUILD_MAP                0
                               6 STORE_FAST               2 (per_weekday)
                
-               1681           8 LOAD_GLOBAL              0 (Holiday)
+               1686           8 LOAD_GLOBAL              0 (Holiday)
                              20 LOAD_ATTR                1 (objects)
                              30 LOAD_METHOD              2 (in_week)
                              52 LOAD_FAST                1 (week)
                              54 PRECALL                  1
                              58 CALL                     1
                              68 STORE_FAST               3 (holidays)
                
-               1683          70 LOAD_GLOBAL              7 (NULL + range)
+               1688          70 LOAD_GLOBAL              7 (NULL + range)
                              82 LOAD_CONST               1 (0)
                              84 LOAD_CONST               2 (7)
                              86 PRECALL                  2
                              90 CALL                     2
                             100 GET_ITER
                         >>  102 FOR_ITER                55 (to 214)
                             104 STORE_FAST               4 (weekday)
                
-               1684         106 LOAD_FAST                1 (week)
+               1689         106 LOAD_FAST                1 (week)
                             108 LOAD_FAST                4 (weekday)
                             110 BINARY_SUBSCR
                             120 STORE_DEREF              6 (holiday_date)
                
-               1685         122 LOAD_GLOBAL              9 (NULL + list)
+               1690         122 LOAD_GLOBAL              9 (NULL + list)
                
-               1686         134 LOAD_GLOBAL             11 (NULL + filter)
+               1691         134 LOAD_GLOBAL             11 (NULL + filter)
                
-               1687         146 LOAD_CLOSURE             6 (holiday_date)
+               1692         146 LOAD_CLOSURE             6 (holiday_date)
                             148 BUILD_TUPLE              1
-                            150 LOAD_CONST               3 (<code object <lambda>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1687>)
+                            150 LOAD_CONST               3 (<code object <lambda>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1692>)
                             152 MAKE_FUNCTION            8 (closure)
                
-               1688         154 LOAD_FAST                3 (holidays)
+               1693         154 LOAD_FAST                3 (holidays)
                
-               1686         156 PRECALL                  2
+               1691         156 PRECALL                  2
                             160 CALL                     2
                
-               1685         170 PRECALL                  1
+               1690         170 PRECALL                  1
                             174 CALL                     1
                             184 STORE_FAST               5 (filtered_holidays)
                
-               1691         186 LOAD_FAST                5 (filtered_holidays)
+               1696         186 LOAD_FAST                5 (filtered_holidays)
                             188 POP_JUMP_FORWARD_IF_FALSE    11 (to 212)
                
-               1692         190 LOAD_FAST                5 (filtered_holidays)
+               1697         190 LOAD_FAST                5 (filtered_holidays)
                             192 LOAD_CONST               1 (0)
                             194 BINARY_SUBSCR
                             204 LOAD_FAST                2 (per_weekday)
                             206 LOAD_FAST                4 (weekday)
                             208 STORE_SUBSCR
                         >>  212 JUMP_BACKWARD           56 (to 102)
                
-               1694     >>  214 LOAD_FAST                2 (per_weekday)
+               1699     >>  214 LOAD_FAST                2 (per_weekday)
                             216 RETURN_VALUE
                consts
                   'Get the holidays that are active in a given week.'
                   0
                   7
                   code
                      argcount  : 1
@@ -13434,15 +13449,15 @@
                      stacksize : 2
                      flags     : 19
                      code
                         0x9501970089017c006a0000000000000000006b05000000006f0a89017c
                         006a0100000000000000006b01000000005300
                                     0 COPY_FREE_VARS           1
                      
-                     1687           2 RESUME                   0
+                     1692           2 RESUME                   0
                                     4 LOAD_DEREF               1 (holiday_date)
                                     6 LOAD_FAST                0 (h)
                                     8 LOAD_ATTR                0 (date_start)
                                    18 COMPARE_OP               5 (>=)
                                    24 JUMP_IF_FALSE_OR_POP    10 (to 46)
                                    26 LOAD_DEREF               1 (holiday_date)
                                    28 LOAD_FAST                0 (h)
@@ -13453,23 +13468,23 @@
                         None
                      names      ('date_start', 'date_end')
                      varnames   ('h',)
                      freevars   ('holiday_date',)
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<lambda>'
-                     firstlineno 1687
+                     firstlineno 1692
                      lnotab 0x
                names      ('Holiday', 'objects', 'in_week', 'range', 'list', 'filter')
                varnames   ('cls', 'week', 'per_weekday', 'holidays', 'weekday', 'filtered_holidays')
                freevars   ()
                cellvars   ('holiday_date',)
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'in_week'
-               firstlineno 1677
+               firstlineno 1682
                lnotab 0x040304013e02240110010c010c01080102fe0eff100604011802
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
@@ -13480,95 +13495,95 @@
                   000000000000000000000000000000000000007c017c02ac02a6020000ab
                   0200000000000000004400a6000000ab0000000000000000008a05880566
                   01640384087c03a0060000000000000000000000000000000000000000a6
                   000000ab0000000000000000004400a6000000ab0000000000000000007d
                   047c045300
                               0 MAKE_CELL                5 (holiday_dates)
                
-               1696           2 RESUME                   0
+               1701           2 RESUME                   0
                
-               1699           4 LOAD_FAST                3 (recurrence)
+               1704           4 LOAD_FAST                3 (recurrence)
                               6 LOAD_ATTR                0 (dtstart)
                              16 LOAD_METHOD              1 (astimezone)
                              38 LOAD_GLOBAL              5 (NULL + timezone)
                              50 LOAD_ATTR                3 (get_current_timezone)
                              60 PRECALL                  0
                              64 CALL                     0
                              74 PRECALL                  1
                              78 CALL                     1
                              88 LOAD_FAST                3 (recurrence)
                              90 STORE_ATTR               0 (dtstart)
                
-               1700         100 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1700>)
+               1705         100 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1705>)
                             102 MAKE_FUNCTION            0
                
-               1702         104 LOAD_GLOBAL              8 (Holiday)
+               1707         104 LOAD_GLOBAL              8 (Holiday)
                             116 LOAD_METHOD              5 (get_single_events)
                             138 LOAD_FAST                1 (datetime_start)
                             140 LOAD_FAST                2 (datetime_end)
                             142 KW_NAMES                 2
                             144 PRECALL                  2
                             148 CALL                     2
                
-               1700         158 GET_ITER
+               1705         158 GET_ITER
                             160 PRECALL                  0
                             164 CALL                     0
                             174 STORE_DEREF              5 (holiday_dates)
                
-               1704         176 LOAD_CLOSURE             5 (holiday_dates)
+               1709         176 LOAD_CLOSURE             5 (holiday_dates)
                             178 BUILD_TUPLE              1
-                            180 LOAD_CONST               3 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1704>)
+                            180 LOAD_CONST               3 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1709>)
                             182 MAKE_FUNCTION            8 (closure)
                
-               1706         184 LOAD_FAST                3 (recurrence)
+               1711         184 LOAD_FAST                3 (recurrence)
                             186 LOAD_METHOD              6 (occurrences)
                             208 PRECALL                  0
                             212 CALL                     0
                
-               1704         222 GET_ITER
+               1709         222 GET_ITER
                             224 PRECALL                  0
                             228 CALL                     0
                             238 STORE_FAST               4 (exdates)
                
-               1709         240 LOAD_FAST                4 (exdates)
+               1714         240 LOAD_FAST                4 (exdates)
                             242 RETURN_VALUE
                consts
                   'Get the dates to exclude for holidays.'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0f7d017c016400190000000000000000006a00000000
                         000000000091028c105300
-                     1700           0 RESUME                   0
+                     1705           0 RESUME                   0
                                     2 BUILD_LIST               0
                                     4 LOAD_FAST                0 (.0)
                               >>    6 FOR_ITER                15 (to 38)
                      
-                     1702           8 STORE_FAST               1 (h)
+                     1707           8 STORE_FAST               1 (h)
                      
-                     1701          10 LOAD_FAST                1 (h)
+                     1706          10 LOAD_FAST                1 (h)
                                    12 LOAD_CONST               0 ('DTSTART')
                                    14 BINARY_SUBSCR
                                    24 LOAD_ATTR                0 (dt)
                      
-                     1700          34 LIST_APPEND              2
+                     1705          34 LIST_APPEND              2
                                    36 JUMP_BACKWARD           16 (to 6)
                               >>   38 RETURN_VALUE
                      consts
                         'DTSTART'
                      names      ('dt',)
                      varnames   ('.0', 'h')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 1700
+                     firstlineno 1705
                      lnotab 0x080202ff18ff
                   ('start', 'end')
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
@@ -13576,107 +13591,107 @@
                         0x9501970067007c005d377d017c01a00000000000000000000000000000
                         00000000000000a6000000ab00000000000000000089027600af187c01a0
                         010000000000000000000000000000000000000000740400000000000000
                         0000006a030000000000000000a6010000ab01000000000000000091028c
                         385300
                                     0 COPY_FREE_VARS           1
                      
-                     1704           2 RESUME                   0
+                     1709           2 RESUME                   0
                                     4 BUILD_LIST               0
                                     6 LOAD_FAST                0 (.0)
                               >>    8 FOR_ITER                55 (to 120)
                      
-                     1706          10 STORE_FAST               1 (h)
+                     1711          10 STORE_FAST               1 (h)
                      
-                     1707          12 LOAD_FAST                1 (h)
+                     1712          12 LOAD_FAST                1 (h)
                                    14 LOAD_METHOD              0 (date)
                                    36 PRECALL                  0
                                    40 CALL                     0
                                    50 LOAD_DEREF               2 (holiday_dates)
                                    52 CONTAINS_OP              0
                                    54 POP_JUMP_BACKWARD_IF_FALSE    24 (to 8)
                      
-                     1705          56 LOAD_FAST                1 (h)
+                     1710          56 LOAD_FAST                1 (h)
                                    58 LOAD_METHOD              1 (astimezone)
                                    80 LOAD_GLOBAL              4 (timezone)
                                    92 LOAD_ATTR                3 (utc)
                                   102 PRECALL                  1
                                   106 CALL                     1
                      
-                     1707         116 LIST_APPEND              2
+                     1712         116 LIST_APPEND              2
                                   118 JUMP_BACKWARD           56 (to 8)
                               >>  120 RETURN_VALUE
                      consts
                      names      ('date', 'astimezone', 'timezone', 'utc')
                      varnames   ('.0', 'h')
                      freevars   ('holiday_dates',)
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 1704
+                     firstlineno 1709
                      lnotab 0x0a0202012cfe3c02
                names      ('dtstart', 'astimezone', 'timezone', 'get_current_timezone', 'Holiday', 'get_single_events', 'occurrences')
                varnames   ('cls', 'datetime_start', 'datetime_end', 'recurrence', 'exdates')
                freevars   ()
                cellvars   ('holiday_dates',)
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_ex_dates'
-               firstlineno 1696
+               firstlineno 1701
                lnotab 0x04036001040236fe1204080226fe1205
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               1711           0 RESUME                   0
+               1716           0 RESUME                   0
                
-               1712           2 LOAD_FAST                0 (self)
+               1717           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (holiday_name)
                              14 RETURN_VALUE
                consts
                   None
                names      ('holiday_name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1711
+               firstlineno 1716
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 4
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a056403020065
                   036404a6010000ab010000000000000000660267015a0664055300
-               1714           0 RESUME                   0
+               1719           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('Holiday.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1715          10 PUSH_NULL
+               1720          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('Holiday')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1716          32 PUSH_NULL
+               1721          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('Holidays')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                
-               1717          54 LOAD_CONST               3 ('view_holiday_calendar')
+               1722          54 LOAD_CONST               3 ('view_holiday_calendar')
                              56 PUSH_NULL
                              58 LOAD_NAME                3 (_)
                              60 LOAD_CONST               4 ('Can view holiday calendar')
                              62 PRECALL                  1
                              66 CALL                     1
                              76 BUILD_TUPLE              2
                              78 BUILD_LIST               1
@@ -13692,25 +13707,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural', 'permissions')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1714
+               firstlineno 1719
                lnotab 0x0a0116011601
             'Meta'
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'name', '_', 'verbose_name', 'permission_required', 'classmethod', 'HttpRequest', 'str', 'value_title', 'value_description', 'get_color', 'PolymorphicBaseManager', 'from_queryset', 'HolidayQuerySet', 'objects', 'models', 'CharField', 'holiday_name', 'Iterator', 'date', 'get_days', 'CalendarWeek', 'dict', 'int', 'Optional', 'in_week', 'get_ex_dates', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'Holiday'
-         firstlineno 1646
+         firstlineno 1651
          lnotab
             0x0a01040204011601040202011aff0e010203020202ff040102ff020108
             ff020202fe06ff0e010205020116ff0e01020330023602180602012aff0e
             010212020104ff0e01020e0c03
       'Holiday'
       code
          argcount  : 0
@@ -13739,286 +13754,286 @@
             107a0700006412651b6516651c6602190000000000000000006606641884
             05a6000000ab0000000000000000005a1d65140900641c6411651564107a
             0700006419651b6516651c66021900000000000000000064107a07000064
             12651e660688006601641a840da6000000ab0000000000000000005a1f88
             0078015a205300
                         0 MAKE_CELL                0 (__class__)
          
-         1720           2 RESUME                   0
+         1725           2 RESUME                   0
                         4 LOAD_NAME                0 (__name__)
                         6 STORE_NAME               1 (__module__)
                         8 LOAD_CONST               0 ('PersonalEvent')
                        10 STORE_NAME               2 (__qualname__)
          
-         1721          12 LOAD_CONST               1 ('personal')
+         1726          12 LOAD_CONST               1 ('personal')
                        14 STORE_NAME               3 (name)
          
-         1722          16 PUSH_NULL
+         1727          16 PUSH_NULL
                        18 LOAD_NAME                4 (_)
                        20 LOAD_CONST               2 ('Personal events')
                        22 PRECALL                  1
                        26 CALL                     1
                        36 STORE_NAME               5 (verbose_name)
          
-         1724          38 PUSH_NULL
+         1729          38 PUSH_NULL
                        40 LOAD_NAME                6 (models)
                        42 LOAD_ATTR                7 (CharField)
                        52 LOAD_CONST               3 (255)
                        54 PUSH_NULL
                        56 LOAD_NAME                4 (_)
                        58 LOAD_CONST               4 ('Title')
                        60 PRECALL                  1
                        64 CALL                     1
                        74 KW_NAMES                 5
                        76 PRECALL                  2
                        80 CALL                     2
                        90 STORE_NAME               8 (title)
          
-         1725          92 PUSH_NULL
+         1730          92 PUSH_NULL
                        94 LOAD_NAME                6 (models)
                        96 LOAD_ATTR                9 (TextField)
                       106 PUSH_NULL
                       108 LOAD_NAME                4 (_)
                       110 LOAD_CONST               6 ('Description')
                       112 PRECALL                  1
                       116 CALL                     1
                       126 LOAD_CONST               7 (True)
                       128 KW_NAMES                 8
                       130 PRECALL                  2
                       134 CALL                     2
                       144 STORE_NAME              10 (description)
          
-         1726         146 PUSH_NULL
+         1731         146 PUSH_NULL
                       148 LOAD_NAME                6 (models)
                       150 LOAD_ATTR                7 (CharField)
                       160 LOAD_CONST               3 (255)
                       162 PUSH_NULL
                       164 LOAD_NAME                4 (_)
                       166 LOAD_CONST               9 ('Location')
                       168 PRECALL                  1
                       172 CALL                     1
                       182 LOAD_CONST               7 (True)
                       184 KW_NAMES                10
                       186 PRECALL                  3
                       190 CALL                     3
                       200 STORE_NAME              11 (location)
          
-         1728         202 PUSH_NULL
+         1733         202 PUSH_NULL
                       204 LOAD_NAME                6 (models)
                       206 LOAD_ATTR               12 (ForeignKey)
          
-         1729         216 LOAD_NAME               13 (Person)
+         1734         216 LOAD_NAME               13 (Person)
          
-         1730         218 LOAD_CONST              11 ('owned_events')
+         1735         218 LOAD_CONST              11 ('owned_events')
          
-         1731         220 LOAD_NAME                6 (models)
+         1736         220 LOAD_NAME                6 (models)
                       222 LOAD_ATTR               14 (CASCADE)
          
-         1732         232 PUSH_NULL
+         1737         232 PUSH_NULL
                       234 LOAD_NAME                4 (_)
                       236 LOAD_CONST              12 ('Owner')
                       238 PRECALL                  1
                       242 CALL                     1
          
-         1728         252 KW_NAMES                13
+         1733         252 KW_NAMES                13
                       254 PRECALL                  4
                       258 CALL                     4
                       268 STORE_NAME              15 (owner)
          
-         1734         270 PUSH_NULL
+         1739         270 PUSH_NULL
                       272 LOAD_NAME                6 (models)
                       274 LOAD_ATTR               16 (ManyToManyField)
                       284 LOAD_NAME               13 (Person)
                       286 LOAD_CONST              14 ('+')
                       288 LOAD_CONST               7 (True)
                       290 KW_NAMES                15
                       292 PRECALL                  3
                       296 CALL                     3
                       306 STORE_NAME              17 (persons)
          
-         1735         308 PUSH_NULL
+         1740         308 PUSH_NULL
                       310 LOAD_NAME                6 (models)
                       312 LOAD_ATTR               16 (ManyToManyField)
                       322 LOAD_NAME               18 (Group)
                       324 LOAD_CONST              14 ('+')
                       326 LOAD_CONST               7 (True)
                       328 KW_NAMES                15
                       330 PRECALL                  3
                       334 CALL                     3
                       344 STORE_NAME              19 (groups)
          
-         1737         346 LOAD_NAME               20 (classmethod)
+         1742         346 LOAD_NAME               20 (classmethod)
          
-         1738         348 LOAD_CONST              27 ((None,))
+         1743         348 LOAD_CONST              27 ((None,))
                       350 LOAD_CONST              17 ('request')
                       352 LOAD_NAME               21 (HttpRequest)
                       354 LOAD_CONST              16 (None)
                       356 BINARY_OP                7 (|)
                       360 LOAD_CONST              18 ('return')
                       362 LOAD_NAME               22 (str)
                       364 BUILD_TUPLE              4
-                      366 LOAD_CONST              19 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1737>)
+                      366 LOAD_CONST              19 (<code object get_color, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1742>)
                       368 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1737         370 PRECALL                  0
+         1742         370 PRECALL                  0
                       374 CALL                     0
          
-         1738         384 STORE_NAME              23 (get_color)
+         1743         384 STORE_NAME              23 (get_color)
          
-         1741         386 LOAD_NAME               20 (classmethod)
+         1746         386 LOAD_NAME               20 (classmethod)
          
-         1743         388 NOP
+         1748         388 NOP
          
-         1742         390 LOAD_CONST              27 ((None,))
+         1747         390 LOAD_CONST              27 ((None,))
                       392 LOAD_CONST              20 ('reference_object')
          
-         1743         394 LOAD_CONST               0 ('PersonalEvent')
+         1748         394 LOAD_CONST               0 ('PersonalEvent')
          
-         1742         396 LOAD_CONST              17 ('request')
+         1747         396 LOAD_CONST              17 ('request')
          
-         1743         398 LOAD_NAME               21 (HttpRequest)
+         1748         398 LOAD_NAME               21 (HttpRequest)
                       400 LOAD_CONST              16 (None)
                       402 BINARY_OP                7 (|)
          
-         1742         406 LOAD_CONST              18 ('return')
+         1747         406 LOAD_CONST              18 ('return')
          
-         1744         408 LOAD_NAME               22 (str)
+         1749         408 LOAD_NAME               22 (str)
          
-         1742         410 BUILD_TUPLE              6
-                      412 LOAD_CONST              21 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1741>)
+         1747         410 BUILD_TUPLE              6
+                      412 LOAD_CONST              21 (<code object value_title, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1746>)
                       414 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1741         416 PRECALL                  0
+         1746         416 PRECALL                  0
                       420 CALL                     0
          
-         1742         430 STORE_NAME              24 (value_title)
+         1747         430 STORE_NAME              24 (value_title)
          
-         1748         432 LOAD_NAME               20 (classmethod)
+         1753         432 LOAD_NAME               20 (classmethod)
          
-         1750         434 NOP
+         1755         434 NOP
          
-         1749         436 LOAD_CONST              27 ((None,))
+         1754         436 LOAD_CONST              27 ((None,))
                       438 LOAD_CONST              20 ('reference_object')
          
-         1750         440 LOAD_CONST               0 ('PersonalEvent')
+         1755         440 LOAD_CONST               0 ('PersonalEvent')
          
-         1749         442 LOAD_CONST              17 ('request')
+         1754         442 LOAD_CONST              17 ('request')
          
-         1750         444 LOAD_NAME               21 (HttpRequest)
+         1755         444 LOAD_NAME               21 (HttpRequest)
                       446 LOAD_CONST              16 (None)
                       448 BINARY_OP                7 (|)
          
-         1749         452 LOAD_CONST              18 ('return')
+         1754         452 LOAD_CONST              18 ('return')
          
-         1751         454 LOAD_NAME               22 (str)
+         1756         454 LOAD_NAME               22 (str)
          
-         1749         456 BUILD_TUPLE              6
-                      458 LOAD_CONST              22 (<code object value_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1748>)
+         1754         456 BUILD_TUPLE              6
+                      458 LOAD_CONST              22 (<code object value_description, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1753>)
                       460 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1748         462 PRECALL                  0
+         1753         462 PRECALL                  0
                       466 CALL                     0
          
-         1749         476 STORE_NAME              25 (value_description)
+         1754         476 STORE_NAME              25 (value_description)
          
-         1755         478 LOAD_NAME               20 (classmethod)
+         1760         478 LOAD_NAME               20 (classmethod)
          
-         1757         480 NOP
+         1762         480 NOP
          
-         1756         482 LOAD_CONST              27 ((None,))
+         1761         482 LOAD_CONST              27 ((None,))
                       484 LOAD_CONST              20 ('reference_object')
          
-         1757         486 LOAD_CONST               0 ('PersonalEvent')
+         1762         486 LOAD_CONST               0 ('PersonalEvent')
          
-         1756         488 LOAD_CONST              17 ('request')
+         1761         488 LOAD_CONST              17 ('request')
          
-         1757         490 LOAD_NAME               21 (HttpRequest)
+         1762         490 LOAD_NAME               21 (HttpRequest)
                       492 LOAD_CONST              16 (None)
                       494 BINARY_OP                7 (|)
          
-         1756         498 LOAD_CONST              18 ('return')
+         1761         498 LOAD_CONST              18 ('return')
          
-         1758         500 LOAD_NAME               22 (str)
+         1763         500 LOAD_NAME               22 (str)
          
-         1756         502 BUILD_TUPLE              6
-                      504 LOAD_CONST              23 (<code object value_location, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1755>)
+         1761         502 BUILD_TUPLE              6
+                      504 LOAD_CONST              23 (<code object value_location, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1760>)
                       506 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1755         508 PRECALL                  0
+         1760         508 PRECALL                  0
                       512 CALL                     0
          
-         1756         522 STORE_NAME              26 (value_location)
+         1761         522 STORE_NAME              26 (value_location)
          
-         1762         524 LOAD_NAME               20 (classmethod)
+         1767         524 LOAD_NAME               20 (classmethod)
          
-         1764         526 NOP
+         1769         526 NOP
          
-         1763         528 LOAD_CONST              27 ((None,))
+         1768         528 LOAD_CONST              27 ((None,))
                       530 LOAD_CONST              20 ('reference_object')
          
-         1764         532 LOAD_CONST               0 ('PersonalEvent')
+         1769         532 LOAD_CONST               0 ('PersonalEvent')
          
-         1763         534 LOAD_CONST              17 ('request')
+         1768         534 LOAD_CONST              17 ('request')
          
-         1764         536 LOAD_NAME               21 (HttpRequest)
+         1769         536 LOAD_NAME               21 (HttpRequest)
                       538 LOAD_CONST              16 (None)
                       540 BINARY_OP                7 (|)
          
-         1763         544 LOAD_CONST              18 ('return')
+         1768         544 LOAD_CONST              18 ('return')
          
-         1765         546 LOAD_NAME               27 (dict)
+         1770         546 LOAD_NAME               27 (dict)
                       548 LOAD_NAME               22 (str)
                       550 LOAD_NAME               28 (any)
                       552 BUILD_TUPLE              2
                       554 BINARY_SUBSCR
          
-         1763         564 BUILD_TUPLE              6
-                      566 LOAD_CONST              24 (<code object value_meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1762>)
+         1768         564 BUILD_TUPLE              6
+                      566 LOAD_CONST              24 (<code object value_meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1767>)
                       568 MAKE_FUNCTION            5 (defaults, annotations)
          
-         1762         570 PRECALL                  0
+         1767         570 PRECALL                  0
                       574 CALL                     0
          
-         1763         584 STORE_NAME              29 (value_meta)
+         1768         584 STORE_NAME              29 (value_meta)
          
-         1793         586 LOAD_NAME               20 (classmethod)
+         1798         586 LOAD_NAME               20 (classmethod)
          
-         1795         588 NOP
+         1800         588 NOP
          
-         1794         590 LOAD_CONST              28 ((None, None))
+         1799         590 LOAD_CONST              28 ((None, None))
                       592 LOAD_CONST              17 ('request')
          
-         1795         594 LOAD_NAME               21 (HttpRequest)
+         1800         594 LOAD_NAME               21 (HttpRequest)
                       596 LOAD_CONST              16 (None)
                       598 BINARY_OP                7 (|)
          
-         1794         602 LOAD_CONST              25 ('params')
+         1799         602 LOAD_CONST              25 ('params')
          
-         1795         604 LOAD_NAME               27 (dict)
+         1800         604 LOAD_NAME               27 (dict)
                       606 LOAD_NAME               22 (str)
                       608 LOAD_NAME               28 (any)
                       610 BUILD_TUPLE              2
                       612 BINARY_SUBSCR
                       622 LOAD_CONST              16 (None)
                       624 BINARY_OP                7 (|)
          
-         1794         628 LOAD_CONST              18 ('return')
+         1799         628 LOAD_CONST              18 ('return')
          
-         1796         630 LOAD_NAME               30 (QuerySet)
+         1801         630 LOAD_NAME               30 (QuerySet)
          
-         1794         632 BUILD_TUPLE              6
+         1799         632 BUILD_TUPLE              6
                       634 LOAD_CLOSURE             0 (__class__)
                       636 BUILD_TUPLE              1
-                      638 LOAD_CONST              26 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1793>)
+                      638 LOAD_CONST              26 (<code object get_objects, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1798>)
                       640 MAKE_FUNCTION           13 (defaults, annotations, closure)
          
-         1793         642 PRECALL                  0
+         1798         642 PRECALL                  0
                       646 CALL                     0
          
-         1794         656 STORE_NAME              31 (get_objects)
+         1799         656 STORE_NAME              31 (get_objects)
                       658 LOAD_CLOSURE             0 (__class__)
                       660 COPY                     1
                       662 STORE_NAME              32 (__classcell__)
                       664 RETURN_VALUE
          consts
             'PersonalEvent'
             'personal'
@@ -14043,96 +14058,96 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab00000000000000000064
                   01190000000000000000005300
-               1737           0 RESUME                   0
+               1742           0 RESUME                   0
                
-               1739           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+               1744           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
                              14 PRECALL                  0
                              18 CALL                     0
                              28 LOAD_CONST               1 ('calendar__personal_event_color')
                              30 BINARY_SUBSCR
                              40 RETURN_VALUE
                consts
                   None
                   'calendar__personal_event_color'
                names      ('get_site_preferences',)
                varnames   ('cls', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_color'
-               firstlineno 1737
+               firstlineno 1742
                lnotab 0x0202
             'reference_object'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007c016a0000000000000000005300
-               1741           0 RESUME                   0
+               1746           0 RESUME                   0
                
-               1746           2 LOAD_FAST                1 (reference_object)
+               1751           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (title)
                              14 RETURN_VALUE
                consts
                   'Return the title of the calendar event.'
                names      ('title',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_title'
-               firstlineno 1741
+               firstlineno 1746
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007c016a0000000000000000005300
-               1748           0 RESUME                   0
+               1753           0 RESUME                   0
                
-               1753           2 LOAD_FAST                1 (reference_object)
+               1758           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (description)
                              14 RETURN_VALUE
                consts
                   'Return the description of the calendar event.'
                names      ('description',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_description'
-               firstlineno 1748
+               firstlineno 1753
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007c016a0000000000000000005300
-               1755           0 RESUME                   0
+               1760           0 RESUME                   0
                
-               1760           2 LOAD_FAST                1 (reference_object)
+               1765           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (location)
                              14 RETURN_VALUE
                consts
                   'Return the location of the calendar event.'
                names      ('location',)
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_location'
-               firstlineno 1755
+               firstlineno 1760
                lnotab 0x0205
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 11
                flags     : 3
                code
@@ -14144,173 +14159,173 @@
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000004400a6000000ab0000000000000000007c016a0700000000000000
                   007411000000000000000000007c016a090000000000000000a6010000ab
                   0100000000000000007c026a0a0000000000000000a00b00000000000000
                   0000000000000000000000000064047c01a6020000ab0200000000000000
                   007c026a0a0000000000000000a00b000000000000000000000000000000
                   000000000064057c01a6020000ab02000000000000000064069c085300
-               1762           0 RESUME                   0
+               1767           0 RESUME                   0
                
-               1769           2 LOAD_FAST                1 (reference_object)
+               1774           2 LOAD_FAST                1 (reference_object)
                               4 LOAD_ATTR                0 (id)
                
-               1771          14 LOAD_FAST                1 (reference_object)
+               1776          14 LOAD_FAST                1 (reference_object)
                              16 LOAD_ATTR                1 (owner)
                              26 LOAD_ATTR                2 (pk)
                
-               1772          36 LOAD_FAST                1 (reference_object)
+               1777          36 LOAD_FAST                1 (reference_object)
                              38 LOAD_ATTR                1 (owner)
                              48 LOAD_ATTR                3 (full_name)
                
-               1770          58 LOAD_CONST               1 (('id', 'full_name'))
+               1775          58 LOAD_CONST               1 (('id', 'full_name'))
                              60 BUILD_CONST_KEY_MAP      2
                
-               1774          62 LOAD_CONST               2 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1774>)
+               1779          62 LOAD_CONST               2 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1779>)
                              64 MAKE_FUNCTION            0
                
-               1779          66 LOAD_FAST                1 (reference_object)
+               1784          66 LOAD_FAST                1 (reference_object)
                              68 LOAD_ATTR                4 (persons)
                              78 LOAD_METHOD              5 (all)
                             100 PRECALL                  0
                             104 CALL                     0
                
-               1774         114 GET_ITER
+               1779         114 GET_ITER
                             116 PRECALL                  0
                             120 CALL                     0
                
-               1781         130 LOAD_CONST               3 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1781>)
+               1786         130 LOAD_CONST               3 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1786>)
                             132 MAKE_FUNCTION            0
                
-               1783         134 LOAD_FAST                1 (reference_object)
+               1788         134 LOAD_FAST                1 (reference_object)
                             136 LOAD_ATTR                6 (groups)
                             146 LOAD_METHOD              5 (all)
                             168 PRECALL                  0
                             172 CALL                     0
                
-               1781         182 GET_ITER
+               1786         182 GET_ITER
                             184 PRECALL                  0
                             188 CALL                     0
                
-               1785         198 LOAD_FAST                1 (reference_object)
+               1790         198 LOAD_FAST                1 (reference_object)
                             200 LOAD_ATTR                7 (description)
                
-               1786         210 LOAD_GLOBAL             17 (NULL + str)
+               1791         210 LOAD_GLOBAL             17 (NULL + str)
                             222 LOAD_FAST                1 (reference_object)
                             224 LOAD_ATTR                9 (recurrences)
                             234 PRECALL                  1
                             238 CALL                     1
                
-               1787         248 LOAD_FAST                2 (request)
+               1792         248 LOAD_FAST                2 (request)
                             250 LOAD_ATTR               10 (user)
                             260 LOAD_METHOD             11 (has_perm)
                             282 LOAD_CONST               4 ('core.edit_personal_event_rule')
                             284 LOAD_FAST                1 (reference_object)
                             286 PRECALL                  2
                             290 CALL                     2
                
-               1788         300 LOAD_FAST                2 (request)
+               1793         300 LOAD_FAST                2 (request)
                             302 LOAD_ATTR               10 (user)
                             312 LOAD_METHOD             11 (has_perm)
                
-               1789         334 LOAD_CONST               5 ('core.delete_personal_event_rule')
+               1794         334 LOAD_CONST               5 ('core.delete_personal_event_rule')
                             336 LOAD_FAST                1 (reference_object)
                
-               1788         338 PRECALL                  2
+               1793         338 PRECALL                  2
                             342 CALL                     2
                
-               1768         352 LOAD_CONST               6 (('id', 'owner', 'persons', 'groups', 'description', 'recurrences', 'can_edit', 'can_delete'))
+               1773         352 LOAD_CONST               6 (('id', 'owner', 'persons', 'groups', 'description', 'recurrences', 'can_edit', 'can_delete'))
                             354 BUILD_CONST_KEY_MAP      8
                             356 RETURN_VALUE
                consts
                   'Get the meta of the event.'
                   ('id', 'full_name')
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d117d017c016a0000000000000000007c016a01000000
                         000000000064009c0291028c125300
-                     1774           0 RESUME                   0
+                     1779           0 RESUME                   0
                                     2 BUILD_LIST               0
                                     4 LOAD_FAST                0 (.0)
                               >>    6 FOR_ITER                17 (to 42)
                      
-                     1779           8 STORE_FAST               1 (p)
+                     1784           8 STORE_FAST               1 (p)
                      
-                     1776          10 LOAD_FAST                1 (p)
+                     1781          10 LOAD_FAST                1 (p)
                                    12 LOAD_ATTR                0 (pk)
                      
-                     1777          22 LOAD_FAST                1 (p)
+                     1782          22 LOAD_FAST                1 (p)
                                    24 LOAD_ATTR                1 (full_name)
                      
-                     1775          34 LOAD_CONST               0 (('id', 'full_name'))
+                     1780          34 LOAD_CONST               0 (('id', 'full_name'))
                                    36 BUILD_CONST_KEY_MAP      2
                      
-                     1774          38 LIST_APPEND              2
+                     1779          38 LIST_APPEND              2
                                    40 JUMP_BACKWARD           18 (to 6)
                               >>   42 RETURN_VALUE
                      consts
                         ('id', 'full_name')
                      names      ('pk', 'full_name')
                      varnames   ('.0', 'p')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 1774
+                     firstlineno 1779
                      lnotab 0x080502fd0c010cfe04ff
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x970067007c005d177d017c016a0000000000000000007c016a01000000
                         00000000007c016a02000000000000000064009c0391028c185300
-                     1781           0 RESUME                   0
+                     1786           0 RESUME                   0
                                     2 BUILD_LIST               0
                                     4 LOAD_FAST                0 (.0)
                               >>    6 FOR_ITER                23 (to 54)
                      
-                     1783           8 STORE_FAST               1 (g)
+                     1788           8 STORE_FAST               1 (g)
                      
-                     1782          10 LOAD_FAST                1 (g)
+                     1787          10 LOAD_FAST                1 (g)
                                    12 LOAD_ATTR                0 (pk)
                                    22 LOAD_FAST                1 (g)
                                    24 LOAD_ATTR                1 (name)
                                    34 LOAD_FAST                1 (g)
                                    36 LOAD_ATTR                2 (short_name)
                                    46 LOAD_CONST               0 (('id', 'name', 'short_name'))
                                    48 BUILD_CONST_KEY_MAP      3
                      
-                     1781          50 LIST_APPEND              2
+                     1786          50 LIST_APPEND              2
                                    52 JUMP_BACKWARD           24 (to 6)
                               >>   54 RETURN_VALUE
                      consts
                         ('id', 'name', 'short_name')
                      names      ('pk', 'name', 'short_name')
                      varnames   ('.0', 'g')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                      name       '<listcomp>'
-                     firstlineno 1781
+                     firstlineno 1786
                      lnotab 0x080202ff28ff
                   'core.edit_personal_event_rule'
                   'core.delete_personal_event_rule'
                   ('id', 'owner', 'persons', 'groups', 'description', 'recurrences', 'can_edit', 'can_delete')
                names      ('id', 'owner', 'pk', 'full_name', 'persons', 'all', 'groups', 'description', 'str', 'recurrences', 'user', 'has_perm')
                varnames   ('cls', 'reference_object', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'value_meta'
-               firstlineno 1762
+               firstlineno 1767
                lnotab
                   0x02070c02160116fe0404040530fb1007040230fe10040c012601340122
                   0104ff0eec
             'params'
             code
                argcount  : 3
                nlocals   : 4
@@ -14326,95 +14341,95 @@
                   00000000000000ac03a6010000ab0100000000000000007a070000740700
                   0000000000000000007c016a0400000000000000006a0500000000000000
                   00ac04a6010000ab0100000000000000007a070000a6010000ab01000000
                   0000000000a0060000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d037c035300
                               0 COPY_FREE_VARS           1
                
-               1793           2 RESUME                   0
+               1798           2 RESUME                   0
                
-               1797           4 LOAD_GLOBAL              1 (NULL + super)
+               1802           4 LOAD_GLOBAL              1 (NULL + super)
                              16 PRECALL                  0
                              20 CALL                     0
                              30 LOAD_METHOD              1 (get_objects)
                              52 LOAD_FAST                1 (request)
                              54 LOAD_FAST                2 (params)
                              56 KW_NAMES                 1
                              58 PRECALL                  2
                              62 CALL                     2
                              72 STORE_FAST               3 (qs)
                
-               1798          74 LOAD_FAST                1 (request)
+               1803          74 LOAD_FAST                1 (request)
                              76 POP_JUMP_FORWARD_IF_FALSE   117 (to 312)
                
-               1799          78 LOAD_FAST                3 (qs)
+               1804          78 LOAD_FAST                3 (qs)
                              80 LOAD_METHOD              2 (filter)
                
-               1800         102 LOAD_GLOBAL              7 (NULL + Q)
+               1805         102 LOAD_GLOBAL              7 (NULL + Q)
                             114 LOAD_FAST                1 (request)
                             116 LOAD_ATTR                4 (user)
                             126 LOAD_ATTR                5 (person)
                             136 KW_NAMES                 2
                             138 PRECALL                  1
                             142 CALL                     1
                
-               1801         152 LOAD_GLOBAL              7 (NULL + Q)
+               1806         152 LOAD_GLOBAL              7 (NULL + Q)
                             164 LOAD_FAST                1 (request)
                             166 LOAD_ATTR                4 (user)
                             176 LOAD_ATTR                5 (person)
                             186 KW_NAMES                 3
                             188 PRECALL                  1
                             192 CALL                     1
                
-               1800         202 BINARY_OP                7 (|)
+               1805         202 BINARY_OP                7 (|)
                
-               1802         206 LOAD_GLOBAL              7 (NULL + Q)
+               1807         206 LOAD_GLOBAL              7 (NULL + Q)
                             218 LOAD_FAST                1 (request)
                             220 LOAD_ATTR                4 (user)
                             230 LOAD_ATTR                5 (person)
                             240 KW_NAMES                 4
                             242 PRECALL                  1
                             246 CALL                     1
                
-               1800         256 BINARY_OP                7 (|)
+               1805         256 BINARY_OP                7 (|)
                
-               1799         260 PRECALL                  1
+               1804         260 PRECALL                  1
                             264 CALL                     1
                
-               1803         274 LOAD_METHOD              6 (distinct)
+               1808         274 LOAD_METHOD              6 (distinct)
                             296 PRECALL                  0
                             300 CALL                     0
                
-               1799         310 STORE_FAST               3 (qs)
+               1804         310 STORE_FAST               3 (qs)
                
-               1804     >>  312 LOAD_FAST                3 (qs)
+               1809     >>  312 LOAD_FAST                3 (qs)
                             314 RETURN_VALUE
                consts
                   None
                   ('request', 'params')
                   ('owner',)
                   ('persons',)
                   ('groups__members',)
                names      ('super', 'get_objects', 'filter', 'Q', 'user', 'person', 'distinct')
                varnames   ('cls', 'request', 'params', 'qs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'get_objects'
-               firstlineno 1793
+               firstlineno 1798
                lnotab 0x0404460104011801320132ff040232fe04ff0e0424fc0205
             (None,)
             (None, None)
          names      ('__name__', '__module__', '__qualname__', 'name', '_', 'verbose_name', 'models', 'CharField', 'title', 'TextField', 'description', 'location', 'ForeignKey', 'Person', 'CASCADE', 'owner', 'ManyToManyField', 'persons', 'Group', 'groups', 'classmethod', 'HttpRequest', 'str', 'get_color', 'value_title', 'value_description', 'value_location', 'dict', 'any', 'value_meta', 'QuerySet', 'get_objects', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'PersonalEvent'
-         firstlineno 1720
+         firstlineno 1725
          lnotab
             0x0c01040116023601360138020e01020102010c0114fc12062601260202
             0116ff0e010203020202ff040102ff020108ff020202fe06ff0e01020602
             0202ff040102ff020108ff020202fe06ff0e010206020202ff040102ff02
             0108ff020202fe06ff0e010206020202ff040102ff020108ff020212fe06
             ff0e01021e020202ff040108ff020118ff020202fe0aff0e01
       'PersonalEvent'
@@ -14428,76 +14443,76 @@
             01a6010000ab0100000000000000006402ac03a6020000ab020000000000
             0000005a06020065036a040000000000000000020065056404a6010000ab
             0100000000000000006402ac03a6020000ab0200000000000000005a0702
             0065036a080000000000000000650965036a0a0000000000000000020065
             056405a6010000ab010000000000000000ac06a6030000ab030000000000
             0000005a0b6407650c6602640884045a0d0200470064098400640aa60200
             00ab0200000000000000005a0e640b5300
-         1807           0 RESUME                   0
+         1812           0 RESUME                   0
                         2 LOAD_NAME                0 (__name__)
                         4 STORE_NAME               1 (__module__)
                         6 LOAD_CONST               0 ('Organisation')
                         8 STORE_NAME               2 (__qualname__)
          
-         1808          10 PUSH_NULL
+         1813          10 PUSH_NULL
                        12 LOAD_NAME                3 (models)
                        14 LOAD_ATTR                4 (CharField)
                        24 PUSH_NULL
                        26 LOAD_NAME                5 (_)
                        28 LOAD_CONST               1 ('Name')
                        30 PRECALL                  1
                        34 CALL                     1
                        44 LOAD_CONST               2 (255)
                        46 KW_NAMES                 3
                        48 PRECALL                  2
                        52 CALL                     2
                        62 STORE_NAME               6 (name)
          
-         1809          64 PUSH_NULL
+         1814          64 PUSH_NULL
                        66 LOAD_NAME                3 (models)
                        68 LOAD_ATTR                4 (CharField)
                        78 PUSH_NULL
                        80 LOAD_NAME                5 (_)
                        82 LOAD_CONST               4 ('Email')
                        84 PRECALL                  1
                        88 CALL                     1
                        98 LOAD_CONST               2 (255)
                       100 KW_NAMES                 3
                       102 PRECALL                  2
                       106 CALL                     2
                       116 STORE_NAME               7 (email)
          
-         1811         118 PUSH_NULL
+         1816         118 PUSH_NULL
                       120 LOAD_NAME                3 (models)
                       122 LOAD_ATTR                8 (ForeignKey)
          
-         1812         132 LOAD_NAME                9 (Group)
+         1817         132 LOAD_NAME                9 (Group)
                       134 LOAD_NAME                3 (models)
                       136 LOAD_ATTR               10 (CASCADE)
                       146 PUSH_NULL
                       148 LOAD_NAME                5 (_)
                       150 LOAD_CONST               5 ('Related group')
                       152 PRECALL                  1
                       156 CALL                     1
          
-         1811         166 KW_NAMES                 6
+         1816         166 KW_NAMES                 6
                       168 PRECALL                  3
                       172 CALL                     3
                       182 STORE_NAME              11 (related_group)
          
-         1815         184 LOAD_CONST               7 ('return')
+         1820         184 LOAD_CONST               7 ('return')
                       186 LOAD_NAME               12 (str)
                       188 BUILD_TUPLE              2
-                      190 LOAD_CONST               8 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1815>)
+                      190 LOAD_CONST               8 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1820>)
                       192 MAKE_FUNCTION            4 (annotations)
                       194 STORE_NAME              13 (__str__)
          
-         1818         196 PUSH_NULL
+         1823         196 PUSH_NULL
                       198 LOAD_BUILD_CLASS
-                      200 LOAD_CONST               9 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1818>)
+                      200 LOAD_CONST               9 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py", line 1823>)
                       202 MAKE_FUNCTION            0
                       204 LOAD_CONST              10 ('Meta')
                       206 PRECALL                  2
                       210 CALL                     2
                       220 STORE_NAME              14 (Meta)
                       222 LOAD_CONST              11 (None)
                       224 RETURN_VALUE
@@ -14512,52 +14527,52 @@
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000009b005300
-               1815           0 RESUME                   0
+               1820           0 RESUME                   0
                
-               1816           2 LOAD_FAST                0 (self)
+               1821           2 LOAD_FAST                0 (self)
                               4 LOAD_ATTR                0 (name)
                              14 FORMAT_VALUE             0
                              16 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       '__str__'
-               firstlineno 1815
+               firstlineno 1820
                lnotab 0x0201
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 3
                flags     : 0
                code
                   0x970065005a0164005a02020065036401a6010000ab0100000000000000
                   005a04020065036402a6010000ab0100000000000000005a0564035300
-               1818           0 RESUME                   0
+               1823           0 RESUME                   0
                               2 LOAD_NAME                0 (__name__)
                               4 STORE_NAME               1 (__module__)
                               6 LOAD_CONST               0 ('Organisation.Meta')
                               8 STORE_NAME               2 (__qualname__)
                
-               1819          10 PUSH_NULL
+               1824          10 PUSH_NULL
                              12 LOAD_NAME                3 (_)
                              14 LOAD_CONST               1 ('Organisation')
                              16 PRECALL                  1
                              20 CALL                     1
                              30 STORE_NAME               4 (verbose_name)
                
-               1820          32 PUSH_NULL
+               1825          32 PUSH_NULL
                              34 LOAD_NAME                3 (_)
                              36 LOAD_CONST               2 ('Organisations')
                              38 PRECALL                  1
                              42 CALL                     1
                              52 STORE_NAME               5 (verbose_name_plural)
                              54 LOAD_CONST               3 (None)
                              56 RETURN_VALUE
@@ -14568,25 +14583,25 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
                name       'Meta'
-               firstlineno 1818
+               firstlineno 1823
                lnotab 0x0a011601
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', '_', 'name', 'email', 'ForeignKey', 'Group', 'CASCADE', 'related_group', 'str', '__str__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
          name       'Organisation'
-         firstlineno 1807
+         firstlineno 1812
          lnotab 0x0a01360136020e0122ff12040c03
       'Organisation'
    names      ('base64', 'datetime', 'date', 'timedelta', 'typing', 'TYPE_CHECKING', 'Any', 'Iterable', 'Iterator', 'List', 'Optional', 'Sequence', 'Union', 'urllib.parse', 'urljoin', 'django.conf', 'settings', 'django.contrib.auth', 'get_user_model', 'django.contrib.auth.models', 'Group', 'DjangoGroup', 'django.contrib.contenttypes.fields', 'GenericForeignKey', 'django.contrib.contenttypes.models', 'ContentType', 'django.contrib.postgres.fields', 'ArrayField', 'django.core.exceptions', 'ValidationError', 'django.core.validators', 'MaxValueValidator', 'django.db', 'models', 'django.db.models', 'Q', 'QuerySet', 'django.dispatch', 'receiver', 'django.forms.widgets', 'Media', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.utils', 'timezone', 'django.utils.formats', 'date_format', 'django.utils.functional', 'classproperty', 'django.utils.translation', 'gettext_lazy', '_', 'customidenticon', 'cachalot.api', 'cachalot_disabled', 'cache_memoize', 'calendarweek', 'CalendarWeek', 'celery.result', 'AsyncResult', 'celery_progress.backend', 'Progress', 'ckeditor.fields', 'RichTextField', 'django_celery_results.models', 'TaskResult', 'django_ical.utils', 'build_rrule_from_recurrences_rrule', 'build_rrule_from_text', 'dynamic_preferences.models', 'PerInstancePreferenceModel', 'guardian.shortcuts', 'get_objects_for_user', 'icalendar', 'vCalAddress', 'vText', 'icalendar.prop', 'vRecur', 'invitations', 'signals', 'invitations.base_invitation', 'AbstractBaseInvitation', 'invitations.models', 'Invitation', 'model_utils', 'FieldTracker', 'model_utils.models', 'TimeStampedModel', 'oauth2_provider.models', 'AbstractAccessToken', 'AbstractApplication', 'AbstractGrant', 'AbstractIDToken', 'AbstractRefreshToken', 'phonenumber_field.modelfields', 'PhoneNumberField', 'polymorphic.models', 'PolymorphicModel', 'recurrence.fields', 'RecurrenceField', 'timezone_field', 'TimeZoneField', 'aleksis.core.data_checks', 'DataCheck', 'managers', 'AlekSISBaseManagerWithoutMigrations', 'GroupManager', 'GroupQuerySet', 'HolidayQuerySet', 'InstalledWidgetsDashboardWidgetOrderManager', 'PolymorphicBaseManager', 'SchoolTermQuerySet', 'UninstallRenitentPolymorphicManager', 'mixins', 'CalendarEventMixin', 'ExtensibleModel', 'ExtensiblePolymorphicModel', 'GlobalPermissionModel', 'PureDjangoModel', 'RegistryObject', 'SchoolTermRelatedExtensibleModel', 'tasks', 'send_notification', 'util.core_helpers', 'generate_random_code', 'get_site_preferences', 'now_tomorrow', 'util.email', 'send_email', 'util.model_helpers', 'ICONS', 'User', 'FIELD_CHOICES', 'SchoolTerm', 'Person', 'DummyPerson', 'PersonGroupThrough', 'm2m_changed', 'owners', 'through', 'Model', 'str', 'bool', 'set', 'save_group_on_m2m_changed', 'Activity', 'Notification', 'AnnouncementQuerySet', 'Announcement', 'AnnouncementRecipient', 'DashboardWidget', 'ExternalLinkWidget', 'StaticContentWidget', 'DashboardWidgetOrder', 'CustomMenu', 'CustomMenuItem', 'DynamicRoute', 'GroupType', 'GlobalPermissions', 'PersonPreferenceModel', 'GroupPreferenceModel', 'DataCheckResult', 'PersonInvitation', 'PDFFile', 'TaskUserAssignment', 'UserAdditionalAttributes', 'OAuthApplication', 'OAuthGrant', 'OAuthAccessToken', 'OAuthIDToken', 'OAuthRefreshToken', 'Room', 'CalendarEvent', 'FreeBusy', 'BirthdayEvent', 'Holiday', 'PersonalEvent', 'Organisation')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/models.py'
@@ -14594,11 +14609,11 @@
    firstlineno 1
    lnotab
       0x00ff02020801140128010c020c010c010c010c010c010c010c010c010c
       0110010c010c010c010c010c010c010c010c0208010c010c010c010c010c
       010c010c0110010c010c0110010c010c010c010c010c010c011c070c010c
       010c010c020c04280a24090c0114010c010c0204010c0318011801180118
       01180118011801180118011801180118f404101c371c7f007f00201c111c
-      7f00091c0b2c014001020126ff02020cfe020302fd020402fc02050cfb02
+      7f000e1c0b2c014001020126ff02020cfe020302fd020402fc02050cfb02
       060efa020802f806ff0eff0e0202211e141e2b26361c2e1c26204d1c0e1c
       0d1c1b1c171c181c081c151c121e091e091c231e331c201c51282b1c221c
       061c061c061c061c161e7f00321c041c381c4a1c57
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/preferences.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/preferences.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 15497
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/registries.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/registries.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 611
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/rules.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/rules.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 17713
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/settings.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/settings.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 39858
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 18
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/__pycache__/tasks.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/__pycache__/tasks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 2330
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/admin.py` & `aleksis_core-4.0.0.dev7/aleksis/core/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/apps.py` & `aleksis_core-4.0.0.dev7/aleksis/core/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/celery.py` & `aleksis_core-4.0.0.dev7/aleksis/core/celery.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/checks.py` & `aleksis_core-4.0.0.dev7/aleksis/core/checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/data_checks.py` & `aleksis_core-4.0.0.dev7/aleksis/core/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/decorators.py` & `aleksis_core-4.0.0.dev7/aleksis/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/filters.py` & `aleksis_core-4.0.0.dev7/aleksis/core/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/forms.py` & `aleksis_core-4.0.0.dev7/aleksis/core/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/apollo.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/apollo.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/dateTimeFormats.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/dateTimeFormats.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/app/vuetify.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/app/vuetify.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/LegacyBaseTemplate.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/LegacyBaseTemplate.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/AboutAleksis.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/AboutAleksis.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppCard.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/InstalledAppCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/about/InstalledAppsList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/about/InstalledAppsList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/AccountMenu.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/AccountMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/App.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/App.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/ErrorPage.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/ErrorPage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/LanguageForm.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/LanguageForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SideNav.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/SideNav.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SidenavSearch.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/SidenavSearch.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/SnackbarItem.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/SnackbarItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/app/Splash.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/app/Splash.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/Calendar.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/Calendar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarControlBar.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarControlBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarOverview.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarSelect.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/CalendarWithControls.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/CalendarWithControls.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/calendarMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/celery_progress/TaskListItem.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/celery_progress/TaskListItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ActionSelect.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/ActionSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/AvatarClickbox.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/AvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ButtonMenu.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/ButtonMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDBar.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CRUDBar.vue`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 <!-- It returns filtered items -->
 <!-- All child components can be toggled -->
 <!-- Search returns a string -->
 <!-- create/patch & del are fully exposed (via ref, see CRUDList) -->
 
 <template>
-  <v-toolbar flat class="height-fit child-height-fit">
+  <v-toolbar class="height-fit child-height-fit" :flat="flat">
     <v-row class="flex-wrap gap align-baseline pt-4">
       <v-toolbar-title class="d-flex flex-wrap w-100 gap">
         <!-- filter-selection -->
         <filter-bar
           v-if="enableFilter"
           v-model="additionalFilters"
           :disabled="loading || lock"
@@ -197,14 +197,22 @@
      * The i18nKey for this component.
      */
     i18nKey: {
       type: String,
       required: true,
     },
     /**
+     * Flat toolbar?
+     */
+    flat: {
+      type: Boolean,
+      required: false,
+      default: true,
+    },
+    /**
      * Lock updating the items
      * Deactivates changing the filter, search, the items themselves (create, edit, delete) and selecting actions.
      * This only prohibits the user from updating the items, props can still influence them.
      * @values true, false
      */
     lock: {
       type: Boolean,
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDIterator.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CRUDIterator.vue`

 * *Files 23% similar despite different names*

```diff
@@ -3,26 +3,32 @@
     v-bind="$attrs"
     v-on="$listeners"
     :items="items"
     :items-per-page="itemsPerPage"
     :loading="loading"
     :class="elevated ? 'elevation-2' : ''"
     :search="search"
+    :custom-filter="deepSearch"
     :sort-by.sync="sortBy"
     :sort-desc.sync="sortDesc"
     multi-sort
     @update:sort-by="handleSortChange"
     @update:sort-desc="handleSortChange"
     :show-select="showSelect"
     selectable-key="selectable"
     @toggle-select-all="handleToggleAll"
   >
     <!-- Bar template -->
     <template #header>
       <c-r-u-d-bar
+        :class="{
+          'c-r-u-d-iterator-fixed-header': fixedHeader,
+          'pa-3': fixedHeader,
+        }"
+        :flat="!fixedHeader"
         v-bind="$attrs"
         v-on="$listeners"
         @mode="$emit('mode', $event)"
         @loading="handleLoading"
         @items="handleItems"
         @lastQuery="$emit('lastQuery', $event)"
         @search="search = $event"
@@ -47,14 +53,18 @@
             :is-create="isCreate"
           />
         </template>
         <template #additionalActions="{ attrs, on }">
           <slot name="additionalActions" :attrs="attrs" :on="on" />
         </template>
       </c-r-u-d-bar>
+      <div
+        v-if="fixedHeader"
+        class="c-r-u-d-iterator-fixed-header-placeholder"
+      />
     </template>
 
     <template #default="slotProps">
       <slot name="default" v-bind="slotProps" />
     </template>
     <template #loading>
       <slot name="loading"></slot>
@@ -67,26 +77,36 @@
     </template>
   </v-data-iterator>
 </template>
 
 <script>
 import CRUDBar from "./CRUDBar.vue";
 
+import deepSearchMixin from "../../mixins/deepSearchMixin";
 import loadingMixin from "../../mixins/loadingMixin.js";
 import syncSortMixin from "../../mixins/syncSortMixin.js";
 
 // TODO: props, data & methods are a subset of CRUDList's -> share?
 
 export default {
   name: "CRUDIterator",
   components: {
     CRUDBar,
   },
-  mixins: [loadingMixin, syncSortMixin],
+  mixins: [deepSearchMixin, loadingMixin, syncSortMixin],
   props: {
+    // fixed-header behaves the same as in v-data-table where it is included by vuetify
+    /**
+     * Fix header to top
+     */
+    fixedHeader: {
+      type: Boolean,
+      required: false,
+      default: false,
+    },
     /**
      * Elevate the iterator?
      * @values true, false
      */
     elevated: {
       type: Boolean,
       required: false,
@@ -116,14 +136,23 @@
   },
   computed: {
     computedHeaders() {
       return "headers" in this.$attrs
         ? this.$attrs.headers.filter((header) => !header.disableEdit)
         : [];
     },
+    fixedHeaderTop() {
+      return `${this.$vuetify.application.top}px`;
+    },
+    fixedHeaderWidth() {
+      return `calc(100vw - ${this.$vuetify.application.left}px - ${this.$vuetify.application.right}px)`;
+    },
+    fixedHeaderLeft() {
+      return `${this.$vuetify.application.left}px`;
+    },
   },
   methods: {
     handleItems(items) {
       this.items = items;
       // Pass on; documented in queryMixin.
       this.$emit("items", items);
     },
@@ -145,7 +174,24 @@
     // Template names
     fieldSlot(header) {
       return header.value + ".field";
     },
   },
 };
 </script>
+
+<style lang="scss">
+.c-r-u-d-iterator-fixed-header {
+  position: fixed;
+  width: v-bind(fixedHeaderWidth);
+  left: v-bind(fixedHeaderLeft);
+  top: v-bind(fixedHeaderTop);
+  z-index: 3;
+}
+
+.c-r-u-d-iterator-fixed-header-placeholder {
+  height: v-bind(fixedHeaderTop);
+  position: sticky;
+  top: v-bind(fixedHeaderTop);
+  z-index: 2;
+}
+</style>
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CRUDList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CRUDList.vue`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
   <v-data-table
     :headers="tableHeaders"
     :items="items"
     :items-per-page="itemsPerPage"
     :loading="loading"
     :class="elevated ? 'elevation-2' : ''"
     :search="search"
+    :custom-filter="deepSearch"
     :sort-by.sync="sortBy"
     :sort-desc.sync="sortDesc"
     multi-sort
     @update:sort-by="handleSortChange"
     @update:sort-desc="handleSortChange"
     :show-select="showSelect"
     selectable-key="selectable"
@@ -111,25 +112,26 @@
 </template>
 
 <script>
 import CRUDBar from "./CRUDBar.vue";
 import EditButton from "./buttons/EditButton.vue";
 import DeleteButton from "./buttons/DeleteButton.vue";
 
+import deepSearchMixin from "../../mixins/deepSearchMixin";
 import loadingMixin from "../../mixins/loadingMixin.js";
 import syncSortMixin from "../../mixins/syncSortMixin.js";
 
 export default {
   name: "CRUDList",
   components: {
     CRUDBar,
     EditButton,
     DeleteButton,
   },
-  mixins: [loadingMixin, syncSortMixin],
+  mixins: [deepSearchMixin, loadingMixin, syncSortMixin],
   props: {
     /**
      * Elevate the table?
      * @values true, false
      */
     elevated: {
       type: Boolean,
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/DetailView.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/DetailView.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/FilterBar.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/FilterBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/InlineCRUDList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/InlineCRUDList.vue`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
       :get-create-data="getCreateData"
       :item-id="itemId"
       :show-create="isCreate"
       :enable-edit="false"
       :show-select="isCreate"
       :show-action-column="isCreate"
       :lock="!isCreate"
+      :use-deep-search="useDeepSearch"
       @lastQuery="affectedQuery = $event"
       @mode="handleMode"
       @loading="handleLoading($event)"
       @items="$emit('items', $event)"
     >
       <template #filters="{ attrs, on }">
         <slot name="filters" :attrs="attrs" :on="on" />
@@ -114,24 +115,25 @@
 <script>
 import CRUDList from "./CRUDList.vue";
 import EditButton from "./buttons/EditButton.vue";
 import CancelButton from "./buttons/CancelButton.vue";
 import SaveButton from "./buttons/SaveButton.vue";
 
 import createOrPatchMixin from "../../mixins/createOrPatchMixin.js";
+import deepSearchMixin from "../../mixins/deepSearchMixin";
 
 export default {
   name: "InlineCRUDList",
   components: {
     CRUDList,
     EditButton,
     CancelButton,
     SaveButton,
   },
-  mixins: [createOrPatchMixin],
+  mixins: [createOrPatchMixin, deepSearchMixin],
   data() {
     return {
       valid: false,
       // Modal state
       mode: false,
       // Store inline edits
       inlineEdits: {},
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/ObjectOverview.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/ObjectOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/UpdateIndicator.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/UpdateIndicator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/BaseButton.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/BaseButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/buttons/FilterButton.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/buttons/FilterButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ColorField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/ColorField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/DateField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/DateTimeField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/DateTimeField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/SexSelect.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/SexSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/TimeField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/TimeField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/generic/forms/WeekDayField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/generic/forms/WeekDayField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group/GroupCollection.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/group/GroupCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group_type/GroupType.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/group_type/GroupType.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/group_type/groupType.graphql` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/group_type/groupType.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/HolidayInlineList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/holiday/HolidayInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/holiday/holiday.graphql` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/holiday/holiday.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationItem.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/notifications/NotificationItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/notifications/NotificationList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/notifications/NotificationList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/pdf/DownloadPDF.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/pdf/DownloadPDF.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AdditionalImage.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/AdditionalImage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/AvatarContent.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/AvatarContent.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonActions.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonActions.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonChip.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonChip.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonCollection.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/PersonOverview.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/PersonOverview.vue`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
                   <v-list-item-content>
                     <v-list-item-title>
                       {{ person.firstName }}
                       {{ person.additionalName }}
                       {{ person.lastName }}
                     </v-list-item-title>
+                    <v-list-item-subtitle>
+                      {{ $t("person.name") }}
+                    </v-list-item-subtitle>
                   </v-list-item-content>
                 </v-list-item>
                 <v-divider inset />
 
                 <v-list-item>
                   <v-list-item-icon>
                     <v-icon> mdi-human-non-binary</v-icon>
@@ -75,31 +78,35 @@
                     <v-list-item-title>
                       {{
                         person.sex
                           ? $t("person.sex." + person.sex.toLowerCase())
                           : "–"
                       }}
                     </v-list-item-title>
+                    <v-list-item-subtitle>
+                      {{ $t("person.sex_description") }}
+                    </v-list-item-subtitle>
                   </v-list-item-content>
                 </v-list-item>
                 <v-divider inset />
 
                 <v-list-item>
                   <v-list-item-icon>
                     <v-icon> mdi-map-marker-outline</v-icon>
                   </v-list-item-icon>
 
                   <v-list-item-content>
-                    <v-list-item-title
-                      >{{ person.street || "–" }}
-                      {{ person.housenumber }}
-                    </v-list-item-title>
-                    <v-list-item-subtitle
-                      >{{ person.postalCode }}
+                    <v-list-item-title>
+                      <!-- eslint-disable-next-line @intlify/vue-i18n/no-raw-text -->
+                      {{ person.street || "–" }} {{ person.housenumber }},
+                      {{ person.postalCode }}
                       {{ person.place }}
+                    </v-list-item-title>
+                    <v-list-item-subtitle>
+                      {{ $t("person.address") }}
                     </v-list-item-subtitle>
                   </v-list-item-content>
                 </v-list-item>
                 <v-divider inset />
 
                 <v-list-item
                   :href="person.phoneNumber ? 'tel:' + person.phoneNumber : ''"
@@ -143,33 +150,57 @@
                     <v-icon>mdi-email-outline</v-icon>
                   </v-list-item-icon>
 
                   <v-list-item-content>
                     <v-list-item-title>
                       {{ person.email || "–" }}
                     </v-list-item-title>
+                    <v-list-item-subtitle>
+                      {{ $t("person.email_address") }}
+                    </v-list-item-subtitle>
                   </v-list-item-content>
                 </v-list-item>
                 <v-divider inset />
 
                 <v-list-item>
                   <v-list-item-icon>
                     <v-icon> mdi-cake-variant-outline</v-icon>
                   </v-list-item-icon>
 
                   <v-list-item-content>
-                    <v-list-item-title
-                      >{{
-                        !!person.dateOfBirth
-                          ? $d($parseISODate(person.dateOfBirth), "short")
-                          : "–"
-                      }}
+                    <v-list-item-title>
+                      <span v-if="person.dateOfBirth && person.placeOfBirth">
+                        {{
+                          $t("person.birth_date_and_birth_place_formatted", {
+                            date: $d(
+                              $parseISODate(person.dateOfBirth),
+                              "short",
+                            ),
+                            place: person.placeOfBirth,
+                          })
+                        }}
+                      </span>
+                      <span v-else-if="person.dateOfBirth">{{
+                        $d($parseISODate(person.dateOfBirth), "short")
+                      }}</span>
+                      <span v-else-if="person.placeOfBirth">{{
+                        person.placeOfBirth
+                      }}</span>
+                      <span v-else>–</span>
                     </v-list-item-title>
-                    <v-list-item-subtitle
-                      >{{ person.placeOfBirth }}
+                    <v-list-item-subtitle>
+                      <span v-if="!person.dateOfBirth === !person.placeOfBirth">
+                        {{ $t("person.birth_date_and_birth_place") }}
+                      </span>
+                      <span v-else-if="person.dateOfBirth">
+                        {{ $t("person.birth_date") }}
+                      </span>
+                      <span v-else-if="person.placeOfBirth">
+                        {{ $t("person.birth_place") }}
+                      </span>
                     </v-list-item-subtitle>
                   </v-list-item-content>
                 </v-list-item>
               </v-list>
             </v-card>
 
             <additional-image :src="person.secondaryImageUrl" />
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/person/personOverview.graphql` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/person/personOverview.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/RoomInlineList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/room/RoomInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/room/room.graphql` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/room/room.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermField.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/school_term/SchoolTermField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/school_term/schoolTerm.graphql` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/school_term/schoolTerm.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactor.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/two_factor/TwoFactor.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/index.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/de.json` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/de.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989010989010989%*

 * *Differences: {"'person'": "{'birth_date_and_birth_place_formatted': '{date} in {place}', "*

 * *             "'birth_date_and_birth_place': 'Geburtsdatum und Geburtsort'}"}*

```diff
@@ -269,14 +269,16 @@
             "menu_title": "Berechtigungen verwalten"
         }
     },
     "person": {
         "account_menu_title": "Konto",
         "additional_image": "Weiteres Bild",
         "avatar": "Avatar",
+        "birth_date_and_birth_place": "Geburtsdatum und Geburtsort",
+        "birth_date_and_birth_place_formatted": "{date} in {place}",
         "children": "Kinder",
         "confirm_delete": "Wollen Sie wirklich diese Person l\u00f6schen?",
         "delete": "L\u00f6schen",
         "details": "Kontaktdaten",
         "first_name": "Vorname",
         "guardians": "Erziehungsberechtigte / Eltern",
         "home": "Festnetz",
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/en.json` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/en.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9686447811447813%*

 * *Differences: {"'date_select'": "OrderedDict([('label', 'Select date')])",*

 * * "'person'": "{'home': 'Home phone', 'mobile': 'Mobile phone', 'short_name': 'Shortname', "*

 * *             "'address': 'Address', 'birth_date': 'Date of birth', 'birth_place': 'Place of "*

 * *             "birth', 'birth_date_and_birth_place_formatted': '{date} in {place}', "*

 * *             "'birth_date_and_birth_place': 'Date of birth and place of birth', 'email_address': "*

 * *             "'Email address', 'sex_description': 'Sex'}"}*

```diff
@@ -152,14 +152,17 @@
             "title_plural": "Dashboard Widgets"
         },
         "menu_title": "Dashboard"
     },
     "data_check": {
         "menu_title": "Data Checks"
     },
+    "date_select": {
+        "label": "Select date"
+    },
     "download_pdf": {
         "download": "Download",
         "notice": "If the download does not start automatically, please click the button below.",
         "title": "Downloading PDF file ..."
     },
     "forms": {
         "date_time": {
@@ -268,44 +271,51 @@
         "manage": {
             "menu_title": "Manage Permissions"
         }
     },
     "person": {
         "account_menu_title": "Account",
         "additional_image": "Additional Image",
+        "address": "Address",
         "avatar": "Avatar",
+        "birth_date": "Date of birth",
+        "birth_date_and_birth_place": "Date of birth and place of birth",
+        "birth_date_and_birth_place_formatted": "{date} in {place}",
+        "birth_place": "Place of birth",
         "children": "Children",
         "confirm_delete": "Do you really want to delete this person?",
         "delete": "Delete",
         "details": "Contact details",
+        "email_address": "Email address",
         "first_name": "First Name",
         "guardians": "Guardians / Parents",
-        "home": "home phone",
+        "home": "Home phone",
         "impersonation": {
             "impersonate": "Impersonate",
             "impersonating": "Impersonating",
             "stop": "Stop Impersonation"
         },
         "invite": "Invite",
         "last_name": "Last Name",
         "logged_in_as": "Logged in as",
         "menu_title": "Persons",
-        "mobile": "mobile phone",
+        "mobile": "Mobile phone",
         "name": "Name",
         "no_additional_image": "The person didn't upload an additional Image",
         "no_persons": "No Persons",
         "page_title": "Person",
         "primary_group": "Primary Group",
         "sex": {
             "f": "Female",
             "field": "Sex",
             "m": "Male",
             "x": "Other"
         },
-        "short_name": "Short Name",
+        "sex_description": "Sex",
+        "short_name": "Shortname",
         "title": "Person",
         "title_plural": "Persons",
         "username": "Username"
     },
     "personal_events": {
         "create_button": "Create event",
         "create_title": "Create personal event",
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/ru.json` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/ru.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/messages/uk.json` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/messages/uk.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/aleksis.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/calendarFeedDetails.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/calendarFeedDetails.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/createOrPatchMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/createOrPatchMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/deleteMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/deleteMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/error404.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/error404.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/formRulesMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/formRulesMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/menus.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/menus.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/mutateMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/mutateMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/offline.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/offline.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/permissions.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/permissions.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/queryMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/queryMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/routes.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/sexChoiceMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/sexChoiceMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/syncSortMixin.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/syncSortMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/mixins/useRegisterSW.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/mixins/useRegisterSW.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/plugins/aleksis.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/plugins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/frontend/routes.js` & `aleksis_core-4.0.0.dev7/aleksis/core/frontend/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/health_checks.py` & `aleksis_core-4.0.0.dev7/aleksis/core/health_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev7/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/management/commands/convert_urls_to_routes.py` & `aleksis_core-4.0.0.dev7/aleksis/core/management/commands/convert_urls_to_routes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/management/commands/vite.py` & `aleksis_core-4.0.0.dev7/aleksis/core/management/commands/vite.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/managers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0001_initial.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0002_school_term.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0002_school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0003_drop_image_cropping.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0003_drop_image_cropping.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0004_add_permissions_for_group_stats.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0004_add_permissions_for_group_stats.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0005_timestamped_activity_notification.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0005_timestamped_activity_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0006_dashboard_widget_size.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0006_dashboard_widget_size.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0007_dashboard_widget_order.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0007_dashboard_widget_order.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0008_data_check_result.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0008_data_check_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0009_default_dashboard.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0009_default_dashboard.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0010_external_link_widget.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0010_external_link_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0011_globalpermissions_options.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0011_globalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0013_pdf_file.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0013_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0014_alter_pdffile_file.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0014_alter_pdffile_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0015_oauth_permissions.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0015_oauth_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0016_taskuserassignment.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0016_taskuserassignment.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0018_pdffile_html_file.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0018_pdffile_html_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0019_fix_uniqueness_per_site.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0019_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0020_pdf_file_person_optional.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0020_pdf_file_person_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0021_drop_persons_accounts_perm.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0021_drop_persons_accounts_perm.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0022_public_favicon.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0022_public_favicon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0023_oauth_application_model.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0023_oauth_application_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0024_oauth_grant_types_optional.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0024_oauth_grant_types_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0025_oauth_align_user_fk.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0025_oauth_align_user_fk.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0028_char_field_not_null.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0028_char_field_not_null.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0029_invitations.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0029_invitations.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0030_user_attributes.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0030_user_attributes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0031_oauthapplication_icon.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0031_oauthapplication_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0033_update_photo_avatar.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0033_update_photo_avatar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0034_invite_permission.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0034_invite_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0035_preference_model_unique.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0035_preference_model_unique.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         db_alias = schema_editor.connection.alias
 
         models = [GroupPreferenceModel, PersonPreferenceModel, SitePreferenceModel]
 
         for model in models:
             duplicates = {}
             for obj in model.objects.using(db_alias).all():
-                key = f"{obj.section}__{obj.name}"
+                instance = obj.instance.pk if hasattr(obj, "instance") else "site"
+                key = f"{instance}__{obj.section}__{obj.name}"
                 duplicates.setdefault(key, [])
                 duplicates[key].append(obj)
 
             for key, objs in duplicates.items():
                 if len(objs) > 1:
                     found = False
                     for obj in objs:
@@ -36,18 +37,18 @@
                             found = True
 
 
     operations = [
         migrations.RunPython(_migrate_preference_models_to_unique),
         migrations.AlterUniqueTogether(
             name='grouppreferencemodel',
-            unique_together={('section', 'name')},
+            unique_together={('instance', 'section', 'name')},
         ),
         migrations.AlterUniqueTogether(
             name='personpreferencemodel',
-            unique_together={('section', 'name')},
+            unique_together={('instance', 'section', 'name')},
         ),
         migrations.AlterUniqueTogether(
             name='sitepreferencemodel',
             unique_together={('section', 'name')},
         ),
     ]
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0036_additionalfields_helptext_required.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0036_additionalfields_helptext_required.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0037_add_static_content_widget.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0037_add_static_content_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0038_notification_send_at.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0038_notification_send_at.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0039_personal_ical_url.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0039_personal_ical_url.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0041_update_gender_choices.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0041_update_gender_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0042_pdffile_empty.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0042_pdffile_empty.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0043_task_assignment_meta.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0043_task_assignment_meta.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0044_task_assignment_result_fetched.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0044_task_assignment_result_fetched.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0046_notification_create_field_icon.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0046_notification_create_field_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0047_add_room_model.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0047_add_room_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0048_delete_personalicalurl.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0048_delete_personalicalurl.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0050_managed_by_app_label.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0050_managed_by_app_label.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0051_calendarevent_and_holiday.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0051_calendarevent_and_holiday.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0052_site_related_name.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0052_site_related_name.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0053_freebusy.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0053_freebusy.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0054_create_organisation_model.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0054_create_organisation_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0055_customevent.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0055_customevent.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0058_migrate_preferences_to_global.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0058_migrate_preferences_to_global.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0059_drop_site.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0059_drop_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/migrations/0060_person_unique_short_name_email.py` & `aleksis_core-4.0.0.dev7/aleksis/core/migrations/0060_person_unique_short_name_email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/mixins.py` & `aleksis_core-4.0.0.dev7/aleksis/core/mixins.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/models.py` & `aleksis_core-4.0.0.dev7/aleksis/core/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,28 +573,33 @@
         # Determine state of object in relation to database
         dirty = self.pk is None or bool(self.group_info_tracker.changed())
 
         super().save(*args, **kwargs)
 
         if force or dirty:
             # Synchronise group to Django group with same name
-            dj_group, _ = DjangoGroup.objects.get_or_create(name=self.name)
-            dj_group.user_set.set(
-                list(
-                    self.members.filter(user__isnull=False)
-                    .values_list("user", flat=True)
-                    .union(self.owners.filter(user__isnull=False).values_list("user", flat=True))
+            dj_group = self.django_group
+            if dj_group:
+                dj_group.user_set.set(
+                    list(
+                        self.members.filter(user__isnull=False)
+                        .values_list("user", flat=True)
+                        .union(
+                            self.owners.filter(user__isnull=False).values_list("user", flat=True)
+                        )
+                    )
                 )
-            )
-            dj_group.save()
+                dj_group.save()
 
     @property
     def django_group(self):
         """Get Django group for this group."""
-        dj_group, _ = DjangoGroup.objects.get_or_create(name=self.name)
+        dj_group = None
+        if not self.school_term or self.school_term == SchoolTerm.current:
+            dj_group, _ = DjangoGroup.objects.get_or_create(name=self.name)
         return dj_group
 
 
 class PersonGroupThrough(ExtensibleModel):
     """Through table for many-to-many relationship of group members.
 
     It does not have any fields on its own; these are generated upon instantiation
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/preferences.py` & `aleksis_core-4.0.0.dev7/aleksis/core/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/registries.py` & `aleksis_core-4.0.0.dev7/aleksis/core/registries.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/rules.py` & `aleksis_core-4.0.0.dev7/aleksis/core/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/__init__.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/base.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/calendar.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/calendar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/celery_progress.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/custom_menu.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/custom_menu.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/group.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/group_type.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/group_type.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/holiday.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/holiday.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/installed_apps.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/installed_apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/notification.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/oauth.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/pdf.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/person.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/person.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/personal_event.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/personal_event.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/room.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/room.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/school_term.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/search.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/site_preferences.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/site_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/system_properties.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/system_properties.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/two_factor.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/two_factor.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/schema/user.py` & `aleksis_core-4.0.0.dev7/aleksis/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/settings.py` & `aleksis_core-4.0.0.dev7/aleksis/core/settings.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-banner.svg` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-banner.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-favicon.png` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-favicon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.png` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon-maskable.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon-maskable.svg` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon-maskable.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.png` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/aleksis-icon.svg` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/aleksis-icon.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/fallback.png` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/fallback.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/img/hero.svg` & `aleksis_core-4.0.0.dev7/aleksis/core/static/img/hero.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/js/edit_dashboard.js` & `aleksis_core-4.0.0.dev7/aleksis/core/static/js/edit_dashboard.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/js/helper.js` & `aleksis_core-4.0.0.dev7/aleksis/core/static/js/helper.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/js/include_ajax_live.js` & `aleksis_core-4.0.0.dev7/aleksis/core/static/js/include_ajax_live.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/js/main.js` & `aleksis_core-4.0.0.dev7/aleksis/core/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/js/multi_select.js` & `aleksis_core-4.0.0.dev7/aleksis/core/static/js/multi_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/js/search.js` & `aleksis_core-4.0.0.dev7/aleksis/core/static/js/search.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/js/serviceworker.js` & `aleksis_core-4.0.0.dev7/aleksis/core/static/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/print.css` & `aleksis_core-4.0.0.dev7/aleksis/core/static/print.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/public/materialize-custom.scss` & `aleksis_core-4.0.0.dev7/aleksis/core/static/public/materialize-custom.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/public/style.scss` & `aleksis_core-4.0.0.dev7/aleksis/core/static/public/style.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/static/public/theme.scss` & `aleksis_core-4.0.0.dev7/aleksis/core/static/public/theme.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tables.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tasks.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/403.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/403.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/404.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/500.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/account_inactive.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/account_inactive.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email/email_confirmation_message.txt` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/email/email_confirmation_message.txt`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/email_confirm.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_change.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_done.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/password_reset_from_key_done.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/signup_closed.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_email_required.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/verification_email_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/account/verification_sent.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/components/chips.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/components/chips.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/components/pagination.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/form.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/announcement/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/announcement/list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/announcement/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_print.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/base_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/base_simple_print.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/base_simple_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/create.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/edit.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/dashboard_widget/list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/dashboard_widget/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/data_check/list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/data_check/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/edit_dashboard.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/edit_dashboard.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/child_groups.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/child_groups.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/edit.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/full.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/group/list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/index.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/delete.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/pages/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/system_status.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/pages/system_status.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/pages/test_pdf.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/pages/test_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/announcements.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/announcements.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/avatar_content.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/avatar_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/crud_events.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/crud_events.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/meta.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/meta.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/partials/splash_screen.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/partials/splash_screen.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/assign.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/perms/assign.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/perms/list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/perms/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/create.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/person/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/edit.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/person/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/person/list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/person/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/core/vue_index.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/core/vue_index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/django_tables2/materialize.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/django_tables2/materialize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/dynamic_preferences/form.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/dynamic_preferences/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/disabled.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/invitations/disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/enter.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/invitations/enter.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/invitations/forms/_invite.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/invitations/forms/_invite.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/colorfield_colorwidget.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/colorfield_colorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/material/fields/django_select2_select2widget.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/material/fields/django_select2_select2widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/create.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/detail.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/edit.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/application/list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/application/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/oauth2_provider/authorize.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/offline.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/offline.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/search/search.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/authentication_error.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/connections.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/login_cancelled.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/login_cancelled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/signup.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/socialaccount/snippets/provider_list.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/base.email` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/base.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/celery_failure.email` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/celery_failure.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/data_checks.email` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/data_checks.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/email.css` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/email.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/invitation.email` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/invitation.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/notification.email` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/notification.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/templated_email/person_changed.email` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/templated_email/person_changed.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/_wizard_actions.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/backup_tokens.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/login.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/otp_required.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/phone_register.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/core/setup_complete.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templates/two_factor/profile/disable.html` & `aleksis_core-4.0.0.dev7/aleksis/core/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templatetags/data_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/templatetags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/templatetags/html_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/templatetags/html_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/browser/test_selenium.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/browser/test_selenium.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/managers/test_aleksisbasemanager.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/managers/test_aleksisbasemanager.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/mixins/test_registry_object.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/mixins/test_registry_object.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test.pdf` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test.pdf`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_group_sync.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test_group_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_notification.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/models/test_pdffile.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/models/test_pdffile.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/test_regression.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/regression/view_oauth.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/regression/view_oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/templatetags/test_data_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/templatetags/test_data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/tests/views/test_account.py` & `aleksis_core-4.0.0.dev7/aleksis/core/tests/views/test_account.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/urls.py` & `aleksis_core-4.0.0.dev7/aleksis/core/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/apps.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/apps.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 11018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 7920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 26
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 18985
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/email.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/email.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 986
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 850
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/notifications.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/notifications.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 3818
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/predicates.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/predicates.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 5801
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 936
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/__pycache__/spdx.cpython-311.pyc` & `aleksis_core-4.0.0.dev7/aleksis/core/util/__pycache__/spdx.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8f4e0e66 (Thu Apr  4 06:54:07 2024 UTC)
+moddate:  0x3ccd2766 (Tue Apr 23 15:01:16 2024 UTC)
 files sz: 125
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/apps.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/auth_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/auth_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,19 @@
         claims = {}
         # Pull together claim data from all apps
         for app in AppConfig.__subclasses__():
             claims.update(app.get_additional_claims(scopes, request))
 
         return claims
 
+    def get_userinfo_claims(self, request: OauthlibRequest) -> dict[str, Any]:
+        oidc_claims = super().get_oidc_claims(request.access_token, None, request)
+        additional_claims = self.get_additional_claims(request)
+        return oidc_claims | additional_claims
+
 
 class AppScopes(BaseScopes):
     """Scopes backend for django-oauth-toolkit gathering scopes from apps.
 
     Will call the respective method on all known AlekSIS app configs and
     join the results.
     """
```

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/celery_progress.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/core_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/email.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/forms.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/frontend_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/frontend_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/ldap.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/licenses.json` & `aleksis_core-4.0.0.dev7/aleksis/core/util/licenses.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/messages.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/messages.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/middlewares.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/middlewares.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/model_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/model_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/notifications.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/pdf.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/predicates.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/sass_helpers.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/sass_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/search.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/util/tables.py` & `aleksis_core-4.0.0.dev7/aleksis/core/util/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/views.py` & `aleksis_core-4.0.0.dev7/aleksis/core/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/aleksis/core/vite.config.js` & `aleksis_core-4.0.0.dev7/aleksis/core/vite.config.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/Makefile` & `aleksis_core-4.0.0.dev7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/2fa.png` & `aleksis_core-4.0.0.dev7/docs/_static/2fa.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/accept_invite.png` & `aleksis_core-4.0.0.dev7/docs/_static/accept_invite.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/create_dashboard_widget.png` & `aleksis_core-4.0.0.dev7/docs/_static/create_dashboard_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/create_social_application.png` & `aleksis_core-4.0.0.dev7/docs/_static/create_social_application.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/dashboard.png` & `aleksis_core-4.0.0.dev7/docs/_static/dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/dashboard_widgets.png` & `aleksis_core-4.0.0.dev7/docs/_static/dashboard_widgets.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/data_checks.png` & `aleksis_core-4.0.0.dev7/docs/_static/data_checks.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/edit_dashboard.png` & `aleksis_core-4.0.0.dev7/docs/_static/edit_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/edit_default_dashboard.png` & `aleksis_core-4.0.0.dev7/docs/_static/edit_default_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/invitations.png` & `aleksis_core-4.0.0.dev7/docs/_static/invitations.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/invite_existing.png` & `aleksis_core-4.0.0.dev7/docs/_static/invite_existing.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/pwa_desktop_chromium.png` & `aleksis_core-4.0.0.dev7/docs/_static/pwa_desktop_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_chromium.png` & `aleksis_core-4.0.0.dev7/docs/_static/pwa_mobile_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_firefox.png` & `aleksis_core-4.0.0.dev7/docs/_static/pwa_mobile_firefox.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/pwa_mobile_safari.png` & `aleksis_core-4.0.0.dev7/docs/_static/pwa_mobile_safari.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/_static/signup.png` & `aleksis_core-4.0.0.dev7/docs/_static/signup.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/01_core_concepts.rst` & `aleksis_core-4.0.0.dev7/docs/admin/01_core_concepts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/10_install.rst` & `aleksis_core-4.0.0.dev7/docs/admin/10_install.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/15_config_files.rst` & `aleksis_core-4.0.0.dev7/docs/admin/15_config_files.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/16_config_options.rst` & `aleksis_core-4.0.0.dev7/docs/admin/16_config_options.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/17_storage.rst` & `aleksis_core-4.0.0.dev7/docs/admin/17_storage.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/18_mail.rst` & `aleksis_core-4.0.0.dev7/docs/admin/18_mail.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/21_ldap.rst` & `aleksis_core-4.0.0.dev7/docs/admin/21_ldap.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/22_registration.rst` & `aleksis_core-4.0.0.dev7/docs/admin/22_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/23_socialaccounts.rst` & `aleksis_core-4.0.0.dev7/docs/admin/23_socialaccounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/31_monitoring.rst` & `aleksis_core-4.0.0.dev7/docs/admin/31_monitoring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/32_tasks.rst` & `aleksis_core-4.0.0.dev7/docs/admin/32_tasks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/33_data_checks.rst` & `aleksis_core-4.0.0.dev7/docs/admin/33_data_checks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/admin/50_dashboard.rst` & `aleksis_core-4.0.0.dev7/docs/admin/50_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/conf.py` & `aleksis_core-4.0.0.dev7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/dev/01_setup.rst` & `aleksis_core-4.0.0.dev7/docs/dev/01_setup.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/dev/02_install_apps.rst` & `aleksis_core-4.0.0.dev7/docs/dev/02_install_apps.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/dev/03_run_tests.rst` & `aleksis_core-4.0.0.dev7/docs/dev/03_run_tests.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/dev/04_materialize_templates.rst` & `aleksis_core-4.0.0.dev7/docs/dev/04_materialize_templates.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/dev/06_merging_app_settings.rst` & `aleksis_core-4.0.0.dev7/docs/dev/06_merging_app_settings.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/dev/10_dashboard_widgets.rst` & `aleksis_core-4.0.0.dev7/docs/dev/10_dashboard_widgets.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/index.rst` & `aleksis_core-4.0.0.dev7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/make.bat` & `aleksis_core-4.0.0.dev7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/ref/core/09_utils.rst` & `aleksis_core-4.0.0.dev7/docs/ref/core/09_utils.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/user/01_registration.rst` & `aleksis_core-4.0.0.dev7/docs/user/01_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/user/02_personal_account.rst` & `aleksis_core-4.0.0.dev7/docs/user/02_personal_account.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/user/10_dashboard.rst` & `aleksis_core-4.0.0.dev7/docs/user/10_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/docs/user/20_pwa.rst` & `aleksis_core-4.0.0.dev7/docs/user/20_pwa.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/pyproject.toml` & `aleksis_core-4.0.0.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Core"
-version = "4.0.0.dev6"
+version = "4.0.0.dev7"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
```

### Comparing `aleksis_core-4.0.0.dev6/tox.ini` & `aleksis_core-4.0.0.dev7/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev6/PKG-INFO` & `aleksis_core-4.0.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlekSIS-Core
-Version: 4.0.0.dev6
+Version: 4.0.0.dev7
 Summary: AlekSIS (School Information System) — Core
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
```

