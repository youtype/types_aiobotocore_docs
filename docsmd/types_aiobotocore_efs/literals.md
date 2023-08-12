# Literals

> [Index](../README.md) > [EFS](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
    type annotations stubs module [types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

## DescribeFileSystemsPaginatorName

```python
# DescribeFileSystemsPaginatorName usage example

from types_aiobotocore_efs.literals import DescribeFileSystemsPaginatorName

def get_value() -> DescribeFileSystemsPaginatorName:
    return "describe_file_systems"
```

```python
# DescribeFileSystemsPaginatorName definition

DescribeFileSystemsPaginatorName = Literal[
    "describe_file_systems",
]
```
## DescribeMountTargetsPaginatorName

```python
# DescribeMountTargetsPaginatorName usage example

from types_aiobotocore_efs.literals import DescribeMountTargetsPaginatorName

def get_value() -> DescribeMountTargetsPaginatorName:
    return "describe_mount_targets"
```

```python
# DescribeMountTargetsPaginatorName definition

DescribeMountTargetsPaginatorName = Literal[
    "describe_mount_targets",
]
```
## DescribeTagsPaginatorName

```python
# DescribeTagsPaginatorName usage example

from types_aiobotocore_efs.literals import DescribeTagsPaginatorName

def get_value() -> DescribeTagsPaginatorName:
    return "describe_tags"
```

```python
# DescribeTagsPaginatorName definition

DescribeTagsPaginatorName = Literal[
    "describe_tags",
]
```
## LifeCycleStateType

```python
# LifeCycleStateType usage example

from types_aiobotocore_efs.literals import LifeCycleStateType

def get_value() -> LifeCycleStateType:
    return "available"
```

```python
# LifeCycleStateType definition

LifeCycleStateType = Literal[
    "available",
    "creating",
    "deleted",
    "deleting",
    "error",
    "updating",
]
```
## PerformanceModeType

```python
# PerformanceModeType usage example

from types_aiobotocore_efs.literals import PerformanceModeType

def get_value() -> PerformanceModeType:
    return "generalPurpose"
```

```python
# PerformanceModeType definition

PerformanceModeType = Literal[
    "generalPurpose",
    "maxIO",
]
```
## ReplicationStatusType

```python
# ReplicationStatusType usage example

from types_aiobotocore_efs.literals import ReplicationStatusType

def get_value() -> ReplicationStatusType:
    return "DELETING"
```

```python
# ReplicationStatusType definition

ReplicationStatusType = Literal[
    "DELETING",
    "ENABLED",
    "ENABLING",
    "ERROR",
    "PAUSED",
    "PAUSING",
]
```
## ResourceIdTypeType

```python
# ResourceIdTypeType usage example

from types_aiobotocore_efs.literals import ResourceIdTypeType

def get_value() -> ResourceIdTypeType:
    return "LONG_ID"
```

```python
# ResourceIdTypeType definition

ResourceIdTypeType = Literal[
    "LONG_ID",
    "SHORT_ID",
]
```
## ResourceType

```python
# ResourceType usage example

from types_aiobotocore_efs.literals import ResourceType

def get_value() -> ResourceType:
    return "FILE_SYSTEM"
```

```python
# ResourceType definition

ResourceType = Literal[
    "FILE_SYSTEM",
    "MOUNT_TARGET",
]
```
## StatusType

```python
# StatusType usage example

from types_aiobotocore_efs.literals import StatusType

def get_value() -> StatusType:
    return "DISABLED"
```

```python
# StatusType definition

StatusType = Literal[
    "DISABLED",
    "DISABLING",
    "ENABLED",
    "ENABLING",
]
```
## ThroughputModeType

```python
# ThroughputModeType usage example

from types_aiobotocore_efs.literals import ThroughputModeType

def get_value() -> ThroughputModeType:
    return "bursting"
```

```python
# ThroughputModeType definition

ThroughputModeType = Literal[
    "bursting",
    "elastic",
    "provisioned",
]
```
## TransitionToIARulesType

```python
# TransitionToIARulesType usage example

from types_aiobotocore_efs.literals import TransitionToIARulesType

def get_value() -> TransitionToIARulesType:
    return "AFTER_14_DAYS"
```

```python
# TransitionToIARulesType definition

TransitionToIARulesType = Literal[
    "AFTER_14_DAYS",
    "AFTER_1_DAY",
    "AFTER_30_DAYS",
    "AFTER_60_DAYS",
    "AFTER_7_DAYS",
    "AFTER_90_DAYS",
]
```
## TransitionToPrimaryStorageClassRulesType

```python
# TransitionToPrimaryStorageClassRulesType usage example

from types_aiobotocore_efs.literals import TransitionToPrimaryStorageClassRulesType

def get_value() -> TransitionToPrimaryStorageClassRulesType:
    return "AFTER_1_ACCESS"
```

```python
# TransitionToPrimaryStorageClassRulesType definition

TransitionToPrimaryStorageClassRulesType = Literal[
    "AFTER_1_ACCESS",
]
```
## EFSServiceName

```python
# EFSServiceName usage example

from types_aiobotocore_efs.literals import EFSServiceName

def get_value() -> EFSServiceName:
    return "efs"
```

```python
# EFSServiceName definition

EFSServiceName = Literal[
    "efs",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_efs.literals import ServiceName

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

from types_aiobotocore_efs.literals import ResourceServiceName

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

from types_aiobotocore_efs.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_file_systems"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_file_systems",
    "describe_mount_targets",
    "describe_tags",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_efs.literals import RegionName

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
