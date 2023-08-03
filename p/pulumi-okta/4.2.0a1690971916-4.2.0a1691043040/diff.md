# Comparing `tmp/pulumi_okta-4.2.0a1690971916.tar.gz` & `tmp/pulumi_okta-4.2.0a1691043040.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.2.0a1690971916.tar", last modified: Wed Aug  2 10:30:49 2023, max compression
+gzip compressed data, was "pulumi_okta-4.2.0a1691043040.tar", last modified: Thu Aug  3 06:22:13 2023, max compression
```

## Comparing `pulumi_okta-4.2.0a1690971916.tar` & `pulumi_okta-4.2.0a1691043040.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.908721 pulumi_okta-4.2.0a1690971916/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 10:30:49.908721 pulumi_okta-4.2.0a1690971916/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.888721 pulumi_okta-4.2.0a1690971916/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20927 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.892721 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)   139451 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   137230 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.896721 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)    18251 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.896721 pulumi_okta-4.2.0a1690971916/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    39997 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.896721 pulumi_okta-4.2.0a1690971916/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.896721 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.900721 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.900721 pulumi_okta-4.2.0a1690971916/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/index/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.900721 pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.900721 pulumi_okta-4.2.0a1690971916/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    33089 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.904721 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.904721 pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.904721 pulumi_okta-4.2.0a1690971916/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.908721 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25582 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    99207 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:30:49.888721 pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 10:30:49.908721 pulumi_okta-4.2.0a1690971916/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-02 10:30:49.000000 pulumi_okta-4.2.0a1690971916/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.307349 pulumi_okta-4.2.0a1691043040/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-03 06:22:13.307349 pulumi_okta-4.2.0a1691043040/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.291349 pulumi_okta-4.2.0a1691043040/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20927 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.295349 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139451 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137230 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.299349 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18251 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.299349 pulumi_okta-4.2.0a1691043040/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39997 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.299349 pulumi_okta-4.2.0a1691043040/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.299349 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.303349 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.303349 pulumi_okta-4.2.0a1691043040/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/index/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.303349 pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.303349 pulumi_okta-4.2.0a1691043040/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33089 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.303349 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.307349 pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.307349 pulumi_okta-4.2.0a1691043040/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.307349 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25582 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99207 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:22:13.295349 pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-03 06:22:13.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-03 06:22:13.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:22:13.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:22:13.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 06:22:13.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 06:22:13.000000 pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:22:13.307349 pulumi_okta-4.2.0a1691043040/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-03 06:22:12.000000 pulumi_okta-4.2.0a1691043040/setup.py
```

### Comparing `pulumi_okta-4.2.0a1690971916/PKG-INFO` & `pulumi_okta-4.2.0a1691043040/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.2.0a1690971916
+Version: 4.2.0a1691043040
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.2.0a1690971916/README.md` & `pulumi_okta-4.2.0a1691043040/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/__init__.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/_inputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/_utilities.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/__init__.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_app.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/saml.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/swa.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/three_field.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app/user.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/authenticator.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/behaviour.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/brand.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/captcha.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/config/vars.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/domain.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/domain_verification.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/email_customization.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/email_sender.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/event_hook.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/factor/factor.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/factor_totp.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_app_user_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_brand.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_brands.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_groups.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_template.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_templates.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_theme.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_themes.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group/get_group.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group/get_rule.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group/get_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group/group.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group/role.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group/rule.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group_memberships.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/saml.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/idp/social.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/index/_inputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/index/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/index/email_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/index/email_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/index/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/index/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/index/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/hook.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/link_definition.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/link_value.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/network/zone.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/org_configuration.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/org_support.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/password.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy/signon.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/provider.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/resource_set.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/role_subscription.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/template_sms.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/theme.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_user.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/get_users.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/outputs.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/user.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user/user_type.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.2.0a1691043040/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-okta
-Version: 4.2.0a1690971916
+Version: 4.2.0a1691043040
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.2.0a1690971916/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.2.0a1691043040/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.2.0a1690971916/setup.py` & `pulumi_okta-4.2.0a1691043040/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.2.0a1690971916"
-PLUGIN_VERSION = "4.2.0-alpha.1690971916+9bacf9ac"
+VERSION = "4.2.0a1691043040"
+PLUGIN_VERSION = "4.2.0-alpha.1691043040+146c1e2a"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'okta', PLUGIN_VERSION])
         except OSError as error:
```

