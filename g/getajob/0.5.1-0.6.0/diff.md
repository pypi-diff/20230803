# Comparing `tmp/getajob-0.5.1.tar.gz` & `tmp/getajob-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.5.1.tar", max compression
+gzip compressed data, was "getajob-0.6.0.tar", max compression
```

## Comparing `getajob-0.5.1.tar` & `getajob-0.6.0.tar`

### file list

```diff
@@ -1,152 +1,184 @@
--rw-r--r--   0        0        0    11357 2023-07-26 20:03:40.893400 getajob-0.5.1/LICENSE
--rw-r--r--   0        0        0       69 2023-07-26 20:03:40.897400 getajob-0.5.1/README.md
--rw-r--r--   0        0        0       22 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/__init__.py
--rw-r--r--   0        0        0     2927 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/abstractions/models.py
--rw-r--r--   0        0        0    16351 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/abstractions/repository.py
--rw-r--r--   0        0        0      385 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/abstractions/vendor_client_factory.py
--rw-r--r--   0        0        0     2121 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      177 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      607 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      844 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applicant_matching/__init__.py
--rw-r--r--   0        0        0     1347 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applicant_matching/models.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/applicant_tracking/__init__.py
--rw-r--r--   0        0        0     1044 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/applicant_tracking/models.py
--rw-r--r--   0        0        0     2498 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/applicant_tracking/repository.py
--rw-r--r--   0        0        0      277 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/enumerations.py
--rw-r--r--   0        0        0      726 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     3635 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     2629 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/message/__init__.py
--rw-r--r--   0        0        0      616 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/message/models.py
--rw-r--r--   0        0        0      889 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/message/repository.py
--rw-r--r--   0        0        0      272 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/models.py
--rw-r--r--   0        0        0     1770 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/repository.py
--rw-r--r--   0        0        0     1650 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/chat/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/__init__.py
--rw-r--r--   0        0        0      331 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/models.py
--rw-r--r--   0        0        0      817 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/audit/__init__.py
--rw-r--r--   0        0        0      482 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/audit/models.py
--rw-r--r--   0        0        0     1101 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/audit/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/details/__init__.py
--rw-r--r--   0        0        0      743 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/details/models.py
--rw-r--r--   0        0        0     1451 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/details/repository.py
--rw-r--r--   0        0        0     1870 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/enumerations.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/invitations/__init__.py
--rw-r--r--   0        0        0      145 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/invitations/models.py
--rw-r--r--   0        0        0      783 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/invitations/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/__init__.py
--rw-r--r--   0        0        0     3174 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/models.py
--rw-r--r--   0        0        0     1422 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/repository.py
--rw-r--r--   0        0        0      533 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/jobs/unit_of_work.py
--rw-r--r--   0        0        0      102 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/recruiters/__init__.py
--rw-r--r--   0        0        0      117 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/recruiters/models.py
--rw-r--r--   0        0        0      741 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/recruiters/repository.py
--rw-r--r--   0        0        0     1353 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0      210 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/enumerations.py
--rw-r--r--   0        0        0      995 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1862 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/search/__init__.py
--rw-r--r--   0        0        0     1732 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/search/models.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      851 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/details/__init__.py
--rw-r--r--   0        0        0     2974 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/details/models.py
--rw-r--r--   0        0        0     1419 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/details/repository.py
--rw-r--r--   0        0        0     1213 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/enumerations.py
--rw-r--r--   0        0        0       89 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/models.py
--rw-r--r--   0        0        0     1358 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      797 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      481 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0     2607 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/static/__init__.py
--rw-r--r--   0        0        0     1518 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/static/enumerations.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/__init__.py
--rw-r--r--   0        0        0     2116 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/application.py
--rw-r--r--   0        0        0     1684 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/chat.py
--rw-r--r--   0        0        0     1027 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/company.py
--rw-r--r--   0        0        0      382 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/job.py
--rw-r--r--   0        0        0     1843 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/recruiter.py
--rw-r--r--   0        0        0      645 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/recruiter_invitation.py
--rw-r--r--   0        0        0     1706 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/scheduled_events.py
--rw-r--r--   0        0        0     2442 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/test_support/fixtures/users.py
--rw-r--r--   0        0        0      886 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/__init__.py
--rw-r--r--   0        0        0      468 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/client_factory.py
--rw-r--r--   0        0        0     1270 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/mock.py
--rw-r--r--   0        0        0      758 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/models.py
--rw-r--r--   0        0        0     1757 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/algolia/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.897400 getajob-0.5.1/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0     2139 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/client.py
--rw-r--r--   0        0        0      340 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/client_factory.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     2694 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0     2553 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/mock.py
--rw-r--r--   0        0        0      413 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2043 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1588 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2371 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0     2318 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1353 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     2642 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/__init__.py
--rw-r--r--   0        0        0      680 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/client_factory.py
--rw-r--r--   0        0        0     1102 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/helpers.py
--rw-r--r--   0        0        0      192 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/mock.py
--rw-r--r--   0        0        0     1975 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/models.py
--rw-r--r--   0        0        0     1212 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firebase_storage/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/__init__.py
--rw-r--r--   0        0        0      582 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/client_factory.py
--rw-r--r--   0        0        0     1102 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/helpers.py
--rw-r--r--   0        0        0      507 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/mock.py
--rw-r--r--   0        0        0     1975 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/models.py
--rw-r--r--   0        0        0     9200 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/firestore/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      725 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0     1369 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/client_factory.py
--rw-r--r--   0        0        0      320 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0      716 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     2087 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0     1517 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/__init__.py
--rw-r--r--   0        0        0      989 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/client_factory.py
--rw-r--r--   0        0        0      282 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/mock.py
--rw-r--r--   0        0        0     1231 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/repository.py
--rw-r--r--   0        0        0      104 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/mailgun/templates/chat_message.html
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/__init__.py
--rw-r--r--   0        0        0      443 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/client_factory.py
--rw-r--r--   0        0        0      690 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/mock.py
--rw-r--r--   0        0        0      985 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/repository.py
--rw-r--r--   0        0        0      590 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/openai/settings.py
--rw-r--r--   0        0        0        0 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/__init__.py
--rw-r--r--   0        0        0      502 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/client_factory.py
--rw-r--r--   0        0        0      343 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/mock.py
--rw-r--r--   0        0        0     2451 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/redis/repository.py
--rw-r--r--   0        0        0      251 2023-07-26 20:03:40.901399 getajob-0.5.1/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1786 2023-07-26 20:03:40.901399 getajob-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 getajob-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 00:23:13.609619 getajob-0.6.0/LICENSE
+-rw-r--r--   0        0        0       69 2023-08-03 00:23:13.609619 getajob-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-03 00:23:13.609619 getajob-0.6.0/getajob/__init__.py
+-rw-r--r--   0        0        0     2980 2023-08-03 00:23:13.609619 getajob-0.6.0/getajob/abstractions/models.py
+-rw-r--r--   0        0        0    16306 2023-08-03 00:23:13.609619 getajob-0.6.0/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0      385 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/abstractions/vendor_client_factory.py
+-rw-r--r--   0        0        0     2161 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      177 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      607 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      844 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/applicant_tracking/__init__.py
+-rw-r--r--   0        0        0     1044 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/applicant_tracking/models.py
+-rw-r--r--   0        0        0     2502 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/applicant_tracking/repository.py
+-rw-r--r--   0        0        0     4438 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/async_service.py
+-rw-r--r--   0        0        0      277 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/enumerations.py
+-rw-r--r--   0        0        0     1851 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     3804 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     1781 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/search.py
+-rw-r--r--   0        0        0     2629 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/__init__.py
+-rw-r--r--   0        0        0     2617 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/message/__init__.py
+-rw-r--r--   0        0        0      616 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/message/models.py
+-rw-r--r--   0        0        0      892 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/message/repository.py
+-rw-r--r--   0        0        0      272 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/models.py
+-rw-r--r--   0        0        0     1899 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/repository.py
+-rw-r--r--   0        0        0     1650 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/chat/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/applicant_tracking_settings/__init__.py
+-rw-r--r--   0        0        0      368 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/applicant_tracking_settings/models.py
+-rw-r--r--   0        0        0      820 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/applicant_tracking_settings/repository.py
+-rw-r--r--   0        0        0     2375 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/audit/__init__.py
+-rw-r--r--   0        0        0     2100 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/audit/async_service.py
+-rw-r--r--   0        0        0      482 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/audit/models.py
+-rw-r--r--   0        0        0     1104 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/audit/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/details/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/details/models.py
+-rw-r--r--   0        0        0     1448 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/details/repository.py
+-rw-r--r--   0        0        0     1870 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/enumerations.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/invitations/__init__.py
+-rw-r--r--   0        0        0      145 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/invitations/models.py
+-rw-r--r--   0        0        0      786 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/invitations/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/jobs/__init__.py
+-rw-r--r--   0        0        0     3865 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/jobs/async_service.py
+-rw-r--r--   0        0        0     3174 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/jobs/models.py
+-rw-r--r--   0        0        0     1421 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/jobs/repository.py
+-rw-r--r--   0        0        0      533 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      102 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/recruiters/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/recruiters/models.py
+-rw-r--r--   0        0        0      744 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/recruiters/repository.py
+-rw-r--r--   0        0        0     1357 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0      210 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/scheduled_events/enumerations.py
+-rw-r--r--   0        0        0      995 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1865 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/search/__init__.py
+-rw-r--r--   0        0        0     1732 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/search/models.py
+-rw-r--r--   0        0        0     5410 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      854 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/details/__init__.py
+-rw-r--r--   0        0        0     2974 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/details/models.py
+-rw-r--r--   0        0        0     1416 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/details/repository.py
+-rw-r--r--   0        0        0     1213 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/enumerations.py
+-rw-r--r--   0        0        0       89 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0     1362 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/extracted_data/__init__.py
+-rw-r--r--   0        0        0     6828 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/extracted_data/extractor.py
+-rw-r--r--   0        0        0     2040 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/extracted_data/models.py
+-rw-r--r--   0        0        0     1841 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/extracted_data/repository.py
+-rw-r--r--   0        0        0     1664 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/extracted_data/unit_of_work.py
+-rw-r--r--   0        0        0      402 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0     1693 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0     2649 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json
+-rw-r--r--   0        0        0     3412 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json
+-rw-r--r--   0        0        0     1591 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json
+-rw-r--r--   0        0        0     4311 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json
+-rw-r--r--   0        0        0     2018 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json
+-rw-r--r--   0        0        0     2479 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json
+-rw-r--r--   0        0        0     2333 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json
+-rw-r--r--   0        0        0     1844 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json
+-rw-r--r--   0        0        0     4264 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json
+-rw-r--r--   0        0        0     1806 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json
+-rw-r--r--   0        0        0     2523 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json
+-rw-r--r--   0        0        0     2028 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json
+-rw-r--r--   0        0        0   107453 2023-08-03 00:23:13.613620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf
+-rw-r--r--   0        0        0   173006 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf
+-rw-r--r--   0        0        0   107503 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf
+-rw-r--r--   0        0        0   111154 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf
+-rw-r--r--   0        0        0   107645 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf
+-rw-r--r--   0        0        0    30834 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf
+-rw-r--r--   0        0        0    30608 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf
+-rw-r--r--   0        0        0    31147 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf
+-rw-r--r--   0        0        0   107907 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf
+-rw-r--r--   0        0        0   106257 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf
+-rw-r--r--   0        0        0   121496 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf
+-rw-r--r--   0        0        0   106308 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf
+-rw-r--r--   0        0        0     2634 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/resumes/unt_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      481 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0     2607 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/static/__init__.py
+-rw-r--r--   0        0        0     1518 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/static/enumerations.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/__init__.py
+-rw-r--r--   0        0        0     2286 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/application.py
+-rw-r--r--   0        0        0     1750 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/chat.py
+-rw-r--r--   0        0        0     1027 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/company.py
+-rw-r--r--   0        0        0      408 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/job.py
+-rw-r--r--   0        0        0     1843 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/recruiter.py
+-rw-r--r--   0        0        0      645 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/recruiter_invitation.py
+-rw-r--r--   0        0        0     1720 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/scheduled_events.py
+-rw-r--r--   0        0        0     2579 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/test_support/fixtures/users.py
+-rw-r--r--   0        0        0     1453 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/algolia/__init__.py
+-rw-r--r--   0        0        0      468 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/algolia/client_factory.py
+-rw-r--r--   0        0        0     2359 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/algolia/mock.py
+-rw-r--r--   0        0        0      758 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     2352 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0     2139 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/client.py
+-rw-r--r--   0        0        0      340 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/client_factory.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     2427 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0     1735 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/companies/unit_of_work.py
+-rw-r--r--   0        0        0     2553 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/mock.py
+-rw-r--r--   0        0        0      413 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2057 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1588 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2385 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     2318 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1353 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     2702 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firebase_storage/__init__.py
+-rw-r--r--   0        0        0      846 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firebase_storage/client_factory.py
+-rw-r--r--   0        0        0      953 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firebase_storage/mock.py
+-rw-r--r--   0        0        0     1727 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firebase_storage/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firestore/__init__.py
+-rw-r--r--   0        0        0      749 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firestore/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firestore/helpers.py
+-rw-r--r--   0        0        0      507 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firestore/mock.py
+-rw-r--r--   0        0        0     1975 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firestore/models.py
+-rw-r--r--   0        0        0     9200 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/firestore/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      725 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0     1369 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/kafka/client_factory.py
+-rw-r--r--   0        0        0      320 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0      716 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     2178 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0     1517 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/mailgun/__init__.py
+-rw-r--r--   0        0        0      989 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/mailgun/client_factory.py
+-rw-r--r--   0        0        0      282 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/mailgun/mock.py
+-rw-r--r--   0        0        0     1231 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/mailgun/repository.py
+-rw-r--r--   0        0        0      104 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/mailgun/templates/chat_message.html
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/openai/__init__.py
+-rw-r--r--   0        0        0      447 2023-08-03 00:23:13.617620 getajob-0.6.0/getajob/vendor/openai/client_factory.py
+-rw-r--r--   0        0        0      521 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/openai/mock.py
+-rw-r--r--   0        0        0     1185 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/openai/repository.py
+-rw-r--r--   0        0        0      572 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/openai/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/redis/__init__.py
+-rw-r--r--   0        0        0      508 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/redis/client_factory.py
+-rw-r--r--   0        0        0      343 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/redis/mock.py
+-rw-r--r--   0        0        0     2463 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/redis/repository.py
+-rw-r--r--   0        0        0      251 2023-08-03 00:23:13.621620 getajob-0.6.0/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1786 2023-08-03 00:23:13.621620 getajob-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 getajob-0.6.0/PKG-INFO
```

### Comparing `getajob-0.5.1/LICENSE` & `getajob-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/abstractions/models.py` & `getajob-0.6.0/getajob/abstractions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 @dataclass
 class EntityModels:
     entity: DataSchema
     create: t.Optional[DataSchema] = None
     update: t.Optional[DataSchema] = None
 
 
+class BaseFileModel(BaseModel):
+    file_type: str
+
+
 class BaseDataModel(BaseModel):
     id: str
     created: datetime
     updated: datetime
 
 
 @dataclass
```

### Comparing `getajob-0.5.1/getajob/abstractions/repository.py` & `getajob-0.6.0/getajob/abstractions/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 from datetime import datetime
 from functools import wraps
 from pydantic import BaseModel
 
 from getajob.abstractions.models import BaseDataModel
-from getajob.utils import generate_random_short_code, get_value_from_enum
+from getajob.utils import generate_random_short_code, get_value_from_enum, update_dict
 from getajob.exceptions import (
     KafkaEventTopicNotProvidedError,
     EntityNotFound,
     MissingParentKeyError,
 )
 from getajob.vendor.firestore.models import (
     FirestoreDocument,
@@ -158,16 +158,16 @@
         object_id: str,
         parent_collections: dict = {},
         data: dict | None = None,
     ):
         if not self.kafka or not self.kafka_event_config:
             return
         event_enum = get_value_from_enum(
-            value=event_type.value, 
-            enumeration=self.kafka_event_config.message_type_enum
+            value=event_type.value,
+            enumeration=self.kafka_event_config.message_type_enum,
         )
         if not event_enum:
             return
         self.kafka.publish(
             topic=self.kafka_event_config.topic,
             message=BaseKafkaMessage(
                 message_type=event_enum.value,
@@ -235,23 +235,21 @@
     def update(
         self,
         doc_id: str,
         data: BaseModel,
         parent_collections: dict = {},
     ) -> BaseDataModel:
         original_item = self.get(doc_id, parent_collections, True).dict()
-        for key, val in data.dict().items():
-            if val is not None:
-                original_item[key] = val
-        original_item["updated"] = datetime.now()
+        updated_item = update_dict(original_item, data.dict())
+        updated_item["updated"] = datetime.now()
         res = self.db.update(
-            parent_collections, self.collection_name, doc_id, original_item
+            parent_collections, self.collection_name, doc_id, updated_item
         )
         self._produce_repository_kafka_event(
-            KafkaEventType.update, doc_id, parent_collections, original_item
+            KafkaEventType.update, doc_id, parent_collections, updated_item
         )
         return format_to_schema(res, self.entity_models.entity)
 
     @ensure_parent_keys
     def delete(
         self,
         doc_id: str,
```

### Comparing `getajob-0.5.1/getajob/config/settings.py` & `getajob-0.6.0/getajob/config/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class AppSettings:
     # General
     APP_VERSION: str = os.getenv("APP_VERSION", "0.0.0")
 
     # Firebase config
+    FIRESTORE_APP_NAME: str = "getajob"
     FIRESTORE_JSON_CONFIG: str = os.getenv("FIRESTORE_JSON_CONFIG", "")
     FIREBASE_FILE_STORAGE_BUCKET: str = os.getenv("FIREBASE_FILE_STORAGE_BUCKET", "")
 
     # Openai config
     OPENAI_API_KEY: str = os.getenv("OPENAI_API_KEY", "")
     OPENAI_MOCK_RESPONSES: str = os.getenv("OPENAI_MOCK_RESPONSES", "false")
     OPENAI_MODEL_ABILITY: int = 1
```

### Comparing `getajob-0.5.1/getajob/contexts/admin/search/repository.py` & `getajob-0.6.0/getajob/contexts/admin/search/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/admin/users/models.py` & `getajob-0.6.0/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/admin/users/repository.py` & `getajob-0.6.0/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/applications/applicant_tracking/models.py` & `getajob-0.6.0/getajob/contexts/applications/applicant_tracking/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/applications/applicant_tracking/repository.py` & `getajob-0.6.0/getajob/contexts/applications/applicant_tracking/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     entity=ATSDetails,
 )
 
 
 class ATSRepository(SingleChildRepository):
     def __init__(
         self,
+        *,
         request_scope: UserAndDatabaseConnection,
-        kafka: KafkaProducerRepository | None = None,
+        kafka: KafkaProducerRepository | None,
     ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.applications, message_type_enum=KafkaApplicationATSEnum
         )
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
```

### Comparing `getajob-0.5.1/getajob/contexts/applications/repository.py` & `getajob-0.6.0/getajob/contexts/applications/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-import typing as t
-
 from getajob.abstractions.models import Entity
 from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.vendor.firestore.models import FirestoreFilters
+from getajob.vendor.firebase_storage.repository import FirebaseStorageRepository
 from getajob.abstractions.models import UserAndDatabaseConnection
 from getajob.vendor.kafka.repository import KafkaProducerRepository
 from getajob.vendor.kafka.models import (
     KafkaEventConfig,
     KafkaTopic,
     KafkaApplicationsEnum,
 )
 from getajob.contexts.users.resumes.repository import ResumeRepository
 from getajob.contexts.companies.jobs.repository import JobsRepository
 from getajob.contexts.applications.applicant_tracking.repository import ATSRepository
 
-from .models import entity_models, UserCreatedApplication
+from .models import (
+    entity_models,
+    UserCreatedApplication,
+)
 from .unit_of_work import ApplicationsUnitOfWork
 
 
 class ApplicationRepository(ParentRepository):
     def __init__(
         self,
+        *,
         request_scope: UserAndDatabaseConnection,
-        kafka: t.Optional[KafkaProducerRepository] = None,
+        kafka: KafkaProducerRepository | None,
     ):
         self.request_scope = request_scope
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.applications, message_type_enum=KafkaApplicationsEnum
         )
         super().__init__(
             RepositoryDependencies(
@@ -40,17 +43,19 @@
         )
 
     def user_creates_application(
         self, user_id: str, application: UserCreatedApplication
     ):
         return ApplicationsUnitOfWork(self).user_creates_application(
             user_id=user_id,
-            resume_repo=ResumeRepository(self.request_scope),
-            job_repo=JobsRepository(self.request_scope),
-            applicant_tracking_repo=ATSRepository(self.request_scope),
+            resume_repo=ResumeRepository(request_scope=self.request_scope),
+            job_repo=JobsRepository(request_scope=self.request_scope, kafka=None),
+            applicant_tracking_repo=ATSRepository(
+                request_scope=self.request_scope, kafka=None
+            ),
             create_application=application,
         )
 
     def get_applications_by_company(self, company_id: str):
         return super().query(
             filters=[
                 FirestoreFilters(field="company_id", operator="==", value=company_id),
```

### Comparing `getajob-0.5.1/getajob/contexts/applications/unit_of_work.py` & `getajob-0.6.0/getajob/contexts/applications/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/chat/message/models.py` & `getajob-0.6.0/getajob/contexts/chat/message/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/chat/message/repository.py` & `getajob-0.6.0/getajob/contexts/chat/message/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 entity_models = EntityModels(
     entity=ChatMessage, create=UserCreateChatMessage, update=UpdateChatMessage
 )
 
 
 class ChatMessageRepository(MultipleChildrenRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.CHAT_MESSAGES.value,
                 entity_models=entity_models,
             ),
```

### Comparing `getajob-0.5.1/getajob/contexts/chat/repository.py` & `getajob-0.6.0/getajob/contexts/chat/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,30 +13,34 @@
 from .unit_of_work import CreateChatUnitOfWork
 
 
 entity_models = EntityModels(entity=Chat, create=UserCreateChat)
 
 
 class ChatRepository(ParentRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.CHAT.value,
                 entity_models=entity_models,
             )
         )
         self.request_scope = request_scope
 
     def create_new_chat(self, create_chat: UserCreateChat):
         return CreateChatUnitOfWork(
-            application_repository=ApplicationRepository(self.request_scope),
-            recruiter_repository=RecruiterRepository(self.request_scope),
-            user_repository=UserRepository(self.request_scope),
+            application_repository=ApplicationRepository(
+                request_scope=self.request_scope, kafka=None
+            ),
+            recruiter_repository=RecruiterRepository(request_scope=self.request_scope),
+            user_repository=UserRepository(
+                request_scope=self.request_scope, kafka=None
+            ),
             chat_repository=self,
         ).create_new_chat(create_chat)
 
     def get_all_chats_user_is_part_of(self, user_id: str, is_recruiter: bool = False):
         query_field = "recruiter_user_id" if is_recruiter else "applicant_user_id"
         return self.query(
             filters=[FirestoreFilters(field=query_field, operator="==", value=user_id)]
```

### Comparing `getajob-0.5.1/getajob/contexts/chat/unit_of_work.py` & `getajob-0.6.0/getajob/contexts/chat/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/companies/applicant_tracking_settings/repository.py` & `getajob-0.6.0/getajob/contexts/companies/applicant_tracking_settings/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     create=SetATSConfig,
     update=SetATSConfig,
     entity=ATSConfig,
 )
 
 
 class CompanyATSConfigRepository(SingleChildRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.COMPANY_ATS_CONFIG.value,
                 entity_models=entity_models,
             ),
```

### Comparing `getajob-0.5.1/getajob/contexts/companies/audit/repository.py` & `getajob-0.6.0/getajob/contexts/companies/audit/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from .models import CreateAuditLog, AuditLog
 
 entity_models = EntityModels(create=CreateAuditLog, entity=AuditLog)
 
 
 class AuditLogRepository(MultipleChildrenRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.COMPANY_AUDITS.value,
                 entity_models=entity_models,
             ),
```

### Comparing `getajob-0.5.1/getajob/contexts/companies/details/models.py` & `getajob-0.6.0/getajob/contexts/companies/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/companies/details/repository.py` & `getajob-0.6.0/getajob/contexts/companies/details/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,18 @@
     entity=CompanyDetails,
 )
 
 
 class CompanyDetailsRepository(SingleChildRepository):
     def __init__(
         self,
+        *,
         request_scope: UserAndDatabaseConnection,
-        redis: RedisRepository | None = None,
-        kafka: KafkaProducerRepository | None = None,
+        redis: RedisRepository | None,
+        kafka: KafkaProducerRepository | None,
     ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.companies, message_type_enum=KafkaCompanyDetailsEnum
         )
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
```

### Comparing `getajob-0.5.1/getajob/contexts/companies/enumerations.py` & `getajob-0.6.0/getajob/contexts/companies/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/companies/invitations/repository.py` & `getajob-0.6.0/getajob/contexts/companies/invitations/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .models import RecruiterInvitation
 
 entity_models = EntityModels(entity=RecruiterInvitation)
 
 
 class RecruiterInvitationsRepository(MultipleChildrenRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.RECRUITER_INVITATIONS.value,
                 entity_models=entity_models,
             ),
```

### Comparing `getajob-0.5.1/getajob/contexts/companies/jobs/models.py` & `getajob-0.6.0/getajob/contexts/companies/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/companies/jobs/repository.py` & `getajob-0.6.0/getajob/contexts/companies/jobs/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 entity_models = EntityModels(entity=Job, create=CreateJob, update=UpdateJob)
 
 
 class JobsRepository(MultipleChildrenRepository):
     def __init__(
         self,
+        *,
         request_scope: UserAndDatabaseConnection,
-        kafka: t.Optional[KafkaProducerRepository] = None,
+        kafka: KafkaProducerRepository | None,
     ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.jobs, message_type_enum=KafkaJobsEnum
         )
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
```

### Comparing `getajob-0.5.1/getajob/contexts/companies/jobs/unit_of_work.py` & `getajob-0.6.0/getajob/contexts/companies/jobs/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/companies/recruiters/repository.py` & `getajob-0.6.0/getajob/contexts/companies/recruiters/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .models import Recruiter
 
 entity_models = EntityModels(entity=Recruiter)
 
 
 class RecruiterRepository(MultipleChildrenRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.RECRUITERS.value,
                 entity_models=entity_models,
             ),
```

### Comparing `getajob-0.5.1/getajob/contexts/companies/repository.py` & `getajob-0.6.0/getajob/contexts/companies/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 entity_models = EntityModels(entity=Company)
 
 
 class CompanyRepository(ParentRepository):
     def __init__(
         self,
+        *,
         request_scope: UserAndDatabaseConnection,
-        kafka: KafkaProducerRepository | None = None,
+        kafka: KafkaProducerRepository | None,
     ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.companies, message_type_enum=KafkaCompanyEnum
         )
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
```

### Comparing `getajob-0.5.1/getajob/contexts/scheduled_events/models.py` & `getajob-0.6.0/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/scheduled_events/repository.py` & `getajob-0.6.0/getajob/contexts/scheduled_events/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     entity=ScheduledEvent,
     create=CreateScheduledEvent,
     update=UpdateScheduledEvent,
 )
 
 
 class ScheduledEventsRepository(ParentRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.SCHEDULED_EVENTS.value,
                 entity_models=entity_models,
             )
```

### Comparing `getajob-0.5.1/getajob/contexts/search/models.py` & `getajob-0.6.0/getajob/contexts/search/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.6.0/getajob/contexts/users/cover_letters/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     entity=CoverLetter,
     create=CreateCoverLetter,
     update=UpdateCoverLetter,
 )
 
 
 class CoverLetterRepository(MultipleChildrenRepository):
-    def __init__(self, request_scope: UserAndDatabaseConnection):
+    def __init__(self, *, request_scope: UserAndDatabaseConnection):
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.COVER_LETTERS.value,
                 entity_models=entity_models,
             ),
```

### Comparing `getajob-0.5.1/getajob/contexts/users/details/models.py` & `getajob-0.6.0/getajob/contexts/users/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/users/details/repository.py` & `getajob-0.6.0/getajob/contexts/users/details/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     update=SetUserDetails,
 )
 
 
 class UserDetailsRepository(SingleChildRepository):
     def __init__(
         self,
+        *,
         request_scope: UserAndDatabaseConnection,
-        redis: RedisRepository | None = None,
-        kafka: KafkaProducerRepository | None = None,
+        redis: RedisRepository | None,
+        kafka: KafkaProducerRepository | None,
     ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.users, message_type_enum=KafkaUsersDetailsEnum
         )
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
```

### Comparing `getajob-0.5.1/getajob/contexts/users/enumerations.py` & `getajob-0.6.0/getajob/contexts/users/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/contexts/users/repository.py` & `getajob-0.6.0/getajob/contexts/users/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 entity_models = EntityModels(entity=User)
 
 
 class UserRepository(ParentRepository):
     def __init__(
         self,
+        *,
         request_scope: UserAndDatabaseConnection,
-        kafka: KafkaProducerRepository | None = None,
+        kafka: KafkaProducerRepository | None,
     ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.users, message_type_enum=KafkaUsersEnum
         )
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
```

### Comparing `getajob-0.5.1/getajob/exceptions.py` & `getajob-0.6.0/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/static/enumerations.py` & `getajob-0.6.0/getajob/static/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/test_support/fixtures/chat.py` & `getajob-0.6.0/getajob/test_support/fixtures/chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def create_chat_with_dependencies(request_scope):
         application_and_dependencies = (
             ApplicationFixture.create_application_with_dependencies(request_scope)
         )
         recruiter = cast(
             Recruiter, RecruiterFixture.create_recruiter_from_webhook(request_scope)
         )
-        repo = ChatRepository(request_scope)
+        repo = ChatRepository(request_scope=request_scope)
         new_chat = repo.create_new_chat(
             UserCreateChat(
                 applicant_user_id=application_and_dependencies.application.user_id,
                 recruiter_user_id=recruiter.user_id,
                 application_id=application_and_dependencies.application.id,
                 company_id=application_and_dependencies.company.id,
             )
@@ -36,8 +36,9 @@
         return ChatWithDependencies(
             chat_id=new_chat.id,
             recruiter_id=recruiter.id,
             application=application_and_dependencies.application,
             company=application_and_dependencies.company,
             job=application_and_dependencies.job,
             resume=application_and_dependencies.resume,
+            user=application_and_dependencies.user,
         )
```

### Comparing `getajob-0.5.1/getajob/test_support/fixtures/company.py` & `getajob-0.6.0/getajob/test_support/fixtures/company.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/test_support/fixtures/recruiter.py` & `getajob-0.6.0/getajob/test_support/fixtures/recruiter.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/test_support/fixtures/recruiter_invitation.py` & `getajob-0.6.0/getajob/test_support/fixtures/recruiter_invitation.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/test_support/fixtures/scheduled_events.py` & `getajob-0.6.0/getajob/test_support/fixtures/scheduled_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,11 +34,11 @@
             name="Test Event 3",
             description="Test Description 3",
             cron="* * * * *",
             event_category=ScheduledEventCategory.REPORT,
             event_type=ReportScheduledEvent.APPLICANT_SUMMARY,
             next_run_time=datetime.utcnow() + timedelta(days=1),
         )
-        repo = ScheduledEventsRepository(request_scope)
+        repo = ScheduledEventsRepository(request_scope=request_scope)
         repo.create(event_1)
         repo.create(event_2)
         repo.create(event_3)
```

### Comparing `getajob-0.5.1/getajob/test_support/fixtures/users.py` & `getajob-0.6.0/getajob/test_support/fixtures/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,13 +48,19 @@
             "type": "user.created",
         }
         user = ClerkUserWebhookEvent(**data)
         repo = WebhookUserRepository(request_scope)
         return repo.create_user(user)
 
     @staticmethod
-    def create_user_resume(request_scope, user_id: str):
-        repo = ResumeRepository(request_scope)
+    def create_user_resume(
+        request_scope,
+        user_id: str,
+    ):
+        repo = ResumeRepository(request_scope=request_scope)
         return repo.create(
-            data=CreateResume(resume="nice resume"),
+            data=CreateResume(
+                resume_url="https://www.resumes.com",
+                remote_file_path="users/resume/abc",
+            ),
             parent_collections={Entity.USERS.value: user_id},
         )
```

### Comparing `getajob-0.5.1/getajob/vendor/algolia/models.py` & `getajob-0.6.0/getajob/vendor/algolia/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/client.py` & `getajob-0.6.0/getajob/vendor/clerk/client.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/companies/models.py` & `getajob-0.6.0/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/companies/repository.py` & `getajob-0.6.0/getajob/vendor/clerk/companies/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from .models import (
     ClerkCompanyWebhookEvent,
     ClerkCompany,
     ClerkCompanyDeleted,
     ClerkCompanyWebhookType,
 )
+from .unit_of_work import ClerkCompanyUnitOfWork
 
 entity_models = EntityModels(entity=ClerkCompany)
 
 
 class WebhookCompanyRepository(ParentRepository):
     def __init__(
         self,
@@ -42,25 +43,18 @@
         event_dict = {
             ClerkCompanyWebhookType.organization_created: self.create_company,
             ClerkCompanyWebhookType.organization_updated: self.update_company,
             ClerkCompanyWebhookType.organization_deleted: self.delete_company,
         }
         return event_dict[event.type](event)
 
-    def _create_default_company_details(self, company_id: str):
-        CompanyDetailsRepository(self.request_scope).set_sub_entity(
-            data=SetCompanyDetails(),
-            parent_collections={Entity.COMPANIES.value: company_id},
-        )
-
     def create_company(self, event: ClerkCompanyWebhookEvent):
-        create_event = ClerkCompany(**event.data)
-        res = self.create(data=create_event, provided_id=create_event.id)
-        self._create_default_company_details(company_id=create_event.id)
-        return res
+        return ClerkCompanyUnitOfWork(
+            request_scope=self.request_scope
+        ).create_new_company(webhook_repository=self, event=event)
 
     def delete_company(self, event: ClerkCompanyWebhookEvent):
         delete_event = ClerkCompanyDeleted(**event.data)
         return self.delete(doc_id=delete_event.id)
 
     def update_company(self, event: ClerkCompanyWebhookEvent):
         update_event = ClerkCompany(**event.data)
```

### Comparing `getajob-0.5.1/getajob/vendor/clerk/mock.py` & `getajob-0.6.0/getajob/vendor/clerk/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.6.0/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.6.0/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 
 entity_models = EntityModels(entity=ClerkCompanyInvitation)
 
 
 class WebhookCompanyInvitationRepository:
     def __init__(self, request_scope: UserAndDatabaseConnection):
-        self.repo = RecruiterInvitationsRepository(request_scope)
+        self.repo = RecruiterInvitationsRepository(request_scope=request_scope)
 
     def handle_webhook_event(self, event: ClerkCompanyInvitationsWebhookEvent):
         event_dict = {
             ClerkCompanyInvitationsWebhookType.organization_invitation_created: self.create_invitation,
             ClerkCompanyInvitationsWebhookType.organization_invitation_revoked: self.revoke_invitation,
             ClerkCompanyInvitationsWebhookType.organization_invitation_accepted: self.accept_invitation,
         }
```

### Comparing `getajob-0.5.1/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.6.0/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.6.0/getajob/vendor/clerk/recruiters/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 
 entity_models = EntityModels(entity=ClerkCompanyMember)
 
 
 class WebhookCompanyMembershipRepository:
     def __init__(self, request_scope: UserAndDatabaseConnection):
-        self.repo = RecruiterRepository(request_scope)
+        self.repo = RecruiterRepository(request_scope=request_scope)
 
     def handle_webhook_event(self, event: ClerkCompanyMembershipWebhookEvent):
         event_dict = {
             ClerkCompanyMembershipWebhookType.organization_membership_created: self.create_recruiter,
             ClerkCompanyMembershipWebhookType.organization_membership_updated: self.update_recruiter,
             ClerkCompanyMembershipWebhookType.organization_membership_deleted: self.delete_recruiter,
         }
```

### Comparing `getajob-0.5.1/getajob/vendor/clerk/repository.py` & `getajob-0.6.0/getajob/vendor/clerk/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/users/models.py` & `getajob-0.6.0/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/clerk/users/repository.py` & `getajob-0.6.0/getajob/vendor/clerk/users/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
             ClerkUserWebhookType.user_created: self.create_user,
             ClerkUserWebhookType.user_updated: self.update_user,
             ClerkUserWebhookType.user_deleted: self.delete_user,
         }
         return event_dict[event.type](event)
 
     def _create_default_user_details(self, user_id: str):
-        UserDetailsRepository(self.request_scope).set_sub_entity(
+        UserDetailsRepository(
+            request_scope=self.request_scope, kafka=None, redis=None
+        ).set_sub_entity(
             data=SetUserDetails(),
             parent_collections={Entity.USERS.value: user_id},
         )
 
     def create_user(self, event: ClerkUserWebhookEvent):
         create_event = ClerkUser(**event.data)
         res = self.create(data=create_event, provided_id=create_event.id)
```

### Comparing `getajob-0.5.1/getajob/vendor/firebase_storage/client_factory.py` & `getajob-0.6.0/getajob/vendor/firebase_storage/client_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import json
 import firebase_admin
-from firebase_admin import credentials, firestore
+from firebase_admin import credentials
+from firebase_admin import storage
 
 from getajob.abstractions.vendor_client_factory import VendorClientFactory
 from getajob.config.settings import SETTINGS
 
 from .mock import MockFirebaseStorageClient
 
 
 class FirebaseStorageClientFactory(VendorClientFactory):
     @staticmethod
     def _return_mock():
         return MockFirebaseStorageClient()
 
     @staticmethod
     def _return_client():
-        cred = credentials.Certificate(json.loads(SETTINGS.FIRESTORE_JSON_CONFIG))
-        firebase_admin.initialize_app(
-            cred, {"storageBucket": SETTINGS.FIREBASE_FILE_STORAGE_BUCKET}
+        if len(firebase_admin._apps) == 0:
+            cred = credentials.Certificate(json.loads(SETTINGS.FIRESTORE_JSON_CONFIG))
+            firebase_admin.initialize_app(cred, name=SETTINGS.FIRESTORE_APP_NAME)
+        return storage.bucket(
+            name=SETTINGS.FIREBASE_FILE_STORAGE_BUCKET,
+            app=firebase_admin.get_app(name=SETTINGS.FIRESTORE_APP_NAME),
         )
-        return firestore.client()
```

### Comparing `getajob-0.5.1/getajob/vendor/firebase_storage/helpers.py` & `getajob-0.6.0/getajob/vendor/firestore/helpers.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/firebase_storage/models.py` & `getajob-0.6.0/getajob/vendor/firestore/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/firebase_storage/repository.py` & `getajob-0.6.0/getajob/vendor/firebase_storage/repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,50 @@
-from google.cloud.firestore_v1.client import Client
-
-from firebase_admin import storage
+from google.cloud.storage import Bucket
 
 from .client_factory import FirebaseStorageClientFactory
 
 
 class FirebaseStorageRepository:
-    def __init__(self, client: Client = FirebaseStorageClientFactory.get_client()):
+    def __init__(self, client: Bucket = FirebaseStorageClientFactory.get_client()):
         self._client = client
-        self._bucket = storage.bucket(app=self._client)
 
-    def upload_bytes(self, file_bytes: bytes, remote_file_path: str) -> str:
-        blob = self._bucket.blob(remote_file_path)
-        blob.upload_from_string(file_bytes)
+    def upload_bytes(
+        self,
+        file_bytes: bytes,
+        content_type: str,
+        remote_file_path: str,
+        publicly_accessible: bool = False,
+    ) -> str:
+        blob = self._client.blob(remote_file_path)
+        blob.upload_from_string(data=file_bytes, content_type=content_type)
+        if publicly_accessible:
+            blob.make_public()
         return blob.public_url
 
-    def upload_file(self, local_file_path, remote_file_path) -> str:
-        blob = self._bucket.blob(remote_file_path)
-        blob.upload_from_filename(local_file_path)
+    # def upload_file(self, local_file_path, remote_file_path, publicly_accessible: bool = False) -> str:
+    #     blob = self._client.blob(remote_file_path)
+    #     blob.upload_from_filename(local_file_path)
+    #     if publicly_accessible:
+    #         blob.make_public()
+    #     return blob.public_url
+
+    def update_file_public_access(
+        self, remote_file_path, publicly_accessible: bool = False
+    ) -> str:
+        blob = self._client.blob(remote_file_path)
+        if publicly_accessible:
+            blob.make_public()
+        else:
+            blob.make_private()
         return blob.public_url
 
-    def download_to_file(self, remote_file_path, local_file_path) -> None:
-        blob = self._bucket.blob(remote_file_path)
-        blob.download_to_filename(local_file_path)
+    # def download_to_file(self, remote_file_path, local_file_path) -> None:
+    #     blob = self._client.blob(remote_file_path)
+    #     blob.download_to_filename(local_file_path)
 
     def get_file_bytes(self, remote_file_path) -> bytes:
-        blob = self._bucket.blob(remote_file_path)
+        blob = self._client.blob(remote_file_path)
         return blob.download_as_bytes()
 
     def delete_file(self, remote_file_path) -> None:
-        blob = self._bucket.blob(remote_file_path)
+        blob = self._client.blob(remote_file_path)
         blob.delete()
```

### Comparing `getajob-0.5.1/getajob/vendor/firestore/repository.py` & `getajob-0.6.0/getajob/vendor/firestore/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/kafka/authentication.py` & `getajob-0.6.0/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/kafka/client_factory.py` & `getajob-0.6.0/getajob/vendor/kafka/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/kafka/mock.py` & `getajob-0.6.0/getajob/vendor/kafka/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/kafka/models.py` & `getajob-0.6.0/getajob/vendor/kafka/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 
 
 class KafkaUsersDetailsEnum(str, Enum):
     update = "update_user_details"
     get = "get_user_details"
 
 
+class KafkaUserResumeExtraction(str, Enum):
+    update = "update_user_resume_extraction"
+
+
 class KafkaJobsEnum(str, Enum):
     create = "create_job"
     update = "update_job"
     delete = "delete_job"
     get = "get_job"
```

### Comparing `getajob-0.5.1/getajob/vendor/kafka/repository.py` & `getajob-0.6.0/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/mailgun/client_factory.py` & `getajob-0.6.0/getajob/vendor/mailgun/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/mailgun/repository.py` & `getajob-0.6.0/getajob/vendor/mailgun/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.5.1/getajob/vendor/openai/settings.py` & `getajob-0.6.0/getajob/vendor/openai/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,8 +9,8 @@
     MODEL_ABILITY: int = int(SETTINGS.OPENAI_MODEL_ABILITY)
     TEMPERATURE: float = 0.5
     TOP_P: float = 1.0
     FREQUENCY_PENALTY: float = 0.8
     PRESENCE_PENALTY: float = 0.0
 
     MODEL_ABILITY_DICT: dict = {1: "text-curie-001", 2: "gpt-3.5-turbo", 3: "gpt-4"}
-    MODEL: str = MODEL_ABILITY_DICT[MODEL_ABILITY]
+    MODEL: str = "gpt-3.5-turbo"
```

### Comparing `getajob-0.5.1/getajob/vendor/redis/repository.py` & `getajob-0.6.0/getajob/vendor/redis/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 from typing import Type
 from pydantic import BaseModel
 from redis import Redis
 
-from .client_factory import RedisFactory
+from .client_factory import RedisClientFactory
 
 
 class RedisRepository:
-    def __init__(self, client: Redis = RedisFactory.get_client()):
+    def __init__(self, client: Redis = RedisClientFactory.get_client()):
         self.client = client
 
     def _get_cached_id(
         self, entity_type: str, entity_id: str, parent_collections: dict
     ) -> str:
         redis_key = ""
         for key, val in parent_collections.items():
```

### Comparing `getajob-0.5.1/pyproject.toml` & `getajob-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.5.1"
+version = "0.6.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.5.1/PKG-INFO` & `getajob-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.5.1
+Version: 0.6.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

