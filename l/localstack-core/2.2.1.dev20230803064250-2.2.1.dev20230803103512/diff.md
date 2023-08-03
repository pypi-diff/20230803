# Comparing `tmp/localstack-core-2.2.1.dev20230803064250.tar.gz` & `tmp/localstack-core-2.2.1.dev20230803103512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.2.1.dev20230803064250.tar", last modified: Thu Aug  3 06:43:05 2023, max compression
+gzip compressed data, was "localstack-core-2.2.1.dev20230803103512.tar", last modified: Thu Aug  3 10:35:28 2023, max compression
```

## Comparing `localstack-core-2.2.1.dev20230803064250.tar` & `localstack-core-2.2.1.dev20230803103512.tar`

### file list

```diff
@@ -1,897 +1,897 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11767 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.228672 localstack-core-2.2.1.dev20230803064250/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.228672 localstack-core-2.2.1.dev20230803064250/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-08-03 06:42:50.000000 localstack-core-2.2.1.dev20230803064250/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    89045 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   761541 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72158 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.232673 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   134503 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27771 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/scheduler/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10043 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.236672 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10618 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49981 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14655 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29492 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28374 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51487 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.240672 localstack-core-2.2.1.dev20230803064250/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.244672 localstack-core-2.2.1.dev20230803064250/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.244672 localstack-core-2.2.1.dev20230803064250/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8744 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.244672 localstack-core-2.2.1.dev20230803064250/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.244672 localstack-core-2.2.1.dev20230803064250/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.244672 localstack-core-2.2.1.dev20230803064250/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.244672 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14992 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    85717 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.248672 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24649 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.248672 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.248672 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20045 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.248672 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   156015 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.252673 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3587 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9266 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.252673 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12539 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50605 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33125 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20288 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      943 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2522 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6543 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2251 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5628 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21069 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2570 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8604 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27126 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3201 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2876 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3337 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4863 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1437 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3655 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13424 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6535 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4826 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10793 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5626 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41357 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26078 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4428 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6060 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24704 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.256672 localstack-core-2.2.1.dev20230803064250/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6650 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12066 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.260672 localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2556 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/cors.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68165 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15016 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17710 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    95615 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33988 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19181 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/scheduler/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/scheduler/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/scheduler/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54706 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.264672 localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1531 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      744 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.268673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.288673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.292672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.292672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.292672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.292672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.296672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.296672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.296672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.296672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.296672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4331 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6029 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.300672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10660 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.304672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.304672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.304672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2954 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1250 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1359 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3273 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6915 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.308673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1602 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1184 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7164 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.308673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1639 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.308673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.308673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6068 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5336 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5863 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5049 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9121 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5199 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.308673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.308673 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3387 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1614 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.312672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.312672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.312672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1682 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5069 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4937 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1539 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1711 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32931 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8923 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13697 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.316672 localstack-core-2.2.1.dev20230803064250/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.320672 localstack-core-2.2.1.dev20230803064250/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.320672 localstack-core-2.2.1.dev20230803064250/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.320672 localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8033 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.320672 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69330 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/marking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.320672 localstack-core-2.2.1.dev20230803064250/localstack/testing/scenario/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/scenario/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6860 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/scenario/provisioning.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.320672 localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.324673 localstack-core-2.2.1.dev20230803064250/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17676 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7676 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26833 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48572 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33233 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4113 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 06:43:05.328673 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-03 06:43:05.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40469 2023-08-03 06:43:05.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 06:43:05.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5400 2023-08-03 06:43:05.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 06:43:00.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5494 2023-08-03 06:43:00.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2871 2023-08-03 06:43:05.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-08-03 06:43:05.000000 localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3251 2023-08-03 06:43:05.332672 localstack-core-2.2.1.dev20230803064250/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-08-03 06:09:10.000000 localstack-core-2.2.1.dev20230803064250/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.337151 localstack-core-2.2.1.dev20230803103512/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-03 10:35:28.337151 localstack-core-2.2.1.dev20230803103512/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11767 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.233149 localstack-core-2.2.1.dev20230803103512/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.233149 localstack-core-2.2.1.dev20230803103512/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-08-03 10:35:12.000000 localstack-core-2.2.1.dev20230803103512/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    89045 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   761541 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.237149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72158 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   134503 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27771 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/scheduler/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10043 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.241149 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10618 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49981 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14655 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29492 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28374 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51487 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.245149 localstack-core-2.2.1.dev20230803103512/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.249149 localstack-core-2.2.1.dev20230803103512/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.249149 localstack-core-2.2.1.dev20230803103512/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8744 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.249149 localstack-core-2.2.1.dev20230803103512/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.249149 localstack-core-2.2.1.dev20230803103512/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.249149 localstack-core-2.2.1.dev20230803103512/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.249149 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    66605 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14992 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2857 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    85717 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.253150 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24649 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.253150 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.253150 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20045 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.253150 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   156015 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.257150 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3587 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9266 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.257150 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12539 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50605 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33125 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20288 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      943 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2522 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6543 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2251 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5628 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21069 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2570 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8604 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27126 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3201 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2876 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3337 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4863 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1437 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3655 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13424 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6535 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4826 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10793 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5626 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41357 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26078 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4547 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6060 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24704 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.261150 localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6650 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12066 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.265150 localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2556 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/cors.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68165 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15016 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17710 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    95615 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33988 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19181 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/scheduler/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/scheduler/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/scheduler/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54706 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.269150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1531 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      744 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.273150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.277150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.277150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.281150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.281150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.281150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.281150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.281150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.281150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.289150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.293150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4331 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6029 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.301150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10660 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.309150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.309150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.309150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2954 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1250 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1359 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3273 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6915 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.309150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1602 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1184 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7164 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.309150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1639 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.309150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2047 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.313150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6068 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5345 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5863 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5049 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9094 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5199 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.313150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.313150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3387 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1614 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.317150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.317150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.317150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1682 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.317150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.317150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5069 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4937 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1539 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1711 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32931 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8923 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13697 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.321150 localstack-core-2.2.1.dev20230803103512/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.325151 localstack-core-2.2.1.dev20230803103512/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.325151 localstack-core-2.2.1.dev20230803103512/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.325151 localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7949 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.325151 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69330 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/marking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.325151 localstack-core-2.2.1.dev20230803103512/localstack/testing/scenario/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/scenario/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6860 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/scenario/provisioning.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.325151 localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.329151 localstack-core-2.2.1.dev20230803103512/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.329151 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.333151 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17941 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7674 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26833 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.333151 localstack-core-2.2.1.dev20230803103512/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.333151 localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48572 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33233 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4113 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.333151 localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.333151 localstack-core-2.2.1.dev20230803103512/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 10:35:28.337151 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-03 10:35:28.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40469 2023-08-03 10:35:28.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 10:35:28.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5400 2023-08-03 10:35:28.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 10:35:23.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5494 2023-08-03 10:35:23.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2871 2023-08-03 10:35:28.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-08-03 10:35:28.000000 localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3251 2023-08-03 10:35:28.337151 localstack-core-2.2.1.dev20230803103512/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-08-03 09:59:31.000000 localstack-core-2.2.1.dev20230803103512/setup.py
```

### Comparing `localstack-core-2.2.1.dev20230803064250/LICENSE.txt` & `localstack-core-2.2.1.dev20230803103512/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/Makefile` & `localstack-core-2.2.1.dev20230803103512/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/PKG-INFO` & `localstack-core-2.2.1.dev20230803103512/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230803064250
+Version: 2.2.1.dev20230803103512
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230803064250/README.md` & `localstack-core-2.2.1.dev20230803103512/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/bin/localstack` & `localstack-core-2.2.1.dev20230803103512/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/bin/localstack-supervisor` & `localstack-core-2.2.1.dev20230803103512/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/accounts.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/acm/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/config/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/core.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/es/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/events/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/iam/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/kms/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/logs/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/route53/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/s3/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/scheduler/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ses/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sns/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/sts/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/support/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/swf/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/app.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/chain.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/client.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/connect.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/forwarder.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/gateway.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/analytics.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/auth.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/codec.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/cors.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/fallback.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/internal.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/legacy.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/logging.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/proxy.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/region.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/routes.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/service.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/mocking.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/op_router.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/parser.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/serializer.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/service_router.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/protocol/validate.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/proxy.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/scaffold.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/asgi.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/edge.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/hypercorn.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/werkzeug.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/serving/wsgi.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/skeleton.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/spec-patches.json` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/spec.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/aws/trace.py` & `localstack-core-2.2.1.dev20230803103512/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/cli/localstack.py` & `localstack-core-2.2.1.dev20230803103512/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/cli/lpm.py` & `localstack-core-2.2.1.dev20230803103512/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/cli/plugin.py` & `localstack-core-2.2.1.dev20230803103512/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/cli/plugins.py` & `localstack-core-2.2.1.dev20230803103512/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/cli/profiles.py` & `localstack-core-2.2.1.dev20230803103512/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/config.py` & `localstack-core-2.2.1.dev20230803103512/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/constants.py` & `localstack-core-2.2.1.dev20230803103512/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/deprecations.py` & `localstack-core-2.2.1.dev20230803103512/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/aws.py` & `localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/extensions/api/extension.py` & `localstack-core-2.2.1.dev20230803103512/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/adapters.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/asgi.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/client.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/dispatcher.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/hypercorn.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/proxy.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/request.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/resource.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/response.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/http/router.py` & `localstack-core-2.2.1.dev20230803103512/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/logging/format.py` & `localstack-core-2.2.1.dev20230803103512/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/logging/setup.py` & `localstack-core-2.2.1.dev20230803103512/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/packages/__init__.py` & `localstack-core-2.2.1.dev20230803103512/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/packages/api.py` & `localstack-core-2.2.1.dev20230803103512/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/packages/core.py` & `localstack-core-2.2.1.dev20230803103512/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/packages/debugpy.py` & `localstack-core-2.2.1.dev20230803103512/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/packages/ffmpeg.py` & `localstack-core-2.2.1.dev20230803103512/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/packages/terraform.py` & `localstack-core-2.2.1.dev20230803103512/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/plugins.py` & `localstack-core-2.2.1.dev20230803103512/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/runtime/analytics.py` & `localstack-core-2.2.1.dev20230803103512/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/runtime/hooks.py` & `localstack-core-2.2.1.dev20230803103512/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/runtime/init.py` & `localstack-core-2.2.1.dev20230803103512/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/runtime/main.py` & `localstack-core-2.2.1.dev20230803103512/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/runtime/shutdown.py` & `localstack-core-2.2.1.dev20230803103512/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/acm/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/context.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/helpers.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/integration.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/invocations.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/patches.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/router_asf.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/apigateway/templates.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/api_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/hooks.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/packages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/plugins.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/deploy.html` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/events.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/packages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/service_models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudformation/stores.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/cloudwatch/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/packages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/server.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodb/utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 ) -> None:
     if not enabled:
         return
 
     store = get_dynamodbstreams_store()
     # create kinesis stream as a backend
     stream_name = get_kinesis_stream_name(table_name)
-    resources.create_kinesis_stream(stream_name)
+    # TODO: The kinesis client must be created for the correct account ID and region
+    resources.create_kinesis_stream(connect_to().kinesis, stream_name=stream_name)
     latest_stream_label = latest_stream_label or "latest"
     stream = {
         "StreamArn": arns.dynamodb_stream_arn(
             table_name=table_name, latest_stream_label=latest_stream_label
         ),
         "TableName": table_name,
         "StreamLabel": latest_stream_label,
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/exceptions.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/ec2/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/edge.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/es/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/events/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/events/scheduler.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/mappers.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/firehose/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/generic_proxy.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/iam/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.2.1.dev20230803103512/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/infra.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/internal.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/packages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kinesis/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kms/local_kms_server.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kms/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kms/packages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kms/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/kms/utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/logs/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/logs/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/messages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/moto.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/motoserver.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/cluster.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/packages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/opensearch/versions.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/plugins.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/providers.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/redshift/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/route53/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/route53resolver/utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/codec.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/constants.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/cors.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/multipart_content.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/s3_listener.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/s3_starter.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/legacy/s3_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/legacy/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/notifications.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/presigned_url.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/provider_stream.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/virtual_host.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/s3/website_hosting.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/secretsmanager/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/ses/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sns/constants.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sns/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sns/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sns/publisher.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/constants.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/exceptions.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/query_api.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sqs/utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.2.1.dev20230803103512/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from botocore.config import Config
 from botocore.exceptions import ClientError
 
 from localstack.aws.api.stepfunctions import HistoryEventType, TaskFailedEventDetails
+from localstack.aws.connect import connect_externally_to
 from localstack.aws.protocol.service_router import get_service_catalog
 from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
     FailureEvent,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name import (
     StatesErrorName,
 )
@@ -14,15 +15,14 @@
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_callback import (
     StateTaskServiceCallback,
 )
 from localstack.services.stepfunctions.asl.component.state.state_props import StateProps
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
-from localstack.utils.aws import aws_stack
 from localstack.utils.common import camel_to_snake_case
 
 
 class StateTaskServiceAwsSdk(StateTaskServiceCallback):
     _NORMALISED_SERVICE_NAMES = {"dynamodb": "DynamoDb"}
     _API_NAMES: dict[str, str] = {"sfn": "stepfunctions"}
     _SFN_TO_BOTO_PARAM_NORMALISERS = {
@@ -101,14 +101,14 @@
 
             cause: str = f"{error_message} ({', '.join(cause_details)})"
             failure_event = self._get_task_failure_event(error=error, cause=cause)
             return failure_event
         return super()._from_error(env=env, ex=ex)
 
     def _eval_service_task(self, env: Environment, parameters: dict) -> None:
-        api_client = aws_stack.create_external_boto_client(
+        api_client = connect_externally_to.get_client(
             service_name=self._normalised_api_name, config=Config(parameter_validation=False)
         )
         response = getattr(api_client, self._normalised_api_action)(**parameters) or dict()
         if response:
             response.pop("ResponseMetadata", None)
         env.stack.append(response)
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from localstack.aws.api.stepfunctions import (
     DescribeExecutionOutput,
     ExecutionStatus,
     HistoryEventType,
     TaskFailedEventDetails,
 )
+from localstack.aws.connect import connect_externally_to
 from localstack.services.stepfunctions.asl.component.common.error_name.custom_error_name import (
     CustomErrorName,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
     FailureEvent,
     FailureEventException,
 )
@@ -24,15 +25,14 @@
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_callback import (
     StateTaskServiceCallback,
 )
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 from localstack.services.stepfunctions.asl.utils.encoding import to_json_str
-from localstack.utils.aws import aws_stack
 from localstack.utils.collections import select_from_typed_dict
 from localstack.utils.strings import camel_to_snake_case
 
 
 class StateTaskServiceSfn(StateTaskServiceCallback):
     _SUPPORTED_API_PARAM_BINDINGS: Final[dict[str, set[str]]] = {
         "startexecution": {"Input", "Name", "StateMachineArn"}
@@ -97,17 +97,15 @@
                     _apply_normalisation(normalised_key[1], dictionary[normalised_key[0]])
 
         lower_to_normalise_key = _build_lower_to_key_dict(keys)
         _apply_normalisation(lower_to_normalise_key, response)
 
     @staticmethod
     def _get_sfn_client():
-        return aws_stack.create_external_boto_client(
-            "stepfunctions", config=Config(parameter_validation=False)
-        )
+        return connect_externally_to(config=Config(parameter_validation=False)).stepfunctions
 
     def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
         if isinstance(ex, ClientError):
             error_code = ex.response["Error"]["Code"]
             error_name: str = f"StepFunctions.{error_code}Exception"
             error_cause_details = [
                 "Service: AWSStepFunctions",
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/program_state.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/program_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/packages.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/stores.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/sts/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/services/transcribe/provider.py` & `localstack-core-2.2.1.dev20230803103512/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/state/core.py` & `localstack-core-2.2.1.dev20230803103512/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/state/inspect.py` & `localstack-core-2.2.1.dev20230803103512/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/state/pickle.py` & `localstack-core-2.2.1.dev20230803103512/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/state/snapshot.py` & `localstack-core-2.2.1.dev20230803103512/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/asf_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/aws/util.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/aws/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 from localstack.utils.sync import poll_condition
 
 
 def is_aws_cloud() -> bool:
     return os.environ.get("TEST_TARGET", "") == "AWS_CLOUD"
 
 
-def get_lambda_logs(func_name, logs_client=None):
-    logs_client = logs_client or aws_stack.create_external_boto_client("logs")
+def get_lambda_logs(func_name, logs_client):
     log_group_name = f"/aws/lambda/{func_name}"
     streams = logs_client.describe_log_streams(logGroupName=log_group_name)["logStreams"]
     streams = sorted(streams, key=lambda x: x["creationTime"], reverse=True)
     log_events = logs_client.get_log_events(
         logGroupName=log_group_name, logStreamName=streams[0]["logStreamName"]
     )["events"]
     return log_events
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/filters.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/fixtures.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/marking.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/marking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/snapshot.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/pytest/util.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/scenario/provisioning.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/scenario/provisioning.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/prototype.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/report.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/transformer.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.2.1.dev20230803103512/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/cli.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/client.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/events.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/logger.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/metadata.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/publisher.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/analytics/usage.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/archives.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/asyncio.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/auth.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/arns.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/aws_models.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/aws_responses.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/aws_stack.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/aws_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,19 @@
     internal=True,
     *args,
     **kwargs,
 ):
     """
     Generic method to obtain an AWS service client using boto3, based on environment, region, or custom endpoint_url.
     """
+    warnings.warn(
+        "`connect_to_service` is obsolete. Use `localstack.aws.connect`",
+        DeprecationWarning,
+    )
+
     # determine context and create cache key
     region_name = region_name or get_region()
     env = get_environment(env, region_name=region_name)
     region = env.region if env.region != REGION_LOCAL else region_name
     key_elements = [service_name, client, env, region, endpoint_url, config, internal, kwargs]
     cache_key = "/".join([str(k) for k in key_elements])
 
@@ -365,14 +370,19 @@
     verify=False,
     cache=True,
     aws_access_key_id=None,
     aws_secret_access_key=None,
     *args,
     **kwargs,
 ):
+    warnings.warn(
+        "`create_external_boto_client` is obsolete. Use `localstack.aws.connect`",
+        DeprecationWarning,
+    )
+
     # Currently we use the Access Key ID field to specify the AWS account ID; this will change when IAM matures.
     # It is important that the correct Account ID is included in the request as that will determine access to namespaced resources.
     if aws_access_key_id is None:
         aws_access_key_id = get_aws_account_id()
 
     if aws_secret_access_key is None:
         aws_secret_access_key = TEST_AWS_SECRET_ACCESS_KEY
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/client.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/client_types.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/queries.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/request_context.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/resources.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,16 +184,15 @@
                 restApiId=api_id,
                 resourceId=resource_id,
                 httpMethod=method["httpMethod"],
                 statusCode=response_config["code"],
             )
 
 
-def create_kinesis_stream(stream_name, shards=1, delete=False):
+def create_kinesis_stream(client, stream_name: str, shards: int = 1, delete: bool = False):
     stream = KinesisStream(id=stream_name, num_shards=shards)
-    conn = connect_to().kinesis
-    stream.connect(conn)
+    stream.connect(client)
     if delete:
         run_safe(lambda: stream.destroy(), print_error=False)
     stream.create()
     # Note: Returning the stream without awaiting its creation (via wait_for()) to avoid API call timeouts/retries.
     return stream
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/aws/templating.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/bootstrap.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/collections.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/common.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/config_listener.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/container_networking.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/container_client.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/coverage_docs.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/crypto.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/diagnose.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/docker_utils.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/files.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/functions.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/http.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/json.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/net.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/numbers.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/objects.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/patch.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/platform.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/run.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/scheduler.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/server/http2_server.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/server/proxy_server.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/serving.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/ssl.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/strings.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/sync.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/tagging.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/tail.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/testutil.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/threads.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/time.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/urls.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/venv.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack/utils/xml.py` & `localstack-core-2.2.1.dev20230803103512/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230803064250
+Version: 2.2.1.dev20230803103512
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/plux.json` & `localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/plux.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8484848484848485%*

 * *Differences: {"'localstack.cloudformation.resource_providers'": '{insert: [(1, '*

 * *                                                   "'AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin')], "*

 * *                                                   'delete: [0]}',*

 * * "'localstack.hooks.on_infra_ready'": '{insert: [(1, '*

 * *                                      "'_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready')], "*

 * *                                […]*

```diff
@@ -44,52 +44,52 @@
         "stepfunctions:v2=localstack.services.providers:stepfunctions_v2",
         "sts:default=localstack.services.providers:sts",
         "support:default=localstack.services.providers:support",
         "swf:default=localstack.services.providers:swf",
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.cloudformation.resource_providers": [
-        "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin",
-        "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user:IAMUserProviderPlugin"
+        "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user:IAMUserProviderPlugin",
+        "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
         "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file",
         "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
+        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
-        "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
+        "terraform/community=localstack.packages.plugins:terraform_package",
         "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package"
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package"
     ]
 }
```

### Comparing `localstack-core-2.2.1.dev20230803064250/localstack_core.egg-info/requires.txt` & `localstack-core-2.2.1.dev20230803103512/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/pyproject.toml` & `localstack-core-2.2.1.dev20230803103512/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230803064250/setup.cfg` & `localstack-core-2.2.1.dev20230803103512/setup.cfg`

 * *Files identical despite different names*

