# Comparing `tmp/nebari-2023.7.1rc1.tar.gz` & `tmp/nebari-2023.7.2rc1.tar.gz`

## Comparing `nebari-2023.7.1rc1.tar` & `nebari-2023.7.2rc1.tar`

### file list

```diff
@@ -1,405 +1,405 @@
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.cirun.yml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/MANIFEST.in
--rw-r--r--   0        0        0    60531 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/RELEASE.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/flake.lock
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/flake.nix
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/actions/publish-from-template/action.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/actions/publish-from-template/render_template.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/failed-workflow-issue-templates/test-provider.md
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/kubernetes_test.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/release.yaml
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.github/workflows/test_helm_charts.yaml
--rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/helm-validate.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/_version.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/constants.py
--rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/deprecate.py
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/destroy.py
--rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/initialize.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/keycloak.py
--rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/render.py
--rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/schema.py
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/upgrade.py
--rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/utils.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/dev.py
--rw-r--r--   0        0        0    22058 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/init.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/keycloak.py
--rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/git.py
--rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/common.py
--rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/__init__.py
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/checks.py
--rw-r--r--   0        0        0    15591 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/input_vars.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/state_imports.py
--rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/stages/tf_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/main.tf
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/main.tf
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/locals.tf
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/main.tf
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/outputs.tf
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/providers.tf
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/versions.tf
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/existing/main.tf
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/outputs.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/provider.tf
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/main.tf
--rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/metallb.yaml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/outputs.tf
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/variables.tf
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/main.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/versions.tf
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/versions.tf
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/outputs.tf
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/versions.tf
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/__init__.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/argo-workflows.tf
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/clearml.tf
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/conda-store.tf
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/forward-auth.tf
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/kbatch.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/locals.tf
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/outputs.tf
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/prefect.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/providers.tf
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/versions.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/__init__.py
--rw-r--r--   0        0        0    15836 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
--rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
--rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
--rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/__init__.py
--rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/__init__.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/__init__.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/__init__.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    16472 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
--rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
--rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
--rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/versions.tf
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/nebari/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/src/nebari/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/__init__.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/conftest.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_cli.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_commons.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_dependencies.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_init.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_links.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_render.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_schema.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/test_upgrade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/notebooks/test-ipython-basic.ipynb
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/scripts/minikube-loadbalancer-ip.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests/vale/styles/vocab.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/constants.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/.env.tpl
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/README.md
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/conftest.py
--rw-r--r--   0        0        0    16199 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/navigator.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/run_notebook.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/test_playwright.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/tests_e2e/playwright/test_data/test_notebook_output.ipynb
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/LICENSE
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/README.md
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/pyproject.toml
--rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 nebari-2023.7.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.cirun.yml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/MANIFEST.in
+-rw-r--r--   0        0        0    64130 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/RELEASE.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/flake.lock
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/flake.nix
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/actions/publish-from-template/action.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/actions/publish-from-template/render_template.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/failed-workflow-issue-templates/test-provider.md
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/workflows/kubernetes_test.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.github/workflows/test_helm_charts.yaml
+-rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/scripts/helm-validate.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/_version.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/constants.py
+-rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/deprecate.py
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/destroy.py
+-rw-r--r--   0        0        0    18171 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/initialize.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/keycloak.py
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/render.py
+-rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/schema.py
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/upgrade.py
+-rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/utils.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/cli/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/cli/dev.py
+-rw-r--r--   0        0        0    22058 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/cli/init.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/cli/keycloak.py
+-rw-r--r--   0        0        0    12596 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/git.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/stages/__init__.py
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/stages/checks.py
+-rw-r--r--   0        0        0    15591 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/stages/input_vars.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/stages/state_imports.py
+-rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/aws/main.tf
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/azure/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/main.tf
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/locals.tf
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/main.tf
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/outputs.tf
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/main.tf
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/providers.tf
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/versions.tf
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/existing/main.tf
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/outputs.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/provider.tf
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/local/main.tf
+-rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/local/metallb.yaml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/local/outputs.tf
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/local/variables.tf
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/main.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/versions.tf
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/versions.tf
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/outputs.tf
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/versions.tf
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/__init__.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/argo-workflows.tf
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/clearml.tf
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/conda-store.tf
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/dask_gateway.tf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/forward-auth.tf
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/kbatch.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/locals.tf
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/outputs.tf
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/prefect.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/providers.tf
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/__init__.py
+-rw-r--r--   0        0        0    15836 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
+-rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
+-rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
+-rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/__init__.py
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/__init__.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/__init__.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/__init__.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    16474 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
+-rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
+-rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
+-rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/providers.tf
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/versions.tf
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/nebari/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/src/nebari/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/__init__.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/conftest.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_cli.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_commons.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_dependencies.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_init.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_links.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_render.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_schema.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/test_upgrade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/notebooks/test-ipython-basic.ipynb
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/scripts/minikube-loadbalancer-ip.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests/vale/styles/vocab.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/playwright/.env.tpl
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/playwright/README.md
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/playwright/conftest.py
+-rw-r--r--   0        0        0    16199 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/playwright/navigator.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/playwright/run_notebook.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/playwright/test_playwright.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/tests_e2e/playwright/test_data/test_notebook_output.ipynb
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/LICENSE
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/README.md
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/pyproject.toml
+-rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 nebari-2023.7.2rc1/PKG-INFO
```

### Comparing `nebari-2023.7.1rc1/.cirun.yml` & `nebari-2023.7.2rc1/.cirun.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.pre-commit-config.yaml` & `nebari-2023.7.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/CODE_OF_CONDUCT.md` & `nebari-2023.7.2rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/CONTRIBUTING.md` & `nebari-2023.7.2rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/RELEASE.md` & `nebari-2023.7.2rc1/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,63 @@
 If you want to update the release notes, open a PR against nebari-dev/nebari.
 This file is copied to nebari-dev/nebari-docs using a GitHub Action. -->
 
 ---
 
 ## Upcoming Release
 
+## Release 2023.7.1 - July 21, 2023
+
+> WARNING: CDS Dashboards will be deprecated soon. Nebari 2023.7.1 will be the last release with support for CDS Dashboards integration. A new dashboard sharing mechanism added in the near future, but some releases in the interim will not have dashboard sharing capabilities..
+
+### Feature changes and enhancements
+
+* Addition of Nebari-Workflow-Controller in [PR 1741](https://github.com/nebari-dev/nebari/pull/1741)
+* Addition of Argo-Jupyter-Scheduler in [PR 1832](https://github.com/nebari-dev/nebari/pull/1832)
+* Make most of the API private
+
+### Breaking Changes
+
+* No known breaking changes.
+
+### What's Changed
+* use conda forge explicitly in conda build test by @pmeier in https://github.com/nebari-dev/nebari/pull/1771
+* document that the upgrade command is for all nebari upgrades by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1794
+* don't fail CI matrices fast by @pmeier in https://github.com/nebari-dev/nebari/pull/1804
+* unvendor keycloak_metrics_spi by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1810
+* Dedent fail-fast by @iameskild in https://github.com/nebari-dev/nebari/pull/1815
+* support deploying on existing vpc on aws by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1807
+* purge most danlging qhub references by @pmeier in https://github.com/nebari-dev/nebari/pull/1802
+* Add Argo Workflow Admission controller by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1741
+* purge infracost CLI command / CI jobs by @pmeier in https://github.com/nebari-dev/nebari/pull/1820
+* remove unused function parameters and CLI flags by @pmeier in https://github.com/nebari-dev/nebari/pull/1725
+* purge docs and nox by @pmeier in https://github.com/nebari-dev/nebari/pull/1801
+* Add Helm chart lint tool by @viniciusdc in https://github.com/nebari-dev/nebari/pull/1679
+* don't set /etc/hosts in CI by @pmeier in https://github.com/nebari-dev/nebari/pull/1729
+* remove execute permissions on templates by @pmeier in https://github.com/nebari-dev/nebari/pull/1798
+* fix deprecated file deletion by @pmeier in https://github.com/nebari-dev/nebari/pull/1799
+* make nebari API private by @pmeier in https://github.com/nebari-dev/nebari/pull/1778
+* [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/nebari-dev/nebari/pull/1831
+* Simplify CI by @iameskild in https://github.com/nebari-dev/nebari/pull/1819
+* Fix edge-case where k8s_version is equal to HIGHEST_SUPPORTED_K8S_VER… by @iameskild in https://github.com/nebari-dev/nebari/pull/1842
+* add more configuration to enable private clusters on AWS by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/1841
+* [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/nebari-dev/nebari/pull/1851
+* AWS gov cloud support by @sblair-metrostar in https://github.com/nebari-dev/nebari/pull/1857
+* Pathlib everywhere by @pmeier in https://github.com/nebari-dev/nebari/pull/1773
+* Initial playwright setup by @kcpevey in https://github.com/nebari-dev/nebari/pull/1665
+* Changes required for Jupyter-Scheduler integration  by @iameskild in https://github.com/nebari-dev/nebari/pull/1832
+* Update upgrade command in preparation for release by @iameskild in https://github.com/nebari-dev/nebari/pull/1868
+* Add release notes by @iameskild in https://github.com/nebari-dev/nebari/issues/1869
+
+### New Contributors
+* @sblair-metrostar made their first contribution in https://github.com/nebari-dev/nebari/pull/1857
+
+**Full Changelog**: https://github.com/nebari-dev/nebari/compare/2023.5.1...2023.7.1
+
+
 ### Release 2023.5.1 - May 5, 2023
 
 ### Feature changes and enhancements
 
 * Upgrade Argo-Workflows to version 3.4.4
 
 ### Breaking Changes
```

### Comparing `nebari-2023.7.1rc1/flake.lock` & `nebari-2023.7.2rc1/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/flake.nix` & `nebari-2023.7.2rc1/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2023.7.2rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2023.7.2rc1/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/actions/publish-from-template/action.yml` & `nebari-2023.7.2rc1/.github/actions/publish-from-template/action.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/workflows/kubernetes_test.yaml` & `nebari-2023.7.2rc1/.github/workflows/kubernetes_test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/workflows/release-notes-sync.yaml` & `nebari-2023.7.2rc1/.github/workflows/release-notes-sync.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/workflows/release.yaml` & `nebari-2023.7.2rc1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/workflows/run-precommit.yaml` & `nebari-2023.7.2rc1/.github/workflows/run-precommit.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/workflows/test-provider.yaml` & `nebari-2023.7.2rc1/.github/workflows/test-provider.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/workflows/test.yaml` & `nebari-2023.7.2rc1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.github/workflows/test_helm_charts.yaml` & `nebari-2023.7.2rc1/.github/workflows/test_helm_charts.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/scripts/aws-force-destroy.py` & `nebari-2023.7.2rc1/scripts/aws-force-destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/scripts/aws-force-destroy.sh` & `nebari-2023.7.2rc1/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/scripts/helm-validate.py` & `nebari-2023.7.2rc1/scripts/helm-validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/scripts/keycloak-export.py` & `nebari-2023.7.2rc1/scripts/keycloak-export.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/deploy.py` & `nebari-2023.7.2rc1/src/_nebari/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/destroy.py` & `nebari-2023.7.2rc1/src/_nebari/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/initialize.py` & `nebari-2023.7.2rc1/src/_nebari/initialize.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/keycloak.py` & `nebari-2023.7.2rc1/src/_nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/render.py` & `nebari-2023.7.2rc1/src/_nebari/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/schema.py` & `nebari-2023.7.2rc1/src/_nebari/schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/upgrade.py` & `nebari-2023.7.2rc1/src/_nebari/upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/utils.py` & `nebari-2023.7.2rc1/src/_nebari/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/version.py` & `nebari-2023.7.2rc1/src/_nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/cli/dev.py` & `nebari-2023.7.2rc1/src/_nebari/cli/dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/cli/init.py` & `nebari-2023.7.2rc1/src/_nebari/cli/init.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/cli/keycloak.py` & `nebari-2023.7.2rc1/src/_nebari/cli/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/cli/main.py` & `nebari-2023.7.2rc1/src/_nebari/cli/main.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/git.py` & `nebari-2023.7.2rc1/src/_nebari/provider/git.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/terraform.py` & `nebari-2023.7.2rc1/src/_nebari/provider/terraform.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/cicd/github.py` & `nebari-2023.7.2rc1/src/_nebari/provider/cicd/github.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/cicd/gitlab.py` & `nebari-2023.7.2rc1/src/_nebari/provider/cicd/gitlab.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/cicd/linter.py` & `nebari-2023.7.2rc1/src/_nebari/provider/cicd/linter.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/cloud/amazon_web_services.py` & `nebari-2023.7.2rc1/src/_nebari/provider/cloud/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/cloud/azure_cloud.py` & `nebari-2023.7.2rc1/src/_nebari/provider/cloud/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/cloud/digital_ocean.py` & `nebari-2023.7.2rc1/src/_nebari/provider/cloud/digital_ocean.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/cloud/google_cloud.py` & `nebari-2023.7.2rc1/src/_nebari/provider/cloud/google_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/dns/cloudflare.py` & `nebari-2023.7.2rc1/src/_nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/provider/oauth/auth0.py` & `nebari-2023.7.2rc1/src/_nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/stages/checks.py` & `nebari-2023.7.2rc1/src/_nebari/stages/checks.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/stages/input_vars.py` & `nebari-2023.7.2rc1/src/_nebari/stages/input_vars.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/stages/state_imports.py` & `nebari-2023.7.2rc1/src/_nebari/stages/state_imports.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/stages/tf_objects.py` & `nebari-2023.7.2rc1/src/_nebari/stages/tf_objects.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/do/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/metallb.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/02-infrastructure/local/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/02-infrastructure/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/argo-workflows.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/argo-workflows.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/clearml.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/clearml.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/conda-store.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/conda-store.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/dask_gateway.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/dask_gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/jupyterhub.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/kbatch.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/kbatch.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/prefect.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/prefect.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     DEVELOPER = "developer"
     ANALYST = "analyst"
 
     base = "argo-"
     argo_sa = None
 
     if ANALYST in groups:
-        argo_sa = base + "view"
+        argo_sa = base + "viewer"
     if DEVELOPER in groups:
         argo_sa = base + "developer"
     if ADMIN in groups:
         argo_sa = base + "admin"
     if not argo_sa:
         return {}
```

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf` & `nebari-2023.7.2rc1/src/_nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/conftest.py` & `nebari-2023.7.2rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/test_cli.py` & `nebari-2023.7.2rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/test_commons.py` & `nebari-2023.7.2rc1/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/test_dependencies.py` & `nebari-2023.7.2rc1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/test_init.py` & `nebari-2023.7.2rc1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/test_render.py` & `nebari-2023.7.2rc1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/test_schema.py` & `nebari-2023.7.2rc1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/test_upgrade.py` & `nebari-2023.7.2rc1/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2023.7.2rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2023.7.2rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/scripts/minikube-loadbalancer-ip.py` & `nebari-2023.7.2rc1/tests/scripts/minikube-loadbalancer-ip.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests/vale/styles/vocab.txt` & `nebari-2023.7.2rc1/tests/vale/styles/vocab.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_deployment/test_dask_gateway.py` & `nebari-2023.7.2rc1/tests_deployment/test_dask_gateway.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2023.7.2rc1/tests_deployment/test_jupyterhub_ssh.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_deployment/utils.py` & `nebari-2023.7.2rc1/tests_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2023.7.2rc1/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/package-lock.json` & `nebari-2023.7.2rc1/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/cypress/integration/main.js` & `nebari-2023.7.2rc1/tests_e2e/cypress/integration/main.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2023.7.2rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/cypress/plugins/index.js` & `nebari-2023.7.2rc1/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/cypress/support/index.js` & `nebari-2023.7.2rc1/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/playwright/README.md` & `nebari-2023.7.2rc1/tests_e2e/playwright/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/playwright/conftest.py` & `nebari-2023.7.2rc1/tests_e2e/playwright/conftest.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/playwright/navigator.py` & `nebari-2023.7.2rc1/tests_e2e/playwright/navigator.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/playwright/run_notebook.py` & `nebari-2023.7.2rc1/tests_e2e/playwright/run_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/tests_e2e/playwright/test_data/test_notebook_output.ipynb` & `nebari-2023.7.2rc1/tests_e2e/playwright/test_data/test_notebook_output.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/.gitignore` & `nebari-2023.7.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/LICENSE` & `nebari-2023.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/README.md` & `nebari-2023.7.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/pyproject.toml` & `nebari-2023.7.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari-2023.7.1rc1/PKG-INFO` & `nebari-2023.7.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari
-Version: 2023.7.1rc1
+Version: 2023.7.2rc1
 Summary: A Jupyter and Dask-powered open source data science platform.
 Project-URL: Documentation, https://www.nebari.dev/docs
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
```

