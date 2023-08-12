# Literals

> [Index](../README.md) > [CodeBuild](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
    type annotations stubs module [types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

## ArtifactNamespaceType

```python
# ArtifactNamespaceType usage example

from types_aiobotocore_codebuild.literals import ArtifactNamespaceType

def get_value() -> ArtifactNamespaceType:
    return "BUILD_ID"
```

```python
# ArtifactNamespaceType definition

ArtifactNamespaceType = Literal[
    "BUILD_ID",
    "NONE",
]
```
## ArtifactPackagingType

```python
# ArtifactPackagingType usage example

from types_aiobotocore_codebuild.literals import ArtifactPackagingType

def get_value() -> ArtifactPackagingType:
    return "NONE"
```

```python
# ArtifactPackagingType definition

ArtifactPackagingType = Literal[
    "NONE",
    "ZIP",
]
```
## ArtifactsTypeType

```python
# ArtifactsTypeType usage example

from types_aiobotocore_codebuild.literals import ArtifactsTypeType

def get_value() -> ArtifactsTypeType:
    return "CODEPIPELINE"
```

```python
# ArtifactsTypeType definition

ArtifactsTypeType = Literal[
    "CODEPIPELINE",
    "NO_ARTIFACTS",
    "S3",
]
```
## AuthTypeType

```python
# AuthTypeType usage example

from types_aiobotocore_codebuild.literals import AuthTypeType

def get_value() -> AuthTypeType:
    return "BASIC_AUTH"
```

```python
# AuthTypeType definition

AuthTypeType = Literal[
    "BASIC_AUTH",
    "OAUTH",
    "PERSONAL_ACCESS_TOKEN",
]
```
## BatchReportModeTypeType

```python
# BatchReportModeTypeType usage example

from types_aiobotocore_codebuild.literals import BatchReportModeTypeType

def get_value() -> BatchReportModeTypeType:
    return "REPORT_AGGREGATED_BATCH"
```

```python
# BatchReportModeTypeType definition

BatchReportModeTypeType = Literal[
    "REPORT_AGGREGATED_BATCH",
    "REPORT_INDIVIDUAL_BUILDS",
]
```
## BucketOwnerAccessType

```python
# BucketOwnerAccessType usage example

from types_aiobotocore_codebuild.literals import BucketOwnerAccessType

def get_value() -> BucketOwnerAccessType:
    return "FULL"
```

```python
# BucketOwnerAccessType definition

BucketOwnerAccessType = Literal[
    "FULL",
    "NONE",
    "READ_ONLY",
]
```
## BuildBatchPhaseTypeType

```python
# BuildBatchPhaseTypeType usage example

from types_aiobotocore_codebuild.literals import BuildBatchPhaseTypeType

def get_value() -> BuildBatchPhaseTypeType:
    return "COMBINE_ARTIFACTS"
```

```python
# BuildBatchPhaseTypeType definition

BuildBatchPhaseTypeType = Literal[
    "COMBINE_ARTIFACTS",
    "DOWNLOAD_BATCHSPEC",
    "FAILED",
    "IN_PROGRESS",
    "STOPPED",
    "SUBMITTED",
    "SUCCEEDED",
]
```
## BuildPhaseTypeType

```python
# BuildPhaseTypeType usage example

from types_aiobotocore_codebuild.literals import BuildPhaseTypeType

def get_value() -> BuildPhaseTypeType:
    return "BUILD"
```

```python
# BuildPhaseTypeType definition

BuildPhaseTypeType = Literal[
    "BUILD",
    "COMPLETED",
    "DOWNLOAD_SOURCE",
    "FINALIZING",
    "INSTALL",
    "POST_BUILD",
    "PRE_BUILD",
    "PROVISIONING",
    "QUEUED",
    "SUBMITTED",
    "UPLOAD_ARTIFACTS",
]
```
## CacheModeType

```python
# CacheModeType usage example

from types_aiobotocore_codebuild.literals import CacheModeType

def get_value() -> CacheModeType:
    return "LOCAL_CUSTOM_CACHE"
```

```python
# CacheModeType definition

CacheModeType = Literal[
    "LOCAL_CUSTOM_CACHE",
    "LOCAL_DOCKER_LAYER_CACHE",
    "LOCAL_SOURCE_CACHE",
]
```
## CacheTypeType

```python
# CacheTypeType usage example

from types_aiobotocore_codebuild.literals import CacheTypeType

def get_value() -> CacheTypeType:
    return "LOCAL"
```

```python
# CacheTypeType definition

CacheTypeType = Literal[
    "LOCAL",
    "NO_CACHE",
    "S3",
]
```
## ComputeTypeType

```python
# ComputeTypeType usage example

from types_aiobotocore_codebuild.literals import ComputeTypeType

def get_value() -> ComputeTypeType:
    return "BUILD_GENERAL1_2XLARGE"
```

```python
# ComputeTypeType definition

ComputeTypeType = Literal[
    "BUILD_GENERAL1_2XLARGE",
    "BUILD_GENERAL1_LARGE",
    "BUILD_GENERAL1_MEDIUM",
    "BUILD_GENERAL1_SMALL",
]
```
## CredentialProviderTypeType

```python
# CredentialProviderTypeType usage example

from types_aiobotocore_codebuild.literals import CredentialProviderTypeType

def get_value() -> CredentialProviderTypeType:
    return "SECRETS_MANAGER"
```

```python
# CredentialProviderTypeType definition

CredentialProviderTypeType = Literal[
    "SECRETS_MANAGER",
]
```
## DescribeCodeCoveragesPaginatorName

```python
# DescribeCodeCoveragesPaginatorName usage example

from types_aiobotocore_codebuild.literals import DescribeCodeCoveragesPaginatorName

def get_value() -> DescribeCodeCoveragesPaginatorName:
    return "describe_code_coverages"
```

```python
# DescribeCodeCoveragesPaginatorName definition

DescribeCodeCoveragesPaginatorName = Literal[
    "describe_code_coverages",
]
```
## DescribeTestCasesPaginatorName

```python
# DescribeTestCasesPaginatorName usage example

from types_aiobotocore_codebuild.literals import DescribeTestCasesPaginatorName

def get_value() -> DescribeTestCasesPaginatorName:
    return "describe_test_cases"
```

```python
# DescribeTestCasesPaginatorName definition

DescribeTestCasesPaginatorName = Literal[
    "describe_test_cases",
]
```
## EnvironmentTypeType

```python
# EnvironmentTypeType usage example

from types_aiobotocore_codebuild.literals import EnvironmentTypeType

def get_value() -> EnvironmentTypeType:
    return "ARM_CONTAINER"
```

```python
# EnvironmentTypeType definition

EnvironmentTypeType = Literal[
    "ARM_CONTAINER",
    "LINUX_CONTAINER",
    "LINUX_GPU_CONTAINER",
    "WINDOWS_CONTAINER",
    "WINDOWS_SERVER_2019_CONTAINER",
]
```
## EnvironmentVariableTypeType

```python
# EnvironmentVariableTypeType usage example

from types_aiobotocore_codebuild.literals import EnvironmentVariableTypeType

def get_value() -> EnvironmentVariableTypeType:
    return "PARAMETER_STORE"
```

```python
# EnvironmentVariableTypeType definition

EnvironmentVariableTypeType = Literal[
    "PARAMETER_STORE",
    "PLAINTEXT",
    "SECRETS_MANAGER",
]
```
## FileSystemTypeType

```python
# FileSystemTypeType usage example

from types_aiobotocore_codebuild.literals import FileSystemTypeType

def get_value() -> FileSystemTypeType:
    return "EFS"
```

```python
# FileSystemTypeType definition

FileSystemTypeType = Literal[
    "EFS",
]
```
## ImagePullCredentialsTypeType

```python
# ImagePullCredentialsTypeType usage example

from types_aiobotocore_codebuild.literals import ImagePullCredentialsTypeType

def get_value() -> ImagePullCredentialsTypeType:
    return "CODEBUILD"
```

```python
# ImagePullCredentialsTypeType definition

ImagePullCredentialsTypeType = Literal[
    "CODEBUILD",
    "SERVICE_ROLE",
]
```
## LanguageTypeType

```python
# LanguageTypeType usage example

from types_aiobotocore_codebuild.literals import LanguageTypeType

def get_value() -> LanguageTypeType:
    return "ANDROID"
```

```python
# LanguageTypeType definition

LanguageTypeType = Literal[
    "ANDROID",
    "BASE",
    "DOCKER",
    "DOTNET",
    "GOLANG",
    "JAVA",
    "NODE_JS",
    "PHP",
    "PYTHON",
    "RUBY",
]
```
## ListBuildBatchesForProjectPaginatorName

```python
# ListBuildBatchesForProjectPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListBuildBatchesForProjectPaginatorName

def get_value() -> ListBuildBatchesForProjectPaginatorName:
    return "list_build_batches_for_project"
```

```python
# ListBuildBatchesForProjectPaginatorName definition

ListBuildBatchesForProjectPaginatorName = Literal[
    "list_build_batches_for_project",
]
```
## ListBuildBatchesPaginatorName

```python
# ListBuildBatchesPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListBuildBatchesPaginatorName

def get_value() -> ListBuildBatchesPaginatorName:
    return "list_build_batches"
```

```python
# ListBuildBatchesPaginatorName definition

ListBuildBatchesPaginatorName = Literal[
    "list_build_batches",
]
```
## ListBuildsForProjectPaginatorName

```python
# ListBuildsForProjectPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListBuildsForProjectPaginatorName

def get_value() -> ListBuildsForProjectPaginatorName:
    return "list_builds_for_project"
```

```python
# ListBuildsForProjectPaginatorName definition

ListBuildsForProjectPaginatorName = Literal[
    "list_builds_for_project",
]
```
## ListBuildsPaginatorName

```python
# ListBuildsPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListBuildsPaginatorName

def get_value() -> ListBuildsPaginatorName:
    return "list_builds"
```

```python
# ListBuildsPaginatorName definition

ListBuildsPaginatorName = Literal[
    "list_builds",
]
```
## ListProjectsPaginatorName

```python
# ListProjectsPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListProjectsPaginatorName

def get_value() -> ListProjectsPaginatorName:
    return "list_projects"
```

```python
# ListProjectsPaginatorName definition

ListProjectsPaginatorName = Literal[
    "list_projects",
]
```
## ListReportGroupsPaginatorName

```python
# ListReportGroupsPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListReportGroupsPaginatorName

def get_value() -> ListReportGroupsPaginatorName:
    return "list_report_groups"
```

```python
# ListReportGroupsPaginatorName definition

ListReportGroupsPaginatorName = Literal[
    "list_report_groups",
]
```
## ListReportsForReportGroupPaginatorName

```python
# ListReportsForReportGroupPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListReportsForReportGroupPaginatorName

def get_value() -> ListReportsForReportGroupPaginatorName:
    return "list_reports_for_report_group"
```

```python
# ListReportsForReportGroupPaginatorName definition

ListReportsForReportGroupPaginatorName = Literal[
    "list_reports_for_report_group",
]
```
## ListReportsPaginatorName

```python
# ListReportsPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListReportsPaginatorName

def get_value() -> ListReportsPaginatorName:
    return "list_reports"
```

```python
# ListReportsPaginatorName definition

ListReportsPaginatorName = Literal[
    "list_reports",
]
```
## ListSharedProjectsPaginatorName

```python
# ListSharedProjectsPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListSharedProjectsPaginatorName

def get_value() -> ListSharedProjectsPaginatorName:
    return "list_shared_projects"
```

```python
# ListSharedProjectsPaginatorName definition

ListSharedProjectsPaginatorName = Literal[
    "list_shared_projects",
]
```
## ListSharedReportGroupsPaginatorName

```python
# ListSharedReportGroupsPaginatorName usage example

from types_aiobotocore_codebuild.literals import ListSharedReportGroupsPaginatorName

def get_value() -> ListSharedReportGroupsPaginatorName:
    return "list_shared_report_groups"
```

```python
# ListSharedReportGroupsPaginatorName definition

ListSharedReportGroupsPaginatorName = Literal[
    "list_shared_report_groups",
]
```
## LogsConfigStatusTypeType

```python
# LogsConfigStatusTypeType usage example

from types_aiobotocore_codebuild.literals import LogsConfigStatusTypeType

def get_value() -> LogsConfigStatusTypeType:
    return "DISABLED"
```

```python
# LogsConfigStatusTypeType definition

LogsConfigStatusTypeType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## PlatformTypeType

```python
# PlatformTypeType usage example

from types_aiobotocore_codebuild.literals import PlatformTypeType

def get_value() -> PlatformTypeType:
    return "AMAZON_LINUX"
```

```python
# PlatformTypeType definition

PlatformTypeType = Literal[
    "AMAZON_LINUX",
    "DEBIAN",
    "UBUNTU",
    "WINDOWS_SERVER",
]
```
## ProjectSortByTypeType

```python
# ProjectSortByTypeType usage example

from types_aiobotocore_codebuild.literals import ProjectSortByTypeType

def get_value() -> ProjectSortByTypeType:
    return "CREATED_TIME"
```

```python
# ProjectSortByTypeType definition

ProjectSortByTypeType = Literal[
    "CREATED_TIME",
    "LAST_MODIFIED_TIME",
    "NAME",
]
```
## ProjectVisibilityTypeType

```python
# ProjectVisibilityTypeType usage example

from types_aiobotocore_codebuild.literals import ProjectVisibilityTypeType

def get_value() -> ProjectVisibilityTypeType:
    return "PRIVATE"
```

```python
# ProjectVisibilityTypeType definition

ProjectVisibilityTypeType = Literal[
    "PRIVATE",
    "PUBLIC_READ",
]
```
## ReportCodeCoverageSortByTypeType

```python
# ReportCodeCoverageSortByTypeType usage example

from types_aiobotocore_codebuild.literals import ReportCodeCoverageSortByTypeType

def get_value() -> ReportCodeCoverageSortByTypeType:
    return "FILE_PATH"
```

```python
# ReportCodeCoverageSortByTypeType definition

ReportCodeCoverageSortByTypeType = Literal[
    "FILE_PATH",
    "LINE_COVERAGE_PERCENTAGE",
]
```
## ReportExportConfigTypeType

```python
# ReportExportConfigTypeType usage example

from types_aiobotocore_codebuild.literals import ReportExportConfigTypeType

def get_value() -> ReportExportConfigTypeType:
    return "NO_EXPORT"
```

```python
# ReportExportConfigTypeType definition

ReportExportConfigTypeType = Literal[
    "NO_EXPORT",
    "S3",
]
```
## ReportGroupSortByTypeType

```python
# ReportGroupSortByTypeType usage example

from types_aiobotocore_codebuild.literals import ReportGroupSortByTypeType

def get_value() -> ReportGroupSortByTypeType:
    return "CREATED_TIME"
```

```python
# ReportGroupSortByTypeType definition

ReportGroupSortByTypeType = Literal[
    "CREATED_TIME",
    "LAST_MODIFIED_TIME",
    "NAME",
]
```
## ReportGroupStatusTypeType

```python
# ReportGroupStatusTypeType usage example

from types_aiobotocore_codebuild.literals import ReportGroupStatusTypeType

def get_value() -> ReportGroupStatusTypeType:
    return "ACTIVE"
```

```python
# ReportGroupStatusTypeType definition

ReportGroupStatusTypeType = Literal[
    "ACTIVE",
    "DELETING",
]
```
## ReportGroupTrendFieldTypeType

```python
# ReportGroupTrendFieldTypeType usage example

from types_aiobotocore_codebuild.literals import ReportGroupTrendFieldTypeType

def get_value() -> ReportGroupTrendFieldTypeType:
    return "BRANCHES_COVERED"
```

```python
# ReportGroupTrendFieldTypeType definition

ReportGroupTrendFieldTypeType = Literal[
    "BRANCH_COVERAGE",
    "BRANCHES_COVERED",
    "BRANCHES_MISSED",
    "DURATION",
    "LINE_COVERAGE",
    "LINES_COVERED",
    "LINES_MISSED",
    "PASS_RATE",
    "TOTAL",
]
```
## ReportPackagingTypeType

```python
# ReportPackagingTypeType usage example

from types_aiobotocore_codebuild.literals import ReportPackagingTypeType

def get_value() -> ReportPackagingTypeType:
    return "NONE"
```

```python
# ReportPackagingTypeType definition

ReportPackagingTypeType = Literal[
    "NONE",
    "ZIP",
]
```
## ReportStatusTypeType

```python
# ReportStatusTypeType usage example

from types_aiobotocore_codebuild.literals import ReportStatusTypeType

def get_value() -> ReportStatusTypeType:
    return "DELETING"
```

```python
# ReportStatusTypeType definition

ReportStatusTypeType = Literal[
    "DELETING",
    "FAILED",
    "GENERATING",
    "INCOMPLETE",
    "SUCCEEDED",
]
```
## ReportTypeType

```python
# ReportTypeType usage example

from types_aiobotocore_codebuild.literals import ReportTypeType

def get_value() -> ReportTypeType:
    return "CODE_COVERAGE"
```

```python
# ReportTypeType definition

ReportTypeType = Literal[
    "CODE_COVERAGE",
    "TEST",
]
```
## RetryBuildBatchTypeType

```python
# RetryBuildBatchTypeType usage example

from types_aiobotocore_codebuild.literals import RetryBuildBatchTypeType

def get_value() -> RetryBuildBatchTypeType:
    return "RETRY_ALL_BUILDS"
```

```python
# RetryBuildBatchTypeType definition

RetryBuildBatchTypeType = Literal[
    "RETRY_ALL_BUILDS",
    "RETRY_FAILED_BUILDS",
]
```
## ServerTypeType

```python
# ServerTypeType usage example

from types_aiobotocore_codebuild.literals import ServerTypeType

def get_value() -> ServerTypeType:
    return "BITBUCKET"
```

```python
# ServerTypeType definition

ServerTypeType = Literal[
    "BITBUCKET",
    "GITHUB",
    "GITHUB_ENTERPRISE",
]
```
## SharedResourceSortByTypeType

```python
# SharedResourceSortByTypeType usage example

from types_aiobotocore_codebuild.literals import SharedResourceSortByTypeType

def get_value() -> SharedResourceSortByTypeType:
    return "ARN"
```

```python
# SharedResourceSortByTypeType definition

SharedResourceSortByTypeType = Literal[
    "ARN",
    "MODIFIED_TIME",
]
```
## SortOrderTypeType

```python
# SortOrderTypeType usage example

from types_aiobotocore_codebuild.literals import SortOrderTypeType

def get_value() -> SortOrderTypeType:
    return "ASCENDING"
```

```python
# SortOrderTypeType definition

SortOrderTypeType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## SourceAuthTypeType

```python
# SourceAuthTypeType usage example

from types_aiobotocore_codebuild.literals import SourceAuthTypeType

def get_value() -> SourceAuthTypeType:
    return "OAUTH"
```

```python
# SourceAuthTypeType definition

SourceAuthTypeType = Literal[
    "OAUTH",
]
```
## SourceTypeType

```python
# SourceTypeType usage example

from types_aiobotocore_codebuild.literals import SourceTypeType

def get_value() -> SourceTypeType:
    return "BITBUCKET"
```

```python
# SourceTypeType definition

SourceTypeType = Literal[
    "BITBUCKET",
    "CODECOMMIT",
    "CODEPIPELINE",
    "GITHUB",
    "GITHUB_ENTERPRISE",
    "NO_SOURCE",
    "S3",
]
```
## StatusTypeType

```python
# StatusTypeType usage example

from types_aiobotocore_codebuild.literals import StatusTypeType

def get_value() -> StatusTypeType:
    return "FAILED"
```

```python
# StatusTypeType definition

StatusTypeType = Literal[
    "FAILED",
    "FAULT",
    "IN_PROGRESS",
    "STOPPED",
    "SUCCEEDED",
    "TIMED_OUT",
]
```
## WebhookBuildTypeType

```python
# WebhookBuildTypeType usage example

from types_aiobotocore_codebuild.literals import WebhookBuildTypeType

def get_value() -> WebhookBuildTypeType:
    return "BUILD"
```

```python
# WebhookBuildTypeType definition

WebhookBuildTypeType = Literal[
    "BUILD",
    "BUILD_BATCH",
]
```
## WebhookFilterTypeType

```python
# WebhookFilterTypeType usage example

from types_aiobotocore_codebuild.literals import WebhookFilterTypeType

def get_value() -> WebhookFilterTypeType:
    return "ACTOR_ACCOUNT_ID"
```

```python
# WebhookFilterTypeType definition

WebhookFilterTypeType = Literal[
    "ACTOR_ACCOUNT_ID",
    "BASE_REF",
    "COMMIT_MESSAGE",
    "EVENT",
    "FILE_PATH",
    "HEAD_REF",
]
```
## CodeBuildServiceName

```python
# CodeBuildServiceName usage example

from types_aiobotocore_codebuild.literals import CodeBuildServiceName

def get_value() -> CodeBuildServiceName:
    return "codebuild"
```

```python
# CodeBuildServiceName definition

CodeBuildServiceName = Literal[
    "codebuild",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_codebuild.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_codebuild.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_codebuild.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_code_coverages"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_code_coverages",
    "describe_test_cases",
    "list_build_batches",
    "list_build_batches_for_project",
    "list_builds",
    "list_builds_for_project",
    "list_projects",
    "list_report_groups",
    "list_reports",
    "list_reports_for_report_group",
    "list_shared_projects",
    "list_shared_report_groups",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_codebuild.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ap-southeast-4",
    "ca-central-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
