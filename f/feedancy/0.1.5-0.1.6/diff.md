# Comparing `tmp/feedancy-0.1.5.tar.gz` & `tmp/feedancy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.1.5.tar", max compression
+gzip compressed data, was "feedancy-0.1.6.tar", max compression
```

## Comparing `feedancy-0.1.5.tar` & `feedancy-0.1.6.tar`

### file list

```diff
@@ -1,139 +1,140 @@
--rw-r--r--   0        0        0      615 2023-08-01 19:37:20.963096 feedancy-0.1.5/README.md
--rw-r--r--   0        0        0      126 2023-08-01 19:37:20.955097 feedancy-0.1.5/feedancy/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 19:37:20.875106 feedancy-0.1.5/feedancy/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 19:37:20.875106 feedancy-0.1.5/feedancy/apis/api/__init__.py
--rw-r--r--   0        0        0    13072 2023-08-01 19:37:20.879106 feedancy-0.1.5/feedancy/apis/api/api.py
--rw-r--r--   0        0        0      896 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      820 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      853 2023-08-01 19:37:20.891104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      908 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      863 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      810 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      830 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      885 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      917 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0     1258 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      813 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0     1222 2023-08-01 19:37:20.895104 feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0     1277 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0     1312 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      899 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      817 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      859 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-08-01 19:37:20.899103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      935 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      813 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      899 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      954 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      876 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      813 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      840 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      895 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      930 2023-08-01 19:37:20.903103 feedancy-0.1.5/feedancy/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      881 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      814 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      844 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      899 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      935 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0     1922 2023-08-01 19:37:20.911102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1941 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0     1883 2023-08-01 19:37:20.907103 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1938 2023-08-01 19:37:20.911102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1976 2023-08-01 19:37:20.911102 feedancy-0.1.5/feedancy/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      917 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      820 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      874 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      929 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      935 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      823 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      889 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      944 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-08-01 19:37:20.915102 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      923 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      821 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      879 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      934 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      977 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0     1627 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      814 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0     1590 2023-08-01 19:37:20.919101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0     1645 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0     1681 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      874 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      812 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      839 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      894 2023-08-01 19:37:20.923101 feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      928 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      969 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      812 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      953 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0     1008 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0     1023 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      966 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      827 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      916 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      971 2023-08-01 19:37:20.927100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0     1020 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      896 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      820 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      890 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      945 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      851 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      811 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      817 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      872 2023-08-01 19:37:20.931100 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      905 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      856 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      812 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      821 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      876 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      910 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      886 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      818 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      845 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      900 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      940 2023-08-01 19:37:20.935099 feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2092 2023-08-01 19:37:20.943098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2169 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3217 2023-08-01 19:37:20.939099 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2166 2023-08-01 19:37:20.943098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2146 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      899 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      817 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      859 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-08-01 19:37:20.947098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0      917 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      820 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      874 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0      929 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      905 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      818 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      864 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      919 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      959 2023-08-01 19:37:20.951098 feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      658 2023-08-01 19:37:20.955097 feedancy-0.1.5/feedancy/client.py
--rw-r--r--   0        0        0        0 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/__init__.py
--rw-r--r--   0        0        0     2818 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/aiohttp.py
--rw-r--r--   0        0        0      235 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/base.py
--rw-r--r--   0        0        0     2680 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/httpx.py
--rw-r--r--   0        0        0     2446 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/params_converter.py
--rw-r--r--   0        0        0     3005 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/adapter/requests.py
--rw-r--r--   0        0        0     2769 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/base.py
--rw-r--r--   0        0        0      685 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/client.py
--rw-r--r--   0        0        0      929 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/configuration.py
--rw-r--r--   0        0        0      466 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/exceptions.py
--rw-r--r--   0        0        0      403 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/json.py
--rw-r--r--   0        0        0      613 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/request.py
--rw-r--r--   0        0        0      384 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/response.py
--rw-r--r--   0        0        0      895 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/response_deserializer.py
--rw-r--r--   0        0        0      564 2023-08-01 19:37:20.959097 feedancy-0.1.5/feedancy/lib/types.py
--rw-r--r--   0        0        0      651 2023-08-01 19:36:14.485587 feedancy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 feedancy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      615 2023-08-03 07:41:59.863729 feedancy-0.1.6/README.md
+-rw-r--r--   0        0        0      126 2023-08-03 07:41:59.831135 feedancy-0.1.6/feedancy/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:41:59.572997 feedancy-0.1.6/feedancy/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:41:59.573132 feedancy-0.1.6/feedancy/apis/api/__init__.py
+-rw-r--r--   0        0        0    13072 2023-08-03 07:41:59.579091 feedancy-0.1.6/feedancy/apis/api/api.py
+-rw-r--r--   0        0        0      896 2023-08-03 07:41:59.600981 feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_create.py
+-rw-r--r--   0        0        0      820 2023-08-03 07:41:59.602959 feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_destroy.py
+-rw-r--r--   0        0        0      853 2023-08-03 07:41:59.600152 feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_retrieve.py
+-rw-r--r--   0        0        0      908 2023-08-03 07:41:59.601690 feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-08-03 07:41:59.602414 feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_update.py
+-rw-r--r--   0        0        0      863 2023-08-03 07:41:59.604484 feedancy-0.1.6/feedancy/apis/api/api_v1_city_create.py
+-rw-r--r--   0        0        0      810 2023-08-03 07:41:59.606591 feedancy-0.1.6/feedancy/apis/api/api_v1_city_destroy.py
+-rw-r--r--   0        0        0      830 2023-08-03 07:41:59.603626 feedancy-0.1.6/feedancy/apis/api/api_v1_city_retrieve.py
+-rw-r--r--   0        0        0      885 2023-08-03 07:41:59.605230 feedancy-0.1.6/feedancy/apis/api/api_v1_city_retrieve_2.py
+-rw-r--r--   0        0        0      917 2023-08-03 07:41:59.606027 feedancy-0.1.6/feedancy/apis/api/api_v1_city_update.py
+-rw-r--r--   0        0        0     1258 2023-08-03 07:41:59.608846 feedancy-0.1.6/feedancy/apis/api/api_v1_company_create.py
+-rw-r--r--   0        0        0      813 2023-08-03 07:41:59.612756 feedancy-0.1.6/feedancy/apis/api/api_v1_company_destroy.py
+-rw-r--r--   0        0        0     1222 2023-08-03 07:41:59.607454 feedancy-0.1.6/feedancy/apis/api/api_v1_company_retrieve.py
+-rw-r--r--   0        0        0     1277 2023-08-03 07:41:59.609981 feedancy-0.1.6/feedancy/apis/api/api_v1_company_retrieve_2.py
+-rw-r--r--   0        0        0     1312 2023-08-03 07:41:59.612059 feedancy-0.1.6/feedancy/apis/api/api_v1_company_update.py
+-rw-r--r--   0        0        0      899 2023-08-03 07:41:59.614322 feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_create.py
+-rw-r--r--   0        0        0      817 2023-08-03 07:41:59.617009 feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_destroy.py
+-rw-r--r--   0        0        0      859 2023-08-03 07:41:59.613469 feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_retrieve.py
+-rw-r--r--   0        0        0      914 2023-08-03 07:41:59.615140 feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_retrieve_2.py
+-rw-r--r--   0        0        0      953 2023-08-03 07:41:59.616102 feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_update.py
+-rw-r--r--   0        0        0      935 2023-08-03 07:41:59.619711 feedancy-0.1.6/feedancy/apis/api/api_v1_contact_create.py
+-rw-r--r--   0        0        0      813 2023-08-03 07:41:59.624427 feedancy-0.1.6/feedancy/apis/api/api_v1_contact_destroy.py
+-rw-r--r--   0        0        0      899 2023-08-03 07:41:59.618090 feedancy-0.1.6/feedancy/apis/api/api_v1_contact_retrieve.py
+-rw-r--r--   0        0        0      954 2023-08-03 07:41:59.621307 feedancy-0.1.6/feedancy/apis/api/api_v1_contact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-08-03 07:41:59.623253 feedancy-0.1.6/feedancy/apis/api/api_v1_contact_update.py
+-rw-r--r--   0        0        0      876 2023-08-03 07:41:59.627474 feedancy-0.1.6/feedancy/apis/api/api_v1_country_create.py
+-rw-r--r--   0        0        0      813 2023-08-03 07:41:59.631765 feedancy-0.1.6/feedancy/apis/api/api_v1_country_destroy.py
+-rw-r--r--   0        0        0      840 2023-08-03 07:41:59.625845 feedancy-0.1.6/feedancy/apis/api/api_v1_country_retrieve.py
+-rw-r--r--   0        0        0      895 2023-08-03 07:41:59.629088 feedancy-0.1.6/feedancy/apis/api/api_v1_country_retrieve_2.py
+-rw-r--r--   0        0        0      930 2023-08-03 07:41:59.630696 feedancy-0.1.6/feedancy/apis/api/api_v1_country_update.py
+-rw-r--r--   0        0        0      881 2023-08-03 07:41:59.634652 feedancy-0.1.6/feedancy/apis/api/api_v1_currency_create.py
+-rw-r--r--   0        0        0      814 2023-08-03 07:41:59.638671 feedancy-0.1.6/feedancy/apis/api/api_v1_currency_destroy.py
+-rw-r--r--   0        0        0      844 2023-08-03 07:41:59.633030 feedancy-0.1.6/feedancy/apis/api/api_v1_currency_retrieve.py
+-rw-r--r--   0        0        0      899 2023-08-03 07:41:59.635984 feedancy-0.1.6/feedancy/apis/api/api_v1_currency_retrieve_2.py
+-rw-r--r--   0        0        0      935 2023-08-03 07:41:59.637657 feedancy-0.1.6/feedancy/apis/api/api_v1_currency_update.py
+-rw-r--r--   0        0        0     1922 2023-08-03 07:41:59.645369 feedancy-0.1.6/feedancy/apis/api/api_v1_internship_create.py
+-rw-r--r--   0        0        0     1941 2023-08-03 07:41:59.654733 feedancy-0.1.6/feedancy/apis/api/api_v1_internship_destroy.py
+-rw-r--r--   0        0        0     1883 2023-08-03 07:41:59.640715 feedancy-0.1.6/feedancy/apis/api/api_v1_internship_retrieve.py
+-rw-r--r--   0        0        0     1938 2023-08-03 07:41:59.647745 feedancy-0.1.6/feedancy/apis/api/api_v1_internship_retrieve_2.py
+-rw-r--r--   0        0        0     1976 2023-08-03 07:41:59.652548 feedancy-0.1.6/feedancy/apis/api/api_v1_internship_update.py
+-rw-r--r--   0        0        0      917 2023-08-03 07:41:59.657213 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_create.py
+-rw-r--r--   0        0        0      820 2023-08-03 07:41:59.661522 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_destroy.py
+-rw-r--r--   0        0        0      874 2023-08-03 07:41:59.655884 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_retrieve.py
+-rw-r--r--   0        0        0      929 2023-08-03 07:41:59.658876 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
+-rw-r--r--   0        0        0      971 2023-08-03 07:41:59.660384 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_update.py
+-rw-r--r--   0        0        0      935 2023-08-03 07:41:59.664420 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_create.py
+-rw-r--r--   0        0        0      823 2023-08-03 07:41:59.668681 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_destroy.py
+-rw-r--r--   0        0        0      889 2023-08-03 07:41:59.663034 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
+-rw-r--r--   0        0        0      944 2023-08-03 07:41:59.665749 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-08-03 07:41:59.667471 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_update.py
+-rw-r--r--   0        0        0      923 2023-08-03 07:41:59.671259 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_create.py
+-rw-r--r--   0        0        0      821 2023-08-03 07:41:59.675214 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_destroy.py
+-rw-r--r--   0        0        0      879 2023-08-03 07:41:59.669927 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_retrieve.py
+-rw-r--r--   0        0        0      934 2023-08-03 07:41:59.672526 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
+-rw-r--r--   0        0        0      977 2023-08-03 07:41:59.674135 feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_update.py
+-rw-r--r--   0        0        0     1627 2023-08-03 07:41:59.681471 feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_create.py
+-rw-r--r--   0        0        0      814 2023-08-03 07:41:59.688296 feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_destroy.py
+-rw-r--r--   0        0        0     1590 2023-08-03 07:41:59.677326 feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_retrieve.py
+-rw-r--r--   0        0        0     1645 2023-08-03 07:41:59.683617 feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
+-rw-r--r--   0        0        0     1681 2023-08-03 07:41:59.687263 feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_update.py
+-rw-r--r--   0        0        0      874 2023-08-03 07:41:59.693559 feedancy-0.1.6/feedancy/apis/api/api_v1_region_create.py
+-rw-r--r--   0        0        0      812 2023-08-03 07:41:59.698122 feedancy-0.1.6/feedancy/apis/api/api_v1_region_destroy.py
+-rw-r--r--   0        0        0      839 2023-08-03 07:41:59.689782 feedancy-0.1.6/feedancy/apis/api/api_v1_region_retrieve.py
+-rw-r--r--   0        0        0      894 2023-08-03 07:41:59.695556 feedancy-0.1.6/feedancy/apis/api/api_v1_region_retrieve_2.py
+-rw-r--r--   0        0        0      928 2023-08-03 07:41:59.697173 feedancy-0.1.6/feedancy/apis/api/api_v1_region_update.py
+-rw-r--r--   0        0        0      969 2023-08-03 07:41:59.701812 feedancy-0.1.6/feedancy/apis/api/api_v1_salary_create.py
+-rw-r--r--   0        0        0      812 2023-08-03 07:41:59.709210 feedancy-0.1.6/feedancy/apis/api/api_v1_salary_destroy.py
+-rw-r--r--   0        0        0      953 2023-08-03 07:41:59.699268 feedancy-0.1.6/feedancy/apis/api/api_v1_salary_retrieve.py
+-rw-r--r--   0        0        0     1008 2023-08-03 07:41:59.703806 feedancy-0.1.6/feedancy/apis/api/api_v1_salary_retrieve_2.py
+-rw-r--r--   0        0        0     1023 2023-08-03 07:41:59.708142 feedancy-0.1.6/feedancy/apis/api/api_v1_salary_update.py
+-rw-r--r--   0        0        0      966 2023-08-03 07:41:59.712051 feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
+-rw-r--r--   0        0        0      827 2023-08-03 07:41:59.716191 feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
+-rw-r--r--   0        0        0      916 2023-08-03 07:41:59.710432 feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
+-rw-r--r--   0        0        0      971 2023-08-03 07:41:59.713767 feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0     1020 2023-08-03 07:41:59.715094 feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
+-rw-r--r--   0        0        0      896 2023-08-03 07:41:59.718563 feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_create.py
+-rw-r--r--   0        0        0      820 2023-08-03 07:41:59.721796 feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_destroy.py
+-rw-r--r--   0        0        0      890 2023-08-03 07:41:59.717421 feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
+-rw-r--r--   0        0        0      945 2023-08-03 07:41:59.719614 feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-08-03 07:41:59.720803 feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_update.py
+-rw-r--r--   0        0        0      851 2023-08-03 07:41:59.723965 feedancy-0.1.6/feedancy/apis/api/api_v1_skill_create.py
+-rw-r--r--   0        0        0      811 2023-08-03 07:41:59.730831 feedancy-0.1.6/feedancy/apis/api/api_v1_skill_destroy.py
+-rw-r--r--   0        0        0      817 2023-08-03 07:41:59.722872 feedancy-0.1.6/feedancy/apis/api/api_v1_skill_retrieve.py
+-rw-r--r--   0        0        0      872 2023-08-03 07:41:59.725126 feedancy-0.1.6/feedancy/apis/api/api_v1_skill_retrieve_2.py
+-rw-r--r--   0        0        0      905 2023-08-03 07:41:59.726285 feedancy-0.1.6/feedancy/apis/api/api_v1_skill_update.py
+-rw-r--r--   0        0        0      856 2023-08-03 07:41:59.734121 feedancy-0.1.6/feedancy/apis/api/api_v1_source_create.py
+-rw-r--r--   0        0        0      812 2023-08-03 07:41:59.740413 feedancy-0.1.6/feedancy/apis/api/api_v1_source_destroy.py
+-rw-r--r--   0        0        0      821 2023-08-03 07:41:59.732067 feedancy-0.1.6/feedancy/apis/api/api_v1_source_retrieve.py
+-rw-r--r--   0        0        0      876 2023-08-03 07:41:59.736437 feedancy-0.1.6/feedancy/apis/api/api_v1_source_retrieve_2.py
+-rw-r--r--   0        0        0      910 2023-08-03 07:41:59.738803 feedancy-0.1.6/feedancy/apis/api/api_v1_source_update.py
+-rw-r--r--   0        0        0      886 2023-08-03 07:41:59.744073 feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_create.py
+-rw-r--r--   0        0        0      818 2023-08-03 07:41:59.751066 feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_destroy.py
+-rw-r--r--   0        0        0      845 2023-08-03 07:41:59.741484 feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
+-rw-r--r--   0        0        0      900 2023-08-03 07:41:59.745661 feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      940 2023-08-03 07:41:59.748691 feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_update.py
+-rw-r--r--   0        0        0     2347 2023-08-03 07:41:59.771910 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_create.py
+-rw-r--r--   0        0        0     2437 2023-08-03 07:41:59.790313 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_destroy.py
+-rw-r--r--   0        0        0     3485 2023-08-03 07:41:59.760408 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_list.py
+-rw-r--r--   0        0        0     2434 2023-08-03 07:41:59.777087 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_retrieve.py
+-rw-r--r--   0        0        0     2401 2023-08-03 07:41:59.787216 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_update.py
+-rw-r--r--   0        0        0      899 2023-08-03 07:41:59.792906 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_create.py
+-rw-r--r--   0        0        0      817 2023-08-03 07:41:59.796975 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_destroy.py
+-rw-r--r--   0        0        0      859 2023-08-03 07:41:59.791527 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_retrieve.py
+-rw-r--r--   0        0        0      914 2023-08-03 07:41:59.794135 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
+-rw-r--r--   0        0        0      953 2023-08-03 07:41:59.795606 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_update.py
+-rw-r--r--   0        0        0     1039 2023-08-03 07:41:59.801028 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_create.py
+-rw-r--r--   0        0        0      820 2023-08-03 07:41:59.806113 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_destroy.py
+-rw-r--r--   0        0        0      996 2023-08-03 07:41:59.798640 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
+-rw-r--r--   0        0        0     1051 2023-08-03 07:41:59.802825 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
+-rw-r--r--   0        0        0     1093 2023-08-03 07:41:59.804954 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_update.py
+-rw-r--r--   0        0        0      905 2023-08-03 07:41:59.809986 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_create.py
+-rw-r--r--   0        0        0      818 2023-08-03 07:41:59.814447 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_destroy.py
+-rw-r--r--   0        0        0      864 2023-08-03 07:41:59.807945 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
+-rw-r--r--   0        0        0      919 2023-08-03 07:41:59.811536 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
+-rw-r--r--   0        0        0      959 2023-08-03 07:41:59.813350 feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_update.py
+-rw-r--r--   0        0        0      658 2023-08-03 07:41:59.841441 feedancy-0.1.6/feedancy/client.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:41:59.846893 feedancy-0.1.6/feedancy/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 07:41:59.856406 feedancy-0.1.6/feedancy/lib/adapter/__init__.py
+-rw-r--r--   0        0        0     2818 2023-08-03 07:41:59.854373 feedancy-0.1.6/feedancy/lib/adapter/aiohttp.py
+-rw-r--r--   0        0        0      235 2023-08-03 07:41:59.858975 feedancy-0.1.6/feedancy/lib/adapter/base.py
+-rw-r--r--   0        0        0     2680 2023-08-03 07:41:59.856041 feedancy-0.1.6/feedancy/lib/adapter/httpx.py
+-rw-r--r--   0        0        0     2446 2023-08-03 07:41:59.857253 feedancy-0.1.6/feedancy/lib/adapter/params_converter.py
+-rw-r--r--   0        0        0     3005 2023-08-03 07:41:59.857992 feedancy-0.1.6/feedancy/lib/adapter/requests.py
+-rw-r--r--   0        0        0     2769 2023-08-03 07:41:59.852280 feedancy-0.1.6/feedancy/lib/base.py
+-rw-r--r--   0        0        0      685 2023-08-03 07:41:59.845651 feedancy-0.1.6/feedancy/lib/client.py
+-rw-r--r--   0        0        0      929 2023-08-03 07:41:59.844367 feedancy-0.1.6/feedancy/lib/configuration.py
+-rw-r--r--   0        0        0      466 2023-08-03 07:41:59.849938 feedancy-0.1.6/feedancy/lib/exceptions.py
+-rw-r--r--   0        0        0      403 2023-08-03 07:41:59.851633 feedancy-0.1.6/feedancy/lib/json.py
+-rw-r--r--   0        0        0      613 2023-08-03 07:41:59.846490 feedancy-0.1.6/feedancy/lib/request.py
+-rw-r--r--   0        0        0      384 2023-08-03 07:41:59.848057 feedancy-0.1.6/feedancy/lib/response.py
+-rw-r--r--   0        0        0      895 2023-08-03 07:41:59.850669 feedancy-0.1.6/feedancy/lib/response_deserializer.py
+-rw-r--r--   0        0        0      564 2023-08-03 07:41:59.849036 feedancy-0.1.6/feedancy/lib/types.py
+-rw-r--r--   0        0        0      651 2023-08-03 07:40:26.421208 feedancy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 feedancy-0.1.6/setup.py
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 feedancy-0.1.6/PKG-INFO
```

### Comparing `feedancy-0.1.5/README.md` & `feedancy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api.py` & `feedancy-0.1.6/feedancy/apis/api/api.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_activitysphere_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_activitysphere_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_city_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_city_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_city_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_city_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_city_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_city_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_city_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_city_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_city_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_company_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_company_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_company_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_company_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_company_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_company_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_company_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_company_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_company_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_companycity_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_companycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_contact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_contact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_contact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_contact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_contact_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_contact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_country_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_country_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_country_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_country_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_country_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_country_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_country_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_country_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_country_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_currency_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_currency_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_currency_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_currency_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_currency_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_currency_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internship_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internship_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internship_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internship_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internship_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internship_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcity_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipcontact_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipcontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_internshipskill_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_internshipskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_jobmixin_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_jobmixin_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_region_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_region_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_region_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_region_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_region_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_region_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_region_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_region_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_region_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_salary_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_salary_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_salary_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_salary_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_salary_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_salary_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchandstopkeywords_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_searchkeywords_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_searchkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_skill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_skill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_skill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_skill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_skill_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_skill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_source_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_source_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_source_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_source_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_source_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_source_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_source_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_source_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_source_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_stopkeywords_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_stopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Contact(BaseModel):
+    data: str 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
+
 class Vacancy(BaseModel):
+    contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_retrieve.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,32 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Contact(BaseModel):
+    data: str 
+    id: int 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
+
 class Salary(BaseModel):
     currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 class Vacancy(BaseModel):
     company: str 
+    contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
@@ -46,15 +56,15 @@
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
+        method="GET",
         path="/api/v1/vacancy/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_list.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,32 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Contact(BaseModel):
+    data: str 
+    id: int 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
+
 class Salary(BaseModel):
     currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 class Vacancy(BaseModel):
     company: str 
+    contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_destroy.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,32 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Contact(BaseModel):
+    data: str 
+    id: int 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
+
 class Salary(BaseModel):
     currency: str 
     id: int 
     max_value: typing.Optional[typing.Union[int, None]]  = None
     min_value: typing.Optional[typing.Union[int, None]]  = None
 
 class Vacancy(BaseModel):
     company: str 
+    contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
@@ -46,15 +56,15 @@
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
+        method="DELETE",
         path="/api/v1/vacancy/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancy_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancy_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Contact(BaseModel):
+    data: str 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
+
 class Vacancy(BaseModel):
+    contacts: typing.Union[typing.List[VacancyContact], None] 
     contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
     has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycity_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Contact(BaseModel):
+    data: str 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
 class VacancyContact(BaseModel):
-    contact: int 
-    vacancy: int 
+    contact: typing.Union[Contact, None] 
 
 def make_request(self: BaseApi,
 
     __request__: VacancyContact,
 
 
 ) -> VacancyContact:
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,35 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
+class Contact(BaseModel):
+    data: str 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
 class VacancyContact(BaseModel):
-    contact: int 
-    id: int 
-    vacancy: int 
+    contact: typing.Union[Contact, None] 
 
 def make_request(self: BaseApi,
 
+    __request__: VacancyContact,
+
+
+    id: str,
 
 ) -> VacancyContact:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/vacancycontact/".format(
+        method="PUT",
+        path="/api/v1/vacancycontact/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
+class Contact(BaseModel):
+    data: str 
     id: int 
-    vacancy: int 
+    name: typing.Optional[typing.Union[str, None]]  = None
+    type: str 
+
+class VacancyContact(BaseModel):
+    contact: typing.Union[Contact, None] 
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
 ) -> VacancyContact:
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancycontact_update.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
+class VacancySkill(BaseModel):
+    skill: int 
     vacancy: int 
 
 def make_request(self: BaseApi,
 
-    __request__: VacancyContact,
+    __request__: VacancySkill,
 
 
     id: str,
 
-) -> VacancyContact:
+) -> VacancySkill:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/vacancycontact/{id}/".format(
+        path="/api/v1/vacancyskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
@@ -43,12 +43,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "application/json": VacancySkill,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_create.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_destroy.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py` & `feedancy-0.1.6/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/client.py` & `feedancy-0.1.6/feedancy/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/adapter/aiohttp.py` & `feedancy-0.1.6/feedancy/lib/adapter/aiohttp.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/adapter/httpx.py` & `feedancy-0.1.6/feedancy/lib/adapter/httpx.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/adapter/params_converter.py` & `feedancy-0.1.6/feedancy/lib/adapter/params_converter.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/adapter/requests.py` & `feedancy-0.1.6/feedancy/lib/adapter/requests.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/base.py` & `feedancy-0.1.6/feedancy/lib/base.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/client.py` & `feedancy-0.1.6/feedancy/lib/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/configuration.py` & `feedancy-0.1.6/feedancy/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/request.py` & `feedancy-0.1.6/feedancy/lib/request.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/response_deserializer.py` & `feedancy-0.1.6/feedancy/lib/response_deserializer.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/feedancy/lib/types.py` & `feedancy-0.1.6/feedancy/lib/types.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.1.5/pyproject.toml` & `feedancy-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feedancy"
-version = "0.1.5"
+version = "0.1.6"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `feedancy-0.1.5/PKG-INFO` & `feedancy-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.1.5
+Version: 0.1.6
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

